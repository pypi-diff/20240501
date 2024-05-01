# Comparing `tmp/highctidh-1.0.2024012400.tar.gz` & `tmp/highctidh-1.0.2024050100.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "highctidh-1.0.2024012400.tar", last modified: Wed Jan 24 15:07:42 2024, max compression
+gzip compressed data, was "highctidh-1.0.2024050100.tar", last modified: Wed May  1 14:22:24 2024, max compression
```

## Comparing `highctidh-1.0.2024012400.tar` & `highctidh-1.0.2024050100.tar`

### file list

```diff
@@ -1,370 +1,373 @@
--rw-r--r--   0        0        0       52 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/MANIFEST.in
--rw-r--r--   0        0        0    52393 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/Makefile
--rw-r--r--   0        0        0     7018 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/Makefile.packages
--rw-r--r--   0        0        0     8019 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/README.md
--rw-r--r--   0        0        0       15 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/VERSION
--rwxr-xr-x   0        0        0     1500 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/analyze-costs
--rwxr-xr-x   0        0        0     1051 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/analyze-pr
--rw-r--r--   0        0        0      424 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/annotations.h
--rwxr-xr-x   0        0        0    52677 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/autogen
--rw-r--r--   0        0        0     3516 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/bench.c
--rw-r--r--   0        0        0      378 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/binding1024.h
--rw-r--r--   0        0        0      378 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/binding2048.h
--rw-r--r--   0        0        0      374 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/binding511.h
--rw-r--r--   0        0        0      374 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/binding512.h
--rw-r--r--   0        0        0      341 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/cgo.h
--rwxr-xr-x   0        0        0     3532 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/chain.py
--rw-r--r--   0        0        0      945 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/checkct.c
--rw-r--r--   0        0        0     4341 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/costisog.py
--rw-r--r--   0        0        0     1564 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/costpoly.c
--rw-r--r--   0        0        0     8258 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/costpoly.py
--rwxr-xr-x   0        0        0     4505 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/costs.py
--rw-r--r--   0        0        0      239 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/cpucycles.h
--rw-r--r--   0        0        0      236 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/crypto_classify.c
--rw-r--r--   0        0        0      195 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/crypto_classify.h
--rw-r--r--   0        0        0       55 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/crypto_classify_namespace.h
--rw-r--r--   0        0        0      236 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/crypto_declassify.c
--rw-r--r--   0        0        0      203 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/crypto_declassify.h
--rw-r--r--   0        0        0       59 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/crypto_declassify_namespace.h
--rw-r--r--   0        0        0    11085 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/csidh.c
--rw-r--r--   0        0        0     3281 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/csidh.h
--rw-r--r--   0        0        0     1352 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/csidh_all_clearnamespaces.h
--rw-r--r--   0        0        0      583 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/csidh_namespace.h
--rw-r--r--   0        0        0      424 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh1024/annotations.h
--rw-r--r--   0        0        0      378 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh1024/binding1024.h
--rw-r--r--   0        0        0      341 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh1024/cgo.h
--rw-r--r--   0        0        0     4232 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh1024/common.go
--rw-r--r--   0        0        0      874 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh1024/common_test.go
--rw-r--r--   0        0        0      236 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh1024/crypto_classify.c
--rw-r--r--   0        0        0      195 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh1024/crypto_classify.h
--rw-r--r--   0        0        0       55 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh1024/crypto_classify_namespace.h
--rw-r--r--   0        0        0      236 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh1024/crypto_declassify.c
--rw-r--r--   0        0        0      203 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh1024/crypto_declassify.h
--rw-r--r--   0        0        0       59 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh1024/crypto_declassify_namespace.h
--rw-r--r--   0        0        0    11085 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh1024/csidh.c
--rw-r--r--   0        0        0     3281 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh1024/csidh.h
--rw-r--r--   0        0        0      583 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh1024/csidh_namespace.h
--rw-r--r--   0        0        0     8023 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh1024/ctidh1024.go
--rw-r--r--   0        0        0     1773 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh1024/ctidh1024_bench_test.go
--rw-r--r--   0        0        0     2389 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh1024/ctidh1024_test.go
--rw-r--r--   0        0        0     1978 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh1024/elligator.c
--rw-r--r--   0        0        0      162 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh1024/elligator.h
--rw-r--r--   0        0        0       43 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh1024/elligator_namespace.h
--rw-r--r--   0        0        0      833 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh1024/error.go
--rw-r--r--   0        0        0   701316 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh1024/fiat_p1024.c
--rw-r--r--   0        0        0     4970 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh1024/fiat_p1024.h
--rw-r--r--   0        0        0     4259 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh1024/fp.h
--rw-r--r--   0        0        0    14161 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh1024/fp1024.S
--rw-r--r--   0        0        0    15533 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh1024/fp2fiat.c
--rw-r--r--   0        0        0    30384 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh1024/fp_inv1024.c
--rw-r--r--   0        0        0     1272 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh1024/fp_namespace.h
--rw-r--r--   0        0        0    30472 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh1024/fp_sqrt1024.c
--rw-r--r--   0        0        0      274 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh1024/golang-misc.c
--rw-r--r--   0        0        0      851 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh1024/int32_minmax.h
--rw-r--r--   0        0        0      985 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh1024/int32_sort.c
--rw-r--r--   0        0        0      794 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh1024/int32_sort.h
--rw-r--r--   0        0        0    36635 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh1024/int32_sort_x86.c
--rw-r--r--   0        0        0      506 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh1024/int32mask.h
--rw-r--r--   0        0        0      506 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh1024/int64mask.h
--rw-r--r--   0        0        0    17478 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh1024/mont.c
--rw-r--r--   0        0        0      950 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh1024/mont.h
--rw-r--r--   0        0        0      850 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh1024/mont_namespace.h
--rw-r--r--   0        0        0      506 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh1024/naidne.h
--rw-r--r--   0        0        0    37107 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh1024/poly.c
--rw-r--r--   0        0        0     2173 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh1024/poly.h
--rw-r--r--   0        0        0     1948 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh1024/poly_namespace.h
--rw-r--r--   0        0        0     1033 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh1024/primes.h
--rw-r--r--   0        0        0     2820 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh1024/primes1024.c
--rw-r--r--   0        0        0      483 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh1024/primes_namespace.h
--rw-r--r--   0        0        0      731 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh1024/proj.h
--rw-r--r--   0        0        0     3860 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh1024/random.c
--rw-r--r--   0        0        0      809 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh1024/random.h
--rw-r--r--   0        0        0      301 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh1024/random_namespace.h
--rw-r--r--   0        0        0      713 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh1024/randombytes.c
--rw-r--r--   0        0        0      224 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh1024/randombytes.h
--rw-r--r--   0        0        0      630 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh1024/skgen.c
--rw-r--r--   0        0        0      730 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh1024/steps.c
--rw-r--r--   0        0        0      541 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh1024/steps.h
--rw-r--r--   0        0        0      163 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh1024/steps_namespace.h
--rw-r--r--   0        0        0      156 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh1024/steps_untuned.c
--rw-r--r--   0        0        0     1688 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh1024/uintbig.h
--rw-r--r--   0        0        0     3513 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh1024/uintbig1024.S
--rw-r--r--   0        0        0      779 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh1024/uintbig_namespace.h
--rw-r--r--   0        0        0     2481 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh1024/validate.c
--rw-r--r--   0        0        0     6948 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh1024/vectors1024_test.go
--rw-r--r--   0        0        0      424 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh2048/annotations.h
--rw-r--r--   0        0        0      378 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh2048/binding2048.h
--rw-r--r--   0        0        0      341 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh2048/cgo.h
--rw-r--r--   0        0        0     4232 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh2048/common.go
--rw-r--r--   0        0        0      874 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh2048/common_test.go
--rw-r--r--   0        0        0      236 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh2048/crypto_classify.c
--rw-r--r--   0        0        0      195 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh2048/crypto_classify.h
--rw-r--r--   0        0        0       55 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh2048/crypto_classify_namespace.h
--rw-r--r--   0        0        0      236 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh2048/crypto_declassify.c
--rw-r--r--   0        0        0      203 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh2048/crypto_declassify.h
--rw-r--r--   0        0        0       59 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh2048/crypto_declassify_namespace.h
--rw-r--r--   0        0        0    11085 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh2048/csidh.c
--rw-r--r--   0        0        0     3281 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh2048/csidh.h
--rw-r--r--   0        0        0      583 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh2048/csidh_namespace.h
--rw-r--r--   0        0        0     8023 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh2048/ctidh2048.go
--rw-r--r--   0        0        0     1773 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh2048/ctidh2048_bench_test.go
--rw-r--r--   0        0        0     2389 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh2048/ctidh2048_test.go
--rw-r--r--   0        0        0     1978 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh2048/elligator.c
--rw-r--r--   0        0        0      162 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh2048/elligator.h
--rw-r--r--   0        0        0       43 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh2048/elligator_namespace.h
--rw-r--r--   0        0        0      833 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh2048/error.go
--rw-r--r--   0        0        0  2648254 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh2048/fiat_p2048.c
--rw-r--r--   0        0        0     3115 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh2048/fiat_p2048.h
--rw-r--r--   0        0        0     4259 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh2048/fp.h
--rw-r--r--   0        0        0    27053 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh2048/fp2048.S
--rw-r--r--   0        0        0    15533 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh2048/fp2fiat.c
--rw-r--r--   0        0        0    93576 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh2048/fp_inv2048.c
--rw-r--r--   0        0        0     1272 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh2048/fp_namespace.h
--rw-r--r--   0        0        0    93008 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh2048/fp_sqrt2048.c
--rw-r--r--   0        0        0      311 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh2048/golang-misc.c
--rw-r--r--   0        0        0      851 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh2048/int32_minmax.h
--rw-r--r--   0        0        0      985 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh2048/int32_sort.c
--rw-r--r--   0        0        0      794 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh2048/int32_sort.h
--rw-r--r--   0        0        0    36635 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh2048/int32_sort_x86.c
--rw-r--r--   0        0        0      506 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh2048/int32mask.h
--rw-r--r--   0        0        0      506 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh2048/int64mask.h
--rw-r--r--   0        0        0    17478 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh2048/mont.c
--rw-r--r--   0        0        0      950 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh2048/mont.h
--rw-r--r--   0        0        0      850 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh2048/mont_namespace.h
--rw-r--r--   0        0        0      506 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh2048/naidne.h
--rw-r--r--   0        0        0    37107 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh2048/poly.c
--rw-r--r--   0        0        0     2173 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh2048/poly.h
--rw-r--r--   0        0        0     1948 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh2048/poly_namespace.h
--rw-r--r--   0        0        0     1033 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh2048/primes.h
--rw-r--r--   0        0        0     4460 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh2048/primes2048.c
--rw-r--r--   0        0        0      483 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh2048/primes_namespace.h
--rw-r--r--   0        0        0      731 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh2048/proj.h
--rw-r--r--   0        0        0     3860 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh2048/random.c
--rw-r--r--   0        0        0      809 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh2048/random.h
--rw-r--r--   0        0        0      301 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh2048/random_namespace.h
--rw-r--r--   0        0        0      713 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh2048/randombytes.c
--rw-r--r--   0        0        0      224 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh2048/randombytes.h
--rw-r--r--   0        0        0      630 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh2048/skgen.c
--rw-r--r--   0        0        0      730 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh2048/steps.c
--rw-r--r--   0        0        0      541 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh2048/steps.h
--rw-r--r--   0        0        0      163 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh2048/steps_namespace.h
--rw-r--r--   0        0        0      156 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh2048/steps_untuned.c
--rw-r--r--   0        0        0     1688 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh2048/uintbig.h
--rw-r--r--   0        0        0     5373 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh2048/uintbig2048.S
--rw-r--r--   0        0        0      779 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh2048/uintbig_namespace.h
--rw-r--r--   0        0        0     2481 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh2048/validate.c
--rw-r--r--   0        0        0    10005 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh2048/vectors2048_test.go
--rw-r--r--   0        0        0      424 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh511/annotations.h
--rw-r--r--   0        0        0      374 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh511/binding511.h
--rw-r--r--   0        0        0      341 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh511/cgo.h
--rw-r--r--   0        0        0     4226 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh511/common.go
--rw-r--r--   0        0        0      873 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh511/common_test.go
--rw-r--r--   0        0        0      236 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh511/crypto_classify.c
--rw-r--r--   0        0        0      195 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh511/crypto_classify.h
--rw-r--r--   0        0        0       55 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh511/crypto_classify_namespace.h
--rw-r--r--   0        0        0      236 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh511/crypto_declassify.c
--rw-r--r--   0        0        0      203 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh511/crypto_declassify.h
--rw-r--r--   0        0        0       59 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh511/crypto_declassify_namespace.h
--rw-r--r--   0        0        0    11085 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh511/csidh.c
--rw-r--r--   0        0        0     3281 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh511/csidh.h
--rw-r--r--   0        0        0      583 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh511/csidh_namespace.h
--rw-r--r--   0        0        0     8016 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh511/ctidh511.go
--rw-r--r--   0        0        0     1772 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh511/ctidh511_bench_test.go
--rw-r--r--   0        0        0     2388 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh511/ctidh511_test.go
--rw-r--r--   0        0        0     1978 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh511/elligator.c
--rw-r--r--   0        0        0      162 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh511/elligator.h
--rw-r--r--   0        0        0       43 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh511/elligator_namespace.h
--rw-r--r--   0        0        0      832 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh511/error.go
--rw-r--r--   0        0        0   199276 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh511/fiat_p511.c
--rw-r--r--   0        0        0     3734 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh511/fiat_p511.h
--rw-r--r--   0        0        0     4259 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh511/fp.h
--rw-r--r--   0        0        0    15533 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh511/fp2fiat.c
--rw-r--r--   0        0        0     7859 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh511/fp511.S
--rw-r--r--   0        0        0    11084 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh511/fp_inv511.c
--rw-r--r--   0        0        0     1272 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh511/fp_namespace.h
--rw-r--r--   0        0        0    10975 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh511/fp_sqrt511.c
--rw-r--r--   0        0        0      272 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh511/golang-misc.c
--rw-r--r--   0        0        0      851 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh511/int32_minmax.h
--rw-r--r--   0        0        0      985 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh511/int32_sort.c
--rw-r--r--   0        0        0      794 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh511/int32_sort.h
--rw-r--r--   0        0        0    36635 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh511/int32_sort_x86.c
--rw-r--r--   0        0        0      506 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh511/int32mask.h
--rw-r--r--   0        0        0      506 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh511/int64mask.h
--rw-r--r--   0        0        0    17478 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh511/mont.c
--rw-r--r--   0        0        0      950 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh511/mont.h
--rw-r--r--   0        0        0      850 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh511/mont_namespace.h
--rw-r--r--   0        0        0      506 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh511/naidne.h
--rw-r--r--   0        0        0    37107 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh511/poly.c
--rw-r--r--   0        0        0     2173 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh511/poly.h
--rw-r--r--   0        0        0     1948 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh511/poly_namespace.h
--rw-r--r--   0        0        0     1033 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh511/primes.h
--rw-r--r--   0        0        0     1826 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh511/primes511.c
--rw-r--r--   0        0        0      483 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh511/primes_namespace.h
--rw-r--r--   0        0        0      731 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh511/proj.h
--rw-r--r--   0        0        0     3860 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh511/random.c
--rw-r--r--   0        0        0      809 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh511/random.h
--rw-r--r--   0        0        0      301 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh511/random_namespace.h
--rw-r--r--   0        0        0      713 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh511/randombytes.c
--rw-r--r--   0        0        0      224 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh511/randombytes.h
--rw-r--r--   0        0        0      630 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh511/skgen.c
--rw-r--r--   0        0        0      730 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh511/steps.c
--rw-r--r--   0        0        0      541 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh511/steps.h
--rw-r--r--   0        0        0      163 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh511/steps_namespace.h
--rw-r--r--   0        0        0      156 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh511/steps_untuned.c
--rw-r--r--   0        0        0     1688 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh511/uintbig.h
--rw-r--r--   0        0        0     2565 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh511/uintbig511.S
--rw-r--r--   0        0        0      779 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh511/uintbig_namespace.h
--rw-r--r--   0        0        0     2481 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh511/validate.c
--rw-r--r--   0        0        0     5360 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh511/vectors511_test.go
--rw-r--r--   0        0        0      424 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh512/annotations.h
--rw-r--r--   0        0        0      374 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh512/binding512.h
--rw-r--r--   0        0        0      341 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh512/cgo.h
--rw-r--r--   0        0        0     4226 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh512/common.go
--rw-r--r--   0        0        0      873 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh512/common_test.go
--rw-r--r--   0        0        0      236 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh512/crypto_classify.c
--rw-r--r--   0        0        0      195 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh512/crypto_classify.h
--rw-r--r--   0        0        0       55 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh512/crypto_classify_namespace.h
--rw-r--r--   0        0        0      236 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh512/crypto_declassify.c
--rw-r--r--   0        0        0      203 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh512/crypto_declassify.h
--rw-r--r--   0        0        0       59 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh512/crypto_declassify_namespace.h
--rw-r--r--   0        0        0    11085 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh512/csidh.c
--rw-r--r--   0        0        0     3281 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh512/csidh.h
--rw-r--r--   0        0        0      583 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh512/csidh_namespace.h
--rw-r--r--   0        0        0     8016 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh512/ctidh512.go
--rw-r--r--   0        0        0     1772 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh512/ctidh512_bench_test.go
--rw-r--r--   0        0        0     2388 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh512/ctidh512_test.go
--rw-r--r--   0        0        0     1978 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh512/elligator.c
--rw-r--r--   0        0        0      162 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh512/elligator.h
--rw-r--r--   0        0        0       43 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh512/elligator_namespace.h
--rw-r--r--   0        0        0      832 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh512/error.go
--rw-r--r--   0        0        0   199276 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh512/fiat_p512.c
--rw-r--r--   0        0        0     3734 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh512/fiat_p512.h
--rw-r--r--   0        0        0     4259 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh512/fp.h
--rw-r--r--   0        0        0    15533 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh512/fp2fiat.c
--rw-r--r--   0        0        0     7859 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh512/fp512.S
--rw-r--r--   0        0        0    11084 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh512/fp_inv512.c
--rw-r--r--   0        0        0     1272 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh512/fp_namespace.h
--rw-r--r--   0        0        0    10975 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh512/fp_sqrt512.c
--rw-r--r--   0        0        0      271 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh512/golang-misc.c
--rw-r--r--   0        0        0      851 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh512/int32_minmax.h
--rw-r--r--   0        0        0      985 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh512/int32_sort.c
--rw-r--r--   0        0        0      794 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh512/int32_sort.h
--rw-r--r--   0        0        0    36635 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh512/int32_sort_x86.c
--rw-r--r--   0        0        0      506 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh512/int32mask.h
--rw-r--r--   0        0        0      506 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh512/int64mask.h
--rw-r--r--   0        0        0    17478 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh512/mont.c
--rw-r--r--   0        0        0      950 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh512/mont.h
--rw-r--r--   0        0        0      850 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh512/mont_namespace.h
--rw-r--r--   0        0        0      506 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh512/naidne.h
--rw-r--r--   0        0        0    37107 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh512/poly.c
--rw-r--r--   0        0        0     2173 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh512/poly.h
--rw-r--r--   0        0        0     1948 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh512/poly_namespace.h
--rw-r--r--   0        0        0     1033 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh512/primes.h
--rw-r--r--   0        0        0     1822 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh512/primes512.c
--rw-r--r--   0        0        0      483 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh512/primes_namespace.h
--rw-r--r--   0        0        0      731 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh512/proj.h
--rw-r--r--   0        0        0     3860 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh512/random.c
--rw-r--r--   0        0        0      809 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh512/random.h
--rw-r--r--   0        0        0      301 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh512/random_namespace.h
--rw-r--r--   0        0        0      713 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh512/randombytes.c
--rw-r--r--   0        0        0      224 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh512/randombytes.h
--rw-r--r--   0        0        0      630 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh512/skgen.c
--rw-r--r--   0        0        0      730 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh512/steps.c
--rw-r--r--   0        0        0      541 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh512/steps.h
--rw-r--r--   0        0        0      163 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh512/steps_namespace.h
--rw-r--r--   0        0        0      156 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh512/steps_untuned.c
--rw-r--r--   0        0        0     1688 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh512/uintbig.h
--rw-r--r--   0        0        0     2565 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh512/uintbig512.S
--rw-r--r--   0        0        0      779 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh512/uintbig_namespace.h
--rw-r--r--   0        0        0     2481 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh512/validate.c
--rw-r--r--   0        0        0     5361 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ctidh512/vectors512_test.go
--rwxr-xr-x   0        0        0      433 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/debian-rules
--rwxr-xr-x   0        0        0     5471 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/distmults.py
--rw-r--r--   0        0        0     1978 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/elligator.c
--rw-r--r--   0        0        0      162 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/elligator.h
--rw-r--r--   0        0        0       43 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/elligator_namespace.h
--rw-r--r--   0        0        0     2908 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/example-ctidh.c
--rw-r--r--   0        0        0     2943 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/examples_static.c
--rw-r--r--   0        0        0   701316 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/fiat_p1024.c
--rw-r--r--   0        0        0     4970 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/fiat_p1024.h
--rw-r--r--   0        0        0  2648254 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/fiat_p2048.c
--rw-r--r--   0        0        0     3115 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/fiat_p2048.h
--rw-r--r--   0        0        0   199276 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/fiat_p511.c
--rw-r--r--   0        0        0     3734 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/fiat_p511.h
--rw-r--r--   0        0        0   199276 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/fiat_p512.c
--rw-r--r--   0        0        0     3734 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/fiat_p512.h
--rw-r--r--   0        0        0     4259 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/fp.h
--rw-r--r--   0        0        0    14161 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/fp1024.S
--rw-r--r--   0        0        0    27053 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/fp2048.S
--rw-r--r--   0        0        0    15533 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/fp2fiat.c
--rw-r--r--   0        0        0     7859 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/fp511.S
--rw-r--r--   0        0        0     7859 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/fp512.S
--rw-r--r--   0        0        0    30384 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/fp_inv1024.c
--rw-r--r--   0        0        0    93576 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/fp_inv2048.c
--rw-r--r--   0        0        0    11084 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/fp_inv511.c
--rw-r--r--   0        0        0    11084 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/fp_inv512.c
--rw-r--r--   0        0        0     1272 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/fp_namespace.h
--rw-r--r--   0        0        0    30472 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/fp_sqrt1024.c
--rw-r--r--   0        0        0    93008 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/fp_sqrt2048.c
--rw-r--r--   0        0        0    10975 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/fp_sqrt511.c
--rw-r--r--   0        0        0    10975 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/fp_sqrt512.c
--rw-r--r--   0        0        0     1923 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/go-tests/ctidh_test.go
--rwxr-xr-x   0        0        0     5846 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/greedy
--rw-r--r--   0        0        0     5286 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/highctidh.h
--rwxr-xr-x   0        0        0    19804 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/highctidh/__init__.py
--rw-r--r--   0        0        0       27 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/highctidh/__version__.py
--rw-r--r--   0        0        0      977 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/highctidh_macros.h
--rw-r--r--   0        0        0      851 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/int32_minmax.h
--rw-r--r--   0        0        0      985 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/int32_sort.c
--rw-r--r--   0        0        0      794 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/int32_sort.h
--rw-r--r--   0        0        0    36635 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/int32_sort_x86.c
--rw-r--r--   0        0        0      506 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/int32mask.h
--rw-r--r--   0        0        0      506 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/int64mask.h
--rwxr-xr-x   0        0        0      452 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/memoized.py
--rw-r--r--   0        0        0    17478 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/mont.c
--rw-r--r--   0        0        0      950 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/mont.h
--rw-r--r--   0        0        0      850 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/mont_namespace.h
--rw-r--r--   0        0        0      506 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/naidne.h
--rw-r--r--   0        0        0    37107 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/poly.c
--rw-r--r--   0        0        0     2173 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/poly.h
--rw-r--r--   0        0        0     1948 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/poly_namespace.h
--rw-r--r--   0        0        0     1033 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/primes.h
--rw-r--r--   0        0        0     2820 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/primes1024.c
--rw-r--r--   0        0        0     4460 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/primes2048.c
--rw-r--r--   0        0        0     1826 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/primes511.c
--rw-r--r--   0        0        0     1822 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/primes512.c
--rw-r--r--   0        0        0      483 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/primes_namespace.h
--rw-r--r--   0        0        0      731 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/proj.h
--rw-r--r--   0        0        0      733 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/pyproject.toml
--rw-r--r--   0        0        0     3860 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/random.c
--rw-r--r--   0        0        0      809 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/random.h
--rw-r--r--   0        0        0      301 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/random_namespace.h
--rw-r--r--   0        0        0      713 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/randombytes.c
--rw-r--r--   0        0        0      224 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/randombytes.h
--rw-r--r--   0        0        0      531 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/setup.cfg
--rw-r--r--   0        0        0    10004 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/setup.py
--rwxr-xr-x   0        0        0     3134 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/sim.py
--rw-r--r--   0        0        0      630 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/skgen.c
--rw-r--r--   0        0        0      319 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/stdeb.cfg
--rw-r--r--   0        0        0      730 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/steps.c
--rw-r--r--   0        0        0      541 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/steps.h
--rw-r--r--   0        0        0      163 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/steps_namespace.h
--rw-r--r--   0        0        0      156 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/steps_untuned.c
--rw-r--r--   0        0        0    62110 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/test.c
--rwxr-xr-x   0        0        0      543 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/test.sh
--rw-r--r--   0        0        0     7155 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/testrandom.c
--rw-r--r--   0        0        0        0 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/tests/__init__.py
--rwxr-xr-x   0        0        0    87795 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/tests/test_highctidh.py
--rwxr-xr-x   0        0        0      749 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/tune2c
--rw-r--r--   0        0        0     2793 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/tunecycles.c
--rw-r--r--   0        0        0     1747 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/tunemults.c
--rw-r--r--   0        0        0     7007 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/ubench.c
--rw-r--r--   0        0        0     1688 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/uintbig.h
--rw-r--r--   0        0        0     3513 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/uintbig1024.S
--rw-r--r--   0        0        0     5373 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/uintbig2048.S
--rw-r--r--   0        0        0     2565 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/uintbig511.S
--rw-r--r--   0        0        0     2565 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/uintbig512.S
--rw-r--r--   0        0        0      779 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/uintbig_namespace.h
--rw-r--r--   0        0        0     3099 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/umults.c
--rw-r--r--   0        0        0     2481 2024-01-24 15:07:42.000000 highctidh-1.0.2024012400/validate.c
--rw-r--r--   0        0        0     8579 1970-01-01 00:00:00.000000 highctidh-1.0.2024012400/PKG-INFO
+-rw-r--r--   0        0        0       52 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/MANIFEST.in
+-rw-r--r--   0        0        0    54119 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/Makefile
+-rw-r--r--   0        0        0     7262 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/Makefile.packages
+-rw-r--r--   0        0        0     9245 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/README.md
+-rw-r--r--   0        0        0       15 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/VERSION
+-rwxr-xr-x   0        0        0     1500 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/analyze-costs
+-rwxr-xr-x   0        0        0     1051 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/analyze-pr
+-rw-r--r--   0        0        0      424 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/annotations.h
+-rwxr-xr-x   0        0        0    55100 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/autogen
+-rw-r--r--   0        0        0     3516 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/bench.c
+-rw-r--r--   0        0        0      378 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/binding1024.h
+-rw-r--r--   0        0        0      378 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/binding2048.h
+-rw-r--r--   0        0        0      374 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/binding511.h
+-rw-r--r--   0        0        0      374 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/binding512.h
+-rw-r--r--   0        0        0      341 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/cgo.h
+-rwxr-xr-x   0        0        0     3532 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/chain.py
+-rw-r--r--   0        0        0      945 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/checkct.c
+-rw-r--r--   0        0        0     4341 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/costisog.py
+-rw-r--r--   0        0        0     1564 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/costpoly.c
+-rw-r--r--   0        0        0     8258 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/costpoly.py
+-rwxr-xr-x   0        0        0     4505 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/costs.py
+-rw-r--r--   0        0        0      239 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/cpucycles.h
+-rw-r--r--   0        0        0      236 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/crypto_classify.c
+-rw-r--r--   0        0        0      195 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/crypto_classify.h
+-rw-r--r--   0        0        0       55 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/crypto_classify_namespace.h
+-rw-r--r--   0        0        0      236 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/crypto_declassify.c
+-rw-r--r--   0        0        0      203 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/crypto_declassify.h
+-rw-r--r--   0        0        0       59 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/crypto_declassify_namespace.h
+-rw-r--r--   0        0        0    11320 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/csidh.c
+-rw-r--r--   0        0        0     3301 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/csidh.h
+-rw-r--r--   0        0        0     1352 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/csidh_all_clearnamespaces.h
+-rw-r--r--   0        0        0      583 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/csidh_namespace.h
+-rw-r--r--   0        0        0      424 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/annotations.h
+-rw-r--r--   0        0        0      378 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/binding1024.h
+-rw-r--r--   0        0        0      341 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/cgo.h
+-rw-r--r--   0        0        0     5446 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/common.go
+-rw-r--r--   0        0        0      874 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/common_test.go
+-rw-r--r--   0        0        0      236 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/crypto_classify.c
+-rw-r--r--   0        0        0      195 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/crypto_classify.h
+-rw-r--r--   0        0        0       55 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/crypto_classify_namespace.h
+-rw-r--r--   0        0        0      236 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/crypto_declassify.c
+-rw-r--r--   0        0        0      203 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/crypto_declassify.h
+-rw-r--r--   0        0        0       59 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/crypto_declassify_namespace.h
+-rw-r--r--   0        0        0    11320 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/csidh.c
+-rw-r--r--   0        0        0     3301 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/csidh.h
+-rw-r--r--   0        0        0      583 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/csidh_namespace.h
+-rw-r--r--   0        0        0     8023 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/ctidh1024.go
+-rw-r--r--   0        0        0     1773 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/ctidh1024_bench_test.go
+-rw-r--r--   0        0        0     2389 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/ctidh1024_test.go
+-rw-r--r--   0        0        0     1978 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/elligator.c
+-rw-r--r--   0        0        0      162 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/elligator.h
+-rw-r--r--   0        0        0       43 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/elligator_namespace.h
+-rw-r--r--   0        0        0      833 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/error.go
+-rw-r--r--   0        0        0   701424 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/fiat_p1024.c
+-rw-r--r--   0        0        0     4970 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/fiat_p1024.h
+-rw-r--r--   0        0        0     4261 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/fp.h
+-rw-r--r--   0        0        0    14162 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/fp1024.S
+-rw-r--r--   0        0        0    15552 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/fp2fiat.c
+-rw-r--r--   0        0        0    30384 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/fp_inv1024.c
+-rw-r--r--   0        0        0     1272 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/fp_namespace.h
+-rw-r--r--   0        0        0    30472 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/fp_sqrt1024.c
+-rw-r--r--   0        0        0      274 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/golang-misc.c
+-rw-r--r--   0        0        0      872 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/int32_minmax.h
+-rw-r--r--   0        0        0      980 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/int32_sort.c
+-rw-r--r--   0        0        0      794 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/int32_sort.h
+-rw-r--r--   0        0        0    36687 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/int32_sort_x86.c
+-rw-r--r--   0        0        0      506 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/int32mask.h
+-rw-r--r--   0        0        0      506 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/int64mask.h
+-rw-r--r--   0        0        0    17478 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/mont.c
+-rw-r--r--   0        0        0      950 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/mont.h
+-rw-r--r--   0        0        0      850 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/mont_namespace.h
+-rw-r--r--   0        0        0     1127 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/naidne.h
+-rw-r--r--   0        0        0    37107 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/poly.c
+-rw-r--r--   0        0        0     2173 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/poly.h
+-rw-r--r--   0        0        0     1948 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/poly_namespace.h
+-rw-r--r--   0        0        0     1033 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/primes.h
+-rw-r--r--   0        0        0     2820 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/primes1024.c
+-rw-r--r--   0        0        0      483 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/primes_namespace.h
+-rw-r--r--   0        0        0      731 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/proj.h
+-rw-r--r--   0        0        0     3860 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/random.c
+-rw-r--r--   0        0        0      809 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/random.h
+-rw-r--r--   0        0        0      301 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/random_namespace.h
+-rw-r--r--   0        0        0     1771 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/randombytes.c
+-rw-r--r--   0        0        0      224 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/randombytes.h
+-rw-r--r--   0        0        0      630 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/skgen.c
+-rw-r--r--   0        0        0      730 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/steps.c
+-rw-r--r--   0        0        0      541 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/steps.h
+-rw-r--r--   0        0        0      163 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/steps_namespace.h
+-rw-r--r--   0        0        0      156 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/steps_untuned.c
+-rw-r--r--   0        0        0     1688 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/uintbig.h
+-rw-r--r--   0        0        0     3514 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/uintbig1024.S
+-rw-r--r--   0        0        0      844 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/uintbig_namespace.h
+-rw-r--r--   0        0        0     2481 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/validate.c
+-rw-r--r--   0        0        0     6948 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/vectors1024_test.go
+-rw-r--r--   0        0        0      424 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/annotations.h
+-rw-r--r--   0        0        0      378 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/binding2048.h
+-rw-r--r--   0        0        0      341 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/cgo.h
+-rw-r--r--   0        0        0     5447 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/common.go
+-rw-r--r--   0        0        0      874 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/common_test.go
+-rw-r--r--   0        0        0      236 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/crypto_classify.c
+-rw-r--r--   0        0        0      195 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/crypto_classify.h
+-rw-r--r--   0        0        0       55 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/crypto_classify_namespace.h
+-rw-r--r--   0        0        0      236 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/crypto_declassify.c
+-rw-r--r--   0        0        0      203 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/crypto_declassify.h
+-rw-r--r--   0        0        0       59 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/crypto_declassify_namespace.h
+-rw-r--r--   0        0        0    11320 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/csidh.c
+-rw-r--r--   0        0        0     3301 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/csidh.h
+-rw-r--r--   0        0        0      583 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/csidh_namespace.h
+-rw-r--r--   0        0        0     8023 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/ctidh2048.go
+-rw-r--r--   0        0        0     1773 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/ctidh2048_bench_test.go
+-rw-r--r--   0        0        0     2389 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/ctidh2048_test.go
+-rw-r--r--   0        0        0     1978 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/elligator.c
+-rw-r--r--   0        0        0      162 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/elligator.h
+-rw-r--r--   0        0        0       43 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/elligator_namespace.h
+-rw-r--r--   0        0        0      833 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/error.go
+-rw-r--r--   0        0        0  2648362 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/fiat_p2048.c
+-rw-r--r--   0        0        0     3115 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/fiat_p2048.h
+-rw-r--r--   0        0        0     4261 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/fp.h
+-rw-r--r--   0        0        0    27054 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/fp2048.S
+-rw-r--r--   0        0        0    15552 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/fp2fiat.c
+-rw-r--r--   0        0        0    93576 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/fp_inv2048.c
+-rw-r--r--   0        0        0     1272 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/fp_namespace.h
+-rw-r--r--   0        0        0    93008 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/fp_sqrt2048.c
+-rw-r--r--   0        0        0      311 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/golang-misc.c
+-rw-r--r--   0        0        0      872 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/int32_minmax.h
+-rw-r--r--   0        0        0      980 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/int32_sort.c
+-rw-r--r--   0        0        0      794 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/int32_sort.h
+-rw-r--r--   0        0        0    36687 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/int32_sort_x86.c
+-rw-r--r--   0        0        0      506 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/int32mask.h
+-rw-r--r--   0        0        0      506 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/int64mask.h
+-rw-r--r--   0        0        0    17478 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/mont.c
+-rw-r--r--   0        0        0      950 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/mont.h
+-rw-r--r--   0        0        0      850 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/mont_namespace.h
+-rw-r--r--   0        0        0     1127 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/naidne.h
+-rw-r--r--   0        0        0    37107 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/poly.c
+-rw-r--r--   0        0        0     2173 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/poly.h
+-rw-r--r--   0        0        0     1948 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/poly_namespace.h
+-rw-r--r--   0        0        0     1033 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/primes.h
+-rw-r--r--   0        0        0     4460 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/primes2048.c
+-rw-r--r--   0        0        0      483 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/primes_namespace.h
+-rw-r--r--   0        0        0      731 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/proj.h
+-rw-r--r--   0        0        0     3860 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/random.c
+-rw-r--r--   0        0        0      809 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/random.h
+-rw-r--r--   0        0        0      301 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/random_namespace.h
+-rw-r--r--   0        0        0     1771 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/randombytes.c
+-rw-r--r--   0        0        0      224 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/randombytes.h
+-rw-r--r--   0        0        0      630 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/skgen.c
+-rw-r--r--   0        0        0      730 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/steps.c
+-rw-r--r--   0        0        0      541 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/steps.h
+-rw-r--r--   0        0        0      163 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/steps_namespace.h
+-rw-r--r--   0        0        0      156 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/steps_untuned.c
+-rw-r--r--   0        0        0     1688 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/uintbig.h
+-rw-r--r--   0        0        0     5374 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/uintbig2048.S
+-rw-r--r--   0        0        0      844 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/uintbig_namespace.h
+-rw-r--r--   0        0        0     2481 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/validate.c
+-rw-r--r--   0        0        0    10005 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/vectors2048_test.go
+-rw-r--r--   0        0        0      424 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/annotations.h
+-rw-r--r--   0        0        0      374 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/binding511.h
+-rw-r--r--   0        0        0      341 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/cgo.h
+-rw-r--r--   0        0        0     5433 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/common.go
+-rw-r--r--   0        0        0      873 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/common_test.go
+-rw-r--r--   0        0        0      236 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/crypto_classify.c
+-rw-r--r--   0        0        0      195 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/crypto_classify.h
+-rw-r--r--   0        0        0       55 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/crypto_classify_namespace.h
+-rw-r--r--   0        0        0      236 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/crypto_declassify.c
+-rw-r--r--   0        0        0      203 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/crypto_declassify.h
+-rw-r--r--   0        0        0       59 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/crypto_declassify_namespace.h
+-rw-r--r--   0        0        0    11320 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/csidh.c
+-rw-r--r--   0        0        0     3301 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/csidh.h
+-rw-r--r--   0        0        0      583 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/csidh_namespace.h
+-rw-r--r--   0        0        0     8016 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/ctidh511.go
+-rw-r--r--   0        0        0     1772 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/ctidh511_bench_test.go
+-rw-r--r--   0        0        0     2388 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/ctidh511_test.go
+-rw-r--r--   0        0        0     1978 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/elligator.c
+-rw-r--r--   0        0        0      162 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/elligator.h
+-rw-r--r--   0        0        0       43 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/elligator_namespace.h
+-rw-r--r--   0        0        0      832 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/error.go
+-rw-r--r--   0        0        0   199383 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/fiat_p511.c
+-rw-r--r--   0        0        0     3734 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/fiat_p511.h
+-rw-r--r--   0        0        0     4261 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/fp.h
+-rw-r--r--   0        0        0    15552 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/fp2fiat.c
+-rw-r--r--   0        0        0     7860 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/fp511.S
+-rw-r--r--   0        0        0    11084 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/fp_inv511.c
+-rw-r--r--   0        0        0     1272 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/fp_namespace.h
+-rw-r--r--   0        0        0    10975 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/fp_sqrt511.c
+-rw-r--r--   0        0        0      272 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/golang-misc.c
+-rw-r--r--   0        0        0      872 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/int32_minmax.h
+-rw-r--r--   0        0        0      980 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/int32_sort.c
+-rw-r--r--   0        0        0      794 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/int32_sort.h
+-rw-r--r--   0        0        0    36687 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/int32_sort_x86.c
+-rw-r--r--   0        0        0      506 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/int32mask.h
+-rw-r--r--   0        0        0      506 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/int64mask.h
+-rw-r--r--   0        0        0    17478 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/mont.c
+-rw-r--r--   0        0        0      950 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/mont.h
+-rw-r--r--   0        0        0      850 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/mont_namespace.h
+-rw-r--r--   0        0        0     1127 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/naidne.h
+-rw-r--r--   0        0        0    37107 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/poly.c
+-rw-r--r--   0        0        0     2173 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/poly.h
+-rw-r--r--   0        0        0     1948 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/poly_namespace.h
+-rw-r--r--   0        0        0     1033 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/primes.h
+-rw-r--r--   0        0        0     1826 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/primes511.c
+-rw-r--r--   0        0        0      483 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/primes_namespace.h
+-rw-r--r--   0        0        0      731 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/proj.h
+-rw-r--r--   0        0        0     3860 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/random.c
+-rw-r--r--   0        0        0      809 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/random.h
+-rw-r--r--   0        0        0      301 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/random_namespace.h
+-rw-r--r--   0        0        0     1771 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/randombytes.c
+-rw-r--r--   0        0        0      224 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/randombytes.h
+-rw-r--r--   0        0        0      630 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/skgen.c
+-rw-r--r--   0        0        0      730 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/steps.c
+-rw-r--r--   0        0        0      541 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/steps.h
+-rw-r--r--   0        0        0      163 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/steps_namespace.h
+-rw-r--r--   0        0        0      156 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/steps_untuned.c
+-rw-r--r--   0        0        0     1688 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/uintbig.h
+-rw-r--r--   0        0        0     2566 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/uintbig511.S
+-rw-r--r--   0        0        0      844 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/uintbig_namespace.h
+-rw-r--r--   0        0        0     2481 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/validate.c
+-rw-r--r--   0        0        0     5360 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/vectors511_test.go
+-rw-r--r--   0        0        0      424 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/annotations.h
+-rw-r--r--   0        0        0      374 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/binding512.h
+-rw-r--r--   0        0        0      341 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/cgo.h
+-rw-r--r--   0        0        0     5433 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/common.go
+-rw-r--r--   0        0        0      873 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/common_test.go
+-rw-r--r--   0        0        0      236 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/crypto_classify.c
+-rw-r--r--   0        0        0      195 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/crypto_classify.h
+-rw-r--r--   0        0        0       55 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/crypto_classify_namespace.h
+-rw-r--r--   0        0        0      236 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/crypto_declassify.c
+-rw-r--r--   0        0        0      203 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/crypto_declassify.h
+-rw-r--r--   0        0        0       59 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/crypto_declassify_namespace.h
+-rw-r--r--   0        0        0    11320 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/csidh.c
+-rw-r--r--   0        0        0     3301 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/csidh.h
+-rw-r--r--   0        0        0      583 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/csidh_namespace.h
+-rw-r--r--   0        0        0     8016 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/ctidh512.go
+-rw-r--r--   0        0        0     1772 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/ctidh512_bench_test.go
+-rw-r--r--   0        0        0     2388 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/ctidh512_test.go
+-rw-r--r--   0        0        0     1978 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/elligator.c
+-rw-r--r--   0        0        0      162 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/elligator.h
+-rw-r--r--   0        0        0       43 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/elligator_namespace.h
+-rw-r--r--   0        0        0      832 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/error.go
+-rw-r--r--   0        0        0   199383 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/fiat_p512.c
+-rw-r--r--   0        0        0     3734 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/fiat_p512.h
+-rw-r--r--   0        0        0     4261 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/fp.h
+-rw-r--r--   0        0        0    15552 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/fp2fiat.c
+-rw-r--r--   0        0        0     7860 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/fp512.S
+-rw-r--r--   0        0        0    11084 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/fp_inv512.c
+-rw-r--r--   0        0        0     1272 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/fp_namespace.h
+-rw-r--r--   0        0        0    10975 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/fp_sqrt512.c
+-rw-r--r--   0        0        0      271 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/golang-misc.c
+-rw-r--r--   0        0        0      872 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/int32_minmax.h
+-rw-r--r--   0        0        0      980 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/int32_sort.c
+-rw-r--r--   0        0        0      794 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/int32_sort.h
+-rw-r--r--   0        0        0    36687 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/int32_sort_x86.c
+-rw-r--r--   0        0        0      506 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/int32mask.h
+-rw-r--r--   0        0        0      506 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/int64mask.h
+-rw-r--r--   0        0        0    17478 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/mont.c
+-rw-r--r--   0        0        0      950 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/mont.h
+-rw-r--r--   0        0        0      850 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/mont_namespace.h
+-rw-r--r--   0        0        0     1127 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/naidne.h
+-rw-r--r--   0        0        0    37107 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/poly.c
+-rw-r--r--   0        0        0     2173 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/poly.h
+-rw-r--r--   0        0        0     1948 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/poly_namespace.h
+-rw-r--r--   0        0        0     1033 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/primes.h
+-rw-r--r--   0        0        0     1822 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/primes512.c
+-rw-r--r--   0        0        0      483 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/primes_namespace.h
+-rw-r--r--   0        0        0      731 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/proj.h
+-rw-r--r--   0        0        0     3860 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/random.c
+-rw-r--r--   0        0        0      809 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/random.h
+-rw-r--r--   0        0        0      301 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/random_namespace.h
+-rw-r--r--   0        0        0     1771 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/randombytes.c
+-rw-r--r--   0        0        0      224 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/randombytes.h
+-rw-r--r--   0        0        0      630 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/skgen.c
+-rw-r--r--   0        0        0      730 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/steps.c
+-rw-r--r--   0        0        0      541 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/steps.h
+-rw-r--r--   0        0        0      163 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/steps_namespace.h
+-rw-r--r--   0        0        0      156 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/steps_untuned.c
+-rw-r--r--   0        0        0     1688 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/uintbig.h
+-rw-r--r--   0        0        0     2566 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/uintbig512.S
+-rw-r--r--   0        0        0      844 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/uintbig_namespace.h
+-rw-r--r--   0        0        0     2481 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/validate.c
+-rw-r--r--   0        0        0     5361 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/vectors512_test.go
+-rwxr-xr-x   0        0        0      433 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/debian-rules
+-rwxr-xr-x   0        0        0     5471 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/distmults.py
+-rw-r--r--   0        0        0     1978 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/elligator.c
+-rw-r--r--   0        0        0      162 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/elligator.h
+-rw-r--r--   0        0        0       43 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/elligator_namespace.h
+-rw-r--r--   0        0        0     2928 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/example-ctidh.c
+-rw-r--r--   0        0        0     2943 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/examples_static.c
+-rw-r--r--   0        0        0   701424 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/fiat_p1024.c
+-rw-r--r--   0        0        0     4970 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/fiat_p1024.h
+-rw-r--r--   0        0        0  2648362 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/fiat_p2048.c
+-rw-r--r--   0        0        0     3115 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/fiat_p2048.h
+-rw-r--r--   0        0        0   199383 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/fiat_p511.c
+-rw-r--r--   0        0        0     3734 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/fiat_p511.h
+-rw-r--r--   0        0        0   199383 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/fiat_p512.c
+-rw-r--r--   0        0        0     3734 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/fiat_p512.h
+-rw-r--r--   0        0        0     4261 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/fp.h
+-rw-r--r--   0        0        0    14162 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/fp1024.S
+-rw-r--r--   0        0        0    27054 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/fp2048.S
+-rw-r--r--   0        0        0    15552 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/fp2fiat.c
+-rw-r--r--   0        0        0     7860 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/fp511.S
+-rw-r--r--   0        0        0     7860 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/fp512.S
+-rw-r--r--   0        0        0    30384 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/fp_inv1024.c
+-rw-r--r--   0        0        0    93576 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/fp_inv2048.c
+-rw-r--r--   0        0        0    11084 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/fp_inv511.c
+-rw-r--r--   0        0        0    11084 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/fp_inv512.c
+-rw-r--r--   0        0        0     1272 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/fp_namespace.h
+-rw-r--r--   0        0        0    30472 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/fp_sqrt1024.c
+-rw-r--r--   0        0        0    93008 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/fp_sqrt2048.c
+-rw-r--r--   0        0        0    10975 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/fp_sqrt511.c
+-rw-r--r--   0        0        0    10975 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/fp_sqrt512.c
+-rw-r--r--   0        0        0     1923 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/go-tests/ctidh_test.go
+-rwxr-xr-x   0        0        0     5846 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/greedy
+-rw-r--r--   0        0        0     5286 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/highctidh.h
+-rwxr-xr-x   0        0        0    19804 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/highctidh/__init__.py
+-rw-r--r--   0        0        0       27 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/highctidh/__version__.py
+-rwxr-xr-x   0        0        0     5176 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/highctidh/bench.py
+-rw-r--r--   0        0        0      977 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/highctidh_macros.h
+-rw-r--r--   0        0        0      872 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/int32_minmax.h
+-rw-r--r--   0        0        0      980 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/int32_sort.c
+-rw-r--r--   0        0        0      794 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/int32_sort.h
+-rw-r--r--   0        0        0    36687 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/int32_sort_x86.c
+-rw-r--r--   0        0        0      506 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/int32mask.h
+-rw-r--r--   0        0        0      506 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/int64mask.h
+-rwxr-xr-x   0        0        0      452 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/memoized.py
+-rw-r--r--   0        0        0    17478 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/mont.c
+-rw-r--r--   0        0        0      950 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/mont.h
+-rw-r--r--   0        0        0      850 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/mont_namespace.h
+-rw-r--r--   0        0        0     1127 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/naidne.h
+-rw-r--r--   0        0        0    37107 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/poly.c
+-rw-r--r--   0        0        0     2173 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/poly.h
+-rw-r--r--   0        0        0     1948 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/poly_namespace.h
+-rw-r--r--   0        0        0     1033 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/primes.h
+-rw-r--r--   0        0        0     2820 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/primes1024.c
+-rw-r--r--   0        0        0     4460 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/primes2048.c
+-rw-r--r--   0        0        0     1826 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/primes511.c
+-rw-r--r--   0        0        0     1822 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/primes512.c
+-rw-r--r--   0        0        0      483 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/primes_namespace.h
+-rw-r--r--   0        0        0      731 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/proj.h
+-rw-r--r--   0        0        0      733 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/pyproject.toml
+-rw-r--r--   0        0        0     3860 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/random.c
+-rw-r--r--   0        0        0      809 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/random.h
+-rw-r--r--   0        0        0      301 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/random_namespace.h
+-rw-r--r--   0        0        0     1771 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/randombytes.c
+-rw-r--r--   0        0        0      224 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/randombytes.h
+-rw-r--r--   0        0        0      531 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/setup.cfg
+-rw-r--r--   0        0        0    14530 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/setup.py
+-rwxr-xr-x   0        0        0     3134 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/sim.py
+-rw-r--r--   0        0        0      630 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/skgen.c
+-rw-r--r--   0        0        0      319 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/stdeb.cfg
+-rw-r--r--   0        0        0      730 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/steps.c
+-rw-r--r--   0        0        0      541 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/steps.h
+-rw-r--r--   0        0        0      163 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/steps_namespace.h
+-rw-r--r--   0        0        0      156 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/steps_untuned.c
+-rwxr-xr-x   0        0        0      487 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/test-python.sh
+-rwxr-xr-x   0        0        0       69 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/test-quick.sh
+-rw-r--r--   0        0        0    63364 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/test.c
+-rwxr-xr-x   0        0        0      543 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/test.sh
+-rw-r--r--   0        0        0     7175 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/testrandom.c
+-rw-r--r--   0        0        0        0 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/tests/__init__.py
+-rwxr-xr-x   0        0        0    87795 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/tests/test_highctidh.py
+-rwxr-xr-x   0        0        0      749 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/tune2c
+-rw-r--r--   0        0        0     2793 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/tunecycles.c
+-rw-r--r--   0        0        0     1747 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/tunemults.c
+-rw-r--r--   0        0        0     7007 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ubench.c
+-rw-r--r--   0        0        0     1688 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/uintbig.h
+-rw-r--r--   0        0        0     3514 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/uintbig1024.S
+-rw-r--r--   0        0        0     5374 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/uintbig2048.S
+-rw-r--r--   0        0        0     2566 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/uintbig511.S
+-rw-r--r--   0        0        0     2566 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/uintbig512.S
+-rw-r--r--   0        0        0      844 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/uintbig_namespace.h
+-rw-r--r--   0        0        0     3099 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/umults.c
+-rw-r--r--   0        0        0     2481 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/validate.c
+-rw-r--r--   0        0        0     9805 1970-01-01 00:00:00.000000 highctidh-1.0.2024050100/PKG-INFO
```

### Comparing `highctidh-1.0.2024012400/Makefile` & `highctidh-1.0.2024050100/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 .PHONY: clean
 HOST_PLATFORM := $(shell uname -m)
 HOST_OS := $(shell uname -s)
 
 ### override these for cross-building:
 PLATFORM ?= $(shell uname -m)
-ifeq	($(PLATFORM), $(filter $(PLATFORM), arm64 amd64 loongarch64 mips64 mips64el ppc64 ppc64le riscv64 s390x sparc64 x86_64))
+ifeq	($(PLATFORM), $(filter $(PLATFORM), arm64 amd64 i86pc loongarch64 mips64 mips64el ppc64 ppc64le riscv64 s390x sparc sparc4v sparc64 x86_64))
 PLATFORM_SIZE ?= 64
 else ifeq ($(PLATFORM), $(filter $(PLATFORM), armv7l i386 i686 mips mipsel))
 PLATFORM_SIZE ?= 32
 else
 PLATFORM_SIZE ?= $(shell getconf LONG_BIT)
 endif
 
@@ -26,29 +26,54 @@
 CC_MTUNE ?= $(CC_MARCH)
 
 SEC_CFLAGS := -Wformat -Werror=format-security -D_FORTIFY_SOURCE=2 -fstack-protector-strong
 BASE_CFLAGS := -fpie -fPIC -Wall -Wextra -pedantic -O2 -fwrapv -DGETRANDOM -Werror
 BASE_CFLAGS+=-DPLATFORM=${PLATFORM} -DPLATFORM_SIZE=${PLATFORM_SIZE}
 BASE_CFLAGS+=$(SEC_CFLAGS)
 BASE_CFLAGS+=$(if $(strip $(CC_MARCH)),-march=$(CC_MARCH) -mtune=$(CC_MTUNE),)
-LDFLAGS := -s -w
+ifeq    ($(HOST_OS), $(filter $(HOST_OS), OpenBSD, DragonFly, Darwin))
+BASE_CFLAGS+=-D__$(HOST_OS)__
+endif
+LDFLAGS :=
 ifeq ($(HOST_OS),Linux)
 LDFLAGS+=-Wl,-z,noexecstack -Wl,-z,relro -Wl,-z,now
 LDFLAGS+=-Wl,-Bsymbolic-functions
 LDFLAGS+=-Wl,--reduce-memory-overheads -Wl,--no-keep-memory
 endif
+ifeq ($(CC),clang)
+BASE_CFLAGS+=-Wno-unused-command-line-argument
+endif
+ifeq ($(CC),gcc)
+BASE_CFLAGS+=
+endif
+ifeq ($(WINDOWS),1)
+BASE_CFLAGS :=-Wall -Wextra -pedantic -O2 -fwrapv -D__Windows__
+HIGHCTIDH_PORTABLE ?=1
+BASE_CFLAGS+=-DPLATFORM=${PLATFORM} -DPLATFORM_SIZE=${PLATFORM_SIZE}
+ifeq ($(CC),x86_64-w64-mingw32-gcc)
+BASE_CFLAGS+=-fpie -fPIC
+CFLAGS = $(BASE_CFLAGS)
+endif
+ifeq ($(CC),clang)
+HIGHCTIDH_PORTABLE ?=1
+BASE_CFLAGS+=-DPLATFORM=${PLATFORM} -DPLATFORM_SIZE=${PLATFORM_SIZE}
+CFLAGS = $(BASE_CFLAGS) -Wno-unused-command-line-argument
+LDFLAGS = -LAdvapi32.dll
+endif
+endif
 # Default to using fiat crypto, safe and portable but slow backend
 HIGHCTIDH_PORTABLE ?= 1
 ifeq	($(HIGHCTIDH_PORTABLE),1)
-BASE_CFLAGS += -DHIGHCTIDH_PORTABLE
+BASE_CFLAGS += -DHIGHCTIDH_PORTABLE=1
 	libhighctidh_511_OBJS := fp2fiat511.o fiat_p511.o
 	libhighctidh_512_OBJS := fp2fiat512.o fiat_p512.o
 	libhighctidh_1024_OBJS := fp2fiat1024.o fiat_p1024.o
 	libhighctidh_2048_OBJS := fp2fiat2048.o fiat_p2048.o
 else
+BASE_CFLAGS += -DHIGHCTIDH_PORTABLE=0
 	libhighctidh_511_OBJS := uintbig511.o fp511.o
 	libhighctidh_512_OBJS := uintbig512.o fp512.o
 	libhighctidh_1024_OBJS := uintbig1024.o fp1024.o
 	libhighctidh_2048_OBJS := uintbig2048.o fp2048.o
 endif
 
 ifeq	($(PLATFORM), $(filter $(PLATFORM), arm64 aarch64))
@@ -86,44 +111,67 @@
 endif
 
 ifeq	($(PLATFORM),ppc64)
 	CFLAGS+= $(BASE_CFLAGS)
 endif
 
 ifeq	($(PLATFORM),riscv64)
-	CFLAGS+= $(BASE_CFLAGS)
+	CFLAGS+= $(BASE_CFLAGS) -D__riscv
 endif
 
 ifeq	($(PLATFORM),s390x)
 	CFLAGS+= $(BASE_CFLAGS) -D__s390x__
 	ifeq ($(CC),clang)
 		CFLAGS+= -march=z10 -mtune=z10
 	endif
 endif
 
-ifeq	($(PLATFORM),sparc64)
-	CFLAGS+= $(BASE_CFLAGS)
+ifeq   ($(HOST_OS), $(filter $(HOST_OS), SunOS))
+ifeq   ($(PLATFORM), $(filter $(PLATFORM), sparc sun4u sun4v sparc64 i86pc i386))
+	BASE_CFLAGS+=$(SEC_CFLAGS)
+	CFLAGS+=$(BASE_CFLAGS) -m64 -D__sun
+	LDFLAGS+=$(LDFLAGS)
+ifeq   ($(PLATFORM), $(filter $(PLATFORM), i86pc))
+	CFLAGS+=-D__i86pc__
+	ifeq ($(CC),gcc)
+		CFLAGS+=-mimpure-text -Wno-attributes
+	endif
+endif
+ifeq   ($(PLATFORM), $(filter $(PLATFORM), i386))
+	CFLAGS+=-D__i386__
+	ifeq ($(CC),gcc)
+		CFLAGS+=-mimpure-text
+	endif
+endif
+ifeq   ($(PLATFORM), $(filter $(PLATFORM), sparc sun4u sun4v sparc64))
+	CFLAGS+=-DHIGHCTIDH_PORTABLE=1 -D__sun4v__
+	ifeq ($(CC),gcc)
+		CFLAGS+=-mcpu=native -mtune=native -D_REENTRANT
+	endif
+endif
+endif
 endif
-
 ifeq	($(PLATFORM),unknown)
 	CFLAGS+= $(BASE_CFLAGS)
 endif
 
+ifneq	($(HOST_OS), $(filter $(HOST_OS), SunOS))
 ifeq	($(PLATFORM), $(filter $(PLATFORM), amd64 x86_64 i386 i686))
 ifeq	($(PLATFORM_SIZE),32)
 	CFLAGS+= $(BASE_CFLAGS) -D__i386__
 	ifeq ($(CC),clang)
 		CFLAGS+= -fforce-enable-int128
 	endif
 else
 
 	CFLAGS+= $(BASE_CFLAGS) -D__x86_64__
 
 endif
 endif
+endif
 
 SCC ?= $(CC) $(CFLAGS) $(LDFLAGS)
 CC += $(CFLAGS) $(LDFLAGS)
 
 default: libhighctidh.so
 
 all: default timecop generic 511 512 1024 2048
@@ -654,43 +702,43 @@
 	$(CC) -DBITS=1024 -D'NAMESPACEBITS(x)=highctidh_1024_##x' -D'NAMESPACEGENERIC(x)=highctidh_##x' \
 		-o csidh1024.o -c csidh.c
 
 csidh2048.o: csidh.c naidne.h csidh.h cgo.h binding511.h binding512.h binding1024.h binding2048.h uintbig.h uintbig_namespace.h annotations.h fp.h fp_namespace.h fiat_p511.h fiat_p512.h fiat_p1024.h fiat_p2048.h randombytes.h crypto_declassify.h crypto_declassify_namespace.h mont.h proj.h mont_namespace.h primes.h primes_namespace.h csidh_namespace.h int64mask.h elligator.h elligator_namespace.h random.h random_namespace.h Makefile
 	$(CC) -DBITS=2048 -D'NAMESPACEBITS(x)=highctidh_2048_##x' -D'NAMESPACEGENERIC(x)=highctidh_##x' \
 		-o csidh2048.o -c csidh.c
 
-validate511.o: validate.c csidh.h cgo.h binding511.h binding512.h binding1024.h binding2048.h uintbig.h uintbig_namespace.h annotations.h fp.h fp_namespace.h fiat_p511.h fiat_p512.h fiat_p1024.h fiat_p2048.h randombytes.h crypto_declassify.h crypto_declassify_namespace.h mont.h proj.h mont_namespace.h primes.h primes_namespace.h csidh_namespace.h Makefile
+validate511.o: validate.c csidh.h cgo.h binding511.h binding512.h binding1024.h binding2048.h naidne.h uintbig.h uintbig_namespace.h annotations.h fp.h fp_namespace.h fiat_p511.h fiat_p512.h fiat_p1024.h fiat_p2048.h randombytes.h crypto_declassify.h crypto_declassify_namespace.h mont.h proj.h mont_namespace.h primes.h primes_namespace.h csidh_namespace.h Makefile
 	$(CC) -DBITS=511 -D'NAMESPACEBITS(x)=highctidh_511_##x' -D'NAMESPACEGENERIC(x)=highctidh_##x' \
 		-o validate511.o -c validate.c
 
-validate512.o: validate.c csidh.h cgo.h binding511.h binding512.h binding1024.h binding2048.h uintbig.h uintbig_namespace.h annotations.h fp.h fp_namespace.h fiat_p511.h fiat_p512.h fiat_p1024.h fiat_p2048.h randombytes.h crypto_declassify.h crypto_declassify_namespace.h mont.h proj.h mont_namespace.h primes.h primes_namespace.h csidh_namespace.h Makefile
+validate512.o: validate.c csidh.h cgo.h binding511.h binding512.h binding1024.h binding2048.h naidne.h uintbig.h uintbig_namespace.h annotations.h fp.h fp_namespace.h fiat_p511.h fiat_p512.h fiat_p1024.h fiat_p2048.h randombytes.h crypto_declassify.h crypto_declassify_namespace.h mont.h proj.h mont_namespace.h primes.h primes_namespace.h csidh_namespace.h Makefile
 	$(CC) -DBITS=512 -D'NAMESPACEBITS(x)=highctidh_512_##x' -D'NAMESPACEGENERIC(x)=highctidh_##x' \
 		-o validate512.o -c validate.c
 
-validate1024.o: validate.c csidh.h cgo.h binding511.h binding512.h binding1024.h binding2048.h uintbig.h uintbig_namespace.h annotations.h fp.h fp_namespace.h fiat_p511.h fiat_p512.h fiat_p1024.h fiat_p2048.h randombytes.h crypto_declassify.h crypto_declassify_namespace.h mont.h proj.h mont_namespace.h primes.h primes_namespace.h csidh_namespace.h Makefile
+validate1024.o: validate.c csidh.h cgo.h binding511.h binding512.h binding1024.h binding2048.h naidne.h uintbig.h uintbig_namespace.h annotations.h fp.h fp_namespace.h fiat_p511.h fiat_p512.h fiat_p1024.h fiat_p2048.h randombytes.h crypto_declassify.h crypto_declassify_namespace.h mont.h proj.h mont_namespace.h primes.h primes_namespace.h csidh_namespace.h Makefile
 	$(CC) -DBITS=1024 -D'NAMESPACEBITS(x)=highctidh_1024_##x' -D'NAMESPACEGENERIC(x)=highctidh_##x' \
 		-o validate1024.o -c validate.c
 
-validate2048.o: validate.c csidh.h cgo.h binding511.h binding512.h binding1024.h binding2048.h uintbig.h uintbig_namespace.h annotations.h fp.h fp_namespace.h fiat_p511.h fiat_p512.h fiat_p1024.h fiat_p2048.h randombytes.h crypto_declassify.h crypto_declassify_namespace.h mont.h proj.h mont_namespace.h primes.h primes_namespace.h csidh_namespace.h Makefile
+validate2048.o: validate.c csidh.h cgo.h binding511.h binding512.h binding1024.h binding2048.h naidne.h uintbig.h uintbig_namespace.h annotations.h fp.h fp_namespace.h fiat_p511.h fiat_p512.h fiat_p1024.h fiat_p2048.h randombytes.h crypto_declassify.h crypto_declassify_namespace.h mont.h proj.h mont_namespace.h primes.h primes_namespace.h csidh_namespace.h Makefile
 	$(CC) -DBITS=2048 -D'NAMESPACEBITS(x)=highctidh_2048_##x' -D'NAMESPACEGENERIC(x)=highctidh_##x' \
 		-o validate2048.o -c validate.c
 
-skgen511.o: skgen.c csidh.h cgo.h binding511.h binding512.h binding1024.h binding2048.h uintbig.h uintbig_namespace.h annotations.h fp.h fp_namespace.h fiat_p511.h fiat_p512.h fiat_p1024.h fiat_p2048.h randombytes.h crypto_declassify.h crypto_declassify_namespace.h mont.h proj.h mont_namespace.h primes.h primes_namespace.h csidh_namespace.h random.h random_namespace.h Makefile
+skgen511.o: skgen.c csidh.h cgo.h binding511.h binding512.h binding1024.h binding2048.h naidne.h uintbig.h uintbig_namespace.h annotations.h fp.h fp_namespace.h fiat_p511.h fiat_p512.h fiat_p1024.h fiat_p2048.h randombytes.h crypto_declassify.h crypto_declassify_namespace.h mont.h proj.h mont_namespace.h primes.h primes_namespace.h csidh_namespace.h random.h random_namespace.h Makefile
 	$(CC) -DBITS=511 -D'NAMESPACEBITS(x)=highctidh_511_##x' -D'NAMESPACEGENERIC(x)=highctidh_##x' \
 		-o skgen511.o -c skgen.c
 
-skgen512.o: skgen.c csidh.h cgo.h binding511.h binding512.h binding1024.h binding2048.h uintbig.h uintbig_namespace.h annotations.h fp.h fp_namespace.h fiat_p511.h fiat_p512.h fiat_p1024.h fiat_p2048.h randombytes.h crypto_declassify.h crypto_declassify_namespace.h mont.h proj.h mont_namespace.h primes.h primes_namespace.h csidh_namespace.h random.h random_namespace.h Makefile
+skgen512.o: skgen.c csidh.h cgo.h binding511.h binding512.h binding1024.h binding2048.h naidne.h uintbig.h uintbig_namespace.h annotations.h fp.h fp_namespace.h fiat_p511.h fiat_p512.h fiat_p1024.h fiat_p2048.h randombytes.h crypto_declassify.h crypto_declassify_namespace.h mont.h proj.h mont_namespace.h primes.h primes_namespace.h csidh_namespace.h random.h random_namespace.h Makefile
 	$(CC) -DBITS=512 -D'NAMESPACEBITS(x)=highctidh_512_##x' -D'NAMESPACEGENERIC(x)=highctidh_##x' \
 		-o skgen512.o -c skgen.c
 
-skgen1024.o: skgen.c csidh.h cgo.h binding511.h binding512.h binding1024.h binding2048.h uintbig.h uintbig_namespace.h annotations.h fp.h fp_namespace.h fiat_p511.h fiat_p512.h fiat_p1024.h fiat_p2048.h randombytes.h crypto_declassify.h crypto_declassify_namespace.h mont.h proj.h mont_namespace.h primes.h primes_namespace.h csidh_namespace.h random.h random_namespace.h Makefile
+skgen1024.o: skgen.c csidh.h cgo.h binding511.h binding512.h binding1024.h binding2048.h naidne.h uintbig.h uintbig_namespace.h annotations.h fp.h fp_namespace.h fiat_p511.h fiat_p512.h fiat_p1024.h fiat_p2048.h randombytes.h crypto_declassify.h crypto_declassify_namespace.h mont.h proj.h mont_namespace.h primes.h primes_namespace.h csidh_namespace.h random.h random_namespace.h Makefile
 	$(CC) -DBITS=1024 -D'NAMESPACEBITS(x)=highctidh_1024_##x' -D'NAMESPACEGENERIC(x)=highctidh_##x' \
 		-o skgen1024.o -c skgen.c
 
-skgen2048.o: skgen.c csidh.h cgo.h binding511.h binding512.h binding1024.h binding2048.h uintbig.h uintbig_namespace.h annotations.h fp.h fp_namespace.h fiat_p511.h fiat_p512.h fiat_p1024.h fiat_p2048.h randombytes.h crypto_declassify.h crypto_declassify_namespace.h mont.h proj.h mont_namespace.h primes.h primes_namespace.h csidh_namespace.h random.h random_namespace.h Makefile
+skgen2048.o: skgen.c csidh.h cgo.h binding511.h binding512.h binding1024.h binding2048.h naidne.h uintbig.h uintbig_namespace.h annotations.h fp.h fp_namespace.h fiat_p511.h fiat_p512.h fiat_p1024.h fiat_p2048.h randombytes.h crypto_declassify.h crypto_declassify_namespace.h mont.h proj.h mont_namespace.h primes.h primes_namespace.h csidh_namespace.h random.h random_namespace.h Makefile
 	$(CC) -DBITS=2048 -D'NAMESPACEBITS(x)=highctidh_2048_##x' -D'NAMESPACEGENERIC(x)=highctidh_##x' \
 		-o skgen2048.o -c skgen.c
 
 elligator511.o: elligator.c crypto_declassify.h cgo.h binding511.h binding512.h binding1024.h binding2048.h crypto_declassify_namespace.h elligator.h proj.h fp.h fp_namespace.h uintbig.h uintbig_namespace.h annotations.h fiat_p511.h fiat_p512.h fiat_p1024.h fiat_p2048.h randombytes.h elligator_namespace.h Makefile
 	$(CC) -DBITS=511 -D'NAMESPACEBITS(x)=highctidh_511_##x' -D'NAMESPACEGENERIC(x)=highctidh_##x' \
 		-o elligator511.o -c elligator.c
 
@@ -924,56 +972,63 @@
 test2048-dyn: test2048 libhighctidh_2048.so
 		$(CC) -DBITS=2048 -D'NAMESPACEBITS(x)=highctidh_2048_##x' -D'NAMESPACEGENERIC(x)=highctidh_##x' -o test2048-dyn test.c -l highctidh_2048 -L .
 
 
 libhighctidh.so: libhighctidh_511.so libhighctidh_512.so libhighctidh_1024.so libhighctidh_2048.so
 		ls -l libhighctidh_*.so
 
-example511: libhighctidh_511.so
+setup-examples: csidh.h
+		-mkdir -p libhighctidh
+		-cp csidh.h libhighctidh/
+
+example511: setup-examples libhighctidh_511.so
 	$(CC) -DBITS=511 -D'NAMESPACEBITS(x)=highctidh_511_##x' \
 	-D'NAMESPACEGENERIC(x)=highctidh_##x' -o example-ctidh511 example-ctidh.c \
-	-l highctidh_511
+	-L. -I. -l highctidh_511
 
-example512: libhighctidh_512.so
+example512: setup-examples libhighctidh_512.so
 	$(CC) -DBITS=512 -D'NAMESPACEBITS(x)=highctidh_512_##x' \
 	-D'NAMESPACEGENERIC(x)=highctidh_##x' -o example-ctidh512 example-ctidh.c \
-	-l highctidh_512
+	-L. -I. -l highctidh_512
 
-example1024: libhighctidh_1024.so
+example1024: setup-examples libhighctidh_1024.so
 	$(CC) -DBITS=1024 -D'NAMESPACEBITS(x)=highctidh_1024_##x' \
 	-D'NAMESPACEGENERIC(x)=highctidh_##x' -o example-ctidh1024 example-ctidh.c \
-	-l highctidh_1024
+	-L. -I. -l highctidh_1024
 
-example2048: libhighctidh_2048.so
+example2048: setup-examples libhighctidh_2048.so
 	$(CC) -DBITS=2048 -D'NAMESPACEBITS(x)=highctidh_2048_##x' \
 	-D'NAMESPACEGENERIC(x)=highctidh_##x' -o example-ctidh2048 example-ctidh.c \
-	-l highctidh_2048
+	-L. -I. -l highctidh_2048
 
 examples: example511 example512 example1024 example2048
 		ls -l example-ctidh511 example-ctidh512 example-ctidh1024 example-ctidh2048
 
 examples-static: examples_static.c libhighctidh.a *.h
 	$(CC) -static -Wall -Werror -Wpedantic examples_static.c -Wl,-Bstatic -L. -l:libhighctidh.a -o examples-static
+
 test: clean libhighctidh.so testrandom test511 test512 test1024 test2048
 		./test.sh
 
 DESTDIR ?= /usr/local
 install: libhighctidh.so libhighctidh.a
 		install -d $(DESTDIR)/include/libhighctidh/
 		install -d $(DESTDIR)/lib/
 		install -v *.h $(DESTDIR)/include/libhighctidh/
 		install -v libhighctidh_*.so $(DESTDIR)/lib/
 		install -v libhighctidh.a $(DESTDIR)/lib/
 
 
 clean:
 		-rm -f *.a *.o *.out *.so
+		-rm -f *.s *.bc
 		-rm -f bench1024cycles bench1024mults bench1024untuned bench2048cycles bench2048mults bench2048untuned bench511cycles bench511mults bench511untuned bench512cycles bench512mults bench512untuned
 		-rm -f checkct1024cycles checkct1024mults checkct1024untuned checkct2048cycles checkct2048mults checkct2048untuned checkct511cycles checkct511mults checkct511untuned checkct512cycles checkct512mults checkct512untuned costpoly1024 costpoly2048 costpoly511 example-ctidh1024 example-ctidh2048
 		-rm -f example-ctidh511 example-ctidh512 test1024 test2048 test511 test511 test512 test512-dyn test*-dyn testrandom tunecycles1024 tunecycles2048 tunecycles511 tunecycles512 tunemults1024 tunemults2048 tunemults511 tunemults512 ubench1024 ubench2048 ubench511 ubench512 umults1024 umults2048 umults511 umults512
 		-rm -rf UNKNOWN.egg-info/ __pycache__/
 		-rm -rf build/ deb_dist/ dist/
 		-rm -rf highctidh.egg-info/ highctidh/__pycache__/
 		-rm -rf tests/__pycache__/
 		-rm -rf docker_build_output/
+		-rm -rf libhighctidh/
 		-rm -rf examples-static
 		-rm -rf highctidh-*.tar.gz
```

### Comparing `highctidh-1.0.2024012400/Makefile.packages` & `highctidh-1.0.2024050100/Makefile.packages`

 * *Files 2% similar despite different names*

```diff
@@ -52,17 +52,17 @@
 	cd ctidh1024 && go test -v;
 	cd ctidh2048 && go test -v;
 
 deb: ${SDIST_GZ} ${DEB_NAME}
 ${DEB_NAME}:
 	-mkdir -p dist/source
 	-mkdir -p build/tmp
-	python3 setup.py --command-packages=stdeb.command sdist_dsc --compat=10 --dist-dir=${WORKDIR}/dist/ --use-premade-distfile=${SDIST_GZ}
+	HIGHCTIDH_PORTABLE=$(HIGHCTIDH_PORTABLE) python3 setup.py --command-packages=stdeb.command sdist_dsc --compat=10 --dist-dir=${WORKDIR}/dist/ --use-premade-distfile=${SDIST_GZ}
 	cp debian-rules ${WORKDIR}/dist/highctidh-$(VERSION)/debian/rules
-	cd ${WORKDIR}/dist/highctidh-$(VERSION) && DEB_BUILD_OPTIONS=nocheck CC=${CC} dpkg-buildpackage -rfakeroot -uc -us
+	cd ${WORKDIR}/dist/highctidh-$(VERSION) && DEB_BUILD_OPTIONS=nocheck CC=${CC} HIGHCTIDH_PORTABLE=$(HIGHCTIDH_PORTABLE) dpkg-buildpackage -rfakeroot -uc -us
 	-ls -alh ${WORKDIR}/dist/*.deb
 	-sha256sum ${WORKDIR}/dist/*.deb
 
 wheel: ${SDIST_GZ} ${WHEEL_NAME}
 ${WHEEL_NAME}:
 	-mkdir -p dist/source
 	-mkdir -p build/tmp
@@ -100,38 +100,39 @@
 docker-fiat-generate: docker-fiat-setup
 	../misc/docker-generate-fiat.sh
 
 # NOTE:
 #   twine accepts our whl files but pypi does not due to not using the
 #   `manywheels` docker trusting trust container
 pypi-upload:
-	python3 -m twine check ${WORKDIR}/docker_build_output/upload/*$(VERSION)*.tar.gz
-	python3 -m twine upload --repository pypi ${WORKDIR}/docker_build_output/upload/*$(VERSION)*.tar.gz
+	python3 -m twine check ${WORKDIR}/docker_build_output/upload/build-artifacts/highctidh-$(VERSION).tar.gz
+	python3 -m twine upload --repository pypi ${WORKDIR}/docker_build_output/upload/build-artifacts/highctidh-$(VERSION).tar.gz
 
 prepare-artifacts-for-upload:
 	mkdir -p ${WORKDIR}/docker_build_output/upload/build-artifacts;
+	cp ${WORKDIR}/dist/highctidh-$(VERSION).tar.gz ${WORKDIR}/docker_build_output/upload/build-artifacts/
 	for arch in $(shell ls -1  ${WORKDIR}/docker_build_output |grep -v upload|grep -v .log); do \
-		echo "Copying deb and whl builds..."; \
+		echo "Copying deb and whl builds for $$arch..."; \
 		cp -v ${WORKDIR}/docker_build_output/$$arch/dist/*.deb \
 			${WORKDIR}/docker_build_output/upload/build-artifacts/ && \
 		cp -v ${WORKDIR}/docker_build_output/$$arch/dist/*.whl \
 			${WORKDIR}/docker_build_output/upload/build-artifacts/; \
 	done
 	for arch in $(shell ls -1  ${WORKDIR}/docker_build_output |grep -v upload|grep -v .log); do \
 		cd ${WORKDIR}/docker_build_output/$$arch/dist/ && \
 		echo "Creating $$arch artefact tar.gz..." && \
 		tar -cvzf \
-		highctidh_${VERSION}-$$arch-src.tar.gz.new \
+		highctidh_${VERSION}-src-$$arch.tar.gz.new \
 		*.buildinfo \
 		*.changes \
 		*.dsc \
 		*.tar.gz \
 		*.tar.xz && \
-		mv -v highctidh_${VERSION}-$$arch-src.tar.gz.new \
-			../../upload/build-artifacts/highctidh_${VERSION}-$$arch-src.tar.gz && \
+		mv -v highctidh_${VERSION}-src-$$arch.tar.gz.new \
+			../../upload/build-artifacts/highctidh_${VERSION}-src-$$arch.tar.gz && \
 		cd ../../../; \
 	done
 
 # This target calls the other targets present in this makefile from within a Docker container.
 # Our use of QEMU means that the Docker container appears to be running on
 # ${ARCH} regardless of the host CPU architecture.
 multi-arch-build: sdist
```

### Comparing `highctidh-1.0.2024012400/README.md` & `highctidh-1.0.2024050100/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -55,18 +55,26 @@
 sudo dpkg -i python3-highctidh_*.deb
 ```
 
 ## Golang bindings
 
 Add the golang bindings to a golang project:
 ```
-go get -u https://codeberg.org/vula/highctidh/ctidh511
-go get -u https://codeberg.org/vula/highctidh/ctidh512
-go get -u https://codeberg.org/vula/highctidh/ctidh1024
-go get -u https://codeberg.org/vula/highctidh/ctidh2048
+go get -u codeberg.org/vula/highctidh/
+```
+
+Use the golang bindings in a `.go` file by importing the field size that is
+desired or by importing any or all of the four field sizes:
+```
+import (
+    ctidh511  "codeberg.org/vula/highctidh/src/ctidh511"
+    ctidh512  "codeberg.org/vula/highctidh/src/ctidh512"
+    ctidh1024 "codeberg.org/vula/highctidh/src/ctidh1024"
+    ctidh2048 "codeberg.org/vula/highctidh/src/ctidh2048"
+) 
 ```
 
 # highctidh improvements
 
 This fork enhances high-ctidh with additional Makefile targets including
 building high-ctidh as four shared libraries, one for each key size of 511,
 512, 1024, and 2048. Python bindings are additionally added, as well as
@@ -77,15 +85,15 @@
 fast on the `amd64`/`x86_64` CPU architecture and functional but much slower
 with other CPU architectures. The portable backend was generated using the
 `fiat-crypto` project which uses a "Correct-by-Construction" approach; see
 `doc/PRIMES.md` for more information.  Tested architectures for the C library
 include: `amd64`/`x86_64`  (with and without avx2), `arm32v5`, `arm32v6`,
 `arm32v7`, `arm64v8`/`aarch64`/`arm64`, `i386`, `loongarch64/Loongson`, `mips`,
 `mipsel`, `mips64`, `mips64el`, `POWER8/ppc64`, `POWER9/ppc64le`, `riscv64`,
-`s390x`, and `sparc64`.
+`s390x`, `sun4v`, and `sparc64`.
 
 ## Golang bindings
 
 The Golang bindings compile and should be functional on `amd64`/`x86_64`,
 `arm32v5`, `arm32v6`, `arm32v7`, `arm64v8`/`aarch64`/`arm64`, `i386`, `ppc64`,
 `ppc64le`, `riscv64`, `s390x`, `mips`, `mipsle`, `mips64`, `mips64le`.  The
 `misc/test-golang-cross.sh` script runs tests on the host build architecture
@@ -124,31 +132,49 @@
 
 To test without installing run the `test` target:
 ```
    make test
 ```
 
 The C library and bindings have been tested on the following operating systems:
-- Alpine v3.18 (musl libc)
-- Alpine v3.19 (musl libc)
-- CheriBSD
-- Debian Sid (GNU libc)
-- Debian Bookworm (GNU libc)
-- FreeBSD
+- AlmaLinux 9.3 (GNU libc)
+- Alpine v3.17 - v3.19.1 (musl libc)
+- Arch latest (GNU libc)
+- CheriBSD 14.0-CURRENT (FreeBSD libc)
+- Clear Linux 41560 (GNU libc)
+- Debian stable, testing, unstable (GNU libc)
+- Devuan latest (GNU libc)
+- DragonFlyBSD 6.4.0 (FreeBSD libc)
+- Fedora 38, 39, 40, 41 (GNU libc)
+- FreeBSD 14.0 (FreeBSD libc)
 - HardenedBSD (FreeBSD libc)
-- MacOS
-- OpenBSD
-- Ubuntu Mantic (GNU libc)
-- Ubuntu Noble (GNU libc)
+- MacOS 11, 12, 13, 14 (BSD libc)
+- NetBSD 10.0 (NetBSD libc)
+- Omnios r151046 (illumos libc)
+- OpenBSD 7.5 (OpenBSD libc)
+- Oracle Linux 9 (GNU libc)
+- Rockylinux 9, 9.3 (GNU libc)
+- Solaris 11.4 (Solaris libc)
+- Ubuntu 22.03, 23.10, 24.04 (GNU libc)
+- Windows Server 2019, 2022 (MSVCRT)
 
 ## Notes on building
 
-Building on CheriBSD, FreeBSD, and OpenBSD building is supported using the
+Building on Solaris, CheriBSD, FreeBSD, NetBSD, and OpenBSD building is supported using the
 `gmake` command. GNU/Linux and MacOS are supported with the `make` command.
 
+Windows support is extremely experimental. The Python and Golang modules may
+not be functional on Windows. Building the main C library on Windows Server
+2019 and Windows Server 2022 should be possible with `clang` as is demonstrated
+in the continuous integration configuration `windows-fiat-c-library-test.yml`.
+It has only been tested with the Windows Server 2022 image preloaded with
+`clang`, `bash`, `make`, and other related tools
+[https://github.com/actions/runner-images/blob/main/images/windows/Windows2022-Readme.md](available
+as a part of the CI configuration).
+
 ### Additional notes on building the C library
  
 To build and install we recommend:
 ```
    sudo apt install gcc clang make
    make
    sudo make install
@@ -207,14 +233,14 @@
 The original website was https://ctidh.isogeny.org/software.html
 
 # Acknowledgements
 
 The original authors of this software released high-ctidh in the public domain.
 All contributions made in this fork are also in the public domain.
 
-Please consult `docs/AUTHORS.md` for the original authorship informaton.
+Please consult `docs/AUTHORS.md` for the original authorship information.
 
 This forked project is funded through the [NGI Assure
 Fund](https://nlnet.nl/assure), a fund established by [NLnet](https://nlnet.nl)
 with financial support from the European Commission's [Next Generation
 Internet](https://ngi.eu) program. Learn more on the [NLnet project
 page](https://nlnet.nl/project/Vula#ack).
```

### Comparing `highctidh-1.0.2024012400/analyze-costs` & `highctidh-1.0.2024050100/analyze-costs`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/analyze-pr` & `highctidh-1.0.2024050100/analyze-pr`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/autogen` & `highctidh-1.0.2024050100/autogen`

 * *Files 5% similar despite different names*

```diff
@@ -280,15 +280,15 @@
     f.write('  return fp_isequal(&check,&origx);\n')
     f.write('}\n')
   maybeupdate(fn)
 
   fn = 'uintbig%s.S'%bits
   with open(fn+'.tmp','w') as f:
     f.write('/* DO NOT EDIT! generated by ./autogen */\n')
-    f.write('#ifndef HIGHCTIDH_PORTABLE\n\n')
+    f.write('#if HIGHCTIDH_PORTABLE == 0\n\n')
     f.write('.intel_syntax noprefix\n')
     f.write('\n')
     f.write('//#include "uintbig_namespace.h"\n')
     f.write('\n')
     f.write('.section .rodata\n')
     f.write('\n')
 
@@ -402,15 +402,15 @@
 
   maybeupdate(fn)
 
   fn = 'fp%s.S'%bits
   prefix = 'highctidh_%s_' % bits
   with open(fn+'.tmp','w') as f:
     f.write('/* DO NOT EDIT! generated by ./autogen */\n')
-    f.write('#ifndef HIGHCTIDH_PORTABLE\n\n')
+    f.write('#if HIGHCTIDH_PORTABLE == 0\n\n')
     f.write('.intel_syntax noprefix\n')
     f.write('\n')
     f.write('//#include "uintbig_namespace.h"\n')
     f.write('//#include "fp_namespace.h"\n')
     f.write('\n')
     f.write('.section .rodata\n')
     f.write('\n')
@@ -919,15 +919,15 @@
 with open(fn+'.tmp','w') as f:
   f.write('# DO NOT EDIT! generated by ./autogen\n\n')
   f.write('.PHONY: clean\n')
   f.write('HOST_PLATFORM := $(shell uname -m)\n')
   f.write('HOST_OS := $(shell uname -s)\n\n')
   f.write('### override these for cross-building:\n')
   f.write('PLATFORM ?= $(shell uname -m)\n')
-  f.write('ifeq\t($(PLATFORM), $(filter $(PLATFORM), arm64 amd64 loongarch64 mips64 mips64el ppc64 ppc64le riscv64 s390x sparc64 x86_64))\n')
+  f.write('ifeq\t($(PLATFORM), $(filter $(PLATFORM), arm64 amd64 i86pc loongarch64 mips64 mips64el ppc64 ppc64le riscv64 s390x sparc sparc4v sparc64 x86_64))\n')
   f.write('PLATFORM_SIZE ?= 64\n')
   f.write('else ifeq ($(PLATFORM), $(filter $(PLATFORM), armv7l i386 i686 mips mipsel))\n')
   f.write('PLATFORM_SIZE ?= 32\n')
   f.write('else\n')
   f.write('PLATFORM_SIZE ?= $(shell getconf LONG_BIT)\n')
   f.write('endif\n\n')
   f.write('ifndef PLATFORM_SIZE\n')
@@ -940,29 +940,54 @@
   f.write('endif\n')
   f.write('CC_MTUNE ?= $(CC_MARCH)\n\n')
   f.write('SEC_CFLAGS := -Wformat -Werror=format-security -D_FORTIFY_SOURCE=2 -fstack-protector-strong\n')
   f.write('BASE_CFLAGS := -fpie -fPIC -Wall -Wextra -pedantic -O2 -fwrapv -DGETRANDOM -Werror\n')
   f.write('BASE_CFLAGS+=-DPLATFORM=${PLATFORM} -DPLATFORM_SIZE=${PLATFORM_SIZE}\n')
   f.write('BASE_CFLAGS+=$(SEC_CFLAGS)\n')
   f.write('BASE_CFLAGS+=$(if $(strip $(CC_MARCH)),-march=$(CC_MARCH) -mtune=$(CC_MTUNE),)\n')
-  f.write('LDFLAGS := -s -w\n')
+  f.write('ifeq    ($(HOST_OS), $(filter $(HOST_OS), OpenBSD, DragonFly, Darwin))\n')
+  f.write('BASE_CFLAGS+=-D__$(HOST_OS)__\n')
+  f.write('endif\n')
+  f.write('LDFLAGS :=\n')
   f.write('ifeq ($(HOST_OS),Linux)\n')
   f.write('LDFLAGS+=-Wl,-z,noexecstack -Wl,-z,relro -Wl,-z,now\n')
   f.write('LDFLAGS+=-Wl,-Bsymbolic-functions\n')
   f.write('LDFLAGS+=-Wl,--reduce-memory-overheads -Wl,--no-keep-memory\n')
   f.write('endif\n')
+  f.write('ifeq ($(CC),clang)\n')
+  f.write('BASE_CFLAGS+=-Wno-unused-command-line-argument\n')
+  f.write('endif\n')
+  f.write('ifeq ($(CC),gcc)\n')
+  f.write('BASE_CFLAGS+=\n')
+  f.write('endif\n')
+  f.write('ifeq ($(WINDOWS),1)\n')
+  f.write('BASE_CFLAGS :=-Wall -Wextra -pedantic -O2 -fwrapv -D__Windows__\n')
+  f.write('HIGHCTIDH_PORTABLE ?=1\n')
+  f.write('BASE_CFLAGS+=-DPLATFORM=${PLATFORM} -DPLATFORM_SIZE=${PLATFORM_SIZE}\n')
+  f.write('ifeq ($(CC),x86_64-w64-mingw32-gcc)\n')
+  f.write('BASE_CFLAGS+=-fpie -fPIC\n')
+  f.write('CFLAGS = $(BASE_CFLAGS)\n')
+  f.write('endif\n')
+  f.write('ifeq ($(CC),clang)\n')
+  f.write('HIGHCTIDH_PORTABLE ?=1\n')
+  f.write('BASE_CFLAGS+=-DPLATFORM=${PLATFORM} -DPLATFORM_SIZE=${PLATFORM_SIZE}\n')
+  f.write('CFLAGS = $(BASE_CFLAGS) -Wno-unused-command-line-argument\n')
+  f.write('LDFLAGS = -LAdvapi32.dll\n')
+  f.write('endif\n')
+  f.write('endif\n')
   f.write('# Default to using fiat crypto, safe and portable but slow backend\n')
   f.write('HIGHCTIDH_PORTABLE ?= 1\n')
   f.write('ifeq\t($(HIGHCTIDH_PORTABLE),1)\n')
-  f.write('BASE_CFLAGS += -DHIGHCTIDH_PORTABLE\n')
+  f.write('BASE_CFLAGS += -DHIGHCTIDH_PORTABLE=1\n')
   f.write('\tlibhighctidh_511_OBJS := fp2fiat511.o fiat_p511.o\n')
   f.write('\tlibhighctidh_512_OBJS := fp2fiat512.o fiat_p512.o\n')
   f.write('\tlibhighctidh_1024_OBJS := fp2fiat1024.o fiat_p1024.o\n')
   f.write('\tlibhighctidh_2048_OBJS := fp2fiat2048.o fiat_p2048.o\n')
   f.write('else\n')
+  f.write('BASE_CFLAGS += -DHIGHCTIDH_PORTABLE=0\n')
   f.write('\tlibhighctidh_511_OBJS := uintbig511.o fp511.o\n')
   f.write('\tlibhighctidh_512_OBJS := uintbig512.o fp512.o\n')
   f.write('\tlibhighctidh_1024_OBJS := uintbig1024.o fp1024.o\n')
   f.write('\tlibhighctidh_2048_OBJS := uintbig2048.o fp2048.o\n')
   f.write('endif\n')
   f.write('\n')
   f.write('ifeq\t($(PLATFORM), $(filter $(PLATFORM), arm64 aarch64))\n')
@@ -992,37 +1017,61 @@
   f.write('ifeq\t($(PLATFORM),ppc64le)\n')
   f.write('\tCFLAGS+= $(BASE_CFLAGS)\n')
   f.write('endif\n\n')
   f.write('ifeq\t($(PLATFORM),ppc64)\n')
   f.write('\tCFLAGS+= $(BASE_CFLAGS)\n')
   f.write('endif\n\n')
   f.write('ifeq\t($(PLATFORM),riscv64)\n')
-  f.write('\tCFLAGS+= $(BASE_CFLAGS)\n')
+  f.write('\tCFLAGS+= $(BASE_CFLAGS) -D__riscv\n')
   f.write('endif\n\n')
   f.write('ifeq\t($(PLATFORM),s390x)\n')
   f.write('\tCFLAGS+= $(BASE_CFLAGS) -D__s390x__\n')
   f.write('\tifeq ($(CC),clang)\n')
   f.write('\t\tCFLAGS+= -march=z10 -mtune=z10\n')
   f.write('\tendif\n')
   f.write('endif\n\n')
-  f.write('ifeq\t($(PLATFORM),sparc64)\n')
-  f.write('\tCFLAGS+= $(BASE_CFLAGS)\n')
-  f.write('endif\n\n')
+  f.write('ifeq   ($(HOST_OS), $(filter $(HOST_OS), SunOS))\n')
+  f.write('ifeq   ($(PLATFORM), $(filter $(PLATFORM), sparc sun4u sun4v sparc64 i86pc i386))\n')
+  f.write('\tBASE_CFLAGS+=$(SEC_CFLAGS)\n')
+  f.write('\tCFLAGS+=$(BASE_CFLAGS) -m64 -D__sun\n')
+  f.write('\tLDFLAGS+=$(LDFLAGS)\n')
+  f.write('ifeq   ($(PLATFORM), $(filter $(PLATFORM), i86pc))\n')
+  f.write('\tCFLAGS+=-D__i86pc__\n')
+  f.write('\tifeq ($(CC),gcc)\n')
+  f.write('\t\tCFLAGS+=-mimpure-text -Wno-attributes\n')
+  f.write('\tendif\n')
+  f.write('endif\n')
+  f.write('ifeq   ($(PLATFORM), $(filter $(PLATFORM), i386))\n')
+  f.write('\tCFLAGS+=-D__i386__\n')
+  f.write('\tifeq ($(CC),gcc)\n')
+  f.write('\t\tCFLAGS+=-mimpure-text\n')
+  f.write('\tendif\n')
+  f.write('endif\n')
+  f.write('ifeq   ($(PLATFORM), $(filter $(PLATFORM), sparc sun4u sun4v sparc64))\n')
+  f.write('\tCFLAGS+=-DHIGHCTIDH_PORTABLE=1 -D__sun4v__\n')
+  f.write('\tifeq ($(CC),gcc)\n')
+  f.write('\t\tCFLAGS+=-mcpu=native -mtune=native -D_REENTRANT\n')
+  f.write('\tendif\n')
+  f.write('endif\n')
+  f.write('endif\n')
+  f.write('endif\n')
   f.write('ifeq\t($(PLATFORM),unknown)\n')
   f.write('\tCFLAGS+= $(BASE_CFLAGS)\n')
   f.write('endif\n\n')
+  f.write('ifneq\t($(HOST_OS), $(filter $(HOST_OS), SunOS))\n')
   f.write('ifeq\t($(PLATFORM), $(filter $(PLATFORM), amd64 x86_64 i386 i686))\n')
   f.write('ifeq\t($(PLATFORM_SIZE),32)\n')
   f.write('\tCFLAGS+= $(BASE_CFLAGS) -D__i386__\n')
   f.write('\tifeq ($(CC),clang)\n')
   f.write('\t\tCFLAGS+= -fforce-enable-int128\n')
   f.write('\tendif\n')
   f.write('else\n\n')
   f.write('\tCFLAGS+= $(BASE_CFLAGS) -D__x86_64__\n\n')
   f.write('endif\n')
+  f.write('endif\n')
   f.write('endif\n\n')
   f.write('SCC ?= $(CC) $(CFLAGS) $(LDFLAGS)\n')
   f.write('CC += $(CFLAGS) $(LDFLAGS)\n')
   f.write('\n')
   f.write('default: libhighctidh.so\n')
   f.write('\n')
   f.write('all: default timecop generic %s\n' % ' '.join('%d'%bits for bits in databits))
@@ -1296,44 +1345,49 @@
       f.write('\t\t$(SCC) -DBITS={0} -D\'NAMESPACEBITS(x)=highctidh_{0}_##x\' -D\'NAMESPACEGENERIC(x)=highctidh_##x\' -shared -o libhighctidh_{0}.so $(libhighctidh_{0}_OBJS) fp_inv{0}.o fp_sqrt{0}.o primes{0}.o poly{0}.o mont{0}.o elligator{0}.o skgen{0}.o validate{0}.o steps.o random.o crypto_classify.o crypto_declassify.o randombytes.o int32_sort.o  steps_untuned.o csidh{0}.o\n'.format(bits))
       f.write('\n\ntest{0}-dyn: test{0} libhighctidh_{0}.so\n'.format(bits))
       f.write('\t\t$(CC) -DBITS={0} -D\'NAMESPACEBITS(x)=highctidh_{0}_##x\' -D\'NAMESPACEGENERIC(x)=highctidh_##x\' -o test{0}-dyn test.c -l highctidh_{0} -L .\n'.format(bits))
 
   f.write('\n\nlibhighctidh.so: libhighctidh_511.so libhighctidh_512.so libhighctidh_1024.so libhighctidh_2048.so\n')
   f.write('\t\tls -l libhighctidh_*.so\n\n')
 
+  f.write('setup-examples: csidh.h\n')
+  f.write('\t\t-mkdir -p libhighctidh\n')
+  f.write('\t\t-cp csidh.h libhighctidh/\n\n')
   for bits in databits:
-      f.write('example{0}: libhighctidh_{0}.so\n'.format(bits))
+      f.write('example{0}: setup-examples libhighctidh_{0}.so\n'.format(bits))
       f.write('\t$(CC) -DBITS={0} -D\'NAMESPACEBITS(x)=highctidh_{0}_##x\' \\\n'.format(bits))
       f.write('\t-D\'NAMESPACEGENERIC(x)=highctidh_##x\' -o example-ctidh{0} example-ctidh.c \\\n'.format(bits))
-      f.write('\t-l highctidh_{0}\n\n'.format(bits))
+      f.write('\t-L. -I. -l highctidh_{0}\n\n'.format(bits))
 
   f.write('examples: example511 example512 example1024 example2048\n')
   f.write('\t\tls -l example-ctidh511 example-ctidh512 example-ctidh1024 example-ctidh2048\n\n')
 
   f.write('examples-static: examples_static.c libhighctidh.a *.h\n')
-  f.write('\t$(CC) -static -Wall -Werror -Wpedantic examples_static.c -Wl,-Bstatic -L. -l:libhighctidh.a -o examples-static\n')
+  f.write('\t$(CC) -static -Wall -Werror -Wpedantic examples_static.c -Wl,-Bstatic -L. -l:libhighctidh.a -o examples-static\n\n')
 
   f.write('test: clean libhighctidh.so testrandom test511 test512 test1024 test2048\n')
   f.write('\t\t./test.sh\n\n')
 
   f.write('DESTDIR ?= /usr/local\n')
   f.write('install: libhighctidh.so libhighctidh.a\n')
   f.write('\t\tinstall -d $(DESTDIR)/include/libhighctidh/\n')
   f.write('\t\tinstall -d $(DESTDIR)/lib/\n')
   f.write('\t\tinstall -v *.h $(DESTDIR)/include/libhighctidh/\n')
   f.write('\t\tinstall -v libhighctidh_*.so $(DESTDIR)/lib/\n')
   f.write('\t\tinstall -v libhighctidh.a $(DESTDIR)/lib/\n')
 
   f.write('\n\nclean:\n')
   f.write('\t\t-rm -f *.a *.o *.out *.so\n')
+  f.write('\t\t-rm -f *.s *.bc\n')
   f.write('\t\t-rm -f bench1024cycles bench1024mults bench1024untuned bench2048cycles bench2048mults bench2048untuned bench511cycles bench511mults bench511untuned bench512cycles bench512mults bench512untuned\n')
   f.write('\t\t-rm -f checkct1024cycles checkct1024mults checkct1024untuned checkct2048cycles checkct2048mults checkct2048untuned checkct511cycles checkct511mults checkct511untuned checkct512cycles checkct512mults checkct512untuned costpoly1024 costpoly2048 costpoly511 example-ctidh1024 example-ctidh2048\n')
   f.write('\t\t-rm -f example-ctidh511 example-ctidh512 test1024 test2048 test511 test511 test512 test512-dyn test*-dyn testrandom tunecycles1024 tunecycles2048 tunecycles511 tunecycles512 tunemults1024 tunemults2048 tunemults511 tunemults512 ubench1024 ubench2048 ubench511 ubench512 umults1024 umults2048 umults511 umults512\n')
   f.write('\t\t-rm -rf UNKNOWN.egg-info/ __pycache__/\n')
   f.write('\t\t-rm -rf build/ deb_dist/ dist/\n')
   f.write('\t\t-rm -rf highctidh.egg-info/ highctidh/__pycache__/\n')
   f.write('\t\t-rm -rf tests/__pycache__/\n')
   f.write('\t\t-rm -rf docker_build_output/\n')
+  f.write('\t\t-rm -rf libhighctidh/\n')
   f.write('\t\t-rm -rf examples-static\n')
   f.write('\t\t-rm -rf highctidh-*.tar.gz\n')
 
 maybeupdate(fn)
```

### Comparing `highctidh-1.0.2024012400/bench.c` & `highctidh-1.0.2024050100/bench.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/chain.py` & `highctidh-1.0.2024050100/chain.py`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/checkct.c` & `highctidh-1.0.2024050100/checkct.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/costisog.py` & `highctidh-1.0.2024050100/costisog.py`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/costpoly.c` & `highctidh-1.0.2024050100/costpoly.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/costpoly.py` & `highctidh-1.0.2024050100/costpoly.py`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/costs.py` & `highctidh-1.0.2024050100/costs.py`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/csidh.c` & `highctidh-1.0.2024050100/csidh.c`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,20 @@
  * big-endian portability.
  */
 void
 public_key_from_bytes(public_key *const pk, const char *const input)
 {
 	uint64_t *input_u64 = (uint64_t *)input;
 	for(size_t i=0; i < sizeof(pk->A.x.c)/sizeof(pk->A.x.c[0]); i++){
-		pk->A.x.c[i] = le64toh(*input_u64++);
+    // We could write this as so on GNU/Linux, BSD, and MacOS
+		// pk->A.x.c[i] = le64toh(*input_u64++);
+    // however on Solaris 11.4 sparcv9 64bit it throws a hard error of
+    // 'multiple unsequenced modifications'
+		pk->A.x.c[i] = le64toh(*input_u64);
+    input_u64++;
 	}
 }
 
 void
 public_key_to_bytes(char *const output, const public_key *const pk)
 {
 	uint64_t *output_u64 = (uint64_t *)output;
```

### Comparing `highctidh-1.0.2024012400/csidh.h` & `highctidh-1.0.2024050100/csidh.h`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #ifndef CSIDH_H
 #define CSIDH_H
 
 #ifdef CGONUTS
 #include "cgo.h"
 #endif // CGONUTS
 
+#include "naidne.h"
 #include "uintbig.h"
 #include "fp.h"
 #include "mont.h"
 #include "primes.h"
 #include "csidh_namespace.h"
 
 extern long long csidh_stattried[primes_batches];
```

### Comparing `highctidh-1.0.2024012400/csidh_all_clearnamespaces.h` & `highctidh-1.0.2024050100/csidh_all_clearnamespaces.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/csidh_namespace.h` & `highctidh-1.0.2024050100/csidh_namespace.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh1024/common.go` & `highctidh-1.0.2024050100/ctidh1024/common.go`

 * *Files 19% similar despite different names*

```diff
@@ -1,63 +1,85 @@
 package ctidh1024
 
 /*
- #cgo CFLAGS: -DBITS=1024 -DGETRANDOM -DCGONUTS -Wformat -Werror=format-security -D_FORTIFY_SOURCE=2 -fstack-protector-all -fpie -fPIC -O2
- #cgo LDFLAGS: -Wl,-z,noexecstack -Wl,-z,relro
+ #cgo CFLAGS: -DBITS=1024 -DGETRANDOM -DCGONUTS -O2
+ #cgo LDFLAGS:
+ #cgo linux CFLAGS: -DBITS=1024 -DGETRANDOM -DCGONUTS -Wformat -Werror=format-security -D_FORTIFY_SOURCE=2 -fstack-protector-all -fpie -fPIC -O2
+ #cgo linux LDFLAGS: -Wl,-z,noexecstack -Wl,-z,relro
+ #cgo windows CFLAGS: -D__Windows__ -DHIGHCTIDH_PORTABLE=1
 
  // The following should work as native builds and as cross compiled builds.
  // Example cross compile build lines are provided as examples.
 
  // CC=aarch64-linux-gnu-gcc CGO_ENABLED=1 GOOS=linux GOARCH=arm64 go build -v
- #cgo arm64 CFLAGS: -DPLATFORM=aarch64 -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE
+ #cgo arm64 CFLAGS: -DPLATFORM=aarch64 -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE=1
+
+ // CC=clang CGO_ENABLED=1 GOOS=darwin GOARCH=arm64 go build -v
+ #cgo darwin/arm64 CFLAGS: -DPLATFORM=aarch64 -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE=1
 
  // export CGO_CFLAGS_ALLOW="-fforce-enable-int128";
  // CC=clang CGO_ENABLED=1 GOOS=linux GOARCH=arm ARMVER=7  go build
- #cgo arm CFLAGS: -DPLATFORM=arm -DPLATFORM_SIZE=32 -D__ARM32__ -DHIGHCTIDH_PORTABLE
+ #cgo arm CFLAGS: -DPLATFORM=arm -DPLATFORM_SIZE=32 -D__ARM32__ -DHIGHCTIDH_PORTABLE=1
+
+ // CC=clang CGO_ENABLED=1 GOOS=darwin GOARCH=amd64 go build -v
+ #cgo darwin/amd64 CFLAGS: -DPLATFORM=x86_64 -DPLATFORM_SIZE=64 -march=native -mtune=native -DHIGHCTIDH_PORTABLE=1
+
+ // Generic flags for amd64
+ #cgo linux/amd64 CFLAGS: -DPLATFORM=x86_64 -DPLATFORM_SIZE=64
 
  // CC=gcc CGO_ENABLED=1 GOOS=linux GOARCH=amd64 go build -v
- #cgo amd64 CFLAGS: -DPLATFORM=x86_64 -DPLATFORM_SIZE=64 -march=native -mtune=native
+ #cgo linux/amd64 CFLAGS: -DPLATFORM=x86_64 -DPLATFORM_SIZE=64 -march=native -mtune=native
+
+ // CC=??? CGO_ENABLED=1 GOOS=windows GOARCH=arm64 go build
+ #cgo windows/arm64 CFLAGS: -DPLATFORM=arm64 -DPLATFORM_SIZE=64 -D__Windows__ -DHIGHCTIDH_PORTABLE=1
+
+ // CC=/usr/bin/x86_64-w64-mingw32-gcc CGO_ENABLED=1 GOOS=windows GOARCH=amd64 go build
+ #cgo windows/amd64 CFLAGS: -DPLATFORM=x86_64 -DPLATFORM_SIZE=64 -D__Windows__ -DHIGHCTIDH_PORTABLE=1
 
  // CC=powerpc64le-linux-gnu-gcc CGO_ENABLED=1 GOOS=linux GOARCH=ppc64le go build -v
- #cgo ppc64le CFLAGS: -DPLATFORM=ppc64le -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE
+ #cgo ppc64le CFLAGS: -DPLATFORM=ppc64le -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE=1
 
  // CC=powerpc64-linux-gnu-gcc CGO_ENABLED=1 GOOS=linux GOARCH=ppc64 go build -v
- #cgo ppc64 CFLAGS: -DPLATFORM=ppc64 -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE
+ #cgo ppc64 CFLAGS: -DPLATFORM=ppc64 -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE=1
 
  // CC=riscv64-linux-gnu-gcc CGO_ENABLED=1 GOOS=linux GOARCH=riscv64 go build -v
- #cgo riscv64 CFLAGS: -DPLATFORM=riscv64 -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE
+ #cgo riscv64 CFLAGS: -DPLATFORM=riscv64 -D__riscv -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE=1
+
+ // CC=gcc CGO_ENABLED=1 GOOS=solaris GOARCH=amd64 go build
+ #cgo solaris/amd64 CFLAGS: -m64 -mimpure-text -Wno-attributes -DPLATFORM=i86pc -DPLATFORM_SIZE=64 -D__sun -D__i86pc__ -DHIGHCTIDH_PORTABLE=0
+
+ // CC=gcc CGO_ENABLED=1 GOOS=solaris GOARCH=sparc64 go build
+ #cgo solaris/sparc64 CFLAGS: -m64 -DPLATFORM=sun4v -DPLATFORM_SIZE=64 -D__sun -DHIGHCTIDH_PORTABLE=1
 
  // CC=s390x-linux-gnu-gcc CGO_ENABLED=1 GOOS=linux GOARCH=s390x go build -v
- #cgo s390x CFLAGS: -DPLATFORM=s390x -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE
+ #cgo s390x CFLAGS: -DPLATFORM=s390x -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE=1
 
  // CC=mips64-linux-gnuabi64-gcc CGO_ENABLED=1 GOOS=linux GOARCH=mips64  go build
  // With clang, -fforce-enable-int128 must be added to the CFLAGS
- #cgo mips64 CFLAGS: -DPLATFORM=mips64 -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE
+ #cgo mips64 CFLAGS: -DPLATFORM=mips64 -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE=1
 
  // CC=mips64-linux-gnuabi64-gcc CGO_ENABLED=1 GOOS=linux GOARCH=mips64  go build
  // With clang, -fforce-enable-int128 must be added to the CFLAGS
- #cgo mips64le CFLAGS: -DPLATFORM=mips64le -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE
+ #cgo mips64le CFLAGS: -DPLATFORM=mips64le -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE=1
 
  // CC=mipsel-linux-gnu-gcc CGO_ENABLED=1 GOOS=linux GOARCH=mipsle  go build
  // With clang, -fforce-enable-int128 must be added to the CFLAGS
- #cgo mipsle CFLAGS: -DPLATFORM=mipsle -DPLATFORM_SIZE=32 -DHIGHCTIDH_PORTABLE
+ #cgo mipsle CFLAGS: -DPLATFORM=mipsle -DPLATFORM_SIZE=32 -DHIGHCTIDH_PORTABLE=1
 
  // CC=mips-linux-gnu-gcc CGO_ENABLED=1 GOOS=linux GOARCH=mips  go build
  // With clang, -fforce-enable-int128 must be added to the CFLAGS
- #cgo mips CFLAGS: -DPLATFORM=mips -DPLATFORM_SIZE=32 -DHIGHCTIDH_PORTABLE
+ #cgo mips CFLAGS: -DPLATFORM=mips -DPLATFORM_SIZE=32 -DHIGHCTIDH_PORTABLE=1
 
  // export CGO_CFLAGS_ALLOW="-fforce-enable-int128";
  // CC=clang CGO_ENABLED=1 GOOS=linux GOARCH=386  go build
- #cgo 386 CFLAGS: -DPLATFORM=i386 -DPLATFORM_SIZE=32 -fforce-enable-int128 -D__i386__ -DHIGHCTIDH_PORTABLE
+ #cgo 386 CFLAGS: -DPLATFORM=i386 -DPLATFORM_SIZE=32 -fforce-enable-int128 -D__i386__ -DHIGHCTIDH_PORTABLE=1
 
  // The following should work as native builds with clang:
 
- #cgo loong64 CFLAGS: -DPLATFORM=loongarch64 -DPLATFORM_SIZE=64 -march=native -mtune=native -DHIGHCTIDH_PORTABLE
-
- #cgo sparc64 CFLAGS: -DPLATFORM=sparc64 -DPLATFORM_SIZE=64 -march=native -mtune=native -DHIGHCTIDH_PORTABLE
+ #cgo loong64 CFLAGS: -DPLATFORM=loongarch64 -DPLATFORM_SIZE=64 -march=native -mtune=native -DHIGHCTIDH_PORTABLE=1
 
  #include "binding1024.h"
 */
 import "C"
 import (
 	"fmt"
 	"io"
```

### Comparing `highctidh-1.0.2024012400/ctidh1024/common_test.go` & `highctidh-1.0.2024050100/ctidh1024/common_test.go`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh1024/csidh.c` & `highctidh-1.0.2024050100/ctidh1024/csidh.c`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,20 @@
  * big-endian portability.
  */
 void
 public_key_from_bytes(public_key *const pk, const char *const input)
 {
 	uint64_t *input_u64 = (uint64_t *)input;
 	for(size_t i=0; i < sizeof(pk->A.x.c)/sizeof(pk->A.x.c[0]); i++){
-		pk->A.x.c[i] = le64toh(*input_u64++);
+    // We could write this as so on GNU/Linux, BSD, and MacOS
+		// pk->A.x.c[i] = le64toh(*input_u64++);
+    // however on Solaris 11.4 sparcv9 64bit it throws a hard error of
+    // 'multiple unsequenced modifications'
+		pk->A.x.c[i] = le64toh(*input_u64);
+    input_u64++;
 	}
 }
 
 void
 public_key_to_bytes(char *const output, const public_key *const pk)
 {
 	uint64_t *output_u64 = (uint64_t *)output;
```

### Comparing `highctidh-1.0.2024012400/ctidh1024/csidh.h` & `highctidh-1.0.2024050100/ctidh1024/csidh.h`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #ifndef CSIDH_H
 #define CSIDH_H
 
 #ifdef CGONUTS
 #include "cgo.h"
 #endif // CGONUTS
 
+#include "naidne.h"
 #include "uintbig.h"
 #include "fp.h"
 #include "mont.h"
 #include "primes.h"
 #include "csidh_namespace.h"
 
 extern long long csidh_stattried[primes_batches];
```

### Comparing `highctidh-1.0.2024012400/ctidh1024/csidh_namespace.h` & `highctidh-1.0.2024050100/ctidh1024/csidh_namespace.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh1024/ctidh1024.go` & `highctidh-1.0.2024050100/ctidh1024/ctidh1024.go`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh1024/ctidh1024_bench_test.go` & `highctidh-1.0.2024050100/ctidh1024/ctidh1024_bench_test.go`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh1024/ctidh1024_test.go` & `highctidh-1.0.2024050100/ctidh1024/ctidh1024_test.go`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh1024/elligator.c` & `highctidh-1.0.2024050100/ctidh1024/elligator.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh1024/error.go` & `highctidh-1.0.2024050100/ctidh1024/error.go`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh1024/fiat_p1024.c` & `highctidh-1.0.2024050100/ctidh1024/fiat_p1024.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#if defined(HIGHCTIDH_PORTABLE)
+#if HIGHCTIDH_PORTABLE == 1
 #include "fiat_p1024.h"
 /* Autogenerated: './src/ExtractionOCaml/word_by_word_montgomery' --widen-bytes --internal-static --lang C -o f_1024.c p1024 64 10397125823368453045280646945602587680645373501407971524723936453540081402468763489237207685909470852314300607054838964876369377755966328162572638385477152807267330439309520268717606043270205686916407950751430775965737505772592082230763227336919124289210653129066316362633007647060631513541162047451995268179 */
 /* curve description: p1024 */
 /* machine_wordsize = 64 (from "64") */
 /* requested operations: (all) */
 /* m = 0xece55ed427012a9d89dec879007ebd7216c22bc86f21a080683cf25db31ad5bf06de2471cf9386e4d6c594a8ad82d2df811d9c419ec83297611ad4f90441c800978dbeed90a2b58b97c56d1de81ede56b317c5431541f40642aca4d5a313709c2cab6a0e287f1bd514ba72cb8d89fd3a1d81eebbc3d344ddbe34c5460e36453 (from "10397125823368453045280646945602587680645373501407971524723936453540081402468763489237207685909470852314300607054838964876369377755966328162572638385477152807267330439309520268717606043270205686916407950751430775965737505772592082230763227336919124289210653129066316362633007647060631513541162047451995268179") */
 /*                                                                    */
@@ -20039,8 +20039,10 @@
   out5[10] = x433;
   out5[11] = x434;
   out5[12] = x435;
   out5[13] = x436;
   out5[14] = x437;
   out5[15] = x438;
 }
+#else
+typedef int no_empty_translation_units_asm_1024; // -> "warning: ISO C forbids an empty translation unit"
 #endif
```

### Comparing `highctidh-1.0.2024012400/ctidh1024/fiat_p1024.h` & `highctidh-1.0.2024050100/ctidh1024/fiat_p1024.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh1024/fp.h` & `highctidh-1.0.2024050100/ctidh1024/fp.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 #ifndef FP_H
 #define FP_H
 
 #include "fp_namespace.h"
 #include "uintbig.h"
 #include "annotations.h"
 
-#if defined(HIGHCTIDH_PORTABLE) || !(defined(__x86_64__) || defined(_M_X64))
+#if HIGHCTIDH_PORTABLE == 1 || !(defined(__x86_64__) || defined(_M_X64))
 /* we only have optimizations for amd64 so far, so on other platforms we
  * default to the portable code by defining HIGHCTIDH_PORTABLE:
  */
 #ifndef HIGHCTIDH_PORTABLE
-#define HIGHCTIDH_PORTABLE
+#define HIGHCTIDH_PORTABLE 1
 #endif
 
 #if 511 == BITS
 #include "fiat_p511.h"
 #elif 512 == BITS
 #include "fiat_p512.h"
 #elif 1024 == BITS
@@ -72,20 +72,22 @@
 void ATTR_INITIALIZE_1st
 __attribute__((nonnull))
 __attribute__((flatten))
 fp_mul3(fp *const x, fp const *const y, fp const *const z)
 	__attribute__ ((alias ("fiat_p512_mul")));
 */
 //void fp_mul3 () __attribute__ ((weak, alias ("fiat_p512_mul")));
-#ifdef HIGHCTIDH_PORTABLE
+#if HIGHCTIDH_PORTABLE == 1
 #define highctidh_511_fp_mul3(a,b,c) FIAT_BITS(mul)((uint64_t *)a,(const uint64_t*)b,(const uint64_t*)c)
 #define highctidh_512_fp_mul3(a,b,c) FIAT_BITS(mul)((uint64_t *)a,(const uint64_t*)b,(const uint64_t*)c)
 #define highctidh_1024_fp_mul3(a,b,c) FIAT_BITS(mul)((uint64_t *)a,(const uint64_t*)b,(const uint64_t*)c)
 #define highctidh_2048_fp_mul3(a,b,c) FIAT_BITS(mul)((uint64_t *)a,(const uint64_t*)b,(const uint64_t*)c)
-#else /* ndef HIGHCTIDH_PORTABLE */
+#endif
+
+#if HIGHCTIDH_PORTABLE == 0
 void fp_mul3(fp *const a, const fp *const b, const fp *const c);
 #endif /* ndef HIGHCTIDH_PORTABLE */
 
 void fp_sq1(fp *x);
 void fp_sq2(fp *const x, fp const *const y);
 
 extern long long fp_mulsq_count;
@@ -108,15 +110,15 @@
 /*
  * a := 0 - b
  */
 static inline
 __attribute__((nonnull))
 void fp_neg2(fp *const x,const fp *const y)
 {
-#ifdef HIGHCTIDH_PORTABLE
+#if HIGHCTIDH_PORTABLE == 1
 	FIAT_BITS(opp)(x->x.c, y->x.c);
 #else
 	fp_sub3(x, &fp_0, y);
 #endif
 }
 
 static inline void fp_double1(fp *const x)
```

### Comparing `highctidh-1.0.2024012400/ctidh1024/fp1024.S` & `highctidh-1.0.2024050100/ctidh1024/fp1024.S`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /* DO NOT EDIT! generated by ./autogen */
-#ifndef HIGHCTIDH_PORTABLE
+#if HIGHCTIDH_PORTABLE == 0
 
 .intel_syntax noprefix
 
 //#include "uintbig_namespace.h"
 //#include "fp_namespace.h"
 
 .section .rodata
```

### Comparing `highctidh-1.0.2024012400/ctidh1024/fp2fiat.c` & `highctidh-1.0.2024050100/ctidh1024/fp2fiat.c`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #include <string.h>
 
 
 #include "uintbig_namespace.h"
 #include "fp.h"
 #include "annotations.h"
 
-#if !defined(HIGHCTIDH_PORTABLE) && !defined(CGONUTS) && defined(__x86_64__)
+#if HIGHCTIDH_PORTABLE == 0 && !defined(CGONUTS) && (defined(__x86_64__) || defined(__i86pc__))
 #define highctidh_macro_stringize(x) #x
 #define highctidh_macro_str(y) highctidh_macro_stringize(y)
 __asm__ (".include \"uintbig" highctidh_macro_str(BITS)  ".S\"");
 __asm__ (".include \"fp" highctidh_macro_str(BITS) ".S\"");
 
 #elif defined(CGONUTS)
 #define DONTMINDIFIDO
```

### Comparing `highctidh-1.0.2024012400/ctidh1024/fp_inv1024.c` & `highctidh-1.0.2024050100/ctidh1024/fp_inv1024.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh1024/fp_namespace.h` & `highctidh-1.0.2024050100/ctidh1024/fp_namespace.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh1024/fp_sqrt1024.c` & `highctidh-1.0.2024050100/ctidh1024/fp_sqrt1024.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh1024/int32_minmax.h` & `highctidh-1.0.2024050100/ctidh1024/int32_minmax.h`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 // This is from the Public Domain djbsort-20190516
 /* this needs __attribute__((optimize)) >= 1 */
 
 #ifndef HIGHCTIDH_INT32_MINMAX_H
 #define HIGHCTIDH_INT32_MINMAX_H
 
-#if defined(__x86_64__) && !defined(HIGHCTIDH_PORTABLE)
+#if ((defined(__x86_64__) || defined(__i86pc__))) && HIGHCTIDH_PORTABLE == 0
 
 #define int32_MINMAX(a,b)			\
 do { \
   int32 temp1; \
   __asm__( \
     ".att_syntax prefix\n\t" \
     "cmpl %1,%0\n\t" \
```

### Comparing `highctidh-1.0.2024012400/ctidh1024/int32_sort.c` & `highctidh-1.0.2024050100/ctidh1024/int32_sort.c`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #ifndef HIGHCTIDH_INT32_SORT_H
 #define HIGHCTIDH_INT32_SORT_H
 
-#if defined(__AVX2__) && !defined(HIGHCTIDH_PORTABLE)
+#if defined(__AVX2__) && HIGHCTIDH_PORTABLE == 0
 
 // This is the original high-ctidh x86_64 sorting code
 #ifndef CGONUTS
 #include "int32_sort_x86.c"
 #endif // CGONUTS
 
 #else /* fallback to portable C code: */
```

### Comparing `highctidh-1.0.2024012400/ctidh1024/int32_sort.h` & `highctidh-1.0.2024050100/ctidh1024/int32_sort.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh1024/int32_sort_x86.c` & `highctidh-1.0.2024050100/ctidh1024/int32_sort_x86.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-#ifndef HIGHCTIDH_PORTABLE
-#ifdef __x86_64__
+#if HIGHCTIDH_PORTABLE == 0
+#if (defined(__x86_64__) || defined(__i86pc__)) && !defined(CGONUTS)
 #include "int32_sort.h"
 #define int32 int32_t
 
 #include <immintrin.h>
 #include "int32_minmax.h"
 
 typedef __m256i int32x8;
```

### Comparing `highctidh-1.0.2024012400/ctidh1024/mont.c` & `highctidh-1.0.2024050100/ctidh1024/mont.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh1024/mont.h` & `highctidh-1.0.2024050100/ctidh1024/mont.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh1024/mont_namespace.h` & `highctidh-1.0.2024050100/ctidh1024/mont_namespace.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh1024/poly.c` & `highctidh-1.0.2024050100/ctidh1024/poly.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh1024/poly.h` & `highctidh-1.0.2024050100/ctidh1024/poly.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh1024/poly_namespace.h` & `highctidh-1.0.2024050100/ctidh1024/poly_namespace.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh1024/primes.h` & `highctidh-1.0.2024050100/ctidh1024/primes.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh1024/primes1024.c` & `highctidh-1.0.2024050100/ctidh1024/primes1024.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh1024/proj.h` & `highctidh-1.0.2024050100/ctidh1024/proj.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh1024/random.c` & `highctidh-1.0.2024050100/ctidh1024/random.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh1024/random.h` & `highctidh-1.0.2024050100/ctidh1024/random.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh1024/skgen.c` & `highctidh-1.0.2024050100/ctidh1024/skgen.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh1024/steps.c` & `highctidh-1.0.2024050100/ctidh1024/steps.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh1024/steps.h` & `highctidh-1.0.2024050100/ctidh1024/steps.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh1024/uintbig.h` & `highctidh-1.0.2024050100/ctidh1024/uintbig.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-#ifndef uintbig_h
-#define uintbig_h
+#ifndef UINTBIG_H
+#define UINTBIG_H
 
 #include "uintbig_namespace.h"
 
 #include <stdbool.h>
 #include <stdint.h>
 #include "annotations.h"
```

### Comparing `highctidh-1.0.2024012400/ctidh1024/uintbig1024.S` & `highctidh-1.0.2024050100/ctidh1024/uintbig1024.S`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /* DO NOT EDIT! generated by ./autogen */
-#ifndef HIGHCTIDH_PORTABLE
+#if HIGHCTIDH_PORTABLE == 0
 
 .intel_syntax noprefix
 
 //#include "uintbig_namespace.h"
 
 .section .rodata
```

### Comparing `highctidh-1.0.2024012400/ctidh1024/uintbig_namespace.h` & `highctidh-1.0.2024050100/ctidh1024/uintbig_namespace.h`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+#ifndef UINTBIG_NAMESPACE_H
+#define UINTBIG_NAMESPACE_H
+
 #ifdef CGONUTS
 #include "cgo.h"
 #endif // CGONUTS
 
 #define uintbig_p NAMESPACEBITS(uintbig_p)
 #define uintbig_1 NAMESPACEBITS(uintbig_1)
 #define uintbig_bit NAMESPACEBITS(uintbig_bit)
@@ -12,7 +15,9 @@
 #define uintbig_mul3_64 NAMESPACEBITS(uintbig_mul3_64)
 #define uintbig_four_sqrt_p NAMESPACEBITS(uintbig_four_sqrt_p)
 #define uintbig NAMESPACEBITS(uintbig)
 #define uintbig_bits_vartime NAMESPACEBITS(uintbig_bits_vartime)
 #define uintbig_uint64_iszero NAMESPACEBITS(uintbig_uint64_iszero)
 #define uintbig_isequal NAMESPACEBITS(uintbig_isequal)
 #define uintbig_iszero NAMESPACEBITS(uintbig_iszero)
+
+#endif
```

### Comparing `highctidh-1.0.2024012400/ctidh1024/validate.c` & `highctidh-1.0.2024050100/ctidh1024/validate.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh1024/vectors1024_test.go` & `highctidh-1.0.2024050100/ctidh1024/vectors1024_test.go`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh2048/common.go` & `highctidh-1.0.2024050100/ctidh2048/common.go`

 * *Files 22% similar despite different names*

```diff
@@ -1,63 +1,85 @@
 package ctidh2048
 
 /*
- #cgo CFLAGS: -DBITS=2048 -DGETRANDOM -DCGONUTS -Wformat -Werror=format-security -D_FORTIFY_SOURCE=2 -fstack-protector-all -fpie -fPIC -O2
- #cgo LDFLAGS: -Wl,-z,noexecstack -Wl,-z,relro
+ #cgo CFLAGS: -DBITS=2048 -DGETRANDOM -DCGONUTS -O2
+ #cgo LDFLAGS:
+ #cgo linux CFLAGS: -DBITS=2048 -DGETRANDOM -DCGONUTS -Wformat -Werror=format-security -D_FORTIFY_SOURCE=2 -fstack-protector-all -fpie -fPIC -O2
+ #cgo linux LDFLAGS: -Wl,-z,noexecstack -Wl,-z,relro
+ #cgo windows CFLAGS: -D__Windows__ -DHIGHCTIDH_PORTABLE=1
 
  // The following should work as native builds and as cross compiled builds.
  // Example cross compile build lines are provided as examples.
 
  // CC=aarch64-linux-gnu-gcc CGO_ENABLED=1 GOOS=linux GOARCH=arm64 go build -v
- #cgo arm64 CFLAGS: -DPLATFORM=aarch64 -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE
+ #cgo arm64 CFLAGS: -DPLATFORM=aarch64 -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE=1
+
+ // CC=clang CGO_ENABLED=1 GOOS=darwin GOARCH=arm64 go build -v
+ #cgo darwin/arm64 CFLAGS: -DPLATFORM=aarch64 -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE=1
 
  // export CGO_CFLAGS_ALLOW="-fforce-enable-int128";
  // CC=clang CGO_ENABLED=1 GOOS=linux GOARCH=arm ARMVER=7  go build
- #cgo arm CFLAGS: -DPLATFORM=arm -DPLATFORM_SIZE=32 -D__ARM32__ -DHIGHCTIDH_PORTABLE
+ #cgo arm CFLAGS: -DPLATFORM=arm -DPLATFORM_SIZE=32 -D__ARM32__ -DHIGHCTIDH_PORTABLE=1
+
+ // CC=clang CGO_ENABLED=1 GOOS=darwin GOARCH=amd64 go build -v
+ #cgo darwin/amd64 CFLAGS: -DPLATFORM=x86_64 -DPLATFORM_SIZE=64 -march=native -mtune=native -DHIGHCTIDH_PORTABLE=1
+
+ // Generic flags for amd64 
+ #cgo linux/amd64 CFLAGS: -DPLATFORM=x86_64 -DPLATFORM_SIZE=64
 
  // CC=gcc CGO_ENABLED=1 GOOS=linux GOARCH=amd64 go build -v
- #cgo amd64 CFLAGS: -DPLATFORM=x86_64 -DPLATFORM_SIZE=64 -march=native -mtune=native
+ #cgo linux/amd64 CFLAGS: -DPLATFORM=x86_64 -DPLATFORM_SIZE=64 -march=native -mtune=native
+
+ // CC=??? CGO_ENABLED=1 GOOS=windows GOARCH=arm64 go build
+ #cgo windows/arm64 CFLAGS: -DPLATFORM=arm64 -DPLATFORM_SIZE=64 -D__Windows__ -DHIGHCTIDH_PORTABLE=1
+
+ // CC=/usr/bin/x86_64-w64-mingw32-gcc CGO_ENABLED=1 GOOS=windows GOARCH=amd64 go build
+ #cgo windows/amd64 CFLAGS: -DPLATFORM=x86_64 -DPLATFORM_SIZE=64 -D__Windows__ -DHIGHCTIDH_PORTABLE=1
 
  // CC=powerpc64le-linux-gnu-gcc CGO_ENABLED=1 GOOS=linux GOARCH=ppc64le go build -v
- #cgo ppc64le CFLAGS: -DPLATFORM=ppc64le -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE
+ #cgo ppc64le CFLAGS: -DPLATFORM=ppc64le -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE=1
 
  // CC=powerpc64-linux-gnu-gcc CGO_ENABLED=1 GOOS=linux GOARCH=ppc64 go build -v
- #cgo ppc64 CFLAGS: -DPLATFORM=ppc64 -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE
+ #cgo ppc64 CFLAGS: -DPLATFORM=ppc64 -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE=1
 
  // CC=riscv64-linux-gnu-gcc CGO_ENABLED=1 GOOS=linux GOARCH=riscv64 go build -v
- #cgo riscv64 CFLAGS: -DPLATFORM=riscv64 -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE
+ #cgo riscv64 CFLAGS: -DPLATFORM=riscv64 -D__riscv -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE=1
+
+ // CC=gcc CGO_ENABLED=1 GOOS=solaris GOARCH=amd64 go build
+ #cgo solaris/amd64 CFLAGS: -m64 -mimpure-text -Wno-attributes -DPLATFORM=i86pc -DPLATFORM_SIZE=64 -D__sun -D__i86pc__ -DHIGHCTIDH_PORTABLE=0
+
+ // CC=gcc CGO_ENABLED=1 GOOS=solaris GOARCH=sparc64 go build
+ #cgo solaris/sparc64 CFLAGS: -m64 -DPLATFORM=sun4v -DPLATFORM_SIZE=64 -D__sun -DHIGHCTIDH_PORTABLE=1
 
  // CC=s390x-linux-gnu-gcc CGO_ENABLED=1 GOOS=linux GOARCH=s390x go build -v
- #cgo s390x CFLAGS: -DPLATFORM=s390x -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE
+ #cgo s390x CFLAGS: -DPLATFORM=s390x -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE=1
 
  // CC=mips64-linux-gnuabi64-gcc CGO_ENABLED=1 GOOS=linux GOARCH=mips64  go build
  // With clang, -fforce-enable-int128 must be added to the CFLAGS
- #cgo mips64 CFLAGS: -DPLATFORM=mips64 -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE
+ #cgo mips64 CFLAGS: -DPLATFORM=mips64 -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE=1
 
  // CC=mips64-linux-gnuabi64-gcc CGO_ENABLED=1 GOOS=linux GOARCH=mips64  go build
  // With clang, -fforce-enable-int128 must be added to the CFLAGS
- #cgo mips64le CFLAGS: -DPLATFORM=mips64le -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE
+ #cgo mips64le CFLAGS: -DPLATFORM=mips64le -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE=1
 
  // CC=mipsel-linux-gnu-gcc CGO_ENABLED=1 GOOS=linux GOARCH=mipsle  go build
  // With clang, -fforce-enable-int128 must be added to the CFLAGS
- #cgo mipsle CFLAGS: -DPLATFORM=mipsle -DPLATFORM_SIZE=32 -DHIGHCTIDH_PORTABLE
+ #cgo mipsle CFLAGS: -DPLATFORM=mipsle -DPLATFORM_SIZE=32 -DHIGHCTIDH_PORTABLE=1
 
  // CC=mips-linux-gnu-gcc CGO_ENABLED=1 GOOS=linux GOARCH=mips  go build
  // With clang, -fforce-enable-int128 must be added to the CFLAGS
- #cgo mips CFLAGS: -DPLATFORM=mips -DPLATFORM_SIZE=32 -DHIGHCTIDH_PORTABLE
+ #cgo mips CFLAGS: -DPLATFORM=mips -DPLATFORM_SIZE=32 -DHIGHCTIDH_PORTABLE=1
 
  // export CGO_CFLAGS_ALLOW="-fforce-enable-int128";
  // CC=clang CGO_ENABLED=1 GOOS=linux GOARCH=386  go build
- #cgo 386 CFLAGS: -DPLATFORM=i386 -DPLATFORM_SIZE=32 -fforce-enable-int128 -D__i386__ -DHIGHCTIDH_PORTABLE
+ #cgo 386 CFLAGS: -DPLATFORM=i386 -DPLATFORM_SIZE=32 -fforce-enable-int128 -D__i386__ -DHIGHCTIDH_PORTABLE=1
 
  // The following should work as native builds with clang:
 
- #cgo loong64 CFLAGS: -DPLATFORM=loongarch64 -DPLATFORM_SIZE=64 -march=native -mtune=native -DHIGHCTIDH_PORTABLE
-
- #cgo sparc64 CFLAGS: -DPLATFORM=sparc64 -DPLATFORM_SIZE=64 -march=native -mtune=native -DHIGHCTIDH_PORTABLE
+ #cgo loong64 CFLAGS: -DPLATFORM=loongarch64 -DPLATFORM_SIZE=64 -march=native -mtune=native -DHIGHCTIDH_PORTABLE=1
 
  #include "binding2048.h"
 */
 import "C"
 import (
 	"fmt"
 	"io"
```

### Comparing `highctidh-1.0.2024012400/ctidh2048/common_test.go` & `highctidh-1.0.2024050100/ctidh2048/common_test.go`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh2048/csidh.c` & `highctidh-1.0.2024050100/ctidh2048/csidh.c`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,20 @@
  * big-endian portability.
  */
 void
 public_key_from_bytes(public_key *const pk, const char *const input)
 {
 	uint64_t *input_u64 = (uint64_t *)input;
 	for(size_t i=0; i < sizeof(pk->A.x.c)/sizeof(pk->A.x.c[0]); i++){
-		pk->A.x.c[i] = le64toh(*input_u64++);
+    // We could write this as so on GNU/Linux, BSD, and MacOS
+		// pk->A.x.c[i] = le64toh(*input_u64++);
+    // however on Solaris 11.4 sparcv9 64bit it throws a hard error of
+    // 'multiple unsequenced modifications'
+		pk->A.x.c[i] = le64toh(*input_u64);
+    input_u64++;
 	}
 }
 
 void
 public_key_to_bytes(char *const output, const public_key *const pk)
 {
 	uint64_t *output_u64 = (uint64_t *)output;
```

### Comparing `highctidh-1.0.2024012400/ctidh2048/csidh.h` & `highctidh-1.0.2024050100/ctidh2048/csidh.h`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #ifndef CSIDH_H
 #define CSIDH_H
 
 #ifdef CGONUTS
 #include "cgo.h"
 #endif // CGONUTS
 
+#include "naidne.h"
 #include "uintbig.h"
 #include "fp.h"
 #include "mont.h"
 #include "primes.h"
 #include "csidh_namespace.h"
 
 extern long long csidh_stattried[primes_batches];
```

### Comparing `highctidh-1.0.2024012400/ctidh2048/csidh_namespace.h` & `highctidh-1.0.2024050100/ctidh2048/csidh_namespace.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh2048/ctidh2048.go` & `highctidh-1.0.2024050100/ctidh2048/ctidh2048.go`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh2048/ctidh2048_bench_test.go` & `highctidh-1.0.2024050100/ctidh2048/ctidh2048_bench_test.go`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh2048/ctidh2048_test.go` & `highctidh-1.0.2024050100/ctidh2048/ctidh2048_test.go`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh2048/elligator.c` & `highctidh-1.0.2024050100/ctidh2048/elligator.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh2048/error.go` & `highctidh-1.0.2024050100/ctidh2048/error.go`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh2048/fiat_p2048.c` & `highctidh-1.0.2024050100/ctidh2048/fiat_p2048.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#if defined(HIGHCTIDH_PORTABLE)
+#if HIGHCTIDH_PORTABLE == 1
 #include "fiat_p2048.h"
 /* Autogenerated: './src/ExtractionOCaml/word_by_word_montgomery' --widen-bytes --internal-static --lang C -o f_2048_high.c p2048 64 8528475943061024837635249434131089507352961229039071418359007853431472824232731281573875097585132124495905689769457289097290485066318818670998665693553484375832840901492721916443754108187759409880104977491168497435797029889150028375522118007040227895709956565527693986603274933373650307807559167751481868507471338172008086897049878117533316735319086656307962660962929231692405440348962572770958110754184132520227272603171250943083809093992306118654477172531039336755846450097401488026516556186294026830749211238807256327438743073467304920067034434209788101583120190178099235423322734627165016835534905946794432350531 */
 /* curve description: p2048 */
 /* machine_wordsize = 64 (from "64") */
 /* requested operations: (all) */
 /* m = 0x438efcab10254c6497fefc90e8196ed94d8854e8b3e19c53ddffdcf1aee53f12dbd1fc2133770253584eb12932f72abb33a8779a1ec8b8c2b8523d6a302abf284dd6024bf2f8feab6557ebe96d91aeddc68049793337525393e73abd17e3aa46095ac8a9f3ce2b0c30d2edfe50198c647d84f102b5fde2eae33586d1208a10179844e5c09baf59ec0da1783672767abb88c691b2d452a8ac7c4cb419996f45e75377d53e856cc9a39796620b3ad8a5d458e89497ef35bbb92842bbe4dbacc65e44084e1a73c76cb244454e851cf305aba7bec86fabaf787f6478407d7a9a56eee111b0d22ab8ecaa95a98036c813c788dc703f0cd8c4d9187790d615ea034943 (from "8528475943061024837635249434131089507352961229039071418359007853431472824232731281573875097585132124495905689769457289097290485066318818670998665693553484375832840901492721916443754108187759409880104977491168497435797029889150028375522118007040227895709956565527693986603274933373650307807559167751481868507471338172008086897049878117533316735319086656307962660962929231692405440348962572770958110754184132520227272603171250943083809093992306118654477172531039336755846450097401488026516556186294026830749211238807256327438743073467304920067034434209788101583120190178099235423322734627165016835534905946794432350531") */
 /*                                                                    */
@@ -73595,8 +73595,10 @@
   out5[26] = x849;
   out5[27] = x850;
   out5[28] = x851;
   out5[29] = x852;
   out5[30] = x853;
   out5[31] = x854;
 }
+#else
+typedef int no_empty_translation_units_asm_2048; // -> "warning: ISO C forbids an empty translation unit"
 #endif
```

### Comparing `highctidh-1.0.2024012400/ctidh2048/fiat_p2048.h` & `highctidh-1.0.2024050100/ctidh2048/fiat_p2048.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh2048/fp.h` & `highctidh-1.0.2024050100/ctidh2048/fp.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 #ifndef FP_H
 #define FP_H
 
 #include "fp_namespace.h"
 #include "uintbig.h"
 #include "annotations.h"
 
-#if defined(HIGHCTIDH_PORTABLE) || !(defined(__x86_64__) || defined(_M_X64))
+#if HIGHCTIDH_PORTABLE == 1 || !(defined(__x86_64__) || defined(_M_X64))
 /* we only have optimizations for amd64 so far, so on other platforms we
  * default to the portable code by defining HIGHCTIDH_PORTABLE:
  */
 #ifndef HIGHCTIDH_PORTABLE
-#define HIGHCTIDH_PORTABLE
+#define HIGHCTIDH_PORTABLE 1
 #endif
 
 #if 511 == BITS
 #include "fiat_p511.h"
 #elif 512 == BITS
 #include "fiat_p512.h"
 #elif 1024 == BITS
@@ -72,20 +72,22 @@
 void ATTR_INITIALIZE_1st
 __attribute__((nonnull))
 __attribute__((flatten))
 fp_mul3(fp *const x, fp const *const y, fp const *const z)
 	__attribute__ ((alias ("fiat_p512_mul")));
 */
 //void fp_mul3 () __attribute__ ((weak, alias ("fiat_p512_mul")));
-#ifdef HIGHCTIDH_PORTABLE
+#if HIGHCTIDH_PORTABLE == 1
 #define highctidh_511_fp_mul3(a,b,c) FIAT_BITS(mul)((uint64_t *)a,(const uint64_t*)b,(const uint64_t*)c)
 #define highctidh_512_fp_mul3(a,b,c) FIAT_BITS(mul)((uint64_t *)a,(const uint64_t*)b,(const uint64_t*)c)
 #define highctidh_1024_fp_mul3(a,b,c) FIAT_BITS(mul)((uint64_t *)a,(const uint64_t*)b,(const uint64_t*)c)
 #define highctidh_2048_fp_mul3(a,b,c) FIAT_BITS(mul)((uint64_t *)a,(const uint64_t*)b,(const uint64_t*)c)
-#else /* ndef HIGHCTIDH_PORTABLE */
+#endif
+
+#if HIGHCTIDH_PORTABLE == 0
 void fp_mul3(fp *const a, const fp *const b, const fp *const c);
 #endif /* ndef HIGHCTIDH_PORTABLE */
 
 void fp_sq1(fp *x);
 void fp_sq2(fp *const x, fp const *const y);
 
 extern long long fp_mulsq_count;
@@ -108,15 +110,15 @@
 /*
  * a := 0 - b
  */
 static inline
 __attribute__((nonnull))
 void fp_neg2(fp *const x,const fp *const y)
 {
-#ifdef HIGHCTIDH_PORTABLE
+#if HIGHCTIDH_PORTABLE == 1
 	FIAT_BITS(opp)(x->x.c, y->x.c);
 #else
 	fp_sub3(x, &fp_0, y);
 #endif
 }
 
 static inline void fp_double1(fp *const x)
```

### Comparing `highctidh-1.0.2024012400/ctidh2048/fp2048.S` & `highctidh-1.0.2024050100/ctidh2048/fp2048.S`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /* DO NOT EDIT! generated by ./autogen */
-#ifndef HIGHCTIDH_PORTABLE
+#if HIGHCTIDH_PORTABLE == 0
 
 .intel_syntax noprefix
 
 //#include "uintbig_namespace.h"
 //#include "fp_namespace.h"
 
 .section .rodata
```

### Comparing `highctidh-1.0.2024012400/ctidh2048/fp2fiat.c` & `highctidh-1.0.2024050100/ctidh2048/fp2fiat.c`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #include <string.h>
 
 
 #include "uintbig_namespace.h"
 #include "fp.h"
 #include "annotations.h"
 
-#if !defined(HIGHCTIDH_PORTABLE) && !defined(CGONUTS) && defined(__x86_64__)
+#if HIGHCTIDH_PORTABLE == 0 && !defined(CGONUTS) && (defined(__x86_64__) || defined(__i86pc__))
 #define highctidh_macro_stringize(x) #x
 #define highctidh_macro_str(y) highctidh_macro_stringize(y)
 __asm__ (".include \"uintbig" highctidh_macro_str(BITS)  ".S\"");
 __asm__ (".include \"fp" highctidh_macro_str(BITS) ".S\"");
 
 #elif defined(CGONUTS)
 #define DONTMINDIFIDO
```

### Comparing `highctidh-1.0.2024012400/ctidh2048/fp_inv2048.c` & `highctidh-1.0.2024050100/ctidh2048/fp_inv2048.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh2048/fp_namespace.h` & `highctidh-1.0.2024050100/ctidh2048/fp_namespace.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh2048/fp_sqrt2048.c` & `highctidh-1.0.2024050100/ctidh2048/fp_sqrt2048.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh2048/int32_minmax.h` & `highctidh-1.0.2024050100/ctidh2048/int32_minmax.h`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 // This is from the Public Domain djbsort-20190516
 /* this needs __attribute__((optimize)) >= 1 */
 
 #ifndef HIGHCTIDH_INT32_MINMAX_H
 #define HIGHCTIDH_INT32_MINMAX_H
 
-#if defined(__x86_64__) && !defined(HIGHCTIDH_PORTABLE)
+#if ((defined(__x86_64__) || defined(__i86pc__))) && HIGHCTIDH_PORTABLE == 0
 
 #define int32_MINMAX(a,b)			\
 do { \
   int32 temp1; \
   __asm__( \
     ".att_syntax prefix\n\t" \
     "cmpl %1,%0\n\t" \
```

### Comparing `highctidh-1.0.2024012400/ctidh2048/int32_sort.c` & `highctidh-1.0.2024050100/ctidh2048/int32_sort.c`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #ifndef HIGHCTIDH_INT32_SORT_H
 #define HIGHCTIDH_INT32_SORT_H
 
-#if defined(__AVX2__) && !defined(HIGHCTIDH_PORTABLE)
+#if defined(__AVX2__) && HIGHCTIDH_PORTABLE == 0
 
 // This is the original high-ctidh x86_64 sorting code
 #ifndef CGONUTS
 #include "int32_sort_x86.c"
 #endif // CGONUTS
 
 #else /* fallback to portable C code: */
```

### Comparing `highctidh-1.0.2024012400/ctidh2048/int32_sort.h` & `highctidh-1.0.2024050100/ctidh2048/int32_sort.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh2048/int32_sort_x86.c` & `highctidh-1.0.2024050100/ctidh2048/int32_sort_x86.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-#ifndef HIGHCTIDH_PORTABLE
-#ifdef __x86_64__
+#if HIGHCTIDH_PORTABLE == 0
+#if (defined(__x86_64__) || defined(__i86pc__)) && !defined(CGONUTS)
 #include "int32_sort.h"
 #define int32 int32_t
 
 #include <immintrin.h>
 #include "int32_minmax.h"
 
 typedef __m256i int32x8;
```

### Comparing `highctidh-1.0.2024012400/ctidh2048/mont.c` & `highctidh-1.0.2024050100/ctidh2048/mont.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh2048/mont.h` & `highctidh-1.0.2024050100/ctidh2048/mont.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh2048/mont_namespace.h` & `highctidh-1.0.2024050100/ctidh2048/mont_namespace.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh2048/poly.c` & `highctidh-1.0.2024050100/ctidh2048/poly.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh2048/poly.h` & `highctidh-1.0.2024050100/ctidh2048/poly.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh2048/poly_namespace.h` & `highctidh-1.0.2024050100/ctidh2048/poly_namespace.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh2048/primes.h` & `highctidh-1.0.2024050100/ctidh2048/primes.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh2048/primes2048.c` & `highctidh-1.0.2024050100/ctidh2048/primes2048.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh2048/proj.h` & `highctidh-1.0.2024050100/ctidh2048/proj.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh2048/random.c` & `highctidh-1.0.2024050100/ctidh2048/random.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh2048/random.h` & `highctidh-1.0.2024050100/ctidh2048/random.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh2048/skgen.c` & `highctidh-1.0.2024050100/ctidh2048/skgen.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh2048/steps.c` & `highctidh-1.0.2024050100/ctidh2048/steps.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh2048/steps.h` & `highctidh-1.0.2024050100/ctidh2048/steps.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh2048/uintbig.h` & `highctidh-1.0.2024050100/ctidh2048/uintbig.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-#ifndef uintbig_h
-#define uintbig_h
+#ifndef UINTBIG_H
+#define UINTBIG_H
 
 #include "uintbig_namespace.h"
 
 #include <stdbool.h>
 #include <stdint.h>
 #include "annotations.h"
```

### Comparing `highctidh-1.0.2024012400/ctidh2048/uintbig2048.S` & `highctidh-1.0.2024050100/ctidh2048/uintbig2048.S`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /* DO NOT EDIT! generated by ./autogen */
-#ifndef HIGHCTIDH_PORTABLE
+#if HIGHCTIDH_PORTABLE == 0
 
 .intel_syntax noprefix
 
 //#include "uintbig_namespace.h"
 
 .section .rodata
```

### Comparing `highctidh-1.0.2024012400/ctidh2048/uintbig_namespace.h` & `highctidh-1.0.2024050100/ctidh2048/uintbig_namespace.h`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+#ifndef UINTBIG_NAMESPACE_H
+#define UINTBIG_NAMESPACE_H
+
 #ifdef CGONUTS
 #include "cgo.h"
 #endif // CGONUTS
 
 #define uintbig_p NAMESPACEBITS(uintbig_p)
 #define uintbig_1 NAMESPACEBITS(uintbig_1)
 #define uintbig_bit NAMESPACEBITS(uintbig_bit)
@@ -12,7 +15,9 @@
 #define uintbig_mul3_64 NAMESPACEBITS(uintbig_mul3_64)
 #define uintbig_four_sqrt_p NAMESPACEBITS(uintbig_four_sqrt_p)
 #define uintbig NAMESPACEBITS(uintbig)
 #define uintbig_bits_vartime NAMESPACEBITS(uintbig_bits_vartime)
 #define uintbig_uint64_iszero NAMESPACEBITS(uintbig_uint64_iszero)
 #define uintbig_isequal NAMESPACEBITS(uintbig_isequal)
 #define uintbig_iszero NAMESPACEBITS(uintbig_iszero)
+
+#endif
```

### Comparing `highctidh-1.0.2024012400/ctidh2048/validate.c` & `highctidh-1.0.2024050100/ctidh2048/validate.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh2048/vectors2048_test.go` & `highctidh-1.0.2024050100/ctidh2048/vectors2048_test.go`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh511/common.go` & `highctidh-1.0.2024050100/ctidh511/common.go`

 * *Files 19% similar despite different names*

```diff
@@ -1,63 +1,85 @@
 package ctidh511
 
 /*
- #cgo CFLAGS: -DBITS=511 -DGETRANDOM -DCGONUTS -Wformat -Werror=format-security -D_FORTIFY_SOURCE=2 -fstack-protector-all -fpie -fPIC -O2
- #cgo LDFLAGS: -Wl,-z,noexecstack -Wl,-z,relro
+ #cgo CFLAGS: -DBITS=511 -DGETRANDOM -DCGONUTS -O2
+ #cgo LDFLAGS:
+ #cgo linux CFLAGS: -DBITS=511 -DGETRANDOM -DCGONUTS -Wformat -Werror=format-security -D_FORTIFY_SOURCE=2 -fstack-protector-all -fpie -fPIC -O2
+ #cgo linux LDFLAGS: -Wl,-z,noexecstack -Wl,-z,relro
+ #cgo windows CFLAGS: -D__Windows__ -DHIGHCTIDH_PORTABLE=1
 
  // The following should work as native builds and as cross compiled builds.
  // Example cross compile build lines are provided as examples.
 
  // CC=aarch64-linux-gnu-gcc CGO_ENABLED=1 GOOS=linux GOARCH=arm64 go build -v
- #cgo arm64 CFLAGS: -DPLATFORM=aarch64 -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE
+ #cgo arm64 CFLAGS: -DPLATFORM=aarch64 -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE=1
+
+ // CC=clang CGO_ENABLED=1 GOOS=darwin GOARCH=arm64 go build -v
+ #cgo darwin/arm64 CFLAGS: -DPLATFORM=aarch64 -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE=1
 
  // export CGO_CFLAGS_ALLOW="-fforce-enable-int128";
  // CC=clang CGO_ENABLED=1 GOOS=linux GOARCH=arm ARMVER=7  go build
- #cgo arm CFLAGS: -DPLATFORM=arm -DPLATFORM_SIZE=32 -D__ARM32__ -DHIGHCTIDH_PORTABLE
+ #cgo arm CFLAGS: -DPLATFORM=arm -DPLATFORM_SIZE=32 -D__ARM32__ -DHIGHCTIDH_PORTABLE=1
+
+ // CC=clang CGO_ENABLED=1 GOOS=darwin GOARCH=amd64 go build -v
+ #cgo darwin/amd64 CFLAGS: -DPLATFORM=x86_64 -DPLATFORM_SIZE=64 -march=native -mtune=native -DHIGHCTIDH_PORTABLE=1
+
+ // Generic flags for amd64
+ #cgo amd64 CFLAGS: -DPLATFORM=x86_64 -DPLATFORM_SIZE=64
 
  // CC=gcc CGO_ENABLED=1 GOOS=linux GOARCH=amd64 go build -v
- #cgo amd64 CFLAGS: -DPLATFORM=x86_64 -DPLATFORM_SIZE=64 -march=native -mtune=native
+ #cgo linux/amd64 CFLAGS: -DPLATFORM=x86_64 -DPLATFORM_SIZE=64 -march=native -mtune=native
+
+ // CC=??? CGO_ENABLED=1 GOOS=windows GOARCH=arm64 go build
+ #cgo windows/arm64 CFLAGS: -DPLATFORM=arm64 -DPLATFORM_SIZE=64 -D__Windows__ -DHIGHCTIDH_PORTABLE=1
+
+ // CC=/usr/bin/x86_64-w64-mingw32-gcc CGO_ENABLED=1 GOOS=windows GOARCH=amd64 go build
+ #cgo windows/amd64 CFLAGS: -DPLATFORM=x86_64 -DPLATFORM_SIZE=64 -D__Windows__ -DHIGHCTIDH_PORTABLE=1
 
  // CC=powerpc64le-linux-gnu-gcc CGO_ENABLED=1 GOOS=linux GOARCH=ppc64le go build -v
- #cgo ppc64le CFLAGS: -DPLATFORM=ppc64le -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE
+ #cgo ppc64le CFLAGS: -DPLATFORM=ppc64le -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE=1
 
  // CC=powerpc64-linux-gnu-gcc CGO_ENABLED=1 GOOS=linux GOARCH=ppc64 go build -v
- #cgo ppc64 CFLAGS: -DPLATFORM=ppc64 -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE
+ #cgo ppc64 CFLAGS: -DPLATFORM=ppc64 -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE=1
 
  // CC=riscv64-linux-gnu-gcc CGO_ENABLED=1 GOOS=linux GOARCH=riscv64 go build -v
- #cgo riscv64 CFLAGS: -DPLATFORM=riscv64 -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE
+ #cgo riscv64 CFLAGS: -DPLATFORM=riscv64 -D__riscv -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE=1
+
+ // CC=gcc CGO_ENABLED=1 GOOS=solaris GOARCH=amd64 go build
+ #cgo solaris/amd64 CFLAGS: -m64 -mimpure-text -Wno-attributes -DPLATFORM=i86pc -DPLATFORM_SIZE=64 -D__sun -D__i86pc__ -DHIGHCTIDH_PORTABLE=0
+
+ // CC=gcc CGO_ENABLED=1 GOOS=solaris GOARCH=sparc64 go build
+ #cgo solaris/sparc64 CFLAGS: -m64 -DPLATFORM=sun4v -DPLATFORM_SIZE=64 -D__sun -DHIGHCTIDH_PORTABLE=1
 
  // CC=s390x-linux-gnu-gcc CGO_ENABLED=1 GOOS=linux GOARCH=s390x go build -v
- #cgo s390x CFLAGS: -DPLATFORM=s390x -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE
+ #cgo s390x CFLAGS: -DPLATFORM=s390x -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE=1
 
  // CC=mips64-linux-gnuabi64-gcc CGO_ENABLED=1 GOOS=linux GOARCH=mips64  go build
  // With clang, -fforce-enable-int128 must be added to the CFLAGS
- #cgo mips64 CFLAGS: -DPLATFORM=mips64 -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE
+ #cgo mips64 CFLAGS: -DPLATFORM=mips64 -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE=1
 
  // CC=mips64-linux-gnuabi64-gcc CGO_ENABLED=1 GOOS=linux GOARCH=mips64  go build
  // With clang, -fforce-enable-int128 must be added to the CFLAGS
- #cgo mips64le CFLAGS: -DPLATFORM=mips64le -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE
+ #cgo mips64le CFLAGS: -DPLATFORM=mips64le -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE=1
 
  // CC=mipsel-linux-gnu-gcc CGO_ENABLED=1 GOOS=linux GOARCH=mipsle  go build
  // With clang, -fforce-enable-int128 must be added to the CFLAGS
- #cgo mipsle CFLAGS: -DPLATFORM=mipsle -DPLATFORM_SIZE=32 -DHIGHCTIDH_PORTABLE
+ #cgo mipsle CFLAGS: -DPLATFORM=mipsle -DPLATFORM_SIZE=32 -DHIGHCTIDH_PORTABLE=1
 
  // CC=mips-linux-gnu-gcc CGO_ENABLED=1 GOOS=linux GOARCH=mips  go build
  // With clang, -fforce-enable-int128 must be added to the CFLAGS
- #cgo mips CFLAGS: -DPLATFORM=mips -DPLATFORM_SIZE=32 -DHIGHCTIDH_PORTABLE
+ #cgo mips CFLAGS: -DPLATFORM=mips -DPLATFORM_SIZE=32 -DHIGHCTIDH_PORTABLE=1
 
  // export CGO_CFLAGS_ALLOW="-fforce-enable-int128";
  // CC=clang CGO_ENABLED=1 GOOS=linux GOARCH=386  go build
- #cgo 386 CFLAGS: -DPLATFORM=i386 -DPLATFORM_SIZE=32 -fforce-enable-int128 -D__i386__ -DHIGHCTIDH_PORTABLE
+ #cgo 386 CFLAGS: -DPLATFORM=i386 -DPLATFORM_SIZE=32 -fforce-enable-int128 -D__i386__ -DHIGHCTIDH_PORTABLE=1
 
  // The following should work as native builds with clang:
 
- #cgo loong64 CFLAGS: -DPLATFORM=loongarch64 -DPLATFORM_SIZE=64 -march=native -mtune=native -DHIGHCTIDH_PORTABLE
-
- #cgo sparc64 CFLAGS: -DPLATFORM=sparc64 -DPLATFORM_SIZE=64 -march=native -mtune=native -DHIGHCTIDH_PORTABLE
+ #cgo loong64 CFLAGS: -DPLATFORM=loongarch64 -DPLATFORM_SIZE=64 -march=native -mtune=native -DHIGHCTIDH_PORTABLE=1
 
  #include "binding511.h"
 */
 import "C"
 import (
 	"fmt"
 	"io"
```

### Comparing `highctidh-1.0.2024012400/ctidh511/common_test.go` & `highctidh-1.0.2024050100/ctidh511/common_test.go`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh511/csidh.c` & `highctidh-1.0.2024050100/ctidh511/csidh.c`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,20 @@
  * big-endian portability.
  */
 void
 public_key_from_bytes(public_key *const pk, const char *const input)
 {
 	uint64_t *input_u64 = (uint64_t *)input;
 	for(size_t i=0; i < sizeof(pk->A.x.c)/sizeof(pk->A.x.c[0]); i++){
-		pk->A.x.c[i] = le64toh(*input_u64++);
+    // We could write this as so on GNU/Linux, BSD, and MacOS
+		// pk->A.x.c[i] = le64toh(*input_u64++);
+    // however on Solaris 11.4 sparcv9 64bit it throws a hard error of
+    // 'multiple unsequenced modifications'
+		pk->A.x.c[i] = le64toh(*input_u64);
+    input_u64++;
 	}
 }
 
 void
 public_key_to_bytes(char *const output, const public_key *const pk)
 {
 	uint64_t *output_u64 = (uint64_t *)output;
```

### Comparing `highctidh-1.0.2024012400/ctidh511/csidh.h` & `highctidh-1.0.2024050100/ctidh511/csidh.h`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #ifndef CSIDH_H
 #define CSIDH_H
 
 #ifdef CGONUTS
 #include "cgo.h"
 #endif // CGONUTS
 
+#include "naidne.h"
 #include "uintbig.h"
 #include "fp.h"
 #include "mont.h"
 #include "primes.h"
 #include "csidh_namespace.h"
 
 extern long long csidh_stattried[primes_batches];
```

### Comparing `highctidh-1.0.2024012400/ctidh511/csidh_namespace.h` & `highctidh-1.0.2024050100/ctidh511/csidh_namespace.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh511/ctidh511.go` & `highctidh-1.0.2024050100/ctidh511/ctidh511.go`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh511/ctidh511_bench_test.go` & `highctidh-1.0.2024050100/ctidh511/ctidh511_bench_test.go`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh511/ctidh511_test.go` & `highctidh-1.0.2024050100/ctidh511/ctidh511_test.go`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh511/elligator.c` & `highctidh-1.0.2024050100/ctidh511/elligator.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh511/error.go` & `highctidh-1.0.2024050100/ctidh511/error.go`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh511/fiat_p511.c` & `highctidh-1.0.2024050100/ctidh511/fiat_p511.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#if defined(HIGHCTIDH_PORTABLE)
+#if HIGHCTIDH_PORTABLE == 1
 #include "fiat_p511.h"
 /* Autogenerated: './src/ExtractionOCaml/word_by_word_montgomery' --internal-static --lang C -o fiat_p511.c p511 64 5326738796327623094747867617954605554069371494832722337612446642054009560026576537626892113026381253624626941643949444792662881241621373288942880288065659 */
 /* curve description: p511 */
 /* machine_wordsize = 64 (from "64") */
 /* requested operations: (all) */
 /* m = 0x65b48e8f740f89bffc8ab0d15e3e4c4ab42d083aedc88c425afbfcc69322c9cda7aac6c567f35507516730cc1f0b4f25c2721bf457aca8351b81b90533c6c87b (from "5326738796327623094747867617954605554069371494832722337612446642054009560026576537626892113026381253624626941643949444792662881241621373288942880288065659") */
 /*                                                                    */
@@ -6003,8 +6003,10 @@
   out5[2] = x225;
   out5[3] = x226;
   out5[4] = x227;
   out5[5] = x228;
   out5[6] = x229;
   out5[7] = x230;
 }
+#else
+typedef int no_empty_translation_units_asm_511; // -> "warning: ISO C forbids an empty translation unit"
 #endif
```

### Comparing `highctidh-1.0.2024012400/ctidh511/fiat_p511.h` & `highctidh-1.0.2024050100/ctidh511/fiat_p511.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh511/fp.h` & `highctidh-1.0.2024050100/ctidh511/fp.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 #ifndef FP_H
 #define FP_H
 
 #include "fp_namespace.h"
 #include "uintbig.h"
 #include "annotations.h"
 
-#if defined(HIGHCTIDH_PORTABLE) || !(defined(__x86_64__) || defined(_M_X64))
+#if HIGHCTIDH_PORTABLE == 1 || !(defined(__x86_64__) || defined(_M_X64))
 /* we only have optimizations for amd64 so far, so on other platforms we
  * default to the portable code by defining HIGHCTIDH_PORTABLE:
  */
 #ifndef HIGHCTIDH_PORTABLE
-#define HIGHCTIDH_PORTABLE
+#define HIGHCTIDH_PORTABLE 1
 #endif
 
 #if 511 == BITS
 #include "fiat_p511.h"
 #elif 512 == BITS
 #include "fiat_p512.h"
 #elif 1024 == BITS
@@ -72,20 +72,22 @@
 void ATTR_INITIALIZE_1st
 __attribute__((nonnull))
 __attribute__((flatten))
 fp_mul3(fp *const x, fp const *const y, fp const *const z)
 	__attribute__ ((alias ("fiat_p512_mul")));
 */
 //void fp_mul3 () __attribute__ ((weak, alias ("fiat_p512_mul")));
-#ifdef HIGHCTIDH_PORTABLE
+#if HIGHCTIDH_PORTABLE == 1
 #define highctidh_511_fp_mul3(a,b,c) FIAT_BITS(mul)((uint64_t *)a,(const uint64_t*)b,(const uint64_t*)c)
 #define highctidh_512_fp_mul3(a,b,c) FIAT_BITS(mul)((uint64_t *)a,(const uint64_t*)b,(const uint64_t*)c)
 #define highctidh_1024_fp_mul3(a,b,c) FIAT_BITS(mul)((uint64_t *)a,(const uint64_t*)b,(const uint64_t*)c)
 #define highctidh_2048_fp_mul3(a,b,c) FIAT_BITS(mul)((uint64_t *)a,(const uint64_t*)b,(const uint64_t*)c)
-#else /* ndef HIGHCTIDH_PORTABLE */
+#endif
+
+#if HIGHCTIDH_PORTABLE == 0
 void fp_mul3(fp *const a, const fp *const b, const fp *const c);
 #endif /* ndef HIGHCTIDH_PORTABLE */
 
 void fp_sq1(fp *x);
 void fp_sq2(fp *const x, fp const *const y);
 
 extern long long fp_mulsq_count;
@@ -108,15 +110,15 @@
 /*
  * a := 0 - b
  */
 static inline
 __attribute__((nonnull))
 void fp_neg2(fp *const x,const fp *const y)
 {
-#ifdef HIGHCTIDH_PORTABLE
+#if HIGHCTIDH_PORTABLE == 1
 	FIAT_BITS(opp)(x->x.c, y->x.c);
 #else
 	fp_sub3(x, &fp_0, y);
 #endif
 }
 
 static inline void fp_double1(fp *const x)
```

### Comparing `highctidh-1.0.2024012400/ctidh511/fp2fiat.c` & `highctidh-1.0.2024050100/ctidh511/fp2fiat.c`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #include <string.h>
 
 
 #include "uintbig_namespace.h"
 #include "fp.h"
 #include "annotations.h"
 
-#if !defined(HIGHCTIDH_PORTABLE) && !defined(CGONUTS) && defined(__x86_64__)
+#if HIGHCTIDH_PORTABLE == 0 && !defined(CGONUTS) && (defined(__x86_64__) || defined(__i86pc__))
 #define highctidh_macro_stringize(x) #x
 #define highctidh_macro_str(y) highctidh_macro_stringize(y)
 __asm__ (".include \"uintbig" highctidh_macro_str(BITS)  ".S\"");
 __asm__ (".include \"fp" highctidh_macro_str(BITS) ".S\"");
 
 #elif defined(CGONUTS)
 #define DONTMINDIFIDO
```

### Comparing `highctidh-1.0.2024012400/ctidh511/fp511.S` & `highctidh-1.0.2024050100/ctidh511/fp511.S`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /* DO NOT EDIT! generated by ./autogen */
-#ifndef HIGHCTIDH_PORTABLE
+#if HIGHCTIDH_PORTABLE == 0
 
 .intel_syntax noprefix
 
 //#include "uintbig_namespace.h"
 //#include "fp_namespace.h"
 
 .section .rodata
```

### Comparing `highctidh-1.0.2024012400/ctidh511/fp_inv511.c` & `highctidh-1.0.2024050100/ctidh511/fp_inv511.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh511/fp_namespace.h` & `highctidh-1.0.2024050100/ctidh511/fp_namespace.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh511/fp_sqrt511.c` & `highctidh-1.0.2024050100/ctidh511/fp_sqrt511.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh511/int32_minmax.h` & `highctidh-1.0.2024050100/ctidh511/int32_minmax.h`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 // This is from the Public Domain djbsort-20190516
 /* this needs __attribute__((optimize)) >= 1 */
 
 #ifndef HIGHCTIDH_INT32_MINMAX_H
 #define HIGHCTIDH_INT32_MINMAX_H
 
-#if defined(__x86_64__) && !defined(HIGHCTIDH_PORTABLE)
+#if ((defined(__x86_64__) || defined(__i86pc__))) && HIGHCTIDH_PORTABLE == 0
 
 #define int32_MINMAX(a,b)			\
 do { \
   int32 temp1; \
   __asm__( \
     ".att_syntax prefix\n\t" \
     "cmpl %1,%0\n\t" \
```

### Comparing `highctidh-1.0.2024012400/ctidh511/int32_sort.c` & `highctidh-1.0.2024050100/ctidh511/int32_sort.c`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #ifndef HIGHCTIDH_INT32_SORT_H
 #define HIGHCTIDH_INT32_SORT_H
 
-#if defined(__AVX2__) && !defined(HIGHCTIDH_PORTABLE)
+#if defined(__AVX2__) && HIGHCTIDH_PORTABLE == 0
 
 // This is the original high-ctidh x86_64 sorting code
 #ifndef CGONUTS
 #include "int32_sort_x86.c"
 #endif // CGONUTS
 
 #else /* fallback to portable C code: */
```

### Comparing `highctidh-1.0.2024012400/ctidh511/int32_sort.h` & `highctidh-1.0.2024050100/ctidh511/int32_sort.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh511/int32_sort_x86.c` & `highctidh-1.0.2024050100/ctidh511/int32_sort_x86.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-#ifndef HIGHCTIDH_PORTABLE
-#ifdef __x86_64__
+#if HIGHCTIDH_PORTABLE == 0
+#if (defined(__x86_64__) || defined(__i86pc__)) && !defined(CGONUTS)
 #include "int32_sort.h"
 #define int32 int32_t
 
 #include <immintrin.h>
 #include "int32_minmax.h"
 
 typedef __m256i int32x8;
```

### Comparing `highctidh-1.0.2024012400/ctidh511/mont.c` & `highctidh-1.0.2024050100/ctidh511/mont.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh511/mont.h` & `highctidh-1.0.2024050100/ctidh511/mont.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh511/mont_namespace.h` & `highctidh-1.0.2024050100/ctidh511/mont_namespace.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh511/poly.c` & `highctidh-1.0.2024050100/ctidh511/poly.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh511/poly.h` & `highctidh-1.0.2024050100/ctidh511/poly.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh511/poly_namespace.h` & `highctidh-1.0.2024050100/ctidh511/poly_namespace.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh511/primes.h` & `highctidh-1.0.2024050100/ctidh511/primes.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh511/primes511.c` & `highctidh-1.0.2024050100/ctidh511/primes511.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh511/proj.h` & `highctidh-1.0.2024050100/ctidh511/proj.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh511/random.c` & `highctidh-1.0.2024050100/ctidh511/random.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh511/random.h` & `highctidh-1.0.2024050100/ctidh511/random.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh511/skgen.c` & `highctidh-1.0.2024050100/ctidh511/skgen.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh511/steps.c` & `highctidh-1.0.2024050100/ctidh511/steps.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh511/steps.h` & `highctidh-1.0.2024050100/ctidh511/steps.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh511/uintbig.h` & `highctidh-1.0.2024050100/ctidh511/uintbig.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-#ifndef uintbig_h
-#define uintbig_h
+#ifndef UINTBIG_H
+#define UINTBIG_H
 
 #include "uintbig_namespace.h"
 
 #include <stdbool.h>
 #include <stdint.h>
 #include "annotations.h"
```

### Comparing `highctidh-1.0.2024012400/ctidh511/uintbig511.S` & `highctidh-1.0.2024050100/ctidh511/uintbig511.S`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /* DO NOT EDIT! generated by ./autogen */
-#ifndef HIGHCTIDH_PORTABLE
+#if HIGHCTIDH_PORTABLE == 0
 
 .intel_syntax noprefix
 
 //#include "uintbig_namespace.h"
 
 .section .rodata
```

### Comparing `highctidh-1.0.2024012400/ctidh511/uintbig_namespace.h` & `highctidh-1.0.2024050100/ctidh511/uintbig_namespace.h`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+#ifndef UINTBIG_NAMESPACE_H
+#define UINTBIG_NAMESPACE_H
+
 #ifdef CGONUTS
 #include "cgo.h"
 #endif // CGONUTS
 
 #define uintbig_p NAMESPACEBITS(uintbig_p)
 #define uintbig_1 NAMESPACEBITS(uintbig_1)
 #define uintbig_bit NAMESPACEBITS(uintbig_bit)
@@ -12,7 +15,9 @@
 #define uintbig_mul3_64 NAMESPACEBITS(uintbig_mul3_64)
 #define uintbig_four_sqrt_p NAMESPACEBITS(uintbig_four_sqrt_p)
 #define uintbig NAMESPACEBITS(uintbig)
 #define uintbig_bits_vartime NAMESPACEBITS(uintbig_bits_vartime)
 #define uintbig_uint64_iszero NAMESPACEBITS(uintbig_uint64_iszero)
 #define uintbig_isequal NAMESPACEBITS(uintbig_isequal)
 #define uintbig_iszero NAMESPACEBITS(uintbig_iszero)
+
+#endif
```

### Comparing `highctidh-1.0.2024012400/ctidh511/validate.c` & `highctidh-1.0.2024050100/ctidh511/validate.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh511/vectors511_test.go` & `highctidh-1.0.2024050100/ctidh511/vectors511_test.go`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh512/common.go` & `highctidh-1.0.2024050100/ctidh512/common.go`

 * *Files 16% similar despite different names*

```diff
@@ -1,63 +1,85 @@
 package ctidh512
 
 /*
- #cgo CFLAGS: -DBITS=512 -DGETRANDOM -DCGONUTS -Wformat -Werror=format-security -D_FORTIFY_SOURCE=2 -fstack-protector-all -fpie -fPIC -O2
- #cgo LDFLAGS: -Wl,-z,noexecstack -Wl,-z,relro
+ #cgo CFLAGS: -DBITS=512 -DGETRANDOM -DCGONUTS -O2
+ #cgo LDFLAGS:
+ #cgo linux CFLAGS: -DBITS=512 -DGETRANDOM -DCGONUTS -Wformat -Werror=format-security -D_FORTIFY_SOURCE=2 -fstack-protector-all -fpie -fPIC -O2
+ #cgo linux LDFLAGS: -Wl,-z,noexecstack -Wl,-z,relro
+ #cgo windows CFLAGS: -D__Windows__ -DHIGHCTIDH_PORTABLE=1
 
  // The following should work as native builds and as cross compiled builds.
  // Example cross compile build lines are provided as examples.
 
  // CC=aarch64-linux-gnu-gcc CGO_ENABLED=1 GOOS=linux GOARCH=arm64 go build -v
- #cgo arm64 CFLAGS: -DPLATFORM=aarch64 -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE
+ #cgo arm64 CFLAGS: -DPLATFORM=aarch64 -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE=1
+
+ // CC=clang CGO_ENABLED=1 GOOS=darwin GOARCH=arm64 go build -v
+ #cgo darwin/arm64 CFLAGS: -DPLATFORM=aarch64 -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE=1
 
  // export CGO_CFLAGS_ALLOW="-fforce-enable-int128";
  // CC=clang CGO_ENABLED=1 GOOS=linux GOARCH=arm ARMVER=7  go build
- #cgo arm CFLAGS: -DPLATFORM=arm -DPLATFORM_SIZE=32 -D__ARM32__ -DHIGHCTIDH_PORTABLE
+ #cgo arm CFLAGS: -DPLATFORM=arm -DPLATFORM_SIZE=32 -D__ARM32__ -DHIGHCTIDH_PORTABLE=1
+
+ // CC=clang CGO_ENABLED=1 GOOS=darwin GOARCH=amd64 go build -v
+ #cgo darwin/amd64 CFLAGS: -DPLATFORM=x86_64 -DPLATFORM_SIZE=64 -march=native -mtune=native -DHIGHCTIDH_PORTABLE=1
+
+ // Generic flags for amd64
+ #cgo amd64 CFLAGS: -DPLATFORM=x86_64 -DPLATFORM_SIZE=64
 
  // CC=gcc CGO_ENABLED=1 GOOS=linux GOARCH=amd64 go build -v
- #cgo amd64 CFLAGS: -DPLATFORM=x86_64 -DPLATFORM_SIZE=64 -march=native -mtune=native
+ #cgo linux/amd64 CFLAGS: -DPLATFORM=x86_64 -DPLATFORM_SIZE=64 -march=native -mtune=native
+
+ // CC=??? CGO_ENABLED=1 GOOS=windows GOARCH=arm64 go build
+ #cgo windows/arm64 CFLAGS: -DPLATFORM=arm64 -DPLATFORM_SIZE=64 -D__Windows__ -DHIGHCTIDH_PORTABLE=1
+
+ // CC=/usr/bin/x86_64-w64-mingw32-gcc CGO_ENABLED=1 GOOS=windows GOARCH=amd64 go build
+ #cgo windows/amd64 CFLAGS: -DPLATFORM=x86_64 -DPLATFORM_SIZE=64 -D__Windows__ -DHIGHCTIDH_PORTABLE=1
 
  // CC=powerpc64le-linux-gnu-gcc CGO_ENABLED=1 GOOS=linux GOARCH=ppc64le go build -v
- #cgo ppc64le CFLAGS: -DPLATFORM=ppc64le -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE
+ #cgo ppc64le CFLAGS: -DPLATFORM=ppc64le -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE=1
 
  // CC=powerpc64-linux-gnu-gcc CGO_ENABLED=1 GOOS=linux GOARCH=ppc64 go build -v
- #cgo ppc64 CFLAGS: -DPLATFORM=ppc64 -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE
+ #cgo ppc64 CFLAGS: -DPLATFORM=ppc64 -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE=1
 
  // CC=riscv64-linux-gnu-gcc CGO_ENABLED=1 GOOS=linux GOARCH=riscv64 go build -v
- #cgo riscv64 CFLAGS: -DPLATFORM=riscv64 -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE
+ #cgo riscv64 CFLAGS: -DPLATFORM=riscv64 -D__riscv -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE=1
+
+ // CC=gcc CGO_ENABLED=1 GOOS=solaris GOARCH=amd64 go build
+ #cgo solaris/amd64 CFLAGS: -m64 -mimpure-text -Wno-attributes -DPLATFORM=i86pc -DPLATFORM_SIZE=64 -D__sun -D__i86pc__ -DHIGHCTIDH_PORTABLE=0
+
+ // CC=gcc CGO_ENABLED=1 GOOS=solaris GOARCH=sparc64 go build
+ #cgo solaris/sparc64 CFLAGS: -m64 -DPLATFORM=sun4v -DPLATFORM_SIZE=64 -D__sun -DHIGHCTIDH_PORTABLE=1
 
  // CC=s390x-linux-gnu-gcc CGO_ENABLED=1 GOOS=linux GOARCH=s390x go build -v
- #cgo s390x CFLAGS: -DPLATFORM=s390x -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE
+ #cgo s390x CFLAGS: -DPLATFORM=s390x -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE=1
 
  // CC=mips64-linux-gnuabi64-gcc CGO_ENABLED=1 GOOS=linux GOARCH=mips64  go build
  // With clang, -fforce-enable-int128 must be added to the CFLAGS
- #cgo mips64 CFLAGS: -DPLATFORM=mips64 -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE
+ #cgo mips64 CFLAGS: -DPLATFORM=mips64 -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE=1
 
  // CC=mips64-linux-gnuabi64-gcc CGO_ENABLED=1 GOOS=linux GOARCH=mips64  go build
  // With clang, -fforce-enable-int128 must be added to the CFLAGS
- #cgo mips64le CFLAGS: -DPLATFORM=mips64le -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE
+ #cgo mips64le CFLAGS: -DPLATFORM=mips64le -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE=1
 
  // CC=mipsel-linux-gnu-gcc CGO_ENABLED=1 GOOS=linux GOARCH=mipsle  go build
  // With clang, -fforce-enable-int128 must be added to the CFLAGS
- #cgo mipsle CFLAGS: -DPLATFORM=mipsle -DPLATFORM_SIZE=32 -DHIGHCTIDH_PORTABLE
+ #cgo mipsle CFLAGS: -DPLATFORM=mipsle -DPLATFORM_SIZE=32 -DHIGHCTIDH_PORTABLE=1
 
  // CC=mips-linux-gnu-gcc CGO_ENABLED=1 GOOS=linux GOARCH=mips  go build
  // With clang, -fforce-enable-int128 must be added to the CFLAGS
- #cgo mips CFLAGS: -DPLATFORM=mips -DPLATFORM_SIZE=32 -DHIGHCTIDH_PORTABLE
+ #cgo mips CFLAGS: -DPLATFORM=mips -DPLATFORM_SIZE=32 -DHIGHCTIDH_PORTABLE=1
 
  // export CGO_CFLAGS_ALLOW="-fforce-enable-int128";
  // CC=clang CGO_ENABLED=1 GOOS=linux GOARCH=386  go build
- #cgo 386 CFLAGS: -DPLATFORM=i386 -DPLATFORM_SIZE=32 -fforce-enable-int128 -D__i386__ -DHIGHCTIDH_PORTABLE
+ #cgo 386 CFLAGS: -DPLATFORM=i386 -DPLATFORM_SIZE=32 -fforce-enable-int128 -D__i386__ -DHIGHCTIDH_PORTABLE=1
 
  // The following should work as native builds with clang:
 
- #cgo loong64 CFLAGS: -DPLATFORM=loongarch64 -DPLATFORM_SIZE=64 -march=native -mtune=native -DHIGHCTIDH_PORTABLE
-
- #cgo sparc64 CFLAGS: -DPLATFORM=sparc64 -DPLATFORM_SIZE=64 -march=native -mtune=native -DHIGHCTIDH_PORTABLE
+ #cgo loong64 CFLAGS: -DPLATFORM=loongarch64 -DPLATFORM_SIZE=64 -march=native -mtune=native -DHIGHCTIDH_PORTABLE=1
 
  #include "binding512.h"
 */
 import "C"
 import (
 	"fmt"
 	"io"
```

### Comparing `highctidh-1.0.2024012400/ctidh512/common_test.go` & `highctidh-1.0.2024050100/ctidh512/common_test.go`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh512/csidh.c` & `highctidh-1.0.2024050100/ctidh512/csidh.c`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,20 @@
  * big-endian portability.
  */
 void
 public_key_from_bytes(public_key *const pk, const char *const input)
 {
 	uint64_t *input_u64 = (uint64_t *)input;
 	for(size_t i=0; i < sizeof(pk->A.x.c)/sizeof(pk->A.x.c[0]); i++){
-		pk->A.x.c[i] = le64toh(*input_u64++);
+    // We could write this as so on GNU/Linux, BSD, and MacOS
+		// pk->A.x.c[i] = le64toh(*input_u64++);
+    // however on Solaris 11.4 sparcv9 64bit it throws a hard error of
+    // 'multiple unsequenced modifications'
+		pk->A.x.c[i] = le64toh(*input_u64);
+    input_u64++;
 	}
 }
 
 void
 public_key_to_bytes(char *const output, const public_key *const pk)
 {
 	uint64_t *output_u64 = (uint64_t *)output;
```

### Comparing `highctidh-1.0.2024012400/ctidh512/csidh.h` & `highctidh-1.0.2024050100/ctidh512/csidh.h`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #ifndef CSIDH_H
 #define CSIDH_H
 
 #ifdef CGONUTS
 #include "cgo.h"
 #endif // CGONUTS
 
+#include "naidne.h"
 #include "uintbig.h"
 #include "fp.h"
 #include "mont.h"
 #include "primes.h"
 #include "csidh_namespace.h"
 
 extern long long csidh_stattried[primes_batches];
```

### Comparing `highctidh-1.0.2024012400/ctidh512/csidh_namespace.h` & `highctidh-1.0.2024050100/ctidh512/csidh_namespace.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh512/ctidh512.go` & `highctidh-1.0.2024050100/ctidh512/ctidh512.go`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh512/ctidh512_bench_test.go` & `highctidh-1.0.2024050100/ctidh512/ctidh512_bench_test.go`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh512/ctidh512_test.go` & `highctidh-1.0.2024050100/ctidh512/ctidh512_test.go`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh512/elligator.c` & `highctidh-1.0.2024050100/ctidh512/elligator.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh512/error.go` & `highctidh-1.0.2024050100/ctidh512/error.go`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh512/fiat_p512.c` & `highctidh-1.0.2024050100/ctidh512/fiat_p512.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#if defined(HIGHCTIDH_PORTABLE)
+#if HIGHCTIDH_PORTABLE == 1
 #include "fiat_p512.h"
 /* Autogenerated: './src/ExtractionOCaml/word_by_word_montgomery' --internal-static --lang C -o fiat_p512.c p512 64 5326738796327623094747867617954605554069371494832722337612446642054009560026576537626892113026381253624626941643949444792662881241621373288942880288065659 */
 /* curve description: p512 */
 /* machine_wordsize = 64 (from "64") */
 /* requested operations: (all) */
 /* m = 0x65b48e8f740f89bffc8ab0d15e3e4c4ab42d083aedc88c425afbfcc69322c9cda7aac6c567f35507516730cc1f0b4f25c2721bf457aca8351b81b90533c6c87b (from "5326738796327623094747867617954605554069371494832722337612446642054009560026576537626892113026381253624626941643949444792662881241621373288942880288065659") */
 /*                                                                    */
@@ -6003,8 +6003,10 @@
   out5[2] = x225;
   out5[3] = x226;
   out5[4] = x227;
   out5[5] = x228;
   out5[6] = x229;
   out5[7] = x230;
 }
+#else
+typedef int no_empty_translation_units_asm_512; // -> "warning: ISO C forbids an empty translation unit"
 #endif
```

### Comparing `highctidh-1.0.2024012400/ctidh512/fiat_p512.h` & `highctidh-1.0.2024050100/ctidh512/fiat_p512.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh512/fp.h` & `highctidh-1.0.2024050100/ctidh512/fp.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 #ifndef FP_H
 #define FP_H
 
 #include "fp_namespace.h"
 #include "uintbig.h"
 #include "annotations.h"
 
-#if defined(HIGHCTIDH_PORTABLE) || !(defined(__x86_64__) || defined(_M_X64))
+#if HIGHCTIDH_PORTABLE == 1 || !(defined(__x86_64__) || defined(_M_X64))
 /* we only have optimizations for amd64 so far, so on other platforms we
  * default to the portable code by defining HIGHCTIDH_PORTABLE:
  */
 #ifndef HIGHCTIDH_PORTABLE
-#define HIGHCTIDH_PORTABLE
+#define HIGHCTIDH_PORTABLE 1
 #endif
 
 #if 511 == BITS
 #include "fiat_p511.h"
 #elif 512 == BITS
 #include "fiat_p512.h"
 #elif 1024 == BITS
@@ -72,20 +72,22 @@
 void ATTR_INITIALIZE_1st
 __attribute__((nonnull))
 __attribute__((flatten))
 fp_mul3(fp *const x, fp const *const y, fp const *const z)
 	__attribute__ ((alias ("fiat_p512_mul")));
 */
 //void fp_mul3 () __attribute__ ((weak, alias ("fiat_p512_mul")));
-#ifdef HIGHCTIDH_PORTABLE
+#if HIGHCTIDH_PORTABLE == 1
 #define highctidh_511_fp_mul3(a,b,c) FIAT_BITS(mul)((uint64_t *)a,(const uint64_t*)b,(const uint64_t*)c)
 #define highctidh_512_fp_mul3(a,b,c) FIAT_BITS(mul)((uint64_t *)a,(const uint64_t*)b,(const uint64_t*)c)
 #define highctidh_1024_fp_mul3(a,b,c) FIAT_BITS(mul)((uint64_t *)a,(const uint64_t*)b,(const uint64_t*)c)
 #define highctidh_2048_fp_mul3(a,b,c) FIAT_BITS(mul)((uint64_t *)a,(const uint64_t*)b,(const uint64_t*)c)
-#else /* ndef HIGHCTIDH_PORTABLE */
+#endif
+
+#if HIGHCTIDH_PORTABLE == 0
 void fp_mul3(fp *const a, const fp *const b, const fp *const c);
 #endif /* ndef HIGHCTIDH_PORTABLE */
 
 void fp_sq1(fp *x);
 void fp_sq2(fp *const x, fp const *const y);
 
 extern long long fp_mulsq_count;
@@ -108,15 +110,15 @@
 /*
  * a := 0 - b
  */
 static inline
 __attribute__((nonnull))
 void fp_neg2(fp *const x,const fp *const y)
 {
-#ifdef HIGHCTIDH_PORTABLE
+#if HIGHCTIDH_PORTABLE == 1
 	FIAT_BITS(opp)(x->x.c, y->x.c);
 #else
 	fp_sub3(x, &fp_0, y);
 #endif
 }
 
 static inline void fp_double1(fp *const x)
```

### Comparing `highctidh-1.0.2024012400/ctidh512/fp2fiat.c` & `highctidh-1.0.2024050100/ctidh512/fp2fiat.c`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #include <string.h>
 
 
 #include "uintbig_namespace.h"
 #include "fp.h"
 #include "annotations.h"
 
-#if !defined(HIGHCTIDH_PORTABLE) && !defined(CGONUTS) && defined(__x86_64__)
+#if HIGHCTIDH_PORTABLE == 0 && !defined(CGONUTS) && (defined(__x86_64__) || defined(__i86pc__))
 #define highctidh_macro_stringize(x) #x
 #define highctidh_macro_str(y) highctidh_macro_stringize(y)
 __asm__ (".include \"uintbig" highctidh_macro_str(BITS)  ".S\"");
 __asm__ (".include \"fp" highctidh_macro_str(BITS) ".S\"");
 
 #elif defined(CGONUTS)
 #define DONTMINDIFIDO
```

### Comparing `highctidh-1.0.2024012400/ctidh512/fp512.S` & `highctidh-1.0.2024050100/ctidh512/fp512.S`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /* DO NOT EDIT! generated by ./autogen */
-#ifndef HIGHCTIDH_PORTABLE
+#if HIGHCTIDH_PORTABLE == 0
 
 .intel_syntax noprefix
 
 //#include "uintbig_namespace.h"
 //#include "fp_namespace.h"
 
 .section .rodata
```

### Comparing `highctidh-1.0.2024012400/ctidh512/fp_inv512.c` & `highctidh-1.0.2024050100/ctidh512/fp_inv512.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh512/fp_namespace.h` & `highctidh-1.0.2024050100/ctidh512/fp_namespace.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh512/fp_sqrt512.c` & `highctidh-1.0.2024050100/ctidh512/fp_sqrt512.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh512/int32_minmax.h` & `highctidh-1.0.2024050100/ctidh512/int32_minmax.h`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 // This is from the Public Domain djbsort-20190516
 /* this needs __attribute__((optimize)) >= 1 */
 
 #ifndef HIGHCTIDH_INT32_MINMAX_H
 #define HIGHCTIDH_INT32_MINMAX_H
 
-#if defined(__x86_64__) && !defined(HIGHCTIDH_PORTABLE)
+#if ((defined(__x86_64__) || defined(__i86pc__))) && HIGHCTIDH_PORTABLE == 0
 
 #define int32_MINMAX(a,b)			\
 do { \
   int32 temp1; \
   __asm__( \
     ".att_syntax prefix\n\t" \
     "cmpl %1,%0\n\t" \
```

### Comparing `highctidh-1.0.2024012400/ctidh512/int32_sort.c` & `highctidh-1.0.2024050100/ctidh512/int32_sort.c`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #ifndef HIGHCTIDH_INT32_SORT_H
 #define HIGHCTIDH_INT32_SORT_H
 
-#if defined(__AVX2__) && !defined(HIGHCTIDH_PORTABLE)
+#if defined(__AVX2__) && HIGHCTIDH_PORTABLE == 0
 
 // This is the original high-ctidh x86_64 sorting code
 #ifndef CGONUTS
 #include "int32_sort_x86.c"
 #endif // CGONUTS
 
 #else /* fallback to portable C code: */
```

### Comparing `highctidh-1.0.2024012400/ctidh512/int32_sort.h` & `highctidh-1.0.2024050100/ctidh512/int32_sort.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh512/int32_sort_x86.c` & `highctidh-1.0.2024050100/ctidh512/int32_sort_x86.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-#ifndef HIGHCTIDH_PORTABLE
-#ifdef __x86_64__
+#if HIGHCTIDH_PORTABLE == 0
+#if (defined(__x86_64__) || defined(__i86pc__)) && !defined(CGONUTS)
 #include "int32_sort.h"
 #define int32 int32_t
 
 #include <immintrin.h>
 #include "int32_minmax.h"
 
 typedef __m256i int32x8;
```

### Comparing `highctidh-1.0.2024012400/ctidh512/mont.c` & `highctidh-1.0.2024050100/ctidh512/mont.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh512/mont.h` & `highctidh-1.0.2024050100/ctidh512/mont.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh512/mont_namespace.h` & `highctidh-1.0.2024050100/ctidh512/mont_namespace.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh512/poly.c` & `highctidh-1.0.2024050100/ctidh512/poly.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh512/poly.h` & `highctidh-1.0.2024050100/ctidh512/poly.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh512/poly_namespace.h` & `highctidh-1.0.2024050100/ctidh512/poly_namespace.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh512/primes.h` & `highctidh-1.0.2024050100/ctidh512/primes.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh512/primes512.c` & `highctidh-1.0.2024050100/ctidh512/primes512.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh512/proj.h` & `highctidh-1.0.2024050100/ctidh512/proj.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh512/random.c` & `highctidh-1.0.2024050100/ctidh512/random.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh512/random.h` & `highctidh-1.0.2024050100/ctidh512/random.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh512/skgen.c` & `highctidh-1.0.2024050100/ctidh512/skgen.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh512/steps.c` & `highctidh-1.0.2024050100/ctidh512/steps.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh512/steps.h` & `highctidh-1.0.2024050100/ctidh512/steps.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh512/uintbig.h` & `highctidh-1.0.2024050100/ctidh512/uintbig.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-#ifndef uintbig_h
-#define uintbig_h
+#ifndef UINTBIG_H
+#define UINTBIG_H
 
 #include "uintbig_namespace.h"
 
 #include <stdbool.h>
 #include <stdint.h>
 #include "annotations.h"
```

### Comparing `highctidh-1.0.2024012400/ctidh512/uintbig512.S` & `highctidh-1.0.2024050100/ctidh512/uintbig512.S`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /* DO NOT EDIT! generated by ./autogen */
-#ifndef HIGHCTIDH_PORTABLE
+#if HIGHCTIDH_PORTABLE == 0
 
 .intel_syntax noprefix
 
 //#include "uintbig_namespace.h"
 
 .section .rodata
```

### Comparing `highctidh-1.0.2024012400/ctidh512/uintbig_namespace.h` & `highctidh-1.0.2024050100/ctidh512/uintbig_namespace.h`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+#ifndef UINTBIG_NAMESPACE_H
+#define UINTBIG_NAMESPACE_H
+
 #ifdef CGONUTS
 #include "cgo.h"
 #endif // CGONUTS
 
 #define uintbig_p NAMESPACEBITS(uintbig_p)
 #define uintbig_1 NAMESPACEBITS(uintbig_1)
 #define uintbig_bit NAMESPACEBITS(uintbig_bit)
@@ -12,7 +15,9 @@
 #define uintbig_mul3_64 NAMESPACEBITS(uintbig_mul3_64)
 #define uintbig_four_sqrt_p NAMESPACEBITS(uintbig_four_sqrt_p)
 #define uintbig NAMESPACEBITS(uintbig)
 #define uintbig_bits_vartime NAMESPACEBITS(uintbig_bits_vartime)
 #define uintbig_uint64_iszero NAMESPACEBITS(uintbig_uint64_iszero)
 #define uintbig_isequal NAMESPACEBITS(uintbig_isequal)
 #define uintbig_iszero NAMESPACEBITS(uintbig_iszero)
+
+#endif
```

### Comparing `highctidh-1.0.2024012400/ctidh512/validate.c` & `highctidh-1.0.2024050100/ctidh512/validate.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ctidh512/vectors512_test.go` & `highctidh-1.0.2024050100/ctidh512/vectors512_test.go`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/distmults.py` & `highctidh-1.0.2024050100/distmults.py`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/elligator.c` & `highctidh-1.0.2024050100/elligator.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/example-ctidh.c` & `highctidh-1.0.2024050100/example-ctidh.c`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,16 @@
   {
     printf("%02x", i[(unsigned char *) k]);
   }
   printf("\n");
   fflush(stdout);
 }
 
-int main()
+int main(void);
+int main(void)
 {
   private_key sk_a, sk_b;
   public_key pk_a, pk_b;
   public_key s_a, s_b;
   bool ok = 0;
 
   printf("CTIDH %i vector example\n\n", BITS);
```

### Comparing `highctidh-1.0.2024012400/examples_static.c` & `highctidh-1.0.2024050100/examples_static.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/fiat_p1024.c` & `highctidh-1.0.2024050100/fiat_p1024.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#if defined(HIGHCTIDH_PORTABLE)
+#if HIGHCTIDH_PORTABLE == 1
 #include "fiat_p1024.h"
 /* Autogenerated: './src/ExtractionOCaml/word_by_word_montgomery' --widen-bytes --internal-static --lang C -o f_1024.c p1024 64 10397125823368453045280646945602587680645373501407971524723936453540081402468763489237207685909470852314300607054838964876369377755966328162572638385477152807267330439309520268717606043270205686916407950751430775965737505772592082230763227336919124289210653129066316362633007647060631513541162047451995268179 */
 /* curve description: p1024 */
 /* machine_wordsize = 64 (from "64") */
 /* requested operations: (all) */
 /* m = 0xece55ed427012a9d89dec879007ebd7216c22bc86f21a080683cf25db31ad5bf06de2471cf9386e4d6c594a8ad82d2df811d9c419ec83297611ad4f90441c800978dbeed90a2b58b97c56d1de81ede56b317c5431541f40642aca4d5a313709c2cab6a0e287f1bd514ba72cb8d89fd3a1d81eebbc3d344ddbe34c5460e36453 (from "10397125823368453045280646945602587680645373501407971524723936453540081402468763489237207685909470852314300607054838964876369377755966328162572638385477152807267330439309520268717606043270205686916407950751430775965737505772592082230763227336919124289210653129066316362633007647060631513541162047451995268179") */
 /*                                                                    */
@@ -20039,8 +20039,10 @@
   out5[10] = x433;
   out5[11] = x434;
   out5[12] = x435;
   out5[13] = x436;
   out5[14] = x437;
   out5[15] = x438;
 }
+#else
+typedef int no_empty_translation_units_asm_1024; // -> "warning: ISO C forbids an empty translation unit"
 #endif
```

### Comparing `highctidh-1.0.2024012400/fiat_p1024.h` & `highctidh-1.0.2024050100/fiat_p1024.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/fiat_p2048.c` & `highctidh-1.0.2024050100/fiat_p2048.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#if defined(HIGHCTIDH_PORTABLE)
+#if HIGHCTIDH_PORTABLE == 1
 #include "fiat_p2048.h"
 /* Autogenerated: './src/ExtractionOCaml/word_by_word_montgomery' --widen-bytes --internal-static --lang C -o f_2048_high.c p2048 64 8528475943061024837635249434131089507352961229039071418359007853431472824232731281573875097585132124495905689769457289097290485066318818670998665693553484375832840901492721916443754108187759409880104977491168497435797029889150028375522118007040227895709956565527693986603274933373650307807559167751481868507471338172008086897049878117533316735319086656307962660962929231692405440348962572770958110754184132520227272603171250943083809093992306118654477172531039336755846450097401488026516556186294026830749211238807256327438743073467304920067034434209788101583120190178099235423322734627165016835534905946794432350531 */
 /* curve description: p2048 */
 /* machine_wordsize = 64 (from "64") */
 /* requested operations: (all) */
 /* m = 0x438efcab10254c6497fefc90e8196ed94d8854e8b3e19c53ddffdcf1aee53f12dbd1fc2133770253584eb12932f72abb33a8779a1ec8b8c2b8523d6a302abf284dd6024bf2f8feab6557ebe96d91aeddc68049793337525393e73abd17e3aa46095ac8a9f3ce2b0c30d2edfe50198c647d84f102b5fde2eae33586d1208a10179844e5c09baf59ec0da1783672767abb88c691b2d452a8ac7c4cb419996f45e75377d53e856cc9a39796620b3ad8a5d458e89497ef35bbb92842bbe4dbacc65e44084e1a73c76cb244454e851cf305aba7bec86fabaf787f6478407d7a9a56eee111b0d22ab8ecaa95a98036c813c788dc703f0cd8c4d9187790d615ea034943 (from "8528475943061024837635249434131089507352961229039071418359007853431472824232731281573875097585132124495905689769457289097290485066318818670998665693553484375832840901492721916443754108187759409880104977491168497435797029889150028375522118007040227895709956565527693986603274933373650307807559167751481868507471338172008086897049878117533316735319086656307962660962929231692405440348962572770958110754184132520227272603171250943083809093992306118654477172531039336755846450097401488026516556186294026830749211238807256327438743073467304920067034434209788101583120190178099235423322734627165016835534905946794432350531") */
 /*                                                                    */
@@ -73595,8 +73595,10 @@
   out5[26] = x849;
   out5[27] = x850;
   out5[28] = x851;
   out5[29] = x852;
   out5[30] = x853;
   out5[31] = x854;
 }
+#else
+typedef int no_empty_translation_units_asm_2048; // -> "warning: ISO C forbids an empty translation unit"
 #endif
```

### Comparing `highctidh-1.0.2024012400/fiat_p2048.h` & `highctidh-1.0.2024050100/fiat_p2048.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/fiat_p511.c` & `highctidh-1.0.2024050100/fiat_p511.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#if defined(HIGHCTIDH_PORTABLE)
+#if HIGHCTIDH_PORTABLE == 1
 #include "fiat_p511.h"
 /* Autogenerated: './src/ExtractionOCaml/word_by_word_montgomery' --internal-static --lang C -o fiat_p511.c p511 64 5326738796327623094747867617954605554069371494832722337612446642054009560026576537626892113026381253624626941643949444792662881241621373288942880288065659 */
 /* curve description: p511 */
 /* machine_wordsize = 64 (from "64") */
 /* requested operations: (all) */
 /* m = 0x65b48e8f740f89bffc8ab0d15e3e4c4ab42d083aedc88c425afbfcc69322c9cda7aac6c567f35507516730cc1f0b4f25c2721bf457aca8351b81b90533c6c87b (from "5326738796327623094747867617954605554069371494832722337612446642054009560026576537626892113026381253624626941643949444792662881241621373288942880288065659") */
 /*                                                                    */
@@ -6003,8 +6003,10 @@
   out5[2] = x225;
   out5[3] = x226;
   out5[4] = x227;
   out5[5] = x228;
   out5[6] = x229;
   out5[7] = x230;
 }
+#else
+typedef int no_empty_translation_units_asm_511; // -> "warning: ISO C forbids an empty translation unit"
 #endif
```

### Comparing `highctidh-1.0.2024012400/fiat_p511.h` & `highctidh-1.0.2024050100/fiat_p511.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/fiat_p512.c` & `highctidh-1.0.2024050100/fiat_p512.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#if defined(HIGHCTIDH_PORTABLE)
+#if HIGHCTIDH_PORTABLE == 1
 #include "fiat_p512.h"
 /* Autogenerated: './src/ExtractionOCaml/word_by_word_montgomery' --internal-static --lang C -o fiat_p512.c p512 64 5326738796327623094747867617954605554069371494832722337612446642054009560026576537626892113026381253624626941643949444792662881241621373288942880288065659 */
 /* curve description: p512 */
 /* machine_wordsize = 64 (from "64") */
 /* requested operations: (all) */
 /* m = 0x65b48e8f740f89bffc8ab0d15e3e4c4ab42d083aedc88c425afbfcc69322c9cda7aac6c567f35507516730cc1f0b4f25c2721bf457aca8351b81b90533c6c87b (from "5326738796327623094747867617954605554069371494832722337612446642054009560026576537626892113026381253624626941643949444792662881241621373288942880288065659") */
 /*                                                                    */
@@ -6003,8 +6003,10 @@
   out5[2] = x225;
   out5[3] = x226;
   out5[4] = x227;
   out5[5] = x228;
   out5[6] = x229;
   out5[7] = x230;
 }
+#else
+typedef int no_empty_translation_units_asm_512; // -> "warning: ISO C forbids an empty translation unit"
 #endif
```

### Comparing `highctidh-1.0.2024012400/fiat_p512.h` & `highctidh-1.0.2024050100/fiat_p512.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/fp.h` & `highctidh-1.0.2024050100/fp.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 #ifndef FP_H
 #define FP_H
 
 #include "fp_namespace.h"
 #include "uintbig.h"
 #include "annotations.h"
 
-#if defined(HIGHCTIDH_PORTABLE) || !(defined(__x86_64__) || defined(_M_X64))
+#if HIGHCTIDH_PORTABLE == 1 || !(defined(__x86_64__) || defined(_M_X64))
 /* we only have optimizations for amd64 so far, so on other platforms we
  * default to the portable code by defining HIGHCTIDH_PORTABLE:
  */
 #ifndef HIGHCTIDH_PORTABLE
-#define HIGHCTIDH_PORTABLE
+#define HIGHCTIDH_PORTABLE 1
 #endif
 
 #if 511 == BITS
 #include "fiat_p511.h"
 #elif 512 == BITS
 #include "fiat_p512.h"
 #elif 1024 == BITS
@@ -72,20 +72,22 @@
 void ATTR_INITIALIZE_1st
 __attribute__((nonnull))
 __attribute__((flatten))
 fp_mul3(fp *const x, fp const *const y, fp const *const z)
 	__attribute__ ((alias ("fiat_p512_mul")));
 */
 //void fp_mul3 () __attribute__ ((weak, alias ("fiat_p512_mul")));
-#ifdef HIGHCTIDH_PORTABLE
+#if HIGHCTIDH_PORTABLE == 1
 #define highctidh_511_fp_mul3(a,b,c) FIAT_BITS(mul)((uint64_t *)a,(const uint64_t*)b,(const uint64_t*)c)
 #define highctidh_512_fp_mul3(a,b,c) FIAT_BITS(mul)((uint64_t *)a,(const uint64_t*)b,(const uint64_t*)c)
 #define highctidh_1024_fp_mul3(a,b,c) FIAT_BITS(mul)((uint64_t *)a,(const uint64_t*)b,(const uint64_t*)c)
 #define highctidh_2048_fp_mul3(a,b,c) FIAT_BITS(mul)((uint64_t *)a,(const uint64_t*)b,(const uint64_t*)c)
-#else /* ndef HIGHCTIDH_PORTABLE */
+#endif
+
+#if HIGHCTIDH_PORTABLE == 0
 void fp_mul3(fp *const a, const fp *const b, const fp *const c);
 #endif /* ndef HIGHCTIDH_PORTABLE */
 
 void fp_sq1(fp *x);
 void fp_sq2(fp *const x, fp const *const y);
 
 extern long long fp_mulsq_count;
@@ -108,15 +110,15 @@
 /*
  * a := 0 - b
  */
 static inline
 __attribute__((nonnull))
 void fp_neg2(fp *const x,const fp *const y)
 {
-#ifdef HIGHCTIDH_PORTABLE
+#if HIGHCTIDH_PORTABLE == 1
 	FIAT_BITS(opp)(x->x.c, y->x.c);
 #else
 	fp_sub3(x, &fp_0, y);
 #endif
 }
 
 static inline void fp_double1(fp *const x)
```

### Comparing `highctidh-1.0.2024012400/fp1024.S` & `highctidh-1.0.2024050100/fp1024.S`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /* DO NOT EDIT! generated by ./autogen */
-#ifndef HIGHCTIDH_PORTABLE
+#if HIGHCTIDH_PORTABLE == 0
 
 .intel_syntax noprefix
 
 //#include "uintbig_namespace.h"
 //#include "fp_namespace.h"
 
 .section .rodata
```

### Comparing `highctidh-1.0.2024012400/fp2048.S` & `highctidh-1.0.2024050100/fp2048.S`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /* DO NOT EDIT! generated by ./autogen */
-#ifndef HIGHCTIDH_PORTABLE
+#if HIGHCTIDH_PORTABLE == 0
 
 .intel_syntax noprefix
 
 //#include "uintbig_namespace.h"
 //#include "fp_namespace.h"
 
 .section .rodata
```

### Comparing `highctidh-1.0.2024012400/fp2fiat.c` & `highctidh-1.0.2024050100/fp2fiat.c`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #include <string.h>
 
 
 #include "uintbig_namespace.h"
 #include "fp.h"
 #include "annotations.h"
 
-#if !defined(HIGHCTIDH_PORTABLE) && !defined(CGONUTS) && defined(__x86_64__)
+#if HIGHCTIDH_PORTABLE == 0 && !defined(CGONUTS) && (defined(__x86_64__) || defined(__i86pc__))
 #define highctidh_macro_stringize(x) #x
 #define highctidh_macro_str(y) highctidh_macro_stringize(y)
 __asm__ (".include \"uintbig" highctidh_macro_str(BITS)  ".S\"");
 __asm__ (".include \"fp" highctidh_macro_str(BITS) ".S\"");
 
 #elif defined(CGONUTS)
 #define DONTMINDIFIDO
```

### Comparing `highctidh-1.0.2024012400/fp511.S` & `highctidh-1.0.2024050100/fp511.S`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /* DO NOT EDIT! generated by ./autogen */
-#ifndef HIGHCTIDH_PORTABLE
+#if HIGHCTIDH_PORTABLE == 0
 
 .intel_syntax noprefix
 
 //#include "uintbig_namespace.h"
 //#include "fp_namespace.h"
 
 .section .rodata
```

### Comparing `highctidh-1.0.2024012400/fp512.S` & `highctidh-1.0.2024050100/fp512.S`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /* DO NOT EDIT! generated by ./autogen */
-#ifndef HIGHCTIDH_PORTABLE
+#if HIGHCTIDH_PORTABLE == 0
 
 .intel_syntax noprefix
 
 //#include "uintbig_namespace.h"
 //#include "fp_namespace.h"
 
 .section .rodata
```

### Comparing `highctidh-1.0.2024012400/fp_inv1024.c` & `highctidh-1.0.2024050100/fp_inv1024.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/fp_inv2048.c` & `highctidh-1.0.2024050100/fp_inv2048.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/fp_inv511.c` & `highctidh-1.0.2024050100/fp_inv511.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/fp_inv512.c` & `highctidh-1.0.2024050100/fp_inv512.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/fp_namespace.h` & `highctidh-1.0.2024050100/fp_namespace.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/fp_sqrt1024.c` & `highctidh-1.0.2024050100/fp_sqrt1024.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/fp_sqrt2048.c` & `highctidh-1.0.2024050100/fp_sqrt2048.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/fp_sqrt511.c` & `highctidh-1.0.2024050100/fp_sqrt511.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/fp_sqrt512.c` & `highctidh-1.0.2024050100/fp_sqrt512.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/go-tests/ctidh_test.go` & `highctidh-1.0.2024050100/go-tests/ctidh_test.go`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/greedy` & `highctidh-1.0.2024050100/greedy`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/highctidh.h` & `highctidh-1.0.2024050100/highctidh.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/highctidh/__init__.py` & `highctidh-1.0.2024050100/highctidh/__init__.py`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/highctidh_macros.h` & `highctidh-1.0.2024050100/highctidh_macros.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/int32_minmax.h` & `highctidh-1.0.2024050100/int32_minmax.h`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 // This is from the Public Domain djbsort-20190516
 /* this needs __attribute__((optimize)) >= 1 */
 
 #ifndef HIGHCTIDH_INT32_MINMAX_H
 #define HIGHCTIDH_INT32_MINMAX_H
 
-#if defined(__x86_64__) && !defined(HIGHCTIDH_PORTABLE)
+#if ((defined(__x86_64__) || defined(__i86pc__))) && HIGHCTIDH_PORTABLE == 0
 
 #define int32_MINMAX(a,b)			\
 do { \
   int32 temp1; \
   __asm__( \
     ".att_syntax prefix\n\t" \
     "cmpl %1,%0\n\t" \
```

### Comparing `highctidh-1.0.2024012400/int32_sort.c` & `highctidh-1.0.2024050100/int32_sort.c`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #ifndef HIGHCTIDH_INT32_SORT_H
 #define HIGHCTIDH_INT32_SORT_H
 
-#if defined(__AVX2__) && !defined(HIGHCTIDH_PORTABLE)
+#if defined(__AVX2__) && HIGHCTIDH_PORTABLE == 0
 
 // This is the original high-ctidh x86_64 sorting code
 #ifndef CGONUTS
 #include "int32_sort_x86.c"
 #endif // CGONUTS
 
 #else /* fallback to portable C code: */
```

### Comparing `highctidh-1.0.2024012400/int32_sort.h` & `highctidh-1.0.2024050100/int32_sort.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/int32_sort_x86.c` & `highctidh-1.0.2024050100/int32_sort_x86.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-#ifndef HIGHCTIDH_PORTABLE
-#ifdef __x86_64__
+#if HIGHCTIDH_PORTABLE == 0
+#if (defined(__x86_64__) || defined(__i86pc__)) && !defined(CGONUTS)
 #include "int32_sort.h"
 #define int32 int32_t
 
 #include <immintrin.h>
 #include "int32_minmax.h"
 
 typedef __m256i int32x8;
```

### Comparing `highctidh-1.0.2024012400/mont.c` & `highctidh-1.0.2024050100/mont.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/mont.h` & `highctidh-1.0.2024050100/mont.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/mont_namespace.h` & `highctidh-1.0.2024050100/mont_namespace.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/poly.c` & `highctidh-1.0.2024050100/poly.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/poly.h` & `highctidh-1.0.2024050100/poly.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/poly_namespace.h` & `highctidh-1.0.2024050100/poly_namespace.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/primes.h` & `highctidh-1.0.2024050100/primes.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/primes1024.c` & `highctidh-1.0.2024050100/primes1024.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/primes2048.c` & `highctidh-1.0.2024050100/primes2048.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/primes511.c` & `highctidh-1.0.2024050100/primes511.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/primes512.c` & `highctidh-1.0.2024050100/primes512.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/proj.h` & `highctidh-1.0.2024050100/proj.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/pyproject.toml` & `highctidh-1.0.2024050100/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "highctidh"
-version = "1.0.2024012400"
+version = "1.0.2024050100"
 description = "highctidh bindings with included C library"
 readme = "README.md"
 requires-python = ">=3.9.6"
 keywords = ["post-quantum cryptography", "cryptography", "csidh", "ctidh", "C", "highctidh"]
 authors = [ {email = "jacob@appelbaum.net"}, {name = "Jacob Appelbaum"} ]
 maintainers = [ {email = "jacob@appelbaum.net"}, {name = "Jacob Appelbaum"} ]
 dependencies = [ ]
```

### Comparing `highctidh-1.0.2024012400/random.c` & `highctidh-1.0.2024050100/random.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/random.h` & `highctidh-1.0.2024050100/random.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/setup.cfg` & `highctidh-1.0.2024050100/setup.cfg`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/sim.py` & `highctidh-1.0.2024050100/sim.py`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/skgen.c` & `highctidh-1.0.2024050100/skgen.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/steps.c` & `highctidh-1.0.2024050100/steps.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/steps.h` & `highctidh-1.0.2024050100/steps.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/test.c` & `highctidh-1.0.2024050100/test.c`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,24 @@
 #include "elligator.h"
 #include "csidh.h"
 #include "primes.h"
 #include "random.h"
 
 #if defined(__ARM32__) || defined(__i386__)
 #define DFMT "%#llxU, "
+#elif defined(__Darwin__)
+#define DFMT "%#llxU, "
+#elif defined(__OpenBSD__)
+#define DFMT "%#llxU, "
+#elif defined(__sun) && !defined(__i86pc__)
+#define DFMT "%#llxU, "
+#elif defined(__sun) && defined(__i86pc__)
+#define DFMT "%#lxU, "
+#elif (defined(__Windows__) || defined(__WIN64))
+#define DFMT "%#llxU, "
 #else
 #define DFMT "%#lxU, "
 #endif
 
 #define dump_uintbig(X) {for (size_t i=0; i<sizeof((X).c)/sizeof((X).c[0]);i++) { printf(DFMT, htole64((X).c[i])); };printf("\n"); }
 #define assert_uintbig_eq(X,Y) { \
 	for (size_t i = 0; i<sizeof(X.c)/sizeof(X.c[0]); i++) { \
@@ -141,16 +151,17 @@
 	struct context_list *next;
 } *test_fillrandom_context_list = NULL;
 
 /*
  * Resets the state of each element in the linked list of contexts,
  * returning the element count.
  */
+static size_t test_fillrandom_context_list_reset(void);
 static size_t
-test_fillrandom_context_list_reset()
+test_fillrandom_context_list_reset(void)
 {
 	size_t count = 0;
 	struct context_list *current = test_fillrandom_context_list;
 	while(current) {
 		count++;
 		current->state = (uintptr_t) current->ctx;
 		current = current->next;
@@ -178,21 +189,21 @@
 		*newcurrent = malloc(sizeof(struct context_list));
 		current = *newcurrent;
 		assert(current);
 		current->ctx = context;
 		current->state = context;
 		current->next = NULL;
 	}
-	assert(current);
-	size_t offset = current->state - context;
-	assert(offset + outsz < sizeof(test_fillrandom_buf)); // works for now
-	for (size_t i = 0; i < outsz; i++) {
-		((char*)out)[i] = test_fillrandom_buf[offset+i];
-	}
-	current->state += outsz;
+  assert(current);
+  size_t offset = current->state - context;
+  assert(offset + outsz < sizeof(test_fillrandom_buf)); // works for now
+  for (size_t i = 0; i < outsz; i++) {
+    ((char*)out)[i] = test_fillrandom_buf[offset+i];
+  }
+  current->state += outsz;
 }
 
 static uint64_t
 test_fillrandom_hash(uint64_t oldhash, char *outptr, size_t outsz)
 {
 	/* modified djb hash, endian-independent, NOT a safe CSPRNG: */
 	assert(outsz % 4 == 0);
@@ -401,45 +412,56 @@
 		}, /* test case 4 */
 	};
 	for (size_t t_idx = 0; t_idx < sizeof(tests)/sizeof(tests[0]); t_idx++)
 	{
 		test_vector *t = &tests[t_idx];
 		test_fillrandom_context_list_reset();
 		for(size_t i = 0; i < t->w + t->s; i++){
-			int32_t tmp = htole32(t->r[i]);
+			//int32_t tmp = htole32(t->r[i]);
+			int32_t tmp = t->r[i];
 			memcpy(test_fillrandom_buf + i*sizeof(tmp),
 			    &tmp, sizeof(tmp));
 		}
 		for(size_t i = 0; i < sizeof(t->r2)/sizeof(t->r2[0]); i++){
-			int32_t tmp = htole32(t->r2[i]);
+			//int32_t tmp = htole32(t->r2[i]);
+			int32_t tmp = t->r2[i];
 			memcpy(test_fillrandom_buf
 			    + (t->w + t->s)*sizeof(int32_t)
 			    + i*sizeof(tmp),
 			    &tmp, sizeof(tmp));
 		}
 		int8_t e[254] = {0};
 		random_boundedl1(e,t->w,t->s, 0, test_fillrandom_context_echoback);
 		if (0 != memcmp(e, t->e, sizeof(e))) {
 			printf("=== testcase %zd\n", t_idx);
+      printf("initial e: [");
+      for(size_t i = 0; i < sizeof(e); i++) {
+        printf("%d,", e[i]);
+      } printf("]\n");
 			printf("r_end: [");
 			for(size_t i = 0; i < sizeof(t->r)/sizeof(t->r[0]); i++) {
 				printf("%d,", t->r[i]);
 			} printf("]\n");
 			printf("e: [");
 			for(size_t i = 0; i < sizeof(e); i++) {
 				printf("%d,", e[i]);
 			} printf("]\n");
+			printf("t->e: [");
+			for(size_t i = 0; i < sizeof(e); i++) {
+				printf("%d,", t->e[i]);
+			} printf("]\n");
 			assert(0);
 		}
 	}
 	fflush(stdout);
 }
 
+static void test_deterministic_keygen(void);
 static void
-test_deterministic_keygen()
+test_deterministic_keygen(void)
 {
 	printf("deterministic_keygen\n"); fflush(stdout);
 	private_key priv_gh1 = {0};
 	private_key priv_gh2 = {0};
 	private_key priv_gh3 = {0};
 	test_fillrandom_global_hash = 0x123456789abcdef0U;
 	csidh_private_withrng(&priv_gh1, (uintptr_t) &priv_gh1, test_fillrandom_impl_global);
@@ -505,19 +527,31 @@
 	/* to_bytes / from_bytes are internally consistent: */
 	char serialized_gh3[sizeof(uintbig)] = {0};
 	public_key_to_bytes(serialized_gh3, &pub_gh3);
 	public_key deserialized_gh3 = {{{{0}}}};
 	public_key_from_bytes(&deserialized_gh3, serialized_gh3);
 	assert_uintbig_eq(pub_gh3.A.x, deserialized_gh3.A.x);
 	/* to_bytes is a no-op on little-endian archs, and not on big-endian: */
+
+// gcc -E -dM - </dev/null|grep -i __BYTE_ORDER
+# if defined(PLATFORM) && PLATFORM == sun4v || PLATFORM == i86pc
+# if __BYTE_ORDER__ == __ORDER_BIG_ENDIAN__
+  assert(0 != memcmp((void*)&pub_gh3, serialized_gh3, sizeof(pub_gh3)));
+# else
+	assert(0 == memcmp((void*)&pub_gh3, serialized_gh3, sizeof(pub_gh3)));
+# endif
+# endif
+
+# if !defined(__sun)
 # if __BYTE_ORDER == __LITTLE_ENDIAN
 	assert(0 == memcmp((void*)&pub_gh3, serialized_gh3, sizeof(pub_gh3)));
 # else
 	assert(0 != memcmp((void*)&pub_gh3, serialized_gh3, sizeof(pub_gh3)));
 # endif
+# endif
 }
 
 static void
 test_fp_sq2(void)
 {
 	printf("fp_sq2\n");
 	fflush(stdout);
@@ -877,16 +911,21 @@
       }
       A1 = A;
       for (long long j = 0;j < t;++j)
         P1[j] = P[j];
       xISOG(&A1,P1,t,&K,primes[i]);
 
       for (long long matryoshka = 0;matryoshka < 10;++matryoshka) {
+#if (defined(__Windows__) || defined(__WIN64))
+        long long ilower = rand()%(i+1);
+        long long iupper = i+(rand()%(primes_num-i));
+#else
         long long ilower = random()%(i+1);
         long long iupper = i+(random()%(primes_num-i));
+#endif
         A2 = A;
         for (long long j = 0;j < t;++j)
           P2[j] = P[j];
         xISOG_matryoshka(&A2,P2,t,&K,primes[i],primes[ilower],primes[iupper]);
         assert(proj_equal(&A2,&A1));
         for (long long j = 0;j < t;++j)
           assert(proj_equal(&P2[j],&P1[j]));
@@ -1453,15 +1492,16 @@
       assert(!memcmp(&check,&shared_alice,sizeof shared_alice));
   
       assert(!memcmp(&shared_alice, &shared_bob, sizeof(public_key)));
     }
   }
 }
 
-int main()
+int main(void);
+int main(void)
 {
   printf("%i tests\n", BITS);
   fflush(stdout);
   test_iszero();
   test_uintbig_bit();
   test_uintbig_mul3_64();
   test_fillrandom();
```

### Comparing `highctidh-1.0.2024012400/test.sh` & `highctidh-1.0.2024050100/test.sh`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/testrandom.c` & `highctidh-1.0.2024050100/testrandom.c`

 * *Files 2% similar despite different names*

```diff
@@ -268,15 +268,16 @@
         assert(freq[i] >= 16384-1536);
         assert(freq[i] <= 16384+1536);
       }
     }
   }
 }
 
-int main()
+int main(void);
+int main(void)
 {
   test_batchkeys();
   test_random_coin();
   test_boundedl1_2();
   test_boundedl1_3();
   test_boundedl1_generic();
   return 0;
```

### Comparing `highctidh-1.0.2024012400/tests/test_highctidh.py` & `highctidh-1.0.2024050100/tests/test_highctidh.py`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/tune2c` & `highctidh-1.0.2024050100/tune2c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/tunecycles.c` & `highctidh-1.0.2024050100/tunecycles.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/tunemults.c` & `highctidh-1.0.2024050100/tunemults.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/ubench.c` & `highctidh-1.0.2024050100/ubench.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/uintbig.h` & `highctidh-1.0.2024050100/uintbig.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-#ifndef uintbig_h
-#define uintbig_h
+#ifndef UINTBIG_H
+#define UINTBIG_H
 
 #include "uintbig_namespace.h"
 
 #include <stdbool.h>
 #include <stdint.h>
 #include "annotations.h"
```

### Comparing `highctidh-1.0.2024012400/uintbig1024.S` & `highctidh-1.0.2024050100/uintbig1024.S`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /* DO NOT EDIT! generated by ./autogen */
-#ifndef HIGHCTIDH_PORTABLE
+#if HIGHCTIDH_PORTABLE == 0
 
 .intel_syntax noprefix
 
 //#include "uintbig_namespace.h"
 
 .section .rodata
```

### Comparing `highctidh-1.0.2024012400/uintbig2048.S` & `highctidh-1.0.2024050100/uintbig2048.S`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /* DO NOT EDIT! generated by ./autogen */
-#ifndef HIGHCTIDH_PORTABLE
+#if HIGHCTIDH_PORTABLE == 0
 
 .intel_syntax noprefix
 
 //#include "uintbig_namespace.h"
 
 .section .rodata
```

### Comparing `highctidh-1.0.2024012400/uintbig511.S` & `highctidh-1.0.2024050100/uintbig511.S`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /* DO NOT EDIT! generated by ./autogen */
-#ifndef HIGHCTIDH_PORTABLE
+#if HIGHCTIDH_PORTABLE == 0
 
 .intel_syntax noprefix
 
 //#include "uintbig_namespace.h"
 
 .section .rodata
```

### Comparing `highctidh-1.0.2024012400/uintbig512.S` & `highctidh-1.0.2024050100/uintbig512.S`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /* DO NOT EDIT! generated by ./autogen */
-#ifndef HIGHCTIDH_PORTABLE
+#if HIGHCTIDH_PORTABLE == 0
 
 .intel_syntax noprefix
 
 //#include "uintbig_namespace.h"
 
 .section .rodata
```

### Comparing `highctidh-1.0.2024012400/uintbig_namespace.h` & `highctidh-1.0.2024050100/uintbig_namespace.h`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+#ifndef UINTBIG_NAMESPACE_H
+#define UINTBIG_NAMESPACE_H
+
 #ifdef CGONUTS
 #include "cgo.h"
 #endif // CGONUTS
 
 #define uintbig_p NAMESPACEBITS(uintbig_p)
 #define uintbig_1 NAMESPACEBITS(uintbig_1)
 #define uintbig_bit NAMESPACEBITS(uintbig_bit)
@@ -12,7 +15,9 @@
 #define uintbig_mul3_64 NAMESPACEBITS(uintbig_mul3_64)
 #define uintbig_four_sqrt_p NAMESPACEBITS(uintbig_four_sqrt_p)
 #define uintbig NAMESPACEBITS(uintbig)
 #define uintbig_bits_vartime NAMESPACEBITS(uintbig_bits_vartime)
 #define uintbig_uint64_iszero NAMESPACEBITS(uintbig_uint64_iszero)
 #define uintbig_isequal NAMESPACEBITS(uintbig_isequal)
 #define uintbig_iszero NAMESPACEBITS(uintbig_iszero)
+
+#endif
```

### Comparing `highctidh-1.0.2024012400/umults.c` & `highctidh-1.0.2024050100/umults.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/validate.c` & `highctidh-1.0.2024050100/validate.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024012400/PKG-INFO` & `highctidh-1.0.2024050100/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: highctidh
-Version: 1.0.2024012400
+Version: 1.0.2024050100
 Summary: highctidh bindings with included C library
 Keywords: post-quantum cryptography,cryptography,csidh,ctidh,C,highctidh
 Author: Jacob Appelbaum
 Author-email: jacob@appelbaum.net
 Maintainer: Jacob Appelbaum
 Maintainer-email: jacob@appelbaum.net
 Requires-Python: >=3.9.6
@@ -71,18 +71,26 @@
 sudo dpkg -i python3-highctidh_*.deb
 ```
 
 ## Golang bindings
 
 Add the golang bindings to a golang project:
 ```
-go get -u https://codeberg.org/vula/highctidh/ctidh511
-go get -u https://codeberg.org/vula/highctidh/ctidh512
-go get -u https://codeberg.org/vula/highctidh/ctidh1024
-go get -u https://codeberg.org/vula/highctidh/ctidh2048
+go get -u codeberg.org/vula/highctidh/
+```
+
+Use the golang bindings in a `.go` file by importing the field size that is
+desired or by importing any or all of the four field sizes:
+```
+import (
+    ctidh511  "codeberg.org/vula/highctidh/src/ctidh511"
+    ctidh512  "codeberg.org/vula/highctidh/src/ctidh512"
+    ctidh1024 "codeberg.org/vula/highctidh/src/ctidh1024"
+    ctidh2048 "codeberg.org/vula/highctidh/src/ctidh2048"
+) 
 ```
 
 # highctidh improvements
 
 This fork enhances high-ctidh with additional Makefile targets including
 building high-ctidh as four shared libraries, one for each key size of 511,
 512, 1024, and 2048. Python bindings are additionally added, as well as
@@ -93,15 +101,15 @@
 fast on the `amd64`/`x86_64` CPU architecture and functional but much slower
 with other CPU architectures. The portable backend was generated using the
 `fiat-crypto` project which uses a "Correct-by-Construction" approach; see
 `doc/PRIMES.md` for more information.  Tested architectures for the C library
 include: `amd64`/`x86_64`  (with and without avx2), `arm32v5`, `arm32v6`,
 `arm32v7`, `arm64v8`/`aarch64`/`arm64`, `i386`, `loongarch64/Loongson`, `mips`,
 `mipsel`, `mips64`, `mips64el`, `POWER8/ppc64`, `POWER9/ppc64le`, `riscv64`,
-`s390x`, and `sparc64`.
+`s390x`, `sun4v`, and `sparc64`.
 
 ## Golang bindings
 
 The Golang bindings compile and should be functional on `amd64`/`x86_64`,
 `arm32v5`, `arm32v6`, `arm32v7`, `arm64v8`/`aarch64`/`arm64`, `i386`, `ppc64`,
 `ppc64le`, `riscv64`, `s390x`, `mips`, `mipsle`, `mips64`, `mips64le`.  The
 `misc/test-golang-cross.sh` script runs tests on the host build architecture
@@ -140,31 +148,49 @@
 
 To test without installing run the `test` target:
 ```
    make test
 ```
 
 The C library and bindings have been tested on the following operating systems:
-- Alpine v3.18 (musl libc)
-- Alpine v3.19 (musl libc)
-- CheriBSD
-- Debian Sid (GNU libc)
-- Debian Bookworm (GNU libc)
-- FreeBSD
+- AlmaLinux 9.3 (GNU libc)
+- Alpine v3.17 - v3.19.1 (musl libc)
+- Arch latest (GNU libc)
+- CheriBSD 14.0-CURRENT (FreeBSD libc)
+- Clear Linux 41560 (GNU libc)
+- Debian stable, testing, unstable (GNU libc)
+- Devuan latest (GNU libc)
+- DragonFlyBSD 6.4.0 (FreeBSD libc)
+- Fedora 38, 39, 40, 41 (GNU libc)
+- FreeBSD 14.0 (FreeBSD libc)
 - HardenedBSD (FreeBSD libc)
-- MacOS
-- OpenBSD
-- Ubuntu Mantic (GNU libc)
-- Ubuntu Noble (GNU libc)
+- MacOS 11, 12, 13, 14 (BSD libc)
+- NetBSD 10.0 (NetBSD libc)
+- Omnios r151046 (illumos libc)
+- OpenBSD 7.5 (OpenBSD libc)
+- Oracle Linux 9 (GNU libc)
+- Rockylinux 9, 9.3 (GNU libc)
+- Solaris 11.4 (Solaris libc)
+- Ubuntu 22.03, 23.10, 24.04 (GNU libc)
+- Windows Server 2019, 2022 (MSVCRT)
 
 ## Notes on building
 
-Building on CheriBSD, FreeBSD, and OpenBSD building is supported using the
+Building on Solaris, CheriBSD, FreeBSD, NetBSD, and OpenBSD building is supported using the
 `gmake` command. GNU/Linux and MacOS are supported with the `make` command.
 
+Windows support is extremely experimental. The Python and Golang modules may
+not be functional on Windows. Building the main C library on Windows Server
+2019 and Windows Server 2022 should be possible with `clang` as is demonstrated
+in the continuous integration configuration `windows-fiat-c-library-test.yml`.
+It has only been tested with the Windows Server 2022 image preloaded with
+`clang`, `bash`, `make`, and other related tools
+[https://github.com/actions/runner-images/blob/main/images/windows/Windows2022-Readme.md](available
+as a part of the CI configuration).
+
 ### Additional notes on building the C library
  
 To build and install we recommend:
 ```
    sudo apt install gcc clang make
    make
    sudo make install
@@ -223,15 +249,15 @@
 The original website was https://ctidh.isogeny.org/software.html
 
 # Acknowledgements
 
 The original authors of this software released high-ctidh in the public domain.
 All contributions made in this fork are also in the public domain.
 
-Please consult `docs/AUTHORS.md` for the original authorship informaton.
+Please consult `docs/AUTHORS.md` for the original authorship information.
 
 This forked project is funded through the [NGI Assure
 Fund](https://nlnet.nl/assure), a fund established by [NLnet](https://nlnet.nl)
 with financial support from the European Commission's [Next Generation
 Internet](https://ngi.eu) program. Learn more on the [NLnet project
 page](https://nlnet.nl/project/Vula#ack).
```

