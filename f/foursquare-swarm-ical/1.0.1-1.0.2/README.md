# Comparing `tmp/foursquare-swarm-ical-1.0.1.tar.gz` & `tmp/foursquare_swarm_ical-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foursquare-swarm-ical-1.0.1.tar", last modified: Wed Feb 14 17:19:00 2024, max compression
+gzip compressed data, was "foursquare_swarm_ical-1.0.2.tar", last modified: Wed May  1 08:05:54 2024, max compression
```

## Comparing `foursquare-swarm-ical-1.0.1.tar` & `foursquare_swarm_ical-1.0.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 17:19:00.734997 foursquare-swarm-ical-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-02-14 17:18:32.000000 foursquare-swarm-ical-1.0.1/.cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 17:19:00.726997 foursquare-swarm-ical-1.0.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-02-14 17:18:32.000000 foursquare-swarm-ical-1.0.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 17:19:00.726997 foursquare-swarm-ical-1.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     5427 2024-02-14 17:18:32.000000 foursquare-swarm-ical-1.0.1/.github/workflows/check.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-02-14 17:18:32.000000 foursquare-swarm-ical-1.0.1/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-02-14 17:18:32.000000 foursquare-swarm-ical-1.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-02-14 17:18:32.000000 foursquare-swarm-ical-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-02-14 17:18:32.000000 foursquare-swarm-ical-1.0.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     6993 2024-02-14 17:19:00.734997 foursquare-swarm-ical-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5032 2024-02-14 17:18:32.000000 foursquare-swarm-ical-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-02-14 17:18:32.000000 foursquare-swarm-ical-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-02-14 17:19:00.734997 foursquare-swarm-ical-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 17:19:00.726997 foursquare-swarm-ical-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 17:19:00.730997 foursquare-swarm-ical-1.0.1/src/foursquare_swarm_ical/
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-02-14 17:18:32.000000 foursquare-swarm-ical-1.0.1/src/foursquare_swarm_ical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-02-14 17:18:32.000000 foursquare-swarm-ical-1.0.1/src/foursquare_swarm_ical/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-02-14 17:18:32.000000 foursquare-swarm-ical-1.0.1/src/foursquare_swarm_ical/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-02-14 17:18:32.000000 foursquare-swarm-ical-1.0.1/src/foursquare_swarm_ical/config_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-02-14 17:18:32.000000 foursquare-swarm-ical-1.0.1/src/foursquare_swarm_ical/db.py
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-02-14 17:18:32.000000 foursquare-swarm-ical-1.0.1/src/foursquare_swarm_ical/emoji.py
--rw-r--r--   0 runner    (1001) docker     (127)    63578 2024-02-14 17:18:32.000000 foursquare-swarm-ical-1.0.1/src/foursquare_swarm_ical/emoji.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-02-14 17:18:32.000000 foursquare-swarm-ical-1.0.1/src/foursquare_swarm_ical/ical.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 17:18:32.000000 foursquare-swarm-ical-1.0.1/src/foursquare_swarm_ical/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 17:19:00.730997 foursquare-swarm-ical-1.0.1/src/foursquare_swarm_ical.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6993 2024-02-14 17:19:00.000000 foursquare-swarm-ical-1.0.1/src/foursquare_swarm_ical.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-02-14 17:19:00.000000 foursquare-swarm-ical-1.0.1/src/foursquare_swarm_ical.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-14 17:19:00.000000 foursquare-swarm-ical-1.0.1/src/foursquare_swarm_ical.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-02-14 17:19:00.000000 foursquare-swarm-ical-1.0.1/src/foursquare_swarm_ical.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-02-14 17:19:00.000000 foursquare-swarm-ical-1.0.1/src/foursquare_swarm_ical.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-14 17:19:00.000000 foursquare-swarm-ical-1.0.1/src/foursquare_swarm_ical.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 17:19:00.730997 foursquare-swarm-ical-1.0.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 17:19:00.726997 foursquare-swarm-ical-1.0.1/tests/cassettes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 17:19:00.730997 foursquare-swarm-ical-1.0.1/tests/cassettes/test_sync/
--rw-r--r--   0 runner    (1001) docker     (127)    13846 2024-02-14 17:18:32.000000 foursquare-swarm-ical-1.0.1/tests/cassettes/test_sync/test_sync.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)      452 2024-02-14 17:18:32.000000 foursquare-swarm-ical-1.0.1/tests/include.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      157 2024-02-14 17:18:32.000000 foursquare-swarm-ical-1.0.1/tests/prysk-noescape.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 17:19:00.730997 foursquare-swarm-ical-1.0.1/tests/readme/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-02-14 17:18:32.000000 foursquare-swarm-ical-1.0.1/tests/readme/config-sample.md
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-02-14 17:18:32.000000 foursquare-swarm-ical-1.0.1/tests/readme/help.md
--rw-r--r--   0 runner    (1001) docker     (127)     7817 2024-02-14 17:18:32.000000 foursquare-swarm-ical-1.0.1/tests/test_ical.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-02-14 17:18:32.000000 foursquare-swarm-ical-1.0.1/tests/test_sync.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:05:54.512749 foursquare_swarm_ical-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-01 08:05:27.000000 foursquare_swarm_ical-1.0.2/.cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:05:54.504749 foursquare_swarm_ical-1.0.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-01 08:05:27.000000 foursquare_swarm_ical-1.0.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:05:54.504749 foursquare_swarm_ical-1.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-05-01 08:05:27.000000 foursquare_swarm_ical-1.0.2/.github/workflows/check.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-01 08:05:27.000000 foursquare_swarm_ical-1.0.2/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-01 08:05:27.000000 foursquare_swarm_ical-1.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-01 08:05:27.000000 foursquare_swarm_ical-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-05-01 08:05:27.000000 foursquare_swarm_ical-1.0.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     6993 2024-05-01 08:05:54.512749 foursquare_swarm_ical-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5032 2024-05-01 08:05:27.000000 foursquare_swarm_ical-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-05-01 08:05:27.000000 foursquare_swarm_ical-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-01 08:05:54.512749 foursquare_swarm_ical-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:05:54.504749 foursquare_swarm_ical-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:05:54.508749 foursquare_swarm_ical-1.0.2/src/foursquare_swarm_ical/
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-01 08:05:27.000000 foursquare_swarm_ical-1.0.2/src/foursquare_swarm_ical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-01 08:05:27.000000 foursquare_swarm_ical-1.0.2/src/foursquare_swarm_ical/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-05-01 08:05:27.000000 foursquare_swarm_ical-1.0.2/src/foursquare_swarm_ical/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-05-01 08:05:27.000000 foursquare_swarm_ical-1.0.2/src/foursquare_swarm_ical/config_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-05-01 08:05:27.000000 foursquare_swarm_ical-1.0.2/src/foursquare_swarm_ical/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-05-01 08:05:27.000000 foursquare_swarm_ical-1.0.2/src/foursquare_swarm_ical/emoji.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63578 2024-05-01 08:05:27.000000 foursquare_swarm_ical-1.0.2/src/foursquare_swarm_ical/emoji.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-01 08:05:27.000000 foursquare_swarm_ical-1.0.2/src/foursquare_swarm_ical/ical.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 08:05:27.000000 foursquare_swarm_ical-1.0.2/src/foursquare_swarm_ical/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:05:54.508749 foursquare_swarm_ical-1.0.2/src/foursquare_swarm_ical.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6993 2024-05-01 08:05:54.000000 foursquare_swarm_ical-1.0.2/src/foursquare_swarm_ical.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-01 08:05:54.000000 foursquare_swarm_ical-1.0.2/src/foursquare_swarm_ical.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 08:05:54.000000 foursquare_swarm_ical-1.0.2/src/foursquare_swarm_ical.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-01 08:05:54.000000 foursquare_swarm_ical-1.0.2/src/foursquare_swarm_ical.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-01 08:05:54.000000 foursquare_swarm_ical-1.0.2/src/foursquare_swarm_ical.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-01 08:05:54.000000 foursquare_swarm_ical-1.0.2/src/foursquare_swarm_ical.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:05:54.508749 foursquare_swarm_ical-1.0.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:05:54.504749 foursquare_swarm_ical-1.0.2/tests/cassettes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:05:54.508749 foursquare_swarm_ical-1.0.2/tests/cassettes/test_sync/
+-rw-r--r--   0 runner    (1001) docker     (127)    13846 2024-05-01 08:05:27.000000 foursquare_swarm_ical-1.0.2/tests/cassettes/test_sync/test_sync.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      452 2024-05-01 08:05:27.000000 foursquare_swarm_ical-1.0.2/tests/include.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      157 2024-05-01 08:05:27.000000 foursquare_swarm_ical-1.0.2/tests/prysk-noescape.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:05:54.508749 foursquare_swarm_ical-1.0.2/tests/readme/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-01 08:05:27.000000 foursquare_swarm_ical-1.0.2/tests/readme/config-sample.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-01 08:05:27.000000 foursquare_swarm_ical-1.0.2/tests/readme/help.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7817 2024-05-01 08:05:27.000000 foursquare_swarm_ical-1.0.2/tests/test_ical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-01 08:05:27.000000 foursquare_swarm_ical-1.0.2/tests/test_sync.py
```

### Comparing `foursquare-swarm-ical-1.0.1/.github/workflows/check.yaml` & `foursquare_swarm_ical-1.0.2/.github/workflows/check.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -118,15 +118,15 @@
             | xargs apt install -y
       - name: Workaround for https://bugs.debian.org/cgi-bin/bugreport.cgi?bug=1057968
         env:
           DEBIAN_FRONTEND: noninteractive
         shell: bash
         run: |
           set -ex
-          grep " noble " /etc/apt/sources.list || exit 0
+          grep "Suites: noble" /etc/apt/sources.list.d/ubuntu.sources || exit 0
           apt install -y debian-archive-keyring
           ln -s /usr/share/keyrings/debian-archive-keyring.gpg /etc/apt/trusted.gpg.d/
           python3_pycodestyle=$(dpkg-query --showformat='${Version}\n' --show python3-pycodestyle)
           python3_flake8=$(dpkg-query --showformat='${Version}\n' --show python3-flake8)
           if [[ $python3_pycodestyle == 2.11.* && $python3_flake8 == 5.* ]]; then
             echo 'deb https://deb.debian.org/debian unstable main' >/etc/apt/sources.list.d/debian-unstable.list
             echo 'APT::Default-Release "noble";' >/etc/apt/apt.conf.d/debian-release
@@ -161,13 +161,13 @@
         run: make readme
       - name: check-wheel
         run: make check-wheel
 
   workflow-keepalive:
     if: github.event_name == 'schedule'
     runs-on: ubuntu-latest
+    permissions:
+      actions: write
     steps:
-      - name: Re-enable workflow
-        env:
+      - uses: liskin/gh-workflow-keepalive@v1
+        with:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
-        run: |
-          gh api -X PUT repos/${{ github.repository }}/actions/workflows/check.yaml/enable
```

### Comparing `foursquare-swarm-ical-1.0.1/.github/workflows/pypi.yaml` & `foursquare_swarm_ical-1.0.2/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `foursquare-swarm-ical-1.0.1/LICENSE` & `foursquare_swarm_ical-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `foursquare-swarm-ical-1.0.1/Makefile` & `foursquare_swarm_ical-1.0.2/Makefile`

 * *Files identical despite different names*

### Comparing `foursquare-swarm-ical-1.0.1/PKG-INFO` & `foursquare_swarm_ical-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foursquare-swarm-ical
-Version: 1.0.1
+Version: 1.0.2
 Summary: Sync Foursquare Swarm check-ins to local sqlite DB and generate iCalendar
 Author-email: Tomáš Janoušek <tomi@nomi.cz>
 License: MIT
 Project-URL: Homepage, https://github.com/liskin/foursquare-swarm-ical
 Project-URL: Release Notes, https://github.com/liskin/foursquare-swarm-ical/releases
 Project-URL: Issues, https://github.com/liskin/foursquare-swarm-ical/issues
 Project-URL: CI, https://github.com/liskin/foursquare-swarm-ical/actions
```

### Comparing `foursquare-swarm-ical-1.0.1/README.md` & `foursquare_swarm_ical-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `foursquare-swarm-ical-1.0.1/pyproject.toml` & `foursquare_swarm_ical-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `foursquare-swarm-ical-1.0.1/src/foursquare_swarm_ical/cli.py` & `foursquare_swarm_ical-1.0.2/src/foursquare_swarm_ical/cli.py`

 * *Files identical despite different names*

### Comparing `foursquare-swarm-ical-1.0.1/src/foursquare_swarm_ical/config_file.py` & `foursquare_swarm_ical-1.0.2/src/foursquare_swarm_ical/config_file.py`

 * *Files identical despite different names*

### Comparing `foursquare-swarm-ical-1.0.1/src/foursquare_swarm_ical/db.py` & `foursquare_swarm_ical-1.0.2/src/foursquare_swarm_ical/db.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
             deleted += len(old_ids)
 
         logging.info(f"checkins upsert stats: {new} new, {seen} seen, {deleted} deleted")
 
 
 def sync(db: sqlite3.Connection, access_token: str, incremental: bool = False) -> None:
     rows = (
-        {'id': checkin['id'], 'createdAt': int(checkin['createdAt']), 'data': json.dumps(checkin)}
+        {'id': checkin['id'], 'createdAt': int(checkin['createdAt']), 'data': json.dumps(checkin, sort_keys=True)}
         for checkin in fetch_checkins(access_token=access_token)
     )
     upsert(db, rows, incremental=incremental)
 
 
 def fetch_checkins(access_token: str) -> Iterator[Any]:
     client = Foursquare(access_token=access_token)
```

### Comparing `foursquare-swarm-ical-1.0.1/src/foursquare_swarm_ical/emoji.py` & `foursquare_swarm_ical-1.0.2/src/foursquare_swarm_ical/emoji.py`

 * *Files identical despite different names*

### Comparing `foursquare-swarm-ical-1.0.1/src/foursquare_swarm_ical/emoji.yaml` & `foursquare_swarm_ical-1.0.2/src/foursquare_swarm_ical/emoji.yaml`

 * *Files identical despite different names*

### Comparing `foursquare-swarm-ical-1.0.1/src/foursquare_swarm_ical/ical.py` & `foursquare_swarm_ical-1.0.2/src/foursquare_swarm_ical/ical.py`

 * *Files identical despite different names*

### Comparing `foursquare-swarm-ical-1.0.1/src/foursquare_swarm_ical.egg-info/PKG-INFO` & `foursquare_swarm_ical-1.0.2/src/foursquare_swarm_ical.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foursquare-swarm-ical
-Version: 1.0.1
+Version: 1.0.2
 Summary: Sync Foursquare Swarm check-ins to local sqlite DB and generate iCalendar
 Author-email: Tomáš Janoušek <tomi@nomi.cz>
 License: MIT
 Project-URL: Homepage, https://github.com/liskin/foursquare-swarm-ical
 Project-URL: Release Notes, https://github.com/liskin/foursquare-swarm-ical/releases
 Project-URL: Issues, https://github.com/liskin/foursquare-swarm-ical/issues
 Project-URL: CI, https://github.com/liskin/foursquare-swarm-ical/actions
```

### Comparing `foursquare-swarm-ical-1.0.1/src/foursquare_swarm_ical.egg-info/SOURCES.txt` & `foursquare_swarm_ical-1.0.2/src/foursquare_swarm_ical.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `foursquare-swarm-ical-1.0.1/tests/cassettes/test_sync/test_sync.yaml` & `foursquare_swarm_ical-1.0.2/tests/cassettes/test_sync/test_sync.yaml`

 * *Files identical despite different names*

### Comparing `foursquare-swarm-ical-1.0.1/tests/readme/config-sample.md` & `foursquare_swarm_ical-1.0.2/tests/readme/config-sample.md`

 * *Files identical despite different names*

### Comparing `foursquare-swarm-ical-1.0.1/tests/readme/help.md` & `foursquare_swarm_ical-1.0.2/tests/readme/help.md`

 * *Files identical despite different names*

### Comparing `foursquare-swarm-ical-1.0.1/tests/test_ical.py` & `foursquare_swarm_ical-1.0.2/tests/test_ical.py`

 * *Files identical despite different names*

### Comparing `foursquare-swarm-ical-1.0.1/tests/test_sync.py` & `foursquare_swarm_ical-1.0.2/tests/test_sync.py`

 * *Files identical despite different names*

