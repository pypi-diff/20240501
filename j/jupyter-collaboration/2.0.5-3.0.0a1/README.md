# Comparing `tmp/jupyter_collaboration-2.0.5.tar.gz` & `tmp/jupyter_collaboration-3.0.0a1.tar.gz`

## Comparing `jupyter_collaboration-2.0.5.tar` & `jupyter_collaboration-3.0.0a1.tar`

### file list

```diff
@@ -1,136 +1,8 @@
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/.eslintignore
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/.eslintrc.js
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/.flake8
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/.gitconfig
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/.licenserc.yaml
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/.npmignore
--rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/.prettierignore
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/.prettierrc
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/.readthedocs.yaml
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/.stylelintrc
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/.yarnrc.yml
--rw-r--r--   0        0        0    56942 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/CHANGELOG.md
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/CONTRIBUTING.md
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/RELEASE.md
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/codecov.yml
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/install.json
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/lerna.json
--rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/package.json
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/setup.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/tsconfig.json
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/tsconfig.test.json
--rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/typedoc.json
--rw-r--r--   0        0        0   489731 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/yarn.lock
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/docs/Makefile
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/docs/make.bat
--rw-r--r--   0        0        0     2975 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/docs/source/conf.py
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/docs/source/configuration.md
--rw-r--r--   0        0        0     2980 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/docs/source/index.md
--rw-r--r--   0        0        0     4126 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/docs/source/_static/jupyter_logo.svg
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/docs/source/_static/logo-icon.png
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/docs/source/developer/architecture.md
--rw-r--r--   0        0        0     5056 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/docs/source/developer/contributing.rst
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/docs/source/developer/javascript_api.rst
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/docs/source/developer/python_api.rst
--rw-r--r--   0        0        0    61242 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/docs/source/images/rtc_shared_cursors.png
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/jupyter-config/jupyter_collaboration.json
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/jupyter_collaboration/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/jupyter_collaboration/_version.py
--rw-r--r--   0        0        0     4445 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/jupyter_collaboration/app.py
--rw-r--r--   0        0        0    15693 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/jupyter_collaboration/handlers.py
--rw-r--r--   0        0        0     9009 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/jupyter_collaboration/loaders.py
--rw-r--r--   0        0        0    10571 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/jupyter_collaboration/rooms.py
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/jupyter_collaboration/stores.py
--rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/jupyter_collaboration/utils.py
--rw-r--r--   0        0        0     4571 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/jupyter_collaboration/websocketserver.py
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/jupyter_collaboration/events/awareness.yaml
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/jupyter_collaboration/events/session.yaml
--rw-r--r--   0        0        0     3985 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/jupyter_collaboration/labextension/package.json
--rw-r--r--   0        0        0     3843 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/jupyter_collaboration/labextension/schemas/@jupyter/collaboration-extension/package.json.orig
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/jupyter_collaboration/labextension/schemas/@jupyter/collaboration-extension/shared-link.json
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/jupyter_collaboration/labextension/schemas/@jupyter/collaboration-extension/user-menu-bar.json
--rw-r--r--   0        0        0     5287 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/jupyter_collaboration/labextension/static/227.cd6709ca5a6949b8626d.js
--rw-r--r--   0        0        0     9334 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/jupyter_collaboration/labextension/static/413.c23fa684c321e1bc178c.js
--rw-r--r--   0        0        0     5287 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/jupyter_collaboration/labextension/static/719.e4e85f2cbf6ea95a330b.js
--rw-r--r--   0        0        0    11302 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/jupyter_collaboration/labextension/static/760.6923bad9d6aab071c5e8.js
--rw-r--r--   0        0        0     8230 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/jupyter_collaboration/labextension/static/839.14d748171b9c87a422f9.js
--rw-r--r--   0        0        0    10893 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/jupyter_collaboration/labextension/static/87.bddd3348a05e00f99dd9.js
--rw-r--r--   0        0        0     7951 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/jupyter_collaboration/labextension/static/899.d8ce2a60114cd6e1ebea.js
--rw-r--r--   0        0        0     9553 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/jupyter_collaboration/labextension/static/remoteEntry.dfc4262e7e9c0ecfa08b.js
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/jupyter_collaboration/labextension/static/style.js
--rw-r--r--   0        0        0     7745 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/jupyter_collaboration/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/scripts/bump_version.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/tests/__init__.py
--rw-r--r--   0        0        0     6554 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/tests/conftest.py
--rw-r--r--   0        0        0     2067 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/tests/test_app.py
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/tests/test_documents.py
--rw-r--r--   0        0        0     4047 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/tests/test_handlers.py
--rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/tests/test_loaders.py
--rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/tests/test_rooms.py
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/tests/utils.py
--rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/ui-tests/README.md
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/ui-tests/package.json
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/ui-tests/playwright.config.js
--rw-r--r--   0        0        0   148764 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/ui-tests/yarn.lock
--rw-r--r--   0        0        0     7593 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/ui-tests/tests/collaborationpanel.spec.ts
--rw-r--r--   0        0        0     9011 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/ui-tests/tests/notebook.spec.ts
--rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/ui-tests/tests/user-menu.spec.ts
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/ui-tests/tests/collaborationpanel.spec.ts-snapshots/collaboration-icon-linux.png
--rw-r--r--   0        0        0     5578 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/ui-tests/tests/collaborationpanel.spec.ts-snapshots/collaborationPanelCollapsed-linux.png
--rw-r--r--   0        0        0    16480 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/ui-tests/tests/collaborationpanel.spec.ts-snapshots/three-client-with-document-linux.png
--rw-r--r--   0        0        0    13211 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/ui-tests/tests/collaborationpanel.spec.ts-snapshots/three-client-without-document-linux.png
--rw-r--r--   0        0        0  5598332 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/ui-tests/tests/data/OutputExamples.ipynb
--rw-r--r--   0        0        0     5431 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/ui-tests/tests/notebook.spec.ts-snapshots/initialization-create-notebook-guest-linux.png
--rw-r--r--   0        0        0     5431 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/ui-tests/tests/notebook.spec.ts-snapshots/initialization-create-notebook-host-linux.png
--rw-r--r--   0        0        0   101300 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/ui-tests/tests/notebook.spec.ts-snapshots/initialization-open-notebook-guest-linux.png
--rw-r--r--   0        0        0   101300 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/ui-tests/tests/notebook.spec.ts-snapshots/initialization-open-notebook-host-linux.png
--rw-r--r--   0        0        0     7537 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/ui-tests/tests/notebook.spec.ts-snapshots/ten-clients-add-a-new-cell-linux.png
--rw-r--r--   0        0        0    11938 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/ui-tests/tests/user-menu.spec.ts-snapshots/shared-link-dialog-linux.png
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/ui-tests/tests/user-menu.spec.ts-snapshots/shared-link-icon-linux.png
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/packages/collaboration/README.md
--rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/packages/collaboration/package.json
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/packages/collaboration/tsconfig.json
--rw-r--r--   0        0        0     3917 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/packages/collaboration/src/collaboratorspanel.tsx
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/packages/collaboration/src/components.tsx
--rw-r--r--   0        0        0    11792 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/packages/collaboration/src/cursors.ts
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/packages/collaboration/src/index.ts
--rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/packages/collaboration/src/menu.ts
--rw-r--r--   0        0        0     5638 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/packages/collaboration/src/sharedlink.ts
--rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/packages/collaboration/src/tokens.ts
--rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/packages/collaboration/src/userinfopanel.tsx
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/packages/collaboration/style/base.css
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/packages/collaboration/style/index.css
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/packages/collaboration/style/index.js
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/packages/collaboration/style/menu.css
--rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/packages/collaboration/style/sidepanel.css
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/packages/collaboration-extension/README.md
--rw-r--r--   0        0        0     3843 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/packages/collaboration-extension/package.json
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/packages/collaboration-extension/tsconfig.json
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/packages/collaboration-extension/schema/shared-link.json
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/packages/collaboration-extension/schema/user-menu-bar.json
--rw-r--r--   0        0        0     5807 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/packages/collaboration-extension/src/collaboration.ts
--rw-r--r--   0        0        0     9459 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/packages/collaboration-extension/src/filebrowser.ts
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/packages/collaboration-extension/src/index.ts
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/packages/collaboration-extension/src/sharedlink.ts
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/packages/collaboration-extension/style/index.css
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/packages/collaboration-extension/style/index.js
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/packages/docprovider/babel.config.js
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/packages/docprovider/jest.config.js
--rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/packages/docprovider/package.json
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/packages/docprovider/tsconfig.json
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/packages/docprovider/tsconfig.test.json
--rw-r--r--   0        0        0     3594 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/packages/docprovider/src/awareness.ts
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/packages/docprovider/src/index.ts
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/packages/docprovider/src/requests.ts
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/packages/docprovider/src/tokens.ts
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/packages/docprovider/src/utils.ts
--rw-r--r--   0        0        0     6975 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/packages/docprovider/src/ydrive.ts
--rw-r--r--   0        0        0     5061 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/packages/docprovider/src/yprovider.ts
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/packages/docprovider/src/__tests__/yprovider.spec.ts
--rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/.gitignore
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/LICENSE
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/README.md
--rw-r--r--   0        0        0     5081 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/pyproject.toml
--rw-r--r--   0        0        0     7015 2020-02-02 00:00:00.000000 jupyter_collaboration-2.0.5/PKG-INFO
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 jupyter_collaboration-3.0.0a1/setup.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 jupyter_collaboration-3.0.0a1/jupyter_collaboration/__init__.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jupyter_collaboration-3.0.0a1/jupyter_collaboration/_version.py
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 jupyter_collaboration-3.0.0a1/.gitignore
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyter_collaboration-3.0.0a1/LICENSE
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 jupyter_collaboration-3.0.0a1/README.md
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 jupyter_collaboration-3.0.0a1/pyproject.toml
+-rw-r--r--   0        0        0     4562 2020-02-02 00:00:00.000000 jupyter_collaboration-3.0.0a1/PKG-INFO
```

### Comparing `jupyter_collaboration-2.0.5/.gitignore` & `jupyter_collaboration-3.0.0a1/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -5,18 +5,16 @@
 .eslintcache
 .stylelintcache
 *.egg-info/
 .ipynb_checkpoints
 *.tsbuildinfo
 package-lock.json
 docs/source/ts
-jupyter_collaboration/labextension
-
-# Version file is handled by hatchling
-jupyter_collaboration/_version.py
+.jupyter
+labextension
 
 # Integration tests
 ui-tests/test-results/
 ui-tests/playwright-report/
 
 # Created by https://www.gitignore.io/api/python
 # Edit at https://www.gitignore.io/?templates=python
```

### Comparing `jupyter_collaboration-2.0.5/LICENSE` & `jupyter_collaboration-3.0.0a1/LICENSE`

 * *Files identical despite different names*

