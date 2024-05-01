# Comparing `tmp/fedrq-1.0.0.tar.gz` & `tmp/fedrq-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fedrq-1.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "fedrq-1.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fedrq-1.0.0.tar` & `fedrq-1.1.0.tar`

### file list

```diff
@@ -1,167 +1,167 @@
--rw-r--r--   0        0        0      532 2023-09-23 07:50:00.855336 fedrq-1.0.0/.builds/epel9.yml
--rw-r--r--   0        0        0     2105 2023-09-23 07:50:00.856336 fedrq-1.0.0/.builds/main.yml
--rw-r--r--   0        0        0      809 2023-09-23 07:50:00.856336 fedrq-1.0.0/.builds/mockbuild.yml
--rw-r--r--   0        0        0      473 2023-12-10 19:23:08.443940 fedrq-1.0.0/.builds/test.yml
--rw-r--r--   0        0        0      384 2024-03-02 00:23:56.673824 fedrq-1.0.0/.copr/Makefile
-lrwxr-xr-x   0        0        0        0 2023-06-26 23:03:24.119349 fedrq-1.0.0/.data/share/licenses/fedrq/GPL-2.0-or-later.txt -> ../../../../LICENSES/GPL-2.0-or-later.txt
-lrwxr-xr-x   0        0        0        0 2023-06-26 23:03:24.119349 fedrq-1.0.0/.data/share/licenses/fedrq/MIT.txt -> ../../../../LICENSES/MIT.txt
-lrwxr-xr-x   0        0        0        0 2023-06-26 23:03:24.119349 fedrq-1.0.0/.data/share/licenses/fedrq/PSF-2.0.txt -> ../../../../LICENSES/PSF-2.0.txt
-lrwxr-xr-x   0        0        0        0 2023-06-26 23:03:24.119349 fedrq-1.0.0/.data/share/licenses/fedrq/Unlicense.txt -> ../../../../LICENSES/Unlicense.txt
-lrwxr-xr-x   0        0        0        0 2024-02-27 23:08:32.868655 fedrq-1.0.0/.dockerignore -> .gitignore
--rw-r--r--   0        0        0      287 2024-04-01 17:06:49.284414 fedrq-1.0.0/.gitignore
--rw-r--r--   0        0        0      155 2023-09-23 07:50:00.857336 fedrq-1.0.0/.reuse/dep5
--rw-r--r--   0        0        0     2553 2023-06-26 23:03:24.119349 fedrq-1.0.0/CONTRIBUTING.md
--rw-r--r--   0        0        0      673 2024-02-28 18:14:09.530518 fedrq-1.0.0/Containerfile
--rw-r--r--   0        0        0      817 2024-02-28 18:14:09.531518 fedrq-1.0.0/Containerfile.rhel
--rw-r--r--   0        0        0     1564 2024-02-28 18:14:09.532518 fedrq-1.0.0/Containerfile.rhel8
--rw-r--r--   0        0        0    17337 2023-06-26 23:03:24.120349 fedrq-1.0.0/LICENSES/GPL-2.0-or-later.txt
--rw-r--r--   0        0        0     1078 2023-06-26 23:03:24.120349 fedrq-1.0.0/LICENSES/MIT.txt
--rw-r--r--   0        0        0     2427 2023-06-26 23:03:24.120349 fedrq-1.0.0/LICENSES/PSF-2.0.txt
--rw-r--r--   0        0        0     1211 2023-06-26 23:03:24.120349 fedrq-1.0.0/LICENSES/Unlicense.txt
--rw-r--r--   0        0        0    19096 2024-04-01 17:09:57.580057 fedrq-1.0.0/NEWS.md
--rw-r--r--   0        0        0       89 2023-06-26 23:03:24.120349 fedrq-1.0.0/NEWS.md.license
--rw-r--r--   0        0        0    13182 2024-02-09 05:24:13.924912 fedrq-1.0.0/README.md
--rwxr-xr-x   0        0        0      687 2023-06-26 23:03:24.121349 fedrq-1.0.0/contrib/add_frag.py
--rwxr-xr-x   0        0        0      906 2023-06-26 23:03:24.121349 fedrq-1.0.0/contrib/api_examples/a_noarch_bash.py
--rwxr-xr-x   0        0        0     2502 2023-06-26 23:03:24.121349 fedrq-1.0.0/contrib/api_examples/ftbfs_retirements.py
--rw-r--r--   0        0        0      103 2023-09-23 07:50:00.861336 fedrq-1.0.0/contrib/container/000-container.toml
--rw-r--r--   0        0        0      641 2024-02-28 18:14:09.532518 fedrq-1.0.0/contrib/container/Containerfile
--rw-r--r--   0        0        0      722 2024-02-28 18:14:09.533518 fedrq-1.0.0/contrib/container/Containerfile.rhel
--rw-r--r--   0        0        0      759 2023-10-15 18:51:34.227066 fedrq-1.0.0/contrib/container/build.yml
--rwxr-xr-x   0        0        0      296 2023-09-23 07:50:00.863336 fedrq-1.0.0/contrib/container/entrypoint.sh
--rw-r--r--   0        0        0      544 2023-09-23 07:50:00.863336 fedrq-1.0.0/contrib/container/rhel.toml
--rw-r--r--   0        0        0      544 2024-02-28 18:14:09.533518 fedrq-1.0.0/contrib/container/rhel8.toml
--rw-r--r--   0        0        0      630 2023-06-26 23:03:24.121349 fedrq-1.0.0/contrib/deploy-docsite/main.yaml
--rw-r--r--   0        0        0      183 2023-06-26 23:03:24.122349 fedrq-1.0.0/contrib/deploy-docsite/roles/configure/handlers/main.yaml
--rw-r--r--   0        0        0      885 2023-06-26 23:03:24.122349 fedrq-1.0.0/contrib/deploy-docsite/roles/configure/tasks/main.yml
--rw-r--r--   0        0        0      284 2023-09-18 05:35:56.213359 fedrq-1.0.0/contrib/deploy-docsite/roles/configure/templates/fedrq.caddyfile
--rw-r--r--   0        0        0      415 2023-06-26 23:03:24.122349 fedrq-1.0.0/contrib/deploy-docsite/roles/deploy/tasks/main.yaml
--rw-r--r--   0        0        0      156 2023-06-26 23:03:24.123349 fedrq-1.0.0/contrib/deploy-docsite/vars.yaml
--rwxr-xr-x   0        0        0      914 2023-06-26 23:03:24.123349 fedrq-1.0.0/contrib/fedoraify.py
--rw-r--r--   0        0        0     6047 2024-03-18 02:08:06.660954 fedrq-1.0.0/doc/API/Summary.md
--rw-r--r--   0        0        0      204 2023-12-08 02:08:39.952633 fedrq-1.0.0/doc/API/_archive.md
--rw-r--r--   0        0        0      147 2023-06-26 23:03:24.123349 fedrq-1.0.0/doc/API/backends/base.md
--rw-r--r--   0        0        0      343 2023-06-26 23:03:24.123349 fedrq-1.0.0/doc/API/backends/dnf.md
--rw-r--r--   0        0        0      532 2023-06-26 23:03:24.123349 fedrq-1.0.0/doc/API/backends/libdnf5.md
--rw-r--r--   0        0        0      133 2023-06-26 23:03:24.123349 fedrq-1.0.0/doc/API/config.md
--rw-r--r--   0        0        0      214 2023-12-08 02:07:21.668887 fedrq-1.0.0/doc/API/release_repo.md
-lrwxr-xr-x   0        0        0        0 2023-06-26 23:03:24.124349 fedrq-1.0.0/doc/News.md -> ../NEWS.md
--rw-r--r--   0        0        0     4254 2024-02-09 05:26:11.065414 fedrq-1.0.0/doc/dnf-repoquery-diff.md
--rw-r--r--   0        0        0    21314 2024-04-01 16:51:28.499461 fedrq-1.0.0/doc/fedrq.1.scd
--rw-r--r--   0        0        0       98 2023-06-26 23:03:24.124349 fedrq-1.0.0/doc/fedrq.1.scd.license
--rw-r--r--   0        0        0     5024 2024-02-08 21:05:40.487851 fedrq-1.0.0/doc/fedrq.5.scd
--rw-r--r--   0        0        0       98 2023-06-26 23:03:24.125349 fedrq-1.0.0/doc/fedrq.5.scd.license
-lrwxr-xr-x   0        0        0        0 2023-06-26 23:03:24.125349 fedrq-1.0.0/doc/index.md -> ../README.md
--rw-r--r--   0        0        0      583 2024-02-08 21:00:35.705899 fedrq-1.0.0/doc/mkdocs_mangen.py
--rw-r--r--   0        0        0      193 2023-06-26 23:03:24.125349 fedrq-1.0.0/fedrq.rpmlintrc
--rw-r--r--   0        0        0     4292 2024-04-01 17:09:56.826058 fedrq-1.0.0/fedrq.spec
--rw-r--r--   0        0        0     2300 2024-02-08 20:47:24.834435 fedrq-1.0.0/mkdocs.yml
--rw-r--r--   0        0        0     8384 2024-04-01 17:08:37.764166 fedrq-1.0.0/noxfile.py
--rw-r--r--   0        0        0     4001 2024-02-09 05:28:42.366800 fedrq-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     4849 2024-04-01 16:53:31.810130 fedrq-1.0.0/requirements/all.txt
--rw-r--r--   0        0        0     1118 2024-03-25 01:38:31.567468 fedrq-1.0.0/requirements/codeqa.txt
--rw-r--r--   0        0        0     3820 2024-04-01 16:53:31.811130 fedrq-1.0.0/requirements/doc.txt
--rw-r--r--   0        0        0     1019 2024-03-18 01:55:52.346007 fedrq-1.0.0/requirements/formatters.txt
--rw-r--r--   0        0        0       13 2023-09-23 07:50:00.868336 fedrq-1.0.0/requirements/pydanticv1.in
--rw-r--r--   0        0        0     1030 2024-03-25 01:38:31.569468 fedrq-1.0.0/requirements/pydanticv1_test.txt
--rw-r--r--   0        0        0     1516 2023-09-23 07:50:00.868336 fedrq-1.0.0/requirements/refresh.yml
--rw-r--r--   0        0        0      703 2024-03-18 01:55:52.346007 fedrq-1.0.0/requirements/requirements.txt
--rw-r--r--   0        0        0        7 2023-09-23 07:50:00.869336 fedrq-1.0.0/requirements/srpm.in
--rw-r--r--   0        0        0      448 2024-04-01 16:53:31.811130 fedrq-1.0.0/requirements/srpm.txt
--rw-r--r--   0        0        0     1044 2024-03-25 01:38:31.570468 fedrq-1.0.0/requirements/test.txt
--rw-r--r--   0        0        0     1056 2024-03-18 01:55:52.346007 fedrq-1.0.0/requirements/typing.txt
--rw-r--r--   0        0        0     1162 2024-03-18 02:02:24.166704 fedrq-1.0.0/ruff.toml
--rw-r--r--   0        0        0      753 2024-04-01 17:09:50.809067 fedrq-1.0.0/src/fedrq/__init__.py
--rw-r--r--   0        0        0      219 2023-06-26 23:03:24.126349 fedrq-1.0.0/src/fedrq/__main__.py
--rw-r--r--   0        0        0     2822 2024-01-07 21:00:32.692014 fedrq-1.0.0/src/fedrq/_archive.py
--rw-r--r--   0        0        0     1713 2023-09-11 04:00:33.008787 fedrq-1.0.0/src/fedrq/_compat.py
--rw-r--r--   0        0        0      173 2023-06-26 23:03:24.126349 fedrq-1.0.0/src/fedrq/_config.py
--rw-r--r--   0        0        0     1370 2023-12-23 06:34:35.309654 fedrq-1.0.0/src/fedrq/_utils.py
--rw-r--r--   0        0        0     2645 2023-12-18 18:23:31.398146 fedrq-1.0.0/src/fedrq/backends/__init__.py
--rw-r--r--   0        0        0    17124 2024-01-30 01:19:25.798526 fedrq-1.0.0/src/fedrq/backends/base/__init__.py
--rw-r--r--   0        0        0      630 2023-06-26 23:03:24.127349 fedrq-1.0.0/src/fedrq/backends/dnf/__init__.py
--rw-r--r--   0        0        0     8305 2024-02-13 03:17:16.970902 fedrq-1.0.0/src/fedrq/backends/dnf/backend/__init__.py
--rw-r--r--   0        0        0      629 2023-09-23 07:50:00.872336 fedrq-1.0.0/src/fedrq/backends/libdnf5/__init__.py
--rw-r--r--   0        0        0    27966 2024-01-08 18:50:00.087299 fedrq-1.0.0/src/fedrq/backends/libdnf5/backend/__init__.py
--rw-r--r--   0        0        0     2667 2024-02-07 02:23:15.413353 fedrq-1.0.0/src/fedrq/cli/__init__.py
--rw-r--r--   0        0        0    17869 2024-02-28 18:14:09.546517 fedrq-1.0.0/src/fedrq/cli/base.py
--rw-r--r--   0        0        0      758 2023-11-06 03:39:21.572134 fedrq-1.0.0/src/fedrq/cli/commands/COMMAND.py.in
--rw-r--r--   0        0        0        0 2023-06-26 23:03:24.129349 fedrq-1.0.0/src/fedrq/cli/commands/__init__.py
--rw-r--r--   0        0        0     1228 2023-11-06 23:45:40.679278 fedrq-1.0.0/src/fedrq/cli/commands/cache.py
--rw-r--r--   0        0        0     2427 2024-02-11 23:38:01.083470 fedrq-1.0.0/src/fedrq/cli/commands/changelogs.py
--rw-r--r--   0        0        0     6390 2024-01-07 21:00:32.693014 fedrq-1.0.0/src/fedrq/cli/commands/download.py
--rw-r--r--   0        0        0     1926 2024-02-07 02:26:01.958945 fedrq-1.0.0/src/fedrq/cli/commands/formatters.py
--rw-r--r--   0        0        0     1729 2023-11-06 04:24:41.488764 fedrq-1.0.0/src/fedrq/cli/commands/pkgs.py
--rw-r--r--   0        0        0     1425 2023-09-23 07:50:00.875336 fedrq-1.0.0/src/fedrq/cli/commands/repolist.py
--rw-r--r--   0        0        0     2394 2023-09-23 07:50:00.876336 fedrq-1.0.0/src/fedrq/cli/commands/subpkgs.py
--rw-r--r--   0        0        0    10927 2024-03-02 04:35:52.918510 fedrq-1.0.0/src/fedrq/cli/commands/whatrequires.py
--rw-r--r--   0        0        0    18643 2024-03-18 01:57:56.367426 fedrq-1.0.0/src/fedrq/cli/formatters.py
--rw-r--r--   0        0        0    16327 2024-01-08 17:19:25.034112 fedrq-1.0.0/src/fedrq/config.py
--rw-r--r--   0        0        0        0 2023-06-26 23:03:24.131349 fedrq-1.0.0/src/fedrq/data/__init__.py
--rw-r--r--   0        0        0     9590 2023-12-20 20:41:15.739589 fedrq-1.0.0/src/fedrq/data/releases.toml
--rw-r--r--   0        0        0        0 2023-06-26 23:03:24.131349 fedrq-1.0.0/src/fedrq/data/repos/__init__.py
--rw-r--r--   0        0        0     2053 2023-06-26 23:03:24.131349 fedrq-1.0.0/src/fedrq/data/repos/almalinux.repo
--rw-r--r--   0        0        0      639 2023-06-26 23:03:24.131349 fedrq-1.0.0/src/fedrq/data/repos/amazonlinux.repo
--rw-r--r--   0        0        0     1386 2023-06-26 23:03:24.132349 fedrq-1.0.0/src/fedrq/data/repos/centos-stream-compose.repo
--rw-r--r--   0        0        0     1850 2023-06-26 23:03:24.132349 fedrq-1.0.0/src/fedrq/data/repos/centos-stream.repo
--rw-r--r--   0        0        0     1494 2023-06-26 23:03:24.132349 fedrq-1.0.0/src/fedrq/data/repos/centos-stream8-compose.repo
--rw-r--r--   0        0        0     1599 2023-06-26 23:03:24.132349 fedrq-1.0.0/src/fedrq/data/repos/centos-stream8.repo
--rw-r--r--   0        0        0     1342 2023-06-26 23:03:24.132349 fedrq-1.0.0/src/fedrq/data/repos/centos7.repo
--rw-r--r--   0        0        0      389 2023-12-20 20:39:55.482913 fedrq-1.0.0/src/fedrq/data/repos/eln-buildroot.repo
--rw-r--r--   0        0        0     1809 2023-06-26 23:03:24.132349 fedrq-1.0.0/src/fedrq/data/repos/eln.repo
--rw-r--r--   0        0        0     2158 2023-06-26 23:03:24.132349 fedrq-1.0.0/src/fedrq/data/repos/epel.repo
--rw-r--r--   0        0        0    14146 2023-06-26 23:03:24.132349 fedrq-1.0.0/src/fedrq/data/repos/fedora-eln.repo
--rw-r--r--   0        0        0     2402 2023-06-26 23:03:24.133349 fedrq-1.0.0/src/fedrq/data/repos/fedora-rawhide.repo
--rw-r--r--   0        0        0     1480 2023-06-26 23:03:24.133349 fedrq-1.0.0/src/fedrq/data/repos/fedora-updates-testing.repo
--rw-r--r--   0        0        0     1422 2023-09-23 07:50:00.878336 fedrq-1.0.0/src/fedrq/data/repos/fedora-updates.repo
--rw-r--r--   0        0        0     1375 2023-09-23 07:50:00.878336 fedrq-1.0.0/src/fedrq/data/repos/fedora.repo
--rw-r--r--   0        0        0     1374 2023-09-23 07:50:00.878336 fedrq-1.0.0/src/fedrq/data/repos/oraclelinux-8.repo
--rw-r--r--   0        0        0     1374 2023-09-23 07:50:00.878336 fedrq-1.0.0/src/fedrq/data/repos/oraclelinux-9.repo
--rw-r--r--   0        0        0      425 2023-06-26 23:03:24.133349 fedrq-1.0.0/src/fedrq/data/repos/rawhide-buildroot.repo
--rw-r--r--   0        0        0     6475 2023-09-23 07:50:00.878336 fedrq-1.0.0/src/fedrq/data/repos/rocky.repo
--rw-r--r--   0        0        0     3505 2023-09-23 07:50:00.878336 fedrq-1.0.0/src/fedrq/data/repos/ubi.repo
--rw-r--r--   0        0        0        0 2023-06-26 23:03:24.133349 fedrq-1.0.0/src/fedrq/py.typed
--rw-r--r--   0        0        0     9259 2024-01-30 01:19:25.593526 fedrq-1.0.0/src/fedrq/release_repo.py
--rw-r--r--   0        0        0     1828 2024-01-08 18:49:59.600302 fedrq-1.0.0/src/fedrq/repoquery.py
--rw-r--r--   0        0        0      154 2023-06-26 23:03:24.134349 fedrq-1.0.0/tests/.gitignore
--rw-r--r--   0        0        0        0 2023-06-26 23:03:24.134349 fedrq-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0     2988 2023-09-23 07:50:00.879336 fedrq-1.0.0/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-06-26 23:03:24.134349 fedrq-1.0.0/tests/integration/__init__.py
--rw-r--r--   0        0        0     1748 2023-09-23 07:50:00.880336 fedrq-1.0.0/tests/integration/test_backends.py
--rw-r--r--   0        0        0      405 2023-11-06 23:48:33.545619 fedrq-1.0.0/tests/integration/test_cache.py
--rw-r--r--   0        0        0      553 2023-09-23 07:50:00.880336 fedrq-1.0.0/tests/integration/test_download.py
--rw-r--r--   0        0        0      988 2023-09-23 07:50:00.880336 fedrq-1.0.0/tests/integration/test_pkgs.py
--rw-r--r--   0        0        0     1483 2023-09-23 07:50:00.880336 fedrq-1.0.0/tests/integration/test_subpkgs.py
--rw-r--r--   0        0        0     1964 2023-09-23 07:50:00.880336 fedrq-1.0.0/tests/integration/test_whatrequires.py
--rw-r--r--   0        0        0     1447 2023-09-23 07:50:00.881336 fedrq-1.0.0/tests/integration/test_whatrequires_src.py
--rw-r--r--   0        0        0        0 2023-06-26 23:03:24.135349 fedrq-1.0.0/tests/test_data/__init__.py
--rw-r--r--   0        0        0      408 2024-02-07 03:25:08.056407 fedrq-1.0.0/tests/test_data/_template.spec
--rwxr-xr-x   0        0        0     1484 2024-02-28 18:14:09.546517 fedrq-1.0.0/tests/test_data/build.sh
--rw-r--r--   0        0        0     1212 2023-09-23 07:50:00.881336 fedrq-1.0.0/tests/test_data/repos/repo1/specs/e1/packageb.spec
--rw-r--r--   0        0        0     1196 2024-01-08 18:49:59.717301 fedrq-1.0.0/tests/test_data/repos/repo1/specs/packagea.spec
--rw-r--r--   0        0        0     1232 2023-09-23 07:50:00.881336 fedrq-1.0.0/tests/test_data/repos/repo1/specs/packageb.spec
--rw-r--r--   0        0        0        0 2023-06-26 23:03:24.136349 fedrq-1.0.0/tests/unit/__init__.py
--rw-r--r--   0        0        0     1193 2023-10-24 21:56:15.297461 fedrq-1.0.0/tests/unit/test_archive.py
--rw-r--r--   0        0        0      722 2023-09-23 07:50:00.882336 fedrq-1.0.0/tests/unit/test_backend_base.py
--rw-r--r--   0        0        0      757 2023-12-18 18:23:31.399147 fedrq-1.0.0/tests/unit/test_backends.py
--rw-r--r--   0        0        0     2066 2023-12-15 04:34:12.105772 fedrq-1.0.0/tests/unit/test_base_maker.py
--rw-r--r--   0        0        0      386 2023-11-06 23:46:04.528187 fedrq-1.0.0/tests/unit/test_cache.py
--rw-r--r--   0        0        0     2113 2023-09-23 07:50:00.882336 fedrq-1.0.0/tests/unit/test_changelog.py
--rw-r--r--   0        0        0     2128 2023-06-26 23:03:24.136349 fedrq-1.0.0/tests/unit/test_checkconfig.py
--rw-r--r--   0        0        0     8696 2023-09-23 07:50:00.882336 fedrq-1.0.0/tests/unit/test_command.py
--rw-r--r--   0        0        0      610 2023-12-15 04:25:23.386435 fedrq-1.0.0/tests/unit/test_dnf.py
--rw-r--r--   0        0        0     1351 2023-09-23 07:50:00.883336 fedrq-1.0.0/tests/unit/test_download.py
--rw-r--r--   0        0        0    13062 2024-03-01 01:14:29.816477 fedrq-1.0.0/tests/unit/test_formatters.py
--rw-r--r--   0        0        0     2407 2024-03-01 01:24:17.512465 fedrq-1.0.0/tests/unit/test_formatters_command.py
--rw-r--r--   0        0        0      860 2024-01-08 18:50:00.087299 fedrq-1.0.0/tests/unit/test_libdnf5.py
--rw-r--r--   0        0        0     3361 2023-06-26 23:03:24.137349 fedrq-1.0.0/tests/unit/test_pkgs.py
--rw-r--r--   0        0        0     1681 2023-06-26 23:03:24.138349 fedrq-1.0.0/tests/unit/test_release.py
--rw-r--r--   0        0        0      562 2023-09-23 07:50:00.883336 fedrq-1.0.0/tests/unit/test_release_repo.py
--rw-r--r--   0        0        0      449 2023-06-26 23:03:24.138349 fedrq-1.0.0/tests/unit/test_repo.py
--rw-r--r--   0        0        0      640 2023-06-26 23:03:24.138349 fedrq-1.0.0/tests/unit/test_repolist.py
--rw-r--r--   0        0        0     3905 2023-12-15 04:34:12.105772 fedrq-1.0.0/tests/unit/test_repoquery.py
--rw-r--r--   0        0        0     2712 2023-06-26 23:03:24.138349 fedrq-1.0.0/tests/unit/test_subbpkgs.py
--rw-r--r--   0        0        0      428 2023-09-23 07:50:00.883336 fedrq-1.0.0/tests/unit/test_util.py
--rw-r--r--   0        0        0     4292 2023-09-23 07:50:00.883336 fedrq-1.0.0/tests/unit/test_whatrequires.py
--rw-r--r--   0        0        0      689 2023-06-26 23:03:24.138349 fedrq-1.0.0/tests/unit/test_whatrequires_src.py
--rw-r--r--   0        0        0    15604 1970-01-01 00:00:00.000000 fedrq-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      532 2023-09-23 07:50:00.855336 fedrq-1.1.0/.builds/epel9.yml
+-rw-r--r--   0        0        0     2105 2023-09-23 07:50:00.856336 fedrq-1.1.0/.builds/main.yml
+-rw-r--r--   0        0        0      809 2023-09-23 07:50:00.856336 fedrq-1.1.0/.builds/mockbuild.yml
+-rw-r--r--   0        0        0      473 2023-12-10 19:23:08.443940 fedrq-1.1.0/.builds/test.yml
+-rw-r--r--   0        0        0      384 2024-04-24 06:57:21.119878 fedrq-1.1.0/.copr/Makefile
+lrwxr-xr-x   0        0        0        0 2023-06-26 23:03:24.119349 fedrq-1.1.0/.data/share/licenses/fedrq/GPL-2.0-or-later.txt -> ../../../../LICENSES/GPL-2.0-or-later.txt
+lrwxr-xr-x   0        0        0        0 2023-06-26 23:03:24.119349 fedrq-1.1.0/.data/share/licenses/fedrq/MIT.txt -> ../../../../LICENSES/MIT.txt
+lrwxr-xr-x   0        0        0        0 2023-06-26 23:03:24.119349 fedrq-1.1.0/.data/share/licenses/fedrq/PSF-2.0.txt -> ../../../../LICENSES/PSF-2.0.txt
+lrwxr-xr-x   0        0        0        0 2023-06-26 23:03:24.119349 fedrq-1.1.0/.data/share/licenses/fedrq/Unlicense.txt -> ../../../../LICENSES/Unlicense.txt
+lrwxr-xr-x   0        0        0        0 2024-02-27 23:08:32.868655 fedrq-1.1.0/.dockerignore -> .gitignore
+-rw-r--r--   0        0        0      287 2024-04-24 06:57:21.119878 fedrq-1.1.0/.gitignore
+-rw-r--r--   0        0        0      155 2023-09-23 07:50:00.857336 fedrq-1.1.0/.reuse/dep5
+-rw-r--r--   0        0        0     2553 2023-06-26 23:03:24.119349 fedrq-1.1.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      673 2024-04-24 06:57:21.119878 fedrq-1.1.0/Containerfile
+-rw-r--r--   0        0        0      817 2024-04-30 22:53:24.279852 fedrq-1.1.0/Containerfile.rhel
+-rw-r--r--   0        0        0     1564 2024-04-24 06:57:21.119878 fedrq-1.1.0/Containerfile.rhel8
+-rw-r--r--   0        0        0    17337 2023-06-26 23:03:24.120349 fedrq-1.1.0/LICENSES/GPL-2.0-or-later.txt
+-rw-r--r--   0        0        0     1078 2023-06-26 23:03:24.120349 fedrq-1.1.0/LICENSES/MIT.txt
+-rw-r--r--   0        0        0     2427 2023-06-26 23:03:24.120349 fedrq-1.1.0/LICENSES/PSF-2.0.txt
+-rw-r--r--   0        0        0     1211 2023-06-26 23:03:24.120349 fedrq-1.1.0/LICENSES/Unlicense.txt
+-rw-r--r--   0        0        0    19273 2024-05-01 17:22:25.679357 fedrq-1.1.0/NEWS.md
+-rw-r--r--   0        0        0       89 2023-06-26 23:03:24.120349 fedrq-1.1.0/NEWS.md.license
+-rw-r--r--   0        0        0    13182 2024-04-24 22:06:37.357420 fedrq-1.1.0/README.md
+-rwxr-xr-x   0        0        0      687 2023-06-26 23:03:24.121349 fedrq-1.1.0/contrib/add_frag.py
+-rwxr-xr-x   0        0        0      906 2023-06-26 23:03:24.121349 fedrq-1.1.0/contrib/api_examples/a_noarch_bash.py
+-rwxr-xr-x   0        0        0     2502 2023-06-26 23:03:24.121349 fedrq-1.1.0/contrib/api_examples/ftbfs_retirements.py
+-rw-r--r--   0        0        0      103 2023-09-23 07:50:00.861336 fedrq-1.1.0/contrib/container/000-container.toml
+-rw-r--r--   0        0        0      641 2024-04-24 06:57:21.121878 fedrq-1.1.0/contrib/container/Containerfile
+-rw-r--r--   0        0        0      722 2024-04-24 06:57:21.121878 fedrq-1.1.0/contrib/container/Containerfile.rhel
+-rw-r--r--   0        0        0      759 2023-10-15 18:51:34.227066 fedrq-1.1.0/contrib/container/build.yml
+-rwxr-xr-x   0        0        0      296 2023-09-23 07:50:00.863336 fedrq-1.1.0/contrib/container/entrypoint.sh
+-rw-r--r--   0        0        0      544 2023-09-23 07:50:00.863336 fedrq-1.1.0/contrib/container/rhel.toml
+-rw-r--r--   0        0        0      544 2024-04-24 06:57:21.121878 fedrq-1.1.0/contrib/container/rhel8.toml
+-rw-r--r--   0        0        0      630 2023-06-26 23:03:24.121349 fedrq-1.1.0/contrib/deploy-docsite/main.yaml
+-rw-r--r--   0        0        0      183 2023-06-26 23:03:24.122349 fedrq-1.1.0/contrib/deploy-docsite/roles/configure/handlers/main.yaml
+-rw-r--r--   0        0        0      885 2023-06-26 23:03:24.122349 fedrq-1.1.0/contrib/deploy-docsite/roles/configure/tasks/main.yml
+-rw-r--r--   0        0        0      284 2023-09-18 05:35:56.213359 fedrq-1.1.0/contrib/deploy-docsite/roles/configure/templates/fedrq.caddyfile
+-rw-r--r--   0        0        0      415 2023-06-26 23:03:24.122349 fedrq-1.1.0/contrib/deploy-docsite/roles/deploy/tasks/main.yaml
+-rw-r--r--   0        0        0      156 2023-06-26 23:03:24.123349 fedrq-1.1.0/contrib/deploy-docsite/vars.yaml
+-rwxr-xr-x   0        0        0      914 2023-06-26 23:03:24.123349 fedrq-1.1.0/contrib/fedoraify.py
+-rw-r--r--   0        0        0     6047 2024-04-24 06:57:21.121878 fedrq-1.1.0/doc/API/Summary.md
+-rw-r--r--   0        0        0      204 2023-12-08 02:08:39.952633 fedrq-1.1.0/doc/API/_archive.md
+-rw-r--r--   0        0        0      147 2023-06-26 23:03:24.123349 fedrq-1.1.0/doc/API/backends/base.md
+-rw-r--r--   0        0        0      343 2023-06-26 23:03:24.123349 fedrq-1.1.0/doc/API/backends/dnf.md
+-rw-r--r--   0        0        0      532 2023-06-26 23:03:24.123349 fedrq-1.1.0/doc/API/backends/libdnf5.md
+-rw-r--r--   0        0        0      133 2023-06-26 23:03:24.123349 fedrq-1.1.0/doc/API/config.md
+-rw-r--r--   0        0        0      214 2023-12-08 02:07:21.668887 fedrq-1.1.0/doc/API/release_repo.md
+lrwxr-xr-x   0        0        0        0 2023-06-26 23:03:24.124349 fedrq-1.1.0/doc/News.md -> ../NEWS.md
+-rw-r--r--   0        0        0     4254 2024-04-24 06:57:21.121878 fedrq-1.1.0/doc/dnf-repoquery-diff.md
+-rw-r--r--   0        0        0    21314 2024-04-24 06:57:21.122878 fedrq-1.1.0/doc/fedrq.1.scd
+-rw-r--r--   0        0        0       98 2023-06-26 23:03:24.124349 fedrq-1.1.0/doc/fedrq.1.scd.license
+-rw-r--r--   0        0        0     5024 2024-04-24 06:57:21.122878 fedrq-1.1.0/doc/fedrq.5.scd
+-rw-r--r--   0        0        0       98 2023-06-26 23:03:24.125349 fedrq-1.1.0/doc/fedrq.5.scd.license
+lrwxr-xr-x   0        0        0        0 2023-06-26 23:03:24.125349 fedrq-1.1.0/doc/index.md -> ../README.md
+-rw-r--r--   0        0        0      583 2024-04-24 06:57:21.122878 fedrq-1.1.0/doc/mkdocs_mangen.py
+-rw-r--r--   0        0        0      193 2023-06-26 23:03:24.125349 fedrq-1.1.0/fedrq.rpmlintrc
+-rw-r--r--   0        0        0     4366 2024-05-01 17:22:25.159359 fedrq-1.1.0/fedrq.spec
+-rw-r--r--   0        0        0     2300 2024-04-24 06:57:21.122878 fedrq-1.1.0/mkdocs.yml
+-rw-r--r--   0        0        0     8384 2024-04-24 06:57:21.123878 fedrq-1.1.0/noxfile.py
+-rw-r--r--   0        0        0     4001 2024-04-24 06:57:47.905787 fedrq-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4834 2024-04-29 02:37:10.716778 fedrq-1.1.0/requirements/all.txt
+-rw-r--r--   0        0        0     1118 2024-04-29 02:37:10.717778 fedrq-1.1.0/requirements/codeqa.txt
+-rw-r--r--   0        0        0     3804 2024-04-29 02:37:10.718778 fedrq-1.1.0/requirements/doc.txt
+-rw-r--r--   0        0        0     1019 2024-04-29 02:37:10.719778 fedrq-1.1.0/requirements/formatters.txt
+-rw-r--r--   0        0        0       13 2023-09-23 07:50:00.868336 fedrq-1.1.0/requirements/pydanticv1.in
+-rw-r--r--   0        0        0     1030 2024-04-29 02:37:10.720778 fedrq-1.1.0/requirements/pydanticv1_test.txt
+-rw-r--r--   0        0        0     1516 2023-09-23 07:50:00.868336 fedrq-1.1.0/requirements/refresh.yml
+-rw-r--r--   0        0        0      703 2024-04-29 02:37:10.721778 fedrq-1.1.0/requirements/requirements.txt
+-rw-r--r--   0        0        0        7 2023-09-23 07:50:00.869336 fedrq-1.1.0/requirements/srpm.in
+-rw-r--r--   0        0        0      448 2024-04-24 06:59:10.775506 fedrq-1.1.0/requirements/srpm.txt
+-rw-r--r--   0        0        0     1044 2024-04-29 02:37:10.721778 fedrq-1.1.0/requirements/test.txt
+-rw-r--r--   0        0        0     1057 2024-04-29 02:37:10.722777 fedrq-1.1.0/requirements/typing.txt
+-rw-r--r--   0        0        0     1162 2024-04-24 06:57:21.124878 fedrq-1.1.0/ruff.toml
+-rw-r--r--   0        0        0      759 2024-05-01 17:22:22.601368 fedrq-1.1.0/src/fedrq/__init__.py
+-rw-r--r--   0        0        0      219 2023-06-26 23:03:24.126349 fedrq-1.1.0/src/fedrq/__main__.py
+-rw-r--r--   0        0        0     2822 2024-01-07 21:00:32.692014 fedrq-1.1.0/src/fedrq/_archive.py
+-rw-r--r--   0        0        0     1713 2023-09-11 04:00:33.008787 fedrq-1.1.0/src/fedrq/_compat.py
+-rw-r--r--   0        0        0      173 2023-06-26 23:03:24.126349 fedrq-1.1.0/src/fedrq/_config.py
+-rw-r--r--   0        0        0     1370 2023-12-23 06:34:35.309654 fedrq-1.1.0/src/fedrq/_utils.py
+-rw-r--r--   0        0        0     2645 2023-12-18 18:23:31.398146 fedrq-1.1.0/src/fedrq/backends/__init__.py
+-rw-r--r--   0        0        0    18400 2024-04-24 06:59:10.674507 fedrq-1.1.0/src/fedrq/backends/base/__init__.py
+-rw-r--r--   0        0        0      630 2023-06-26 23:03:24.127349 fedrq-1.1.0/src/fedrq/backends/dnf/__init__.py
+-rw-r--r--   0        0        0     8553 2024-04-29 15:53:54.934651 fedrq-1.1.0/src/fedrq/backends/dnf/backend/__init__.py
+-rw-r--r--   0        0        0      629 2023-09-23 07:50:00.872336 fedrq-1.1.0/src/fedrq/backends/libdnf5/__init__.py
+-rw-r--r--   0        0        0    29648 2024-04-30 12:09:56.370424 fedrq-1.1.0/src/fedrq/backends/libdnf5/backend/__init__.py
+-rw-r--r--   0        0        0     2667 2024-04-24 06:57:21.125878 fedrq-1.1.0/src/fedrq/cli/__init__.py
+-rw-r--r--   0        0        0    17869 2024-04-25 02:14:03.408884 fedrq-1.1.0/src/fedrq/cli/base.py
+-rw-r--r--   0        0        0      758 2023-11-06 03:39:21.572134 fedrq-1.1.0/src/fedrq/cli/commands/COMMAND.py.in
+-rw-r--r--   0        0        0        0 2023-06-26 23:03:24.129349 fedrq-1.1.0/src/fedrq/cli/commands/__init__.py
+-rw-r--r--   0        0        0     1228 2023-11-06 23:45:40.679278 fedrq-1.1.0/src/fedrq/cli/commands/cache.py
+-rw-r--r--   0        0        0     2427 2024-04-24 06:57:21.126878 fedrq-1.1.0/src/fedrq/cli/commands/changelogs.py
+-rw-r--r--   0        0        0     6390 2024-01-07 21:00:32.693014 fedrq-1.1.0/src/fedrq/cli/commands/download.py
+-rw-r--r--   0        0        0     1926 2024-04-24 06:57:21.126878 fedrq-1.1.0/src/fedrq/cli/commands/formatters.py
+-rw-r--r--   0        0        0     1729 2023-11-06 04:24:41.488764 fedrq-1.1.0/src/fedrq/cli/commands/pkgs.py
+-rw-r--r--   0        0        0     1425 2023-09-23 07:50:00.875336 fedrq-1.1.0/src/fedrq/cli/commands/repolist.py
+-rw-r--r--   0        0        0     2394 2023-09-23 07:50:00.876336 fedrq-1.1.0/src/fedrq/cli/commands/subpkgs.py
+-rw-r--r--   0        0        0    10927 2024-03-02 04:35:52.918510 fedrq-1.1.0/src/fedrq/cli/commands/whatrequires.py
+-rw-r--r--   0        0        0    18643 2024-04-24 06:57:21.127878 fedrq-1.1.0/src/fedrq/cli/formatters.py
+-rw-r--r--   0        0        0    16327 2024-04-24 21:45:32.639603 fedrq-1.1.0/src/fedrq/config.py
+-rw-r--r--   0        0        0        0 2023-06-26 23:03:24.131349 fedrq-1.1.0/src/fedrq/data/__init__.py
+-rw-r--r--   0        0        0     9590 2024-04-24 06:57:21.127878 fedrq-1.1.0/src/fedrq/data/releases.toml
+-rw-r--r--   0        0        0        0 2023-06-26 23:03:24.131349 fedrq-1.1.0/src/fedrq/data/repos/__init__.py
+-rw-r--r--   0        0        0     2053 2023-06-26 23:03:24.131349 fedrq-1.1.0/src/fedrq/data/repos/almalinux.repo
+-rw-r--r--   0        0        0      639 2023-06-26 23:03:24.131349 fedrq-1.1.0/src/fedrq/data/repos/amazonlinux.repo
+-rw-r--r--   0        0        0     1386 2023-06-26 23:03:24.132349 fedrq-1.1.0/src/fedrq/data/repos/centos-stream-compose.repo
+-rw-r--r--   0        0        0     1850 2023-06-26 23:03:24.132349 fedrq-1.1.0/src/fedrq/data/repos/centos-stream.repo
+-rw-r--r--   0        0        0     1494 2023-06-26 23:03:24.132349 fedrq-1.1.0/src/fedrq/data/repos/centos-stream8-compose.repo
+-rw-r--r--   0        0        0     1599 2023-06-26 23:03:24.132349 fedrq-1.1.0/src/fedrq/data/repos/centos-stream8.repo
+-rw-r--r--   0        0        0     1342 2023-06-26 23:03:24.132349 fedrq-1.1.0/src/fedrq/data/repos/centos7.repo
+-rw-r--r--   0        0        0      389 2024-04-24 06:57:21.127878 fedrq-1.1.0/src/fedrq/data/repos/eln-buildroot.repo
+-rw-r--r--   0        0        0     1809 2023-06-26 23:03:24.132349 fedrq-1.1.0/src/fedrq/data/repos/eln.repo
+-rw-r--r--   0        0        0     2158 2023-06-26 23:03:24.132349 fedrq-1.1.0/src/fedrq/data/repos/epel.repo
+-rw-r--r--   0        0        0    14146 2023-06-26 23:03:24.132349 fedrq-1.1.0/src/fedrq/data/repos/fedora-eln.repo
+-rw-r--r--   0        0        0     2402 2023-06-26 23:03:24.133349 fedrq-1.1.0/src/fedrq/data/repos/fedora-rawhide.repo
+-rw-r--r--   0        0        0     1480 2023-06-26 23:03:24.133349 fedrq-1.1.0/src/fedrq/data/repos/fedora-updates-testing.repo
+-rw-r--r--   0        0        0     1422 2023-09-23 07:50:00.878336 fedrq-1.1.0/src/fedrq/data/repos/fedora-updates.repo
+-rw-r--r--   0        0        0     1375 2023-09-23 07:50:00.878336 fedrq-1.1.0/src/fedrq/data/repos/fedora.repo
+-rw-r--r--   0        0        0     1374 2023-09-23 07:50:00.878336 fedrq-1.1.0/src/fedrq/data/repos/oraclelinux-8.repo
+-rw-r--r--   0        0        0     1374 2023-09-23 07:50:00.878336 fedrq-1.1.0/src/fedrq/data/repos/oraclelinux-9.repo
+-rw-r--r--   0        0        0      425 2023-06-26 23:03:24.133349 fedrq-1.1.0/src/fedrq/data/repos/rawhide-buildroot.repo
+-rw-r--r--   0        0        0     6475 2023-09-23 07:50:00.878336 fedrq-1.1.0/src/fedrq/data/repos/rocky.repo
+-rw-r--r--   0        0        0     3505 2023-09-23 07:50:00.878336 fedrq-1.1.0/src/fedrq/data/repos/ubi.repo
+-rw-r--r--   0        0        0        0 2023-06-26 23:03:24.133349 fedrq-1.1.0/src/fedrq/py.typed
+-rw-r--r--   0        0        0     9259 2024-04-24 06:57:21.127878 fedrq-1.1.0/src/fedrq/release_repo.py
+-rw-r--r--   0        0        0     1828 2024-04-24 06:57:21.128878 fedrq-1.1.0/src/fedrq/repoquery.py
+-rw-r--r--   0        0        0      154 2023-06-26 23:03:24.134349 fedrq-1.1.0/tests/.gitignore
+-rw-r--r--   0        0        0        0 2023-06-26 23:03:24.134349 fedrq-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     2988 2023-09-23 07:50:00.879336 fedrq-1.1.0/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-06-26 23:03:24.134349 fedrq-1.1.0/tests/integration/__init__.py
+-rw-r--r--   0        0        0     1748 2023-09-23 07:50:00.880336 fedrq-1.1.0/tests/integration/test_backends.py
+-rw-r--r--   0        0        0      405 2023-11-06 23:48:33.545619 fedrq-1.1.0/tests/integration/test_cache.py
+-rw-r--r--   0        0        0      553 2023-09-23 07:50:00.880336 fedrq-1.1.0/tests/integration/test_download.py
+-rw-r--r--   0        0        0      988 2023-09-23 07:50:00.880336 fedrq-1.1.0/tests/integration/test_pkgs.py
+-rw-r--r--   0        0        0     1483 2023-09-23 07:50:00.880336 fedrq-1.1.0/tests/integration/test_subpkgs.py
+-rw-r--r--   0        0        0     1964 2023-09-23 07:50:00.880336 fedrq-1.1.0/tests/integration/test_whatrequires.py
+-rw-r--r--   0        0        0     1447 2023-09-23 07:50:00.881336 fedrq-1.1.0/tests/integration/test_whatrequires_src.py
+-rw-r--r--   0        0        0        0 2023-06-26 23:03:24.135349 fedrq-1.1.0/tests/test_data/__init__.py
+-rw-r--r--   0        0        0      408 2024-02-07 03:25:08.056407 fedrq-1.1.0/tests/test_data/_template.spec
+-rwxr-xr-x   0        0        0     1484 2024-04-24 06:57:21.128878 fedrq-1.1.0/tests/test_data/build.sh
+-rw-r--r--   0        0        0     1212 2023-09-23 07:50:00.881336 fedrq-1.1.0/tests/test_data/repos/repo1/specs/e1/packageb.spec
+-rw-r--r--   0        0        0     1196 2024-04-24 06:57:21.128878 fedrq-1.1.0/tests/test_data/repos/repo1/specs/packagea.spec
+-rw-r--r--   0        0        0     1232 2023-09-23 07:50:00.881336 fedrq-1.1.0/tests/test_data/repos/repo1/specs/packageb.spec
+-rw-r--r--   0        0        0        0 2023-06-26 23:03:24.136349 fedrq-1.1.0/tests/unit/__init__.py
+-rw-r--r--   0        0        0     1193 2023-10-24 21:56:15.297461 fedrq-1.1.0/tests/unit/test_archive.py
+-rw-r--r--   0        0        0      722 2023-09-23 07:50:00.882336 fedrq-1.1.0/tests/unit/test_backend_base.py
+-rw-r--r--   0        0        0      757 2023-12-18 18:23:31.399147 fedrq-1.1.0/tests/unit/test_backends.py
+-rw-r--r--   0        0        0     2066 2023-12-15 04:34:12.105772 fedrq-1.1.0/tests/unit/test_base_maker.py
+-rw-r--r--   0        0        0      386 2023-11-06 23:46:04.528187 fedrq-1.1.0/tests/unit/test_cache.py
+-rw-r--r--   0        0        0     2113 2023-09-23 07:50:00.882336 fedrq-1.1.0/tests/unit/test_changelog.py
+-rw-r--r--   0        0        0     2128 2023-06-26 23:03:24.136349 fedrq-1.1.0/tests/unit/test_checkconfig.py
+-rw-r--r--   0        0        0     8696 2023-09-23 07:50:00.882336 fedrq-1.1.0/tests/unit/test_command.py
+-rw-r--r--   0        0        0      610 2023-12-15 04:25:23.386435 fedrq-1.1.0/tests/unit/test_dnf.py
+-rw-r--r--   0        0        0     1351 2023-09-23 07:50:00.883336 fedrq-1.1.0/tests/unit/test_download.py
+-rw-r--r--   0        0        0    13062 2024-04-24 06:57:21.128878 fedrq-1.1.0/tests/unit/test_formatters.py
+-rw-r--r--   0        0        0     2407 2024-04-24 06:57:21.128878 fedrq-1.1.0/tests/unit/test_formatters_command.py
+-rw-r--r--   0        0        0      860 2024-04-24 06:57:21.128878 fedrq-1.1.0/tests/unit/test_libdnf5.py
+-rw-r--r--   0        0        0     3361 2023-06-26 23:03:24.137349 fedrq-1.1.0/tests/unit/test_pkgs.py
+-rw-r--r--   0        0        0     1681 2023-06-26 23:03:24.138349 fedrq-1.1.0/tests/unit/test_release.py
+-rw-r--r--   0        0        0      562 2023-09-23 07:50:00.883336 fedrq-1.1.0/tests/unit/test_release_repo.py
+-rw-r--r--   0        0        0      449 2023-06-26 23:03:24.138349 fedrq-1.1.0/tests/unit/test_repo.py
+-rw-r--r--   0        0        0      640 2023-06-26 23:03:24.138349 fedrq-1.1.0/tests/unit/test_repolist.py
+-rw-r--r--   0        0        0     3905 2023-12-15 04:34:12.105772 fedrq-1.1.0/tests/unit/test_repoquery.py
+-rw-r--r--   0        0        0     2712 2023-06-26 23:03:24.138349 fedrq-1.1.0/tests/unit/test_subbpkgs.py
+-rw-r--r--   0        0        0      428 2023-09-23 07:50:00.883336 fedrq-1.1.0/tests/unit/test_util.py
+-rw-r--r--   0        0        0     4292 2023-09-23 07:50:00.883336 fedrq-1.1.0/tests/unit/test_whatrequires.py
+-rw-r--r--   0        0        0      689 2023-06-26 23:03:24.138349 fedrq-1.1.0/tests/unit/test_whatrequires_src.py
+-rw-r--r--   0        0        0    15604 1970-01-01 00:00:00.000000 fedrq-1.1.0/PKG-INFO
```

### Comparing `fedrq-1.0.0/.builds/epel9.yml` & `fedrq-1.1.0/.builds/epel9.yml`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/.builds/main.yml` & `fedrq-1.1.0/.builds/main.yml`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/.builds/mockbuild.yml` & `fedrq-1.1.0/.builds/mockbuild.yml`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/CONTRIBUTING.md` & `fedrq-1.1.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/Containerfile` & `fedrq-1.1.0/Containerfile`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/Containerfile.rhel` & `fedrq-1.1.0/Containerfile.rhel`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/Containerfile.rhel8` & `fedrq-1.1.0/Containerfile.rhel8`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/LICENSES/GPL-2.0-or-later.txt` & `fedrq-1.1.0/LICENSES/GPL-2.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/LICENSES/MIT.txt` & `fedrq-1.1.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/LICENSES/PSF-2.0.txt` & `fedrq-1.1.0/LICENSES/PSF-2.0.txt`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/LICENSES/Unlicense.txt` & `fedrq-1.1.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/NEWS.md` & `fedrq-1.1.0/NEWS.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 NEWS
 =====
 
+## 1.1.0 - 2024-05-01 <a id='1.1.0'></a>
+
+### Added
+
+- backends libdnf5: add dnf 5.2.0.x compatibility
+
+### Changed
+
+- backends: revamp typing for `Package` and `PackageQuery`
+
 ## 1.0.0 - 2024-04-01 <a id='1.0.0'></a>
 
 First stable release
 
 ### Added
 
 - Containerfiles: add experimental UBI 8–based Containerfile
```

### Comparing `fedrq-1.0.0/README.md` & `fedrq-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/contrib/add_frag.py` & `fedrq-1.1.0/contrib/add_frag.py`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/contrib/api_examples/a_noarch_bash.py` & `fedrq-1.1.0/contrib/api_examples/a_noarch_bash.py`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/contrib/api_examples/ftbfs_retirements.py` & `fedrq-1.1.0/contrib/api_examples/ftbfs_retirements.py`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/contrib/container/Containerfile` & `fedrq-1.1.0/contrib/container/Containerfile`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/contrib/container/Containerfile.rhel` & `fedrq-1.1.0/contrib/container/Containerfile.rhel`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/contrib/container/build.yml` & `fedrq-1.1.0/contrib/container/build.yml`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/contrib/container/rhel.toml` & `fedrq-1.1.0/contrib/container/rhel.toml`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/contrib/container/rhel8.toml` & `fedrq-1.1.0/contrib/container/rhel8.toml`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/contrib/deploy-docsite/main.yaml` & `fedrq-1.1.0/contrib/deploy-docsite/main.yaml`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/contrib/deploy-docsite/roles/configure/tasks/main.yml` & `fedrq-1.1.0/contrib/deploy-docsite/roles/configure/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/contrib/fedoraify.py` & `fedrq-1.1.0/contrib/fedoraify.py`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/doc/API/Summary.md` & `fedrq-1.1.0/doc/API/Summary.md`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/doc/API/backends/libdnf5.md` & `fedrq-1.1.0/doc/API/backends/libdnf5.md`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/doc/dnf-repoquery-diff.md` & `fedrq-1.1.0/doc/dnf-repoquery-diff.md`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/doc/fedrq.1.scd` & `fedrq-1.1.0/doc/fedrq.1.scd`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/doc/fedrq.5.scd` & `fedrq-1.1.0/doc/fedrq.5.scd`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/doc/mkdocs_mangen.py` & `fedrq-1.1.0/doc/mkdocs_mangen.py`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/fedrq.spec` & `fedrq-1.1.0/fedrq.spec`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Copyright (C) 2022 Maxwell G <gotmax@e.email>
 # SPDX-License-Identifier: MIT
 # License text: https://spdx.org/licenses/MIT.html
 
 %bcond libdnf5 %[0%{?fedora} >= 38]
 
 Name:           fedrq
-Version:        1.0.0
+Version:        1.1.0
 Release:        1%{?dist}
 Summary:        A tool to query the Fedora and EPEL repositories
 
 # - code is GPL-2.0-or-later
 # - the data and config files in fedrq/data are UNLICENSEed
 # - Embeded repo defs are MIT.
 # - PSF-2.0 code copied from Cpython 3.11 for older Python versions
@@ -102,14 +102,17 @@
 %{bash_completions_dir}/fedrq
 %{fish_completions_dir}/fedrq.fish
 %{_mandir}/man1/fedrq.1*
 %{_mandir}/man5/fedrq.5*
 
 
 %changelog
+* Wed May 01 2024 Maxwell G <maxwell@gtmx.me> - 1.1.0-1
+- Release 1.1.0.
+
 * Mon Apr 01 2024 Maxwell G <maxwell@gtmx.me> - 1.0.0-1
 - Release 1.0.0.
 
 * Tue Feb 13 2024 Maxwell G <maxwell@gtmx.me> - 0.15.0-1
 - Release 0.15.0.
 
 * Wed Feb 07 2024 Maxwell G <maxwell@gtmx.me> - 0.14.0-1
```

### Comparing `fedrq-1.0.0/mkdocs.yml` & `fedrq-1.1.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/noxfile.py` & `fedrq-1.1.0/noxfile.py`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/pyproject.toml` & `fedrq-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/requirements/all.txt` & `fedrq-1.1.0/requirements/all.txt`

 * *Files 4% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 #
 #    pip-compile --allow-unsafe --extra=codeqa --extra=doc --extra=formatters --extra=test --extra=typing --output-file=requirements/all.txt --strip-extras
 #
 annotated-types==0.6.0
     # via pydantic
 anyio==4.3.0
     # via httpx
-argcomplete==3.2.3
+argcomplete==3.3.0
     # via fedrq (pyproject.toml)
 babel==2.14.0
     # via mkdocs-material
 binaryornot==0.4.4
     # via reuse
-black==24.3.0
+black==24.4.2
     # via fedrq (pyproject.toml)
 boolean-py==4.0
     # via
     #   license-expression
     #   reuse
 certifi==2024.2.2
     # via
@@ -32,105 +32,109 @@
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via
     #   black
     #   mkdocs
     #   mkdocstrings
-    #   typer-slim
+    #   typer
 colorama==0.4.6
     # via
     #   griffe
     #   mkdocs-material
-exceptiongroup==1.2.0
+exceptiongroup==1.2.1
     # via
     #   anyio
     #   pytest
 ghp-import==2.1.0
     # via mkdocs
-griffe==0.42.1
+griffe==0.44.0
     # via
     #   fedrq (pyproject.toml)
     #   mkdocstrings-python
 h11==0.14.0
     # via httpcore
 httpcore==1.0.5
     # via httpx
 httpx==0.27.0
     # via
     #   releaserr
     #   sourcehutx
-idna==3.6
+idna==3.7
     # via
     #   anyio
     #   httpx
     #   requests
 importlib-metadata==7.1.0
     # via
     #   markdown
     #   mkdocs
+    #   mkdocs-get-deps
     #   mkdocstrings
 iniconfig==2.0.0
     # via pytest
 isort==5.13.2
     # via fedrq (pyproject.toml)
 jinja2==3.1.3
     # via
     #   mkdocs
     #   mkdocs-material
     #   mkdocstrings
     #   releaserr
     #   reuse
 license-expression==30.3.0
     # via reuse
-markdown==3.5.2
+markdown==3.6
     # via
     #   mkdocs
     #   mkdocs-autorefs
     #   mkdocs-material
     #   mkdocstrings
-    #   mkdocstrings-python
     #   pymdown-extensions
 markdown-it-py==3.0.0
     # via rich
 markupsafe==2.1.5
     # via
     #   jinja2
     #   mkdocs
     #   mkdocs-autorefs
     #   mkdocstrings
 mdurl==0.1.2
     # via markdown-it-py
 mergedeep==1.3.4
-    # via mkdocs
-mkdocs==1.5.3
+    # via
+    #   mkdocs
+    #   mkdocs-get-deps
+mkdocs==1.6.0
     # via
     #   fedrq (pyproject.toml)
     #   mkdocs-autorefs
     #   mkdocs-exclude
     #   mkdocs-gen-files
     #   mkdocs-material
     #   mkdocstrings
 mkdocs-autorefs==1.0.1
     # via mkdocstrings
 mkdocs-exclude==1.0.2
     # via fedrq (pyproject.toml)
 mkdocs-gen-files==0.5.0
     # via fedrq (pyproject.toml)
-mkdocs-material==9.5.16
+mkdocs-get-deps==0.2.0
+    # via mkdocs
+mkdocs-material==9.5.19
     # via fedrq (pyproject.toml)
 mkdocs-material-extensions==1.3.1
     # via mkdocs-material
-mkdocstrings==0.24.1
+mkdocstrings==0.25.0
     # via
     #   fedrq (pyproject.toml)
     #   mkdocstrings-python
-mkdocstrings-python==1.9.0
+mkdocstrings-python==1.10.0
     # via mkdocstrings
-mypy==1.9.0
+mypy==1.10.0
     # via fedrq (pyproject.toml)
 mypy-extensions==1.0.0
     # via
     #   black
     #   mypy
 packaging==24.0
     # via
@@ -139,73 +143,74 @@
     #   pytest
 paginate==0.5.6
     # via mkdocs-material
 pathspec==0.12.1
     # via
     #   black
     #   mkdocs
-platformdirs==4.2.0
+platformdirs==4.2.1
     # via
     #   black
-    #   mkdocs
+    #   mkdocs-get-deps
     #   mkdocstrings
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
-pydantic==2.6.4
+pydantic==2.7.1
     # via
     #   fedrq (pyproject.toml)
     #   releaserr
     #   sourcehutx
-pydantic-core==2.16.3
+pydantic-core==2.18.2
     # via pydantic
 pygments==2.17.2
     # via
     #   mkdocs-material
     #   rich
-pymdown-extensions==10.7.1
+pymdown-extensions==10.8.1
     # via
     #   mkdocs-material
     #   mkdocstrings
-pytest==8.1.1
+pytest==8.2.0
     # via
     #   fedrq (pyproject.toml)
     #   pytest-mock
 pytest-mock==3.14.0
     # via fedrq (pyproject.toml)
 python-dateutil==2.9.0.post0
     # via ghp-import
 python-debian==0.1.49
     # via reuse
 pyyaml==6.0.1
     # via
     #   mkdocs
+    #   mkdocs-get-deps
     #   pymdown-extensions
     #   pyyaml-env-tag
 pyyaml-env-tag==0.1
     # via mkdocs
-regex==2023.12.25
+regex==2024.4.28
     # via mkdocs-material
-releaserr==0.1.dev127
+releaserr==0.1.dev131
     # via fedrq (pyproject.toml)
 requests==2.31.0
     # via
     #   fedrq (pyproject.toml)
     #   mkdocs-material
-reuse==3.0.1
+reuse==3.0.2
     # via fedrq (pyproject.toml)
 rich==13.7.1
     # via
     #   releaserr
-    #   typer-slim
+    #   typer
 rpm==0.1.0
     # via fedrq (pyproject.toml)
-ruff==0.3.4
+ruff==0.4.2
     # via fedrq (pyproject.toml)
 shellingham==1.5.4
-    # via typer-slim
+    # via typer
 six==1.16.0
     # via python-dateutil
 sniffio==1.3.1
     # via
     #   anyio
     #   httpx
 sourcehutx==0.3.0
@@ -215,35 +220,29 @@
     #   black
     #   fedrq (pyproject.toml)
     #   mypy
     #   pytest
     #   sourcehutx
 tomli-w==1.0.0
     # via fedrq (pyproject.toml)
-typer==0.12.0
+typer==0.12.3
     # via releaserr
-typer-cli==0.12.0
-    # via typer
-typer-slim==0.12.0
-    # via
-    #   typer
-    #   typer-cli
-types-requests==2.31.0.20240311
+types-requests==2.31.0.20240406
     # via fedrq (pyproject.toml)
-typing-extensions==4.10.0
+typing-extensions==4.11.0
     # via
     #   anyio
     #   black
     #   fedrq (pyproject.toml)
     #   mkdocstrings
     #   mypy
     #   pydantic
     #   pydantic-core
     #   releaserr
-    #   typer-slim
+    #   typer
 urllib3==2.2.1
     # via
     #   requests
     #   types-requests
 watchdog==4.0.0
     # via mkdocs
 zipp==3.18.1
```

### Comparing `fedrq-1.0.0/requirements/codeqa.txt` & `fedrq-1.1.0/requirements/codeqa.txt`

 * *Files 12% similar despite different names*

```diff
@@ -16,37 +16,37 @@
     # via requests
 chardet==5.2.0
     # via
     #   binaryornot
     #   python-debian
 charset-normalizer==3.3.2
     # via requests
-idna==3.6
+idna==3.7
     # via requests
 jinja2==3.1.3
     # via reuse
 license-expression==30.3.0
     # via reuse
 markupsafe==2.1.5
     # via jinja2
-pydantic==2.6.4
+pydantic==2.7.1
     # via fedrq (pyproject.toml)
-pydantic-core==2.16.3
+pydantic-core==2.18.2
     # via pydantic
 python-debian==0.1.49
     # via reuse
 requests==2.31.0
     # via fedrq (pyproject.toml)
-reuse==3.0.1
+reuse==3.0.2
     # via fedrq (pyproject.toml)
 rpm==0.1.0
     # via fedrq (pyproject.toml)
-ruff==0.3.4
+ruff==0.4.2
     # via fedrq (pyproject.toml)
 tomli==2.0.1 ; python_version < "3.11"
     # via fedrq (pyproject.toml)
-typing-extensions==4.10.0
+typing-extensions==4.11.0
     # via
     #   pydantic
     #   pydantic-core
 urllib3==2.2.1
     # via requests
```

### Comparing `fedrq-1.0.0/requirements/doc.txt` & `fedrq-1.1.0/requirements/doc.txt`

 * *Files 4% similar despite different names*

```diff
@@ -6,195 +6,194 @@
 #
 annotated-types==0.6.0
     # via pydantic
 anyio==4.3.0
     # via httpx
 babel==2.14.0
     # via mkdocs-material
-black==24.3.0
+black==24.4.2
     # via fedrq (pyproject.toml)
 certifi==2024.2.2
     # via
     #   httpcore
     #   httpx
     #   requests
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via
     #   black
     #   mkdocs
     #   mkdocstrings
-    #   typer-slim
+    #   typer
 colorama==0.4.6
     # via
     #   griffe
     #   mkdocs-material
-exceptiongroup==1.2.0
+exceptiongroup==1.2.1
     # via anyio
 ghp-import==2.1.0
     # via mkdocs
-griffe==0.42.1
+griffe==0.44.0
     # via
     #   fedrq (pyproject.toml)
     #   mkdocstrings-python
 h11==0.14.0
     # via httpcore
 httpcore==1.0.5
     # via httpx
 httpx==0.27.0
     # via
     #   releaserr
     #   sourcehutx
-idna==3.6
+idna==3.7
     # via
     #   anyio
     #   httpx
     #   requests
 importlib-metadata==7.1.0
     # via
     #   markdown
     #   mkdocs
+    #   mkdocs-get-deps
     #   mkdocstrings
 jinja2==3.1.3
     # via
     #   mkdocs
     #   mkdocs-material
     #   mkdocstrings
     #   releaserr
-markdown==3.5.2
+markdown==3.6
     # via
     #   mkdocs
     #   mkdocs-autorefs
     #   mkdocs-material
     #   mkdocstrings
-    #   mkdocstrings-python
     #   pymdown-extensions
 markdown-it-py==3.0.0
     # via rich
 markupsafe==2.1.5
     # via
     #   jinja2
     #   mkdocs
     #   mkdocs-autorefs
     #   mkdocstrings
 mdurl==0.1.2
     # via markdown-it-py
 mergedeep==1.3.4
-    # via mkdocs
-mkdocs==1.5.3
+    # via
+    #   mkdocs
+    #   mkdocs-get-deps
+mkdocs==1.6.0
     # via
     #   fedrq (pyproject.toml)
     #   mkdocs-autorefs
     #   mkdocs-exclude
     #   mkdocs-gen-files
     #   mkdocs-material
     #   mkdocstrings
 mkdocs-autorefs==1.0.1
     # via mkdocstrings
 mkdocs-exclude==1.0.2
     # via fedrq (pyproject.toml)
 mkdocs-gen-files==0.5.0
     # via fedrq (pyproject.toml)
-mkdocs-material==9.5.16
+mkdocs-get-deps==0.2.0
+    # via mkdocs
+mkdocs-material==9.5.19
     # via fedrq (pyproject.toml)
 mkdocs-material-extensions==1.3.1
     # via mkdocs-material
-mkdocstrings==0.24.1
+mkdocstrings==0.25.0
     # via
     #   fedrq (pyproject.toml)
     #   mkdocstrings-python
-mkdocstrings-python==1.9.0
+mkdocstrings-python==1.10.0
     # via mkdocstrings
 mypy-extensions==1.0.0
     # via black
 packaging==24.0
     # via
     #   black
     #   mkdocs
 paginate==0.5.6
     # via mkdocs-material
 pathspec==0.12.1
     # via
     #   black
     #   mkdocs
-platformdirs==4.2.0
+platformdirs==4.2.1
     # via
     #   black
-    #   mkdocs
+    #   mkdocs-get-deps
     #   mkdocstrings
-pydantic==2.6.4
+pydantic==2.7.1
     # via
     #   fedrq (pyproject.toml)
     #   releaserr
     #   sourcehutx
-pydantic-core==2.16.3
+pydantic-core==2.18.2
     # via pydantic
 pygments==2.17.2
     # via
     #   mkdocs-material
     #   rich
-pymdown-extensions==10.7.1
+pymdown-extensions==10.8.1
     # via
     #   mkdocs-material
     #   mkdocstrings
 python-dateutil==2.9.0.post0
     # via ghp-import
 pyyaml==6.0.1
     # via
     #   mkdocs
+    #   mkdocs-get-deps
     #   pymdown-extensions
     #   pyyaml-env-tag
 pyyaml-env-tag==0.1
     # via mkdocs
-regex==2023.12.25
+regex==2024.4.28
     # via mkdocs-material
-releaserr==0.1.dev127
+releaserr==0.1.dev131
     # via fedrq (pyproject.toml)
 requests==2.31.0
     # via
     #   fedrq (pyproject.toml)
     #   mkdocs-material
 rich==13.7.1
     # via
     #   releaserr
-    #   typer-slim
+    #   typer
 rpm==0.1.0
     # via fedrq (pyproject.toml)
 shellingham==1.5.4
-    # via typer-slim
+    # via typer
 six==1.16.0
     # via python-dateutil
 sniffio==1.3.1
     # via
     #   anyio
     #   httpx
 sourcehutx==0.3.0
     # via releaserr
 tomli==2.0.1 ; python_version < "3.11"
     # via
     #   black
     #   fedrq (pyproject.toml)
     #   sourcehutx
-typer==0.12.0
+typer==0.12.3
     # via releaserr
-typer-cli==0.12.0
-    # via typer
-typer-slim==0.12.0
-    # via
-    #   typer
-    #   typer-cli
-typing-extensions==4.10.0
+typing-extensions==4.11.0
     # via
     #   anyio
     #   black
     #   mkdocstrings
     #   pydantic
     #   pydantic-core
     #   releaserr
-    #   typer-slim
+    #   typer
 urllib3==2.2.1
     # via requests
 watchdog==4.0.0
     # via mkdocs
 zipp==3.18.1
     # via importlib-metadata
```

### Comparing `fedrq-1.0.0/requirements/formatters.txt` & `fedrq-1.1.0/requirements/formatters.txt`

 * *Files 13% similar despite different names*

```diff
@@ -2,46 +2,46 @@
 # This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
 #    pip-compile --allow-unsafe --extra=formatters --output-file=requirements/formatters.txt --strip-extras
 #
 annotated-types==0.6.0
     # via pydantic
-black==24.3.0
+black==24.4.2
     # via fedrq (pyproject.toml)
 certifi==2024.2.2
     # via requests
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via black
-idna==3.6
+idna==3.7
     # via requests
 isort==5.13.2
     # via fedrq (pyproject.toml)
 mypy-extensions==1.0.0
     # via black
 packaging==24.0
     # via black
 pathspec==0.12.1
     # via black
-platformdirs==4.2.0
+platformdirs==4.2.1
     # via black
-pydantic==2.6.4
+pydantic==2.7.1
     # via fedrq (pyproject.toml)
-pydantic-core==2.16.3
+pydantic-core==2.18.2
     # via pydantic
 requests==2.31.0
     # via fedrq (pyproject.toml)
 rpm==0.1.0
     # via fedrq (pyproject.toml)
 tomli==2.0.1 ; python_version < "3.11"
     # via
     #   black
     #   fedrq (pyproject.toml)
-typing-extensions==4.10.0
+typing-extensions==4.11.0
     # via
     #   black
     #   pydantic
     #   pydantic-core
 urllib3==2.2.1
     # via requests
```

### Comparing `fedrq-1.0.0/requirements/pydanticv1_test.txt` & `fedrq-1.1.0/requirements/pydanticv1_test.txt`

 * *Files 0% similar despite different names*

```diff
@@ -4,29 +4,29 @@
 #
 #    pip-compile --allow-unsafe --constraint=requirements/pydanticv1.in --extra=test --output-file=requirements/pydanticv1_test.txt --strip-extras
 #
 certifi==2024.2.2
     # via requests
 charset-normalizer==3.3.2
     # via requests
-exceptiongroup==1.2.0
+exceptiongroup==1.2.1
     # via pytest
-idna==3.6
+idna==3.7
     # via requests
 iniconfig==2.0.0
     # via pytest
 packaging==24.0
     # via pytest
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
-pydantic==1.10.14
+pydantic==1.10.15
     # via
     #   -c requirements/pydanticv1.in
     #   fedrq (pyproject.toml)
-pytest==8.1.1
+pytest==8.2.0
     # via
     #   fedrq (pyproject.toml)
     #   pytest-mock
 pytest-mock==3.14.0
     # via fedrq (pyproject.toml)
 requests==2.31.0
     # via fedrq (pyproject.toml)
@@ -34,11 +34,11 @@
     # via fedrq (pyproject.toml)
 tomli==2.0.1 ; python_version < "3.11"
     # via
     #   fedrq (pyproject.toml)
     #   pytest
 tomli-w==1.0.0
     # via fedrq (pyproject.toml)
-typing-extensions==4.10.0
+typing-extensions==4.11.0
     # via pydantic
 urllib3==2.2.1
     # via requests
```

### Comparing `fedrq-1.0.0/requirements/refresh.yml` & `fedrq-1.1.0/requirements/refresh.yml`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/requirements/requirements.txt` & `fedrq-1.1.0/requirements/requirements.txt`

 * *Files 13% similar despite different names*

```diff
@@ -6,25 +6,25 @@
 #
 annotated-types==0.6.0
     # via pydantic
 certifi==2024.2.2
     # via requests
 charset-normalizer==3.3.2
     # via requests
-idna==3.6
+idna==3.7
     # via requests
-pydantic==2.6.4
+pydantic==2.7.1
     # via fedrq (pyproject.toml)
-pydantic-core==2.16.3
+pydantic-core==2.18.2
     # via pydantic
 requests==2.31.0
     # via fedrq (pyproject.toml)
 rpm==0.1.0
     # via fedrq (pyproject.toml)
 tomli==2.0.1 ; python_version < "3.11"
     # via fedrq (pyproject.toml)
-typing-extensions==4.10.0
+typing-extensions==4.11.0
     # via
     #   pydantic
     #   pydantic-core
 urllib3==2.2.1
     # via requests
```

### Comparing `fedrq-1.0.0/requirements/test.txt` & `fedrq-1.1.0/requirements/test.txt`

 * *Files 5% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 #
 annotated-types==0.6.0
     # via pydantic
 certifi==2024.2.2
     # via requests
 charset-normalizer==3.3.2
     # via requests
-exceptiongroup==1.2.0
+exceptiongroup==1.2.1
     # via pytest
-idna==3.6
+idna==3.7
     # via requests
 iniconfig==2.0.0
     # via pytest
 packaging==24.0
     # via pytest
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
-pydantic==2.6.4
+pydantic==2.7.1
     # via fedrq (pyproject.toml)
-pydantic-core==2.16.3
+pydantic-core==2.18.2
     # via pydantic
-pytest==8.1.1
+pytest==8.2.0
     # via
     #   fedrq (pyproject.toml)
     #   pytest-mock
 pytest-mock==3.14.0
     # via fedrq (pyproject.toml)
 requests==2.31.0
     # via fedrq (pyproject.toml)
@@ -36,13 +36,13 @@
     # via fedrq (pyproject.toml)
 tomli==2.0.1 ; python_version < "3.11"
     # via
     #   fedrq (pyproject.toml)
     #   pytest
 tomli-w==1.0.0
     # via fedrq (pyproject.toml)
-typing-extensions==4.10.0
+typing-extensions==4.11.0
     # via
     #   pydantic
     #   pydantic-core
 urllib3==2.2.1
     # via requests
```

### Comparing `fedrq-1.0.0/requirements/typing.txt` & `fedrq-1.1.0/requirements/typing.txt`

 * *Files 14% similar despite different names*

```diff
@@ -2,43 +2,43 @@
 # This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
 #    pip-compile --allow-unsafe --extra=typing --output-file=requirements/typing.txt --strip-extras
 #
 annotated-types==0.6.0
     # via pydantic
-argcomplete==3.2.3
+argcomplete==3.3.0
     # via fedrq (pyproject.toml)
 certifi==2024.2.2
     # via requests
 charset-normalizer==3.3.2
     # via requests
-idna==3.6
+idna==3.7
     # via requests
-mypy==1.9.0
+mypy==1.10.0
     # via fedrq (pyproject.toml)
 mypy-extensions==1.0.0
     # via mypy
-pydantic==2.6.4
+pydantic==2.7.1
     # via fedrq (pyproject.toml)
-pydantic-core==2.16.3
+pydantic-core==2.18.2
     # via pydantic
 requests==2.31.0
     # via fedrq (pyproject.toml)
 rpm==0.1.0
     # via fedrq (pyproject.toml)
 tomli==2.0.1 ; python_version < "3.11"
     # via
     #   fedrq (pyproject.toml)
     #   mypy
 tomli-w==1.0.0
     # via fedrq (pyproject.toml)
-types-requests==2.31.0.20240311
+types-requests==2.31.0.20240406
     # via fedrq (pyproject.toml)
-typing-extensions==4.10.0
+typing-extensions==4.11.0
     # via
     #   fedrq (pyproject.toml)
     #   mypy
     #   pydantic
     #   pydantic-core
 urllib3==2.2.1
     # via
```

### Comparing `fedrq-1.0.0/ruff.toml` & `fedrq-1.1.0/ruff.toml`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/src/fedrq/__init__.py` & `fedrq-1.1.0/src/fedrq/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 
 import logging
 import os
 import warnings
 
 import pydantic
 
-__version__ = "1.0.0"
+__version__ = "1.1.0"
 
 
 def _filter_pydantic_v2_warnings() -> None:
-    typ: DeprecationWarning | None
+    typ: type[DeprecationWarning] | None
     if typ := getattr(pydantic, "PydanticDeprecatedSince20", None):
         warnings.simplefilter(action="ignore", category=typ)
 
 
 if "_FEDRQ_SHOW_PYDANTIC_WARNINGS" not in os.environ:
     _filter_pydantic_v2_warnings()
```

### Comparing `fedrq-1.0.0/src/fedrq/_archive.py` & `fedrq-1.1.0/src/fedrq/_archive.py`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/src/fedrq/_compat.py` & `fedrq-1.1.0/src/fedrq/_compat.py`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/src/fedrq/_utils.py` & `fedrq-1.1.0/src/fedrq/_utils.py`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/src/fedrq/backends/__init__.py` & `fedrq-1.1.0/src/fedrq/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/src/fedrq/backends/base/__init__.py` & `fedrq-1.1.0/src/fedrq/config.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,621 +1,461 @@
-# SPDX-FileCopyrightText: 2023 Maxwell G <gotmax@e.email>
+# SPDX-FileCopyrightText: 2022 Maxwell G <gotmax@e.email>
 # SPDX-License-Identifier: GPL-2.0-or-later
 
+"""
+This module houses code to load configuration from the filesystem and validate
+it.
+"""
+
 from __future__ import annotations
 
-import abc
-import dataclasses
-import importlib.resources
+import importlib.resources as importlib_resources
+import itertools
 import logging
-from collections.abc import Callable, Collection, Iterable, Iterator
-from datetime import date
-from typing import TYPE_CHECKING, Any, Optional, Protocol, TypeVar, runtime_checkable
-from warnings import warn
-
-if TYPE_CHECKING:
-    from _typeshed import StrPath
+import os
+import re
+import sys
+import typing as t
+import zipfile
+from collections.abc import Callable
+from enum import auto as auto_enum
+from pathlib import Path
+
+if sys.version_info < (3, 11):
+    from importlib.abc import Traversable
+
+    import tomli as tomllib
+else:
+    from importlib.resources.abc import Traversable
+
+    import tomllib
+
+from pydantic import BaseModel, Field, PrivateAttr, validator
+
+from fedrq._compat import StrEnum
+from fedrq._config import ConfigError
+from fedrq._utils import merge_dict, mklog
+from fedrq.backends import BACKENDS, get_default_backend
+from fedrq.backends.base import BaseMakerBase
+from fedrq.release_repo import AliasRepoG, DefaultRepoGs, RepoG, Repos
+
+if t.TYPE_CHECKING:
+    import dnf
+    import libdnf5
+
+    from fedrq.backends.base import BackendMod, RepoqueryBase
+
+CONFIG_DIRS = (Path.home() / ".config/fedrq", Path("/etc/fedrq"))
+DEFAULT_REPO_CLASS = "base"
+DEFAULT_COPR_BASEURL = "https://copr.fedoraproject.org"
+logger = logging.getLogger(__name__)
+
+
+class LoadFilelists(StrEnum):
+    auto = auto_enum()
+    always = auto_enum()
+    never = auto_enum()
+
+    @classmethod
+    def from_bool(cls, /, boolean: bool) -> LoadFilelists:
+        return cls.always if boolean else cls.never
+
+    def __bool__(self) -> bool:
+        return self == LoadFilelists.always
+
+
+class ReleaseConfig(BaseModel):
+    name: str = Field(exclude=True)
+    defs: dict[str, list[str]]
+    version: t.Optional[str] = None
+    matcher: t.Pattern
+    repo_dirs: list[Path] = Field(
+        default_factory=lambda: [
+            directory.joinpath("repos") for directory in CONFIG_DIRS
+        ]
+    )
+    defpaths: set[str] = Field(default_factory=set)
+    # full_def_paths is undocumented.
+    # It'll be set based on defpaths during model validation.
+    full_def_paths: list[t.Union[Traversable, Path]] = []
+    system_repos: bool = True
+    append_system_repos: bool = False
+
+    koschei_collection: t.Optional[str] = None
+    copr_chroot_fmt: t.Optional[str] = None
+
+    repo_aliases: dict[str, str] = {}
+    repogs: Repos = Field(DefaultRepoGs, exclude=True)
+
+    class Config:
+        arbitrary_types_allowed = True
+
+    @validator("repogs", always=True)
+    def _v_repogs(cls, value: Repos, values: dict[str, t.Any]) -> Repos:
+        return (
+            value | values["defs"] | AliasRepoG.from_str_mapping(values["repo_aliases"])
+        )
+
+    @validator("full_def_paths", always=True, pre=True)
+    def _v_full_def_paths(cls, value, values) -> list[t.Union[Traversable, Path]]:
+        # We don't care about what `value` is set to.
+        # It should be computed based on defpaths.
+        del value
+
+        defpaths = values["defpaths"].copy()
+        flog = mklog(__name__, "ReleaseConfig", "_get_full_defpaths")
+        flog.debug(f"Getting defpaths for {values['name']}: {defpaths}")
+        return cls._get_full_defpaths(values["name"], defpaths, values["repo_dirs"])
+
+    @validator("matcher")
+    def _v_matcher(cls, value: t.Pattern, values: dict[str, t.Any]) -> t.Pattern:
+        if not values["version"] and value.groups != 1:
+            raise ValueError("'matcher' must have exactly one capture group")
+        return value
+
+    @validator("repo_dirs", pre=True)
+    def _v_repo_dirs(cls, value: str | list[Path]) -> list[Path]:
+        if not isinstance(value, str):
+            return value
+        return [Path(directory) for directory in value.split(":")]
+
+    @validator("append_system_repos", always=True)
+    def _v_append_system_repos(cls, value: bool, values: dict[str, t.Any]) -> bool:
+        if value:
+            values["system_repos"] = True
+        return value
+
+    def is_match(self, val: str) -> bool:
+        return bool(re.fullmatch(self.matcher, val))
+
+    def is_valid_repo(self, val: str) -> bool:
+        try:
+            self.repogs.get_repo(val)
+        except ConfigError:
+            return False
+        else:
+            return True
 
-    from fedrq.config import Release
+    @staticmethod
+    def _repo_dir_iterator(
+        repo_dirs: list[Path],
+    ) -> t.Iterator[t.Union[Traversable, Path]]:
+        flog = mklog(__name__, "ReleaseConfig", "_repo_dir_iterator")
+        topdirs: tuple[t.Union[Traversable, Path], ...] = (
+            *repo_dirs,
+            importlib_resources.files("fedrq.data.repos"),
+        )
+        flog.debug("topdirs = %s", topdirs)
+        for topdir in topdirs:
+            if isinstance(topdir, Path):
+                topdir = topdir.expanduser()
+            if not topdir.is_dir():
+                continue
+            for file in topdir.iterdir():
+                if file.is_file():
+                    yield file
+
+    @classmethod
+    def _get_full_defpaths(
+        cls, name: str, defpaths: set[str], repo_dirs: list[Path]
+    ) -> list[t.Union[Traversable, Path]]:
+        missing_absolute: list[t.Union[Traversable, Path]] = []
+        full_defpaths: list[t.Union[Traversable, Path]] = []
+        flog = mklog(__name__, cls.__name__, "_get_full_defpaths")
+        flog.debug(f"Searching for absolute defpaths: {defpaths}")
+        for defpath in defpaths.copy():
+            if (path := Path(defpath).expanduser()).is_absolute():
+                flog.debug(f"Is absolute: {path}")
+                defpaths.discard(defpath)
+                if path.is_file():
+                    flog.debug(f"Exists: {path}")
+                    full_defpaths.append(path)
+                else:
+                    flog.debug(f"Doesn't Exist: {path}")
+                    missing_absolute.append(path)
+        flog.debug(f"Getting relative defpaths: {defpaths}")
+        files = cls._repo_dir_iterator(repo_dirs)
+        while defpaths:
+            try:
+                file = next(files)
+                flog.debug(f"file={file}")
+            except StopIteration:
+                flog.debug(msg="StopIteration")
+                break
+            if file.name in defpaths:
+                flog.debug(f"{file.name} in {defpaths}")
+                full_defpaths.append(file)
+                defpaths.discard(file.name)
+        if defpaths:
+            _missing = ", ".join(
+                sorted(str(p) for p in ((*defpaths, *missing_absolute)))
+            )
+            raise ConfigError(f"Missing defpaths in {name}: {_missing}")
+        return full_defpaths
 
-_QueryT = TypeVar("_QueryT", bound="PackageQueryCompat")
-LOG = logging.getLogger("fedrq.backends")
+    def get_release(
+        self, config: RQConfig, branch: str, repo_name: str = "base"
+    ) -> Release:
+        return Release(
+            config=config, release_config=self, branch=branch, repo_name=repo_name
+        )
 
 
-@runtime_checkable
-class PackageCompat(Protocol):  # pragma: no cover
+class Release:
     """
-    Common interface provided by dnf.package.Package and other backends
+    Encapsulates a ReleaseConfig with a specific version and repo name.
+    This SHOULD NOT be instantiated directly.
+    The __init__() has no stability promises.
+    Use the [`RQConfig.get_release()`][fedrq.config.RQConfig.get_release]
+    factory instead.
     """
 
-    @property
-    def name(self) -> str: ...
-
-    @property
-    def arch(self) -> str: ...
-
-    @property
-    def a(self) -> str: ...
-
-    @property
-    def epoch(self) -> int: ...
-
-    @property
-    def e(self) -> int: ...
-
-    @property
-    def version(self) -> str: ...
-
-    @property
-    def v(self) -> str: ...
-
-    @property
-    def release(self) -> str: ...
-
-    @property
-    def r(self) -> str: ...
-
-    @property
-    def from_repo(self) -> str: ...
-
-    @property
-    def evr(self) -> str: ...
-
-    @property
-    def debug_name(self) -> str: ...
-
-    @property
-    def source_name(self) -> Optional[str]: ...
-
-    @property
-    def source_debug_name(self) -> str: ...
-
-    @property
-    def installtime(self) -> int: ...
-
-    @property
-    def buildtime(self) -> int: ...
-
-    @property
-    def size(self) -> int: ...
-
-    @property
-    def downloadsize(self) -> int: ...
-
-    @property
-    def installsize(self) -> int: ...
-
-    @property
-    def provides(self) -> Iterable: ...
-
-    @property
-    def requires(self) -> Iterable: ...
-
-    @property
-    def recommends(self) -> Iterable: ...
-
-    @property
-    def suggests(self) -> Iterable: ...
-
-    @property
-    def supplements(self) -> Iterable: ...
-
-    @property
-    def enhances(self) -> Iterable: ...
-
-    @property
-    def obsoletes(self) -> Iterable: ...
-
-    @property
-    def conflicts(self) -> Iterable: ...
-
-    @property
-    def sourcerpm(self) -> Optional[str]: ...
-
-    @property
-    def description(self) -> str: ...
-
-    @property
-    def summary(self) -> str: ...
-
-    @property
-    def license(self) -> str: ...
-
-    @property
-    def url(self) -> str: ...
-
-    @property
-    def reason(self) -> Optional[str]: ...
-
-    @property
-    def files(self) -> Iterable[str]: ...
-
-    @property
-    def reponame(self) -> str: ...
-
-    @property
-    def repoid(self) -> str: ...
-
-    @property
-    def vendor(self) -> str: ...
+    def __init__(
+        self,
+        config: RQConfig,
+        release_config: ReleaseConfig,
+        branch: str,
+        repo_name: str = "base",
+    ) -> None:
+        self.config = config
+        self.release_config = release_config
+        if not self.release_config.is_match(branch):
+            raise ConfigError(
+                f"Branch {branch} does not match {self.release_config.name}"
+            )
+        self.branch = branch
+        self.repo_name = repo_name
+        self.repog: RepoG = self.get_repog(repo_name)
 
-    @property
-    def packager(self) -> str: ...
+    def get_repog(self, key: str) -> RepoG:
+        return self.release_config.repogs.get_repo(key)
 
     @property
-    def location(self) -> str: ...
+    def version(self) -> str:
+        v: str | None = None
+        if self.release_config.version:
+            v = self.release_config.version
+        elif match := re.fullmatch(self.release_config.matcher, self.branch):
+            v = match.group(1)
+        if v is None:
+            raise ValueError(f"{self.branch} does not match {self.release_config.name}")
+        # Special case
+        if v == "$releasever":
+            v = self.config.backend_mod.get_releasever()
+        return v
 
     @property
-    def repo(self) -> Any:
-        """
-        Return the package's Repo object.
-        The exact object depends on which backend is used.
-        """
-
-    @abc.abstractmethod
-    def remote_location(
-        self, schemes: Collection[str] | None = ("http", "ftp", "file", "https")
-    ) -> str | None: ...
-
-    def __hash__(self) -> int: ...
-
-    def __lt__(self, other) -> bool: ...
-
-    def __le__(self, other) -> bool: ...
-
-    def __gt__(self, other) -> bool: ...
-
-    def __ge__(self, other) -> bool: ...
-
-
-@runtime_checkable
-class PackageQueryCompat(Protocol):  # pragma: no cover
-    """
-    Common PackageQuery interface provided by hawkey.Query and other backends.
-    """
-
-    def filter(self, **kwargs) -> PackageQueryCompat:
-        """
-        Filter the PackageQuery.
-        Depending on the backend, this either modifies 'self' in place and
-        return 'self' or return a new PackageQuery object.
-        See https://dnf.readthedocs.io/en/latest/api_queries.html#dnf.query.Query.filter
-        for the allowed kwargs.
-        """
-        ...
-
-    def filterm(self, **kwargs) -> PackageQueryCompat:
-        """
-        Filter the PackageQuery in place and return 'self'.
-        See https://dnf.readthedocs.io/en/latest/api_queries.html#dnf.query.Query.filter
-        for the allowed kwargs.
-        """
-        ...
-
-    def union(self: _QueryT, other: _QueryT) -> _QueryT:
-        """
-        Combine two PackageQuery objects.
-        Depending on the backend, this either modifies 'self' in place and
-        returns 'self' or returns a new PackageQuery object.
-        """
-        ...
-
-    def __len__(self) -> int: ...
-
-    def __iter__(self) -> Iterator[PackageCompat]: ...
-
-
-class BaseMakerBase(metaclass=abc.ABCMeta):
-    """
-    Create a Base object, set configuration, and load repos
-    """
-
-    base: Any
-
-    def __init__(self, base=None) -> None:
-        self.base = base
+    def copr_chroot_fmt(self) -> str | None:
+        return self.release_config.copr_chroot_fmt
 
     @property
-    @abc.abstractmethod
-    def conf(self) -> Any:
-        """
-        Return the backend's Config object
-        """
-        ...
+    def koschei_collection(self) -> str | None:
+        return self.release_config.koschei_collection
 
-    @abc.abstractmethod
-    def fill_sack(
+    def make_base(
         self,
-        *,
-        from_cache: bool = False,
-        load_system_repo: bool = False,
-    ):
+        config: RQConfig | None = None,
+        base_conf: dict[str, t.Any] | None = None,
+        base_vars: dict[str, t.Any] | None = None,
+        base_maker: BaseMakerBase | None = None,
+        fill_sack: bool = True,
+    ) -> dnf.Base | libdnf5.base.Base:
         """
-        Fill the sack and returns the Base object.
-        The repository configuration shouldn't be manipulated after this.
-        'from_cache' isn't currently supported by the libdnf5 backend.
-        """
-        ...
-
-    @abc.abstractmethod
-    def read_system_repos(self, disable: bool = True) -> None:
-        """
-        Load system repositories into the base object.
-        By default, they are all disabled even if 'enabled=1' is in the
-        repository configuration.
-        """
-
-    @abc.abstractmethod
-    def enable_repos(self, repos: Collection[str]) -> None:
-        """
-        Enable a list of repositories by their repoid.
-        Raise a ValueError if the repoid is not in `self.base`'s configuration.
-        """
-
-    @abc.abstractmethod
-    def enable_repo(self, repo: str) -> None:
-        """
-        Enable a repo by its id.
-        Raise a ValueError if the repoid is not in `self.base`'s configuration.
-        """
-
-    @abc.abstractmethod
-    def disable_repo(self, repo: str, ignore_missing: bool = True) -> None:
-        """
-        Disable a repo by its id.
-        Raise a ValueError if the repoid is not in `self.base`'s configuration
-        when ignore_missing is False.
-        """
-
-    @abc.abstractmethod
-    def read_repofile(self, file: StrPath) -> None:
-        """
-        Load repositories from a repo file
-        """
-
-    @abc.abstractmethod
-    def set(self, key: str, value: Any) -> None:
-        """
-        Set configuration options. Must be called before reading repos.
-        """
-        ...
-
-    @abc.abstractmethod
-    def set_var(self, key: str, value: Any) -> None:
-        """
-        Set substitutions (e.g. arch, basearch, releasever).
-        Needs to be called before reading repos.
-        """
-        ...
-
-    # Private for now
-    @abc.abstractmethod
-    def _read_repofile_new(self, file: StrPath, ensure_enabled: bool = False) -> None:
-        """
-        Load repositories from a repo file if they're not already in the
-        configuration.
-        """
-
-    def sets(self, conf: dict[str, Any], substitutions: dict[str, Any]) -> None:
-        """
-        Set options on the base object
-
         Args:
-            conf:
-                A dict of configuration options. Call self.set() for each k-v
-                pair.
-            substitutions:
-                A dict of substitutions/vars options. Call self.set_var() for
-                each k-v pair.
-        """
-        for opt in conf.items():
-            self.set(*opt)
-        for opt in substitutions.items():
-            self.set_var(*opt)
-
-    def load_filelists(self, enable: bool = True) -> None:  # noqa: ARG002
-        # Can be overriden by subclasses. Purposely isn't an @abstractmethod.
-        """
-        Load the filelists if they're not already enabled by default
-
-        Args:
-            enable:
-                Whether to enable or disable filelists
-        """
-        return None
-
-    @abc.abstractmethod
-    def load_changelogs(self, enable: bool = True) -> None:
-        """
-        Load changelog metadata
-
-        Args:
-            enable:
-                Whether to enable or disable filelists
-        """
-
-    def load_release_repos(self, release: Release, set_releasever: bool = True) -> None:
-        """
-        Load the repositories from a fedrq.config.Release object
-
-        Args:
-            release:
-                [`Release`][fedrq.config.Release] object
-            set_releasever:
-                Whether to set the `$releasever` based on the release or just
-                leave it alone
-        """
-        if set_releasever:
-            self.set_var("releasever", release.version)
-        if release.release_config.system_repos:
-            self.read_system_repos(
-                disable=not release.release_config.append_system_repos
+            config:
+                An RQConfig object. If this is not passed, `self.config` is used.
+            base_conf:
+                Base session configuration
+            base_vars:
+                Base session vars/substitutions (arch, basearch,
+                                                           releasever, etc.)
+            base_maker:
+                Existing BaseMaker object to configure. If base_maker is None,
+                a new one will be created.
+            fill_sack:
+                Whether to fill the Base object's package sack or just return
+                the Base object after applying configuration.
+        """
+        if config is None:
+            config = self.config
+        base_conf = base_conf or {}
+        base_vars = base_vars or {}
+        releasever = config.backend_mod.get_releasever()
+        if (
+            "cachedir" not in base_conf
+            and config.smartcache
+            and (config.smartcache == "always" or self.version != releasever)
+        ):
+            logger.debug("Using smartcache")
+            base_conf["cachedir"] = str(get_smartcache_basedir() / str(self.version))
+        bm = base_maker or config.backend_mod.BaseMaker()
+        bm.sets(base_conf, base_vars)
+        bm.load_release_repos(self, "releasever" not in base_vars)
+        if config.load_filelists:
+            bm.load_filelists()
+        if config.load_other_metadata is not None:
+            bm.load_changelogs(config.load_other_metadata)
+        return bm.fill_sack() if fill_sack else bm.base
+
+    def _copr_repo(
+        self, value: str, default_copr_baseurl: str = DEFAULT_COPR_BASEURL
+    ) -> str:
+        value = value.rstrip("/")
+        if not self.copr_chroot_fmt:
+            raise ValueError(
+                f"{self.release_config.name} does not have 'copr_chroot_fmt' set"
             )
-        for path in release.release_config.full_def_paths:
-            with importlib.resources.as_file(path) as fp:
-                LOG.debug("Reading %s", fp)
-                self._read_repofile_new(fp)
-        release.repog.load(self, release.config, release)
-
-    @abc.abstractmethod
-    def create_repo(self, repoid: str, **kwargs: Any) -> None:
-        """
-        Add a Repo object to the repo sack and configure it.
-
-        Args:
-            repoid:
-                Repository ID
-            kwargs:
-                key-values options that should be set on the Repo object values
-                (like $basearch) will be substituted automatically.
-        """
-        ...
-
-    @property
-    @abc.abstractmethod
-    def backend(self) -> BackendMod: ...
-
-    @abc.abstractmethod
-    def repolist(self, enabled: bool | None = None) -> list[str]: ...
-
-    @abc.abstractmethod
-    def enable_source_repos(self) -> None:
-        """
-        Enable the corresponding -source repos of the currently enabled
-        repositories
-        """
-        ...
-
-
-class NEVRAFormsCompat(Protocol):
-    NEVRA: int
-    NEVR: int
-    NEV: int
-    NA: int
-    NAME: int
-
-
-class RepoqueryBase(metaclass=abc.ABCMeta):
-    """
-    Helpers to query a repository.
-    Provides a unified repoquery interface for different backends.
-    """
-
-    def __init__(self, base) -> None:
-        self.base = base
-
-    @property
-    @abc.abstractmethod
-    def base_arches(self) -> set[str]:
-        """
-        Return a set of the system's arch and basearch.
-        """
-        ...
-
-    def _get_resolve_options(
-        self,
-        resolve: bool,
-        with_filenames: bool | None,
-        with_provides: bool | None,
-        resolve_provides: bool | None,
-    ) -> dict[str, Any]:
-        opts: dict[str, bool | None] = {
-            "with_filenames": with_filenames,
-            "with_provides": with_provides,
-            "resolve_provides": resolve_provides,
+        chroot = re.sub("-{arch}$", "", self.copr_chroot_fmt).format(
+            version=self.version
+        )
+        if value.startswith(("http://", "https://")):
+            return value + "/" + chroot
+
+        frag = "coprs/"
+        if value.startswith("@"):
+            frag += "g/"
+            value = value[1:]
+        value, sep, copr_baseurl = value.partition("@")
+        if not sep:
+            copr_baseurl = default_copr_baseurl.rstrip("/")
+        elif not copr_baseurl.startswith(("http://", "https://")):
+            copr_baseurl = "https://" + copr_baseurl
+        frag += value
+        return f"{copr_baseurl}/{frag}/repo/{chroot}"
+
+
+class RQConfig(BaseModel):
+    backend: t.Optional[str] = os.environ.get("FEDRQ_BACKEND")
+    releases: dict[str, ReleaseConfig]
+    default_branch: str = os.environ.get("FEDRQ_BRANCH", "rawhide")
+    smartcache: t.Union[bool, t.Literal["always"]] = True
+    load_other_metadata: t.Optional[bool] = None
+    load_filelists: LoadFilelists = LoadFilelists.auto
+    _backend_mod: BackendMod | None = PrivateAttr(None)
+    copr_baseurl: str = DEFAULT_COPR_BASEURL
+
+    class Config:
+        json_encoders: dict[t.Any, Callable[[t.Any], str]] = {
+            re.Pattern: lambda pattern: pattern.pattern,
+            zipfile.Path: lambda path: str(path),
         }
-        return {key: resolve if opt is None else opt for key, opt in opts.items()}
-
-    @abc.abstractmethod
-    def resolve_pkg_specs(
-        self,
-        specs: Collection[str],
-        resolve: bool = False,
-        latest: int | None = None,
-        with_src: bool = True,
-        *,
-        with_filenames: bool | None = None,
-        with_provides: bool | None = None,
-        resolve_provides: bool | None = None,
-    ) -> PackageQueryCompat:
-        """
-        Resolve pkg specs.
-        See
-        https://dnf.readthedocs.io/en/latest/command_ref.html?highlight=spec#specifying-packages
-        or
-        https://dnf5.readthedocs.io/en/latest/misc/specs.7.html
-        for valid forms.
-
-        Args:
-            specs:
-                Package specs to resolve.
-            resolve:
-                Whether to resolve file paths or virtual Provides in addition
-                to package specs
-            latest:
-                Limit packages with the same name and arch.
-            with_src:
-                Whether to consider `.src` packages when resolving `specs`
-        """
-        ...
-
-    def arch_filterm(
-        self, query: PackageQueryCompat, arch: str | Iterable[str] | None = None
-    ) -> PackageQueryCompat:
-        """
-        Filter a query's architectures in place and return it.
-        It includes a little more functionality than query.filterm(arch=...).
-
-        - When arch is None, the query is left untouched.
-        - If arch equals 'notsrc', all src and multilib packages are
-          excluded.
-        - If arch equals 'arched', all noarch, multilib, and source
-          packages are excluded.
-        - Otherwise, arch is passed to query.filterm(arch=...) and no other
-          validation is preformed.
-        """
-        if not arch:
-            return query
-        if arch == "notsrc":
-            return query.filterm(arch=(*self.base_arches, "noarch"))  # type: ignore
-        elif arch == "arched":
-            return query.filterm(arch=self.base.conf.basearch)
-        else:
-            return query.filterm(arch=arch)
-
-    def arch_filter(
-        self, query: PackageQueryCompat, arch: str | Iterable[str] | None = None
-    ) -> PackageQueryCompat:
-        """
-        Filter a query's architectures and return it.
-        It includes a little more functionality than query.filter(arch=...).
-
-        - When arch is None, the query is left untouched.
-        - If arch equals 'notsrc', all src and multilib packages are
-          excluded.
-        - If arch equals 'arched', all noarch, multilib, and source
-          packages are excluded.
-        - Otherwise, arch is passed to query.filterm(arch=...) and no other
-          validation is preformed.
-        """
-        if not arch:
-            return query
-        if arch == "notsrc":
-            return query.filter(arch=(*self.base_arches, "noarch"))  # type: ignore
-        if arch == "arched":
-            return query.filter(arch=list(self.base_arches))
-        return query.filter(arch=arch)
-
-    @abc.abstractmethod
-    def _query(self) -> PackageQueryCompat:
-        """
-        Return the PackageQuery object for this backend
-        """
-        return self.base.sack.query()
+        validate_assignment = True
 
-    def query(
-        self, *, arch: str | Iterable[str] | None = None, **kwargs
-    ) -> PackageQueryCompat:
-        """
-        Return an inital PackageQuery that's filtered with **kwargs.
-        Further filtering can be applied with the PackageQuery's filter and
-        filterm methods.
-        """
-        if kwargs.get("latest") is None:
-            kwargs.pop("latest", None)
-        query = self._query()
-        query.filterm(**kwargs)
-        self.arch_filterm(query, arch)
-        return query
-
-    def get_package(
-        self,
-        name: str,
-        arch: str | Iterable[str] | None = None,
-    ) -> PackageCompat:
-        """
-        Return the latest Package that matches the 'name' and 'arch'.
-        A ValueError is raised when no matches are found.
-        """
-        query = self.query(name=name, arch=arch, latest=1)
-        if len(query) < 1:
-            raise ValueError(f"Zero packages found for {name} on {arch}")
-        return next(iter(query))
-
-    def get_subpackages(
-        self, packages: Iterable[PackageCompat], **kwargs
-    ) -> PackageQueryCompat:
-        """
-        Return a PackageQuery containing the binary RPMS/subpackages produced
-        by {packages}.
+    @validator("backend")
+    def _v_backend(cls, value) -> str:
+        assert (
+            value is None or value in BACKENDS
+        ), f"Valid backends are: {', '.join(BACKENDS)}"
+        return value
+
+    @property
+    def backend_mod(self) -> BackendMod:
+        if not self._backend_mod:
+            self._backend_mod = get_default_backend(
+                self.backend,
+                # allow falling back to a non default backend
+                # (i.e. not backends.DEFAULT_BACKEND)
+                # when the user does not explicitly request a backend.
+                fallback=not bool(self.backend),
+            )
+        return self._backend_mod
 
-        Args:
-            packages:
-                An interable of `PackageCompat` containing source packages
-        """
-        arch = kwargs.get("arch")
-        if arch == "src":
-            raise ValueError("{arch} cannot be 'src'")
-        elif not arch:
-            kwargs.setdefault("arch__neq", "src")
-        if val := kwargs.pop("sourcerpm", None):
-            warn(f"Removing invalid kwarg: 'sourcerpm={val}")
-
-        for package in packages:
-            if package.arch != "src":
-                raise ValueError(f"{package} must be a source package.")
-
-        sourcerpms = [
-            f"{package.name}-{package.version}-{package.release}.src.rpm"
-            for package in packages
-        ]
-        query = self.query(sourcerpm=sourcerpms, **kwargs)
-        return query
+    def get_release(
+        self, branch: str | None = None, repo_name: str | None = None
+    ) -> Release:
+        flog = mklog(__name__, "RQConfig", "get_releases")
+        branch = branch or self.default_branch
+        repo_name = repo_name or DEFAULT_REPO_CLASS
+        pair = (branch, repo_name)
+        for release in sorted(
+            self.releases.values(), key=lambda r: r.name, reverse=True
+        ):
+            try:
+                r = release.get_release(self, branch=branch, repo_name=repo_name)
+            except ConfigError as exc:
+                logger.debug(f"{release.name} does not match {pair}: {exc}")
+            else:
+                flog.debug("%s matches %s", release.name, pair)
+                return r
+        raise ConfigError(
+            "{} does not much any of the configured releases: {}".format(
+                pair, self.release_names
+            )
+        )
 
     @property
-    @abc.abstractmethod
-    def backend(self) -> BackendMod: ...
-
-
-@dataclasses.dataclass(frozen=True)
-class ChangelogEntry:
-    """
-    Data class for changelog entry data.
-    Do not instantiate directly!
-    """
-
-    text: str
-    author: str
-    date: date
-
-    def __str__(self) -> str:
-        date_str = format(self.date, "%a %b %d %Y")
-        return f"* {date_str} {self.author}\n{self.text}"
+    def release_names(self) -> list[str]:
+        return [rc.name for rc in self.releases.values()]
 
+    def get_rq(
+        self,
+        branch: str | None = None,
+        repo: str | None = None,
+        base_conf: dict[str, t.Any] | None = None,
+        base_vars: dict[str, t.Any] | None = None,
+    ) -> RepoqueryBase:
+        """
+        Higher level interface that finds the Release object that mathces
+        {branch} and {repo}, creates a (lib)dnf(5).base.Base session, and
+        returns a Repoquery object.
 
-class _get_changelogs(Protocol):
-    def __call__(self, package: Any) -> Iterator[ChangelogEntry]:
-        """
         Args:
-            package:
-                A backend's Package object
-        """
-        ...
-
-
-class BackendMod(Protocol):
-    """
-    Protocol for a fedrq backend module.
-    Each backend module (e.g.
-    [`fedrq.backends.dnf.backend`][fedrq.backends.dnf.backend])
-    implements this interface.
-    """
-
-    BACKEND: str
-    BaseMaker: type[BaseMakerBase]
-    Package: type[PackageCompat]
-    NEVRAForms: type[NEVRAFormsCompat]
-    PackageQuery: type[PackageQueryCompat]
-    Repoquery: type[RepoqueryBase]
-    RepoError: type[BaseException]
-    get_releasever: Callable[[], str]
-    get_changelogs: _get_changelogs
+            branch:
+                branch name
+            repo:
+                repo class. defaults to 'base'.
+            base_conf:
+                Base session configuration
+            base_vars:
+                Base session vars/substitutions (arch, basearch, releasever,
+                                                 etc.)
+        """
+        release = self.get_release(branch, repo)
+        return self.backend_mod.Repoquery(release.make_base(self, base_conf, base_vars))
+
+
+def get_smartcache_basedir() -> Path:
+    basedir = Path(os.environ.get("XDG_CACHE_HOME", Path("~/.cache").expanduser()))
+    return basedir.joinpath("fedrq").resolve()
+
+
+def _get_files(
+    directory: t.Union[Traversable, Path], suffix: str, reverse: bool = True
+) -> list[t.Union[Traversable, Path]]:
+    files: list[t.Union[Traversable, Path]] = []
+    if not directory.is_dir():
+        return files
+    for file in directory.iterdir():
+        if file.name.endswith(suffix) and file.is_file():
+            files.append(file)
+    return sorted(files, key=lambda f: f.name, reverse=reverse)
+
+
+def get_config(**overrides: t.Any) -> RQConfig:
+    """
+    Retrieve config files from CONFIG_DIRS and fedrq.data.
+    Perform naive top-level merging of the 'releases' table.
+    """
+    flog = mklog(__name__, "get_config")
+    flog.debug(f"CONFIG_DIRS = {CONFIG_DIRS}")
+    config: dict[str, t.Any] = {}
+    all_files: list[list[t.Union[Traversable, Path]]] = [
+        _get_files(importlib_resources.files("fedrq.data"), ".toml"),
+        *(_get_files(p, ".toml") for p in reversed(CONFIG_DIRS)),
+    ]
+    flog.debug("all_files = %s", all_files)
+    for path in itertools.chain.from_iterable(all_files):
+        flog.debug("Loading config file: %s", path)
+        with path.open("rb") as fp:
+            data = tomllib.load(t.cast("t.BinaryIO", fp))
+        merge_dict(data, config)
+    merge_dict(overrides, config)
+    config["releases"] = _get_releases(config["releases"])
+    flog.debug("Final config: %s", config)
+    return RQConfig(**config)
+
+
+def _get_releases(rdict: dict[str, dict[str, t.Any]]) -> dict[str, t.Any]:
+    releases: dict[str, t.Any] = {}
+    for name, data in rdict.items():
+        releases[name] = dict(name=name, **data)
+    return releases
```

### Comparing `fedrq-1.0.0/src/fedrq/backends/dnf/__init__.py` & `fedrq-1.1.0/src/fedrq/backends/dnf/__init__.py`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/src/fedrq/backends/dnf/backend/__init__.py` & `fedrq-1.1.0/src/fedrq/backends/dnf/backend/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,14 +35,20 @@
     raise MissingBackendError from None
 
 if t.TYPE_CHECKING:
     from _typeshed import StrPath
 
 LOG = logging.getLogger(__name__)
 
+PackageCompat.register(dnf.package.Package)
+Package: type[PackageCompat] = dnf.package.Package
+PackageQueryCompat.register(dnf.query.Query)
+PackageQuery: type[PackageQueryCompat] = dnf.query.Query
+RepoError = dnf.exceptions.RepoError
+
 
 class BaseMaker(BaseMakerBase):
     """
     Create a Base object and load repos
     """
 
     base: dnf.Base
@@ -191,15 +197,17 @@
     NEVRA = hawkey.FORM_NEVRA
     NEVR = hawkey.FORM_NEVR
     NEV = hawkey.FORM_NEV
     NA = hawkey.FORM_NA
     NAME = hawkey.FORM_NAME
 
 
-class Repoquery(RepoqueryBase):
+# Use PackageCompat and PackageQueryCompat as the TypeVar, as the the native dnf objects
+# don't provide typing.
+class Repoquery(RepoqueryBase[PackageQueryCompat[PackageCompat]]):
     def __init__(self, base: dnf.Base) -> None:
         self.base: dnf.Base = base
 
     @property
     def base_arches(self) -> set[str]:
         return {self.base.conf.arch, self.base.conf.basearch}
 
@@ -244,19 +252,14 @@
 def get_releasever():
     """
     Return the system releasever
     """
     return dnf.rpm.detect_releasever("/")
 
 
-Package: PackageCompat = dnf.package.Package
-PackageQuery: PackageQueryCompat = dnf.query.Query
-RepoError = dnf.exceptions.RepoError
-
-
 def get_changelogs(package: t.Any) -> Iterator[ChangelogEntry]:
     for entry in package.changelogs:
         yield ChangelogEntry(
             text=entry["text"], author=entry["author"], date=entry["timestamp"]
         )
```

### Comparing `fedrq-1.0.0/src/fedrq/backends/libdnf5/__init__.py` & `fedrq-1.1.0/src/fedrq/backends/libdnf5/__init__.py`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/src/fedrq/backends/libdnf5/backend/__init__.py` & `fedrq-1.1.0/src/fedrq/backends/libdnf5/backend/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,22 @@
 from datetime import timezone as TZ
 from enum import Enum
 from os.path import join as path_join
 from urllib.parse import urlparse
 
 from fedrq._utils import filter_latest
 from fedrq.backends import MissingBackendError
-from fedrq.backends.base import BackendMod, BaseMakerBase, ChangelogEntry, RepoqueryBase
+from fedrq.backends.base import (
+    BackendMod,
+    BaseMakerBase,
+    ChangelogEntry,
+    PackageCompat,
+    PackageQueryCompat,
+    RepoqueryBase,
+)
 from fedrq.backends.libdnf5 import BACKEND  # noqa: F401
 
 if t.TYPE_CHECKING:
     from _typeshed import StrPath
     from typing_extensions import TypeAlias, Unpack
 
 
@@ -203,15 +210,19 @@
             config_loaded:
                 Set to True if base.load_config_from_file() has already been
                 called. Only applies when `base` is passed.
         """
         self.base = base or libdnf5.base.Base()
         self.initialized = initialized if base else False
         if not base or not config_loaded:
-            self.base.load_config_from_file()
+            # dnf 5.2.0
+            try:
+                self.base.load_config()
+            except AttributeError:
+                self.base.load_config_from_file()
 
     def setup(self) -> None:
         if not self.initialized:
             self.base.setup()
             self.initialized = True
 
     @property
@@ -264,15 +275,22 @@
         Fill the sack and returns the Base object.
         The repository configuration shouldn't be manipulated after this.
 
         Note that the `_cachedir` arg is private and subject to removal.
         """
         if from_cache:
             raise NotImplementedError
-        self.rs.update_and_load_enabled_repos(load_system_repo)
+        try:
+            self.rs.load_repos(
+                libdnf5.repo.Repo.Type_SYSTEM
+                if load_system_repo
+                else libdnf5.repo.Repo.Type_AVAILABLE
+            )
+        except AttributeError:
+            self.rs.update_and_load_enabled_repos(load_system_repo)
         return self.base
 
     def read_system_repos(self, disable: bool = True) -> None:
         """
         Load system repositories into the base object.
         By default, they are all disabled even if 'enabled=1' is in the
         repository configuration.
@@ -433,16 +451,15 @@
             repoq.filter_enabled(enabled)
         return [r.get_id() for r in repoq]
 
     def enable_source_repos(self) -> None:
         self.rs.enable_source_repos()
 
 
-@functools.total_ordering
-class Package(libdnf5.rpm.Package):
+class Package(libdnf5.rpm.Package, PackageCompat):
     DEBUGINFO_SUFFIX = "-debuginfo"
     DEBUGSOURCE_SUFFIX = "-debugsource"
     """
     libdnf5.rpm.Package subclass with strong dnf.package.Package compatability
     """
 
     def __hash__(self) -> int:
@@ -454,17 +471,23 @@
         if self.name != other.name:
             return self.name > other.name
         evrcmp = libdnf5.rpm.rpmvercmp(self.get_evr(), other.get_evr())
         if evrcmp != 0:
             return evrcmp > 0
         return self.get_arch() > other.get_arch()
 
+    def __ge__(self, other) -> bool:
+        return self > other or self == other
+
     def __lt__(self, other) -> bool:
         return not (self > other)
 
+    def __le__(self, other) -> bool:
+        return self < other or self == other
+
     @property
     def name(self) -> str:
         return self.get_name()
 
     @property
     def arch(self) -> str:
         return self.get_arch()
@@ -663,15 +686,44 @@
     def __str__(self) -> str:
         return self.to_string()
 
 
 libdnf5._rpm.Reldep_swigregister(Reldep5)
 
 
-class PackageQuery(libdnf5.rpm.PackageQuery):
+def _getattr_compat(obj: t.Any, attr: str, /) -> t.Any:
+    """
+    Compatability with `get_foo()` methods from dnf 5.2.0
+    """
+    meth_name = f"get_{attr}"
+    if meth := getattr(obj, meth_name, None):
+        return meth()
+    return getattr(obj, attr)
+
+
+_gc = _getattr_compat
+
+
+def _setattr_compat(obj: t.Any, attr: str, value: t.Any, /) -> None:
+    """
+    Compatability with `set_foo()` methods from dnf 5.2.0
+    """
+    meth_name = f"set_{attr}"
+    if meth := getattr(obj, meth_name, None):
+        meth(value)
+    elif hasattr(obj, attr):
+        setattr(obj, attr, value)
+    else:
+        raise AttributeError(attr)
+
+
+_sc = _setattr_compat
+
+
+class PackageQuery(libdnf5.rpm.PackageQuery, PackageQueryCompat[Package]):
     __rq__: Repoquery
 
     """
     Subclass of libdnf5.rpm.PackageQuery with hawkey.Query compatability
     """
 
     def _filter(  # type: ignore[override]
@@ -705,14 +757,17 @@
             self.clear()
             return None
         if kwargs.pop("downgrades", None):
             self.filter_downgrades()
         for key, value in kwargs.items():
             split = key.rsplit("__", 1)
             name = "filter_" + filter_mapping.get(split[0], split[0])
+            # TODO: Remove _convert_value once we drop support for libdnf5
+            # 5.2.0 and can rely on support for passing plain strings to query
+            # functions.
             args = [_convert_value(key, value)]
             if len(split) == 2:
                 args.append(comp_mapping[split[1]])
             getattr(self, name)(*args)
 
     def filterm(  # type: ignore[override]
         self,
@@ -805,15 +860,15 @@
     NEVRA = libdnf5.rpm.Nevra.Form_NEVRA
     NEVR = libdnf5.rpm.Nevra.Form_NEVR
     NEV = libdnf5.rpm.Nevra.Form_NEV
     NA = libdnf5.rpm.Nevra.Form_NA
     NAME = libdnf5.rpm.Nevra.Form_NAME
 
 
-class Repoquery(RepoqueryBase):
+class Repoquery(RepoqueryBase[PackageQuery]):
     def __init__(self, base: libdnf5.base.Base) -> None:
         self.base: libdnf5.base.Base = base
 
     @property
     def base_arches(self) -> set[str]:
         base_vars = self.base.get_vars()
         return {base_vars.get_value("arch"), base_vars.get_value("basearch")}
@@ -840,20 +895,22 @@
         resolve_provides: bool | None = None,
         nevra_forms: list[NEVRAForms] | None = None,
     ) -> PackageQuery:
         opts = self._get_resolve_options(
             resolve, with_filenames, with_provides, resolve_provides
         )
         settings = libdnf5.base.ResolveSpecSettings()
-        settings.with_filenames = opts["with_filenames"]
-        settings.with_provides = opts["with_provides"]
+        _sc(settings, "with_filenames", opts["with_filenames"])
+        _sc(settings, "with_provides", opts["with_provides"])
+        _sc(settings, "nevra_forms", libdnf5.rpm.VectorNevraForm())
         if nevra_forms:
+            v_nevra_forms = libdnf5.rpm.VectorNevraForm()
             for form in nevra_forms:
-                settings.nevra_forms.append(form)
-
+                v_nevra_forms.append(form)
+            _sc(settings, "nevra_forms", v_nevra_forms)
         r_query = self.query(empty=True)
         for spec in specs:
             query = self._query()
             query.resolve_pkg_spec(spec, settings, with_src)
             r_query.union(query)
         if opts["resolve_provides"]:
             r_query = r_query.union(self.query(provides=specs))
@@ -875,16 +932,18 @@
     base = libdnf5.base.Base()
     return libdnf5.conf.Vars.detect_release(base.get_weak_ptr(), "/").get()
 
 
 def get_changelogs(package: Package) -> Iterator[ChangelogEntry]:
     entries = package.get_changelogs()
     for entry in entries:
-        date_obj = DT.fromtimestamp(entry.timestamp, tz=TZ.utc).date()
-        yield ChangelogEntry(text=entry.text, author=entry.author, date=date_obj)
+        date_obj = DT.fromtimestamp(_gc(entry, "timestamp"), tz=TZ.utc).date()
+        yield ChangelogEntry(
+            text=_gc(entry, "text"), author=_gc(entry, "author"), date=date_obj
+        )
 
 
 RepoError = RuntimeError
 
 __all__ = (
     "BACKEND",
     "BaseMaker",
```

### Comparing `fedrq-1.0.0/src/fedrq/cli/__init__.py` & `fedrq-1.1.0/src/fedrq/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/src/fedrq/cli/base.py` & `fedrq-1.1.0/src/fedrq/cli/base.py`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/src/fedrq/cli/commands/COMMAND.py.in` & `fedrq-1.1.0/src/fedrq/cli/commands/COMMAND.py.in`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/src/fedrq/cli/commands/cache.py` & `fedrq-1.1.0/src/fedrq/cli/commands/cache.py`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/src/fedrq/cli/commands/changelogs.py` & `fedrq-1.1.0/src/fedrq/cli/commands/changelogs.py`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/src/fedrq/cli/commands/download.py` & `fedrq-1.1.0/src/fedrq/cli/commands/download.py`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/src/fedrq/cli/commands/formatters.py` & `fedrq-1.1.0/src/fedrq/cli/commands/formatters.py`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/src/fedrq/cli/commands/pkgs.py` & `fedrq-1.1.0/src/fedrq/cli/commands/pkgs.py`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/src/fedrq/cli/commands/repolist.py` & `fedrq-1.1.0/src/fedrq/cli/commands/repolist.py`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/src/fedrq/cli/commands/subpkgs.py` & `fedrq-1.1.0/src/fedrq/cli/commands/subpkgs.py`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/src/fedrq/cli/commands/whatrequires.py` & `fedrq-1.1.0/src/fedrq/cli/commands/whatrequires.py`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/src/fedrq/cli/formatters.py` & `fedrq-1.1.0/src/fedrq/cli/formatters.py`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/src/fedrq/data/releases.toml` & `fedrq-1.1.0/src/fedrq/data/releases.toml`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/src/fedrq/data/repos/almalinux.repo` & `fedrq-1.1.0/src/fedrq/data/repos/almalinux.repo`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/src/fedrq/data/repos/amazonlinux.repo` & `fedrq-1.1.0/src/fedrq/data/repos/amazonlinux.repo`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/src/fedrq/data/repos/centos-stream-compose.repo` & `fedrq-1.1.0/src/fedrq/data/repos/centos-stream-compose.repo`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/src/fedrq/data/repos/centos-stream.repo` & `fedrq-1.1.0/src/fedrq/data/repos/centos-stream.repo`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/src/fedrq/data/repos/centos-stream8-compose.repo` & `fedrq-1.1.0/src/fedrq/data/repos/centos-stream8-compose.repo`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/src/fedrq/data/repos/centos-stream8.repo` & `fedrq-1.1.0/src/fedrq/data/repos/centos-stream8.repo`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/src/fedrq/data/repos/centos7.repo` & `fedrq-1.1.0/src/fedrq/data/repos/centos7.repo`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/src/fedrq/data/repos/eln.repo` & `fedrq-1.1.0/src/fedrq/data/repos/eln.repo`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/src/fedrq/data/repos/epel.repo` & `fedrq-1.1.0/src/fedrq/data/repos/epel.repo`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/src/fedrq/data/repos/fedora-eln.repo` & `fedrq-1.1.0/src/fedrq/data/repos/fedora-eln.repo`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/src/fedrq/data/repos/fedora-rawhide.repo` & `fedrq-1.1.0/src/fedrq/data/repos/fedora-rawhide.repo`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/src/fedrq/data/repos/fedora-updates-testing.repo` & `fedrq-1.1.0/src/fedrq/data/repos/fedora-updates-testing.repo`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/src/fedrq/data/repos/fedora-updates.repo` & `fedrq-1.1.0/src/fedrq/data/repos/fedora-updates.repo`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/src/fedrq/data/repos/fedora.repo` & `fedrq-1.1.0/src/fedrq/data/repos/fedora.repo`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/src/fedrq/data/repos/oraclelinux-8.repo` & `fedrq-1.1.0/src/fedrq/data/repos/oraclelinux-8.repo`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/src/fedrq/data/repos/oraclelinux-9.repo` & `fedrq-1.1.0/src/fedrq/data/repos/oraclelinux-9.repo`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/src/fedrq/data/repos/rocky.repo` & `fedrq-1.1.0/src/fedrq/data/repos/rocky.repo`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/src/fedrq/data/repos/ubi.repo` & `fedrq-1.1.0/src/fedrq/data/repos/ubi.repo`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/src/fedrq/release_repo.py` & `fedrq-1.1.0/src/fedrq/release_repo.py`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/src/fedrq/repoquery.py` & `fedrq-1.1.0/src/fedrq/repoquery.py`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/tests/conftest.py` & `fedrq-1.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/tests/integration/test_backends.py` & `fedrq-1.1.0/tests/integration/test_backends.py`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/tests/integration/test_download.py` & `fedrq-1.1.0/tests/integration/test_download.py`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/tests/integration/test_pkgs.py` & `fedrq-1.1.0/tests/integration/test_pkgs.py`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/tests/integration/test_subpkgs.py` & `fedrq-1.1.0/tests/integration/test_subpkgs.py`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/tests/integration/test_whatrequires.py` & `fedrq-1.1.0/tests/integration/test_whatrequires.py`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/tests/integration/test_whatrequires_src.py` & `fedrq-1.1.0/tests/integration/test_whatrequires_src.py`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/tests/test_data/build.sh` & `fedrq-1.1.0/tests/test_data/build.sh`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/tests/test_data/repos/repo1/specs/e1/packageb.spec` & `fedrq-1.1.0/tests/test_data/repos/repo1/specs/e1/packageb.spec`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/tests/test_data/repos/repo1/specs/packagea.spec` & `fedrq-1.1.0/tests/test_data/repos/repo1/specs/packagea.spec`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/tests/test_data/repos/repo1/specs/packageb.spec` & `fedrq-1.1.0/tests/test_data/repos/repo1/specs/packageb.spec`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/tests/unit/test_archive.py` & `fedrq-1.1.0/tests/unit/test_archive.py`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/tests/unit/test_backend_base.py` & `fedrq-1.1.0/tests/unit/test_backend_base.py`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/tests/unit/test_backends.py` & `fedrq-1.1.0/tests/unit/test_backends.py`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/tests/unit/test_base_maker.py` & `fedrq-1.1.0/tests/unit/test_base_maker.py`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/tests/unit/test_changelog.py` & `fedrq-1.1.0/tests/unit/test_changelog.py`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/tests/unit/test_checkconfig.py` & `fedrq-1.1.0/tests/unit/test_checkconfig.py`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/tests/unit/test_command.py` & `fedrq-1.1.0/tests/unit/test_command.py`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/tests/unit/test_dnf.py` & `fedrq-1.1.0/tests/unit/test_dnf.py`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/tests/unit/test_download.py` & `fedrq-1.1.0/tests/unit/test_download.py`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/tests/unit/test_formatters.py` & `fedrq-1.1.0/tests/unit/test_formatters.py`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/tests/unit/test_formatters_command.py` & `fedrq-1.1.0/tests/unit/test_formatters_command.py`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/tests/unit/test_libdnf5.py` & `fedrq-1.1.0/tests/unit/test_libdnf5.py`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/tests/unit/test_pkgs.py` & `fedrq-1.1.0/tests/unit/test_pkgs.py`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/tests/unit/test_release.py` & `fedrq-1.1.0/tests/unit/test_release.py`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/tests/unit/test_release_repo.py` & `fedrq-1.1.0/tests/unit/test_release_repo.py`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/tests/unit/test_repolist.py` & `fedrq-1.1.0/tests/unit/test_repolist.py`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/tests/unit/test_repoquery.py` & `fedrq-1.1.0/tests/unit/test_repoquery.py`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/tests/unit/test_subbpkgs.py` & `fedrq-1.1.0/tests/unit/test_subbpkgs.py`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/tests/unit/test_whatrequires.py` & `fedrq-1.1.0/tests/unit/test_whatrequires.py`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/tests/unit/test_whatrequires_src.py` & `fedrq-1.1.0/tests/unit/test_whatrequires_src.py`

 * *Files identical despite different names*

### Comparing `fedrq-1.0.0/PKG-INFO` & `fedrq-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedrq
-Version: 1.0.0
+Version: 1.1.0
 Summary: fedrq is a tool to query the Fedora and EPEL repositories
 Author-email: Maxwell G <gotmax@e.email>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

