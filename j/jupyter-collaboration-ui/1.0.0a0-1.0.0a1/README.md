# Comparing `tmp/jupyter_collaboration_ui-1.0.0a0.tar.gz` & `tmp/jupyter_collaboration_ui-1.0.0a1.tar.gz`

## Comparing `jupyter_collaboration_ui-1.0.0a0.tar` & `jupyter_collaboration_ui-1.0.0a1.tar`

### file list

```diff
@@ -1,1725 +1,71 @@
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/install.json
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/setup.py
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/jupyter_collaboration_ui/__init__.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/jupyter_collaboration_ui/_version.py
--rw-r--r--   0        0        0     3750 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/jupyter_collaboration_ui/labextension/package.json
--rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/jupyter_collaboration_ui/labextension/schemas/@jupyter/collaboration-extension/package.json.orig
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/jupyter_collaboration_ui/labextension/schemas/@jupyter/collaboration-extension/shared-link.json
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/jupyter_collaboration_ui/labextension/schemas/@jupyter/collaboration-extension/user-menu-bar.json
--rw-r--r--   0        0        0     5287 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/jupyter_collaboration_ui/labextension/static/341.f4c7f164b4cd115c5478.js
--rw-r--r--   0        0        0     3255 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/jupyter_collaboration_ui/labextension/static/422.c33fd4bf2f8b13b1f430.js
--rw-r--r--   0        0        0    11313 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/jupyter_collaboration_ui/labextension/static/44.432895baa828dc568436.js
--rw-r--r--   0        0        0     5287 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/jupyter_collaboration_ui/labextension/static/722.260709dc491d985c4f31.js
--rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/jupyter_collaboration_ui/labextension/static/784.1e2f345c812db2777387.js
--rw-r--r--   0        0        0     3464 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/jupyter_collaboration_ui/labextension/static/842.b8a53bb7e5d9e0593385.js
--rw-r--r--   0        0        0     8224 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/jupyter_collaboration_ui/labextension/static/944.0167e5870ff1c1e28b32.js
--rw-r--r--   0        0        0     9385 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/jupyter_collaboration_ui/labextension/static/952.e3c8e98af75bf2e2b0f2.js
--rw-r--r--   0        0        0     9314 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/jupyter_collaboration_ui/labextension/static/remoteEntry.4f29d48a8c309dadd4a6.js
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/jupyter_collaboration_ui/labextension/static/style.js
--rw-r--r--   0        0        0     7762 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/jupyter_collaboration_ui/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/README.md
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/package.json
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/tsconfig.json
--rw-r--r--   0        0        0    59498 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/tsconfig.tsbuildinfo
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/lib/collaboratorspanel.d.ts
--rw-r--r--   0        0        0     3630 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/lib/collaboratorspanel.js
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/lib/components.d.ts
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/lib/components.js
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/lib/cursors.d.ts
--rw-r--r--   0        0        0    11806 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/lib/cursors.js
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/lib/index.d.ts
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/lib/index.js
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/lib/menu.d.ts
--rw-r--r--   0        0        0     2531 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/lib/menu.js
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/lib/sharedlink.d.ts
--rw-r--r--   0        0        0     5465 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/lib/sharedlink.js
--rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/lib/tokens.d.ts
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/lib/tokens.js
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/lib/userinfopanel.d.ts
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/lib/userinfopanel.js
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/observables/README.md
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/observables/package.json
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/observables/lib/index.d.ts
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/observables/lib/index.js
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/observables/lib/index.js.map
--rw-r--r--   0        0        0    11923 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/observables/lib/modeldb.d.ts
--rw-r--r--   0        0        0     7771 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/observables/lib/modeldb.js
--rw-r--r--   0        0        0     4552 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/observables/lib/modeldb.js.map
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/observables/lib/observablejson.d.ts
--rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/observables/lib/observablejson.js
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/observables/lib/observablejson.js.map
--rw-r--r--   0        0        0    13574 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/observables/lib/observablelist.d.ts
--rw-r--r--   0        0        0    10600 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/observables/lib/observablelist.js
--rw-r--r--   0        0        0     5415 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/observables/lib/observablelist.js.map
--rw-r--r--   0        0        0     5533 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/observables/lib/observablemap.d.ts
--rw-r--r--   0        0        0     4474 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/observables/lib/observablemap.js
--rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/observables/lib/observablemap.js.map
--rw-r--r--   0        0        0     3598 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/observables/lib/observablestring.d.ts
--rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/observables/lib/observablestring.js
--rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/observables/lib/observablestring.js.map
--rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/observables/lib/undoablelist.d.ts
--rw-r--r--   0        0        0     6313 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/observables/lib/undoablelist.js
--rw-r--r--   0        0        0     5042 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/observables/lib/undoablelist.js.map
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/observables/src/index.ts
--rw-r--r--   0        0        0    13906 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/observables/src/modeldb.ts
--rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/observables/src/observablejson.ts
--rw-r--r--   0        0        0    16451 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/observables/src/observablelist.ts
--rw-r--r--   0        0        0     7293 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/observables/src/observablemap.ts
--rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/observables/src/observablestring.ts
--rw-r--r--   0        0        0     6938 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/observables/src/undoablelist.ts
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/rendermime-interfaces/README.md
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/rendermime-interfaces/package.json
--rw-r--r--   0        0        0    20160 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/rendermime-interfaces/lib/index.d.ts
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/rendermime-interfaces/lib/index.js
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/rendermime-interfaces/lib/index.js.map
--rw-r--r--   0        0        0    18715 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/rendermime-interfaces/src/index.ts
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/statedb/package.json
--rw-r--r--   0        0        0     2803 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/statedb/lib/dataconnector.d.ts
--rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/statedb/lib/dataconnector.js
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/statedb/lib/dataconnector.js.map
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/statedb/lib/index.d.ts
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/statedb/lib/index.js
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/statedb/lib/index.js.map
--rw-r--r--   0        0        0     8115 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/statedb/lib/interfaces.d.ts
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/statedb/lib/interfaces.js
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/statedb/lib/interfaces.js.map
--rw-r--r--   0        0        0     4814 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/statedb/lib/restorablepool.d.ts
--rw-r--r--   0        0        0     9787 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/statedb/lib/restorablepool.js
--rw-r--r--   0        0        0     6469 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/statedb/lib/restorablepool.js.map
--rw-r--r--   0        0        0     6621 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/statedb/lib/statedb.d.ts
--rw-r--r--   0        0        0     7682 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/statedb/lib/statedb.js
--rw-r--r--   0        0        0     4490 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/statedb/lib/statedb.js.map
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/statedb/lib/tokens.d.ts
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/statedb/lib/tokens.js
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/statedb/lib/tokens.js.map
--rw-r--r--   0        0        0     3053 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/statedb/src/dataconnector.ts
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/statedb/src/index.ts
--rw-r--r--   0        0        0     7839 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/statedb/src/interfaces.ts
--rw-r--r--   0        0        0     9580 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/statedb/src/restorablepool.ts
--rw-r--r--   0        0        0     9489 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/statedb/src/statedb.ts
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/statedb/src/tokens.ts
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/translation/README.md
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/translation/package.json
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/translation/lib/base.d.ts
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/translation/lib/base.js
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/translation/lib/base.js.map
--rw-r--r--   0        0        0    10433 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/translation/lib/gettext.d.ts
--rw-r--r--   0        0        0    16610 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/translation/lib/gettext.js
--rw-r--r--   0        0        0     8576 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/translation/lib/gettext.js.map
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/translation/lib/index.d.ts
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/translation/lib/index.js
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/translation/lib/index.js.map
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/translation/lib/manager.d.ts
--rw-r--r--   0        0        0     3582 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/translation/lib/manager.js
--rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/translation/lib/manager.js.map
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/translation/lib/server.d.ts
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/translation/lib/server.js
--rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/translation/lib/server.js.map
--rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/translation/lib/tokens.d.ts
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/translation/lib/tokens.js
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/translation/lib/tokens.js.map
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/translation/lib/utils.d.ts
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/translation/lib/utils.js
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/translation/lib/utils.js.map
--rw-r--r--   0        0        0     2247 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/translation/src/base.ts
--rw-r--r--   0        0        0    18944 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/translation/src/gettext.ts
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/translation/src/index.ts
--rw-r--r--   0        0        0     3303 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/translation/src/manager.ts
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/translation/src/server.ts
--rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/translation/src/tokens.ts
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/translation/src/utils.ts
--rw-r--r--   0        0        0    11754 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/README.md
--rw-r--r--   0        0        0     2477 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/package.json
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/FormRendererRegistry.d.ts
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/FormRendererRegistry.js
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/FormRendererRegistry.js.map
--rw-r--r--   0        0        0     3835 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/hoverbox.d.ts
--rw-r--r--   0        0        0    10279 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/hoverbox.js
--rw-r--r--   0        0        0     7792 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/hoverbox.js.map
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/index.d.ts
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/index.js
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/index.js.map
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/tokens.d.ts
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/tokens.js
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/tokens.js.map
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/utils.d.ts
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/utils.js
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/utils.js.map
--rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/accordiontoolbar.d.ts
--rw-r--r--   0        0        0     7922 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/accordiontoolbar.js
--rw-r--r--   0        0        0     3750 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/accordiontoolbar.js.map
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/button.d.ts
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/button.js
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/button.js.map
--rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/collapser.d.ts
--rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/collapser.js
--rw-r--r--   0        0        0     3882 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/collapser.js.map
--rw-r--r--   0        0        0     3450 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/form.d.ts
--rw-r--r--   0        0        0    15525 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/form.js
--rw-r--r--   0        0        0    11514 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/form.js.map
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/htmlselect.d.ts
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/htmlselect.js
--rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/htmlselect.js.map
--rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/iframe.d.ts
--rw-r--r--   0        0        0     2749 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/iframe.js
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/iframe.js.map
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/index.d.ts
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/index.js
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/index.js.map
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/inputgroup.d.ts
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/inputgroup.js
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/inputgroup.js.map
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/interface.d.ts
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/interface.js
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/interface.js.map
--rw-r--r--   0        0        0     4385 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/menu.d.ts
--rw-r--r--   0        0        0     8343 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/menu.js
--rw-r--r--   0        0        0     5842 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/menu.js.map
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/panelwithtoolbar.d.ts
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/panelwithtoolbar.js
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/panelwithtoolbar.js.map
--rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/search.d.ts
--rw-r--r--   0        0        0     3780 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/search.js
--rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/search.js.map
--rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/sidepanel.d.ts
--rw-r--r--   0        0        0     3189 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/sidepanel.js
--rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/sidepanel.js.map
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/spinner.d.ts
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/spinner.js
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/spinner.js.map
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/styling.d.ts
--rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/styling.js
--rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/styling.js.map
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/switch.d.ts
--rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/switch.js
--rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/switch.js.map
--rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/table.d.ts
--rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/table.js
--rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/table.js.map
--rw-r--r--   0        0        0    14473 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/toolbar.d.ts
--rw-r--r--   0        0        0    37396 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/toolbar.js
--rw-r--r--   0        0        0    23630 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/toolbar.js.map
--rw-r--r--   0        0        0     5635 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/vdom.d.ts
--rw-r--r--   0        0        0     6383 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/vdom.js
--rw-r--r--   0        0        0     3921 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/vdom.js.map
--rw-r--r--   0        0        0    28187 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/windowedlist.d.ts
--rw-r--r--   0        0        0    53471 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/windowedlist.js
--rw-r--r--   0        0        0    32391 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/windowedlist.js.map
--rw-r--r--   0        0        0     4514 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/icon/iconimports.d.ts
--rw-r--r--   0        0        0    17726 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/icon/iconimports.js
--rw-r--r--   0        0        0    14441 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/icon/iconimports.js.map
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/icon/index.d.ts
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/icon/index.js
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/icon/index.js.map
--rw-r--r--   0        0        0    11503 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/icon/labicon.d.ts
--rw-r--r--   0        0        0    25278 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/icon/labicon.js
--rw-r--r--   0        0        0    14573 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/icon/labicon.js.map
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/icon/widgets/commandpalettesvg.d.ts
--rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/icon/widgets/commandpalettesvg.js
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/icon/widgets/commandpalettesvg.js.map
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/icon/widgets/index.d.ts
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/icon/widgets/index.js
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/icon/widgets/index.js.map
--rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/icon/widgets/menusvg.d.ts
--rw-r--r--   0        0        0     6138 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/icon/widgets/menusvg.js
--rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/icon/widgets/menusvg.js.map
--rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/icon/widgets/tabbarsvg.d.ts
--rw-r--r--   0        0        0     3788 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/icon/widgets/tabbarsvg.js
--rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/icon/widgets/tabbarsvg.js.map
--rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/style/icon.d.ts
--rw-r--r--   0        0        0    11068 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/style/icon.js
--rw-r--r--   0        0        0     7175 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/style/icon.js.map
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/style/index.d.ts
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/style/index.js
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/style/index.js.map
--rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/src/FormRendererRegistry.tsx
--rw-r--r--   0        0        0    11545 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/src/hoverbox.ts
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/src/index.ts
--rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/src/svg.d.ts
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/src/tokens.ts
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/src/utils.ts
--rw-r--r--   0        0        0     7363 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/src/components/accordiontoolbar.ts
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/src/components/button.tsx
--rw-r--r--   0        0        0     4821 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/src/components/collapser.ts
--rw-r--r--   0        0        0    18987 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/src/components/form.tsx
--rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/src/components/htmlselect.tsx
--rw-r--r--   0        0        0     4216 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/src/components/iframe.ts
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/src/components/index.ts
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/src/components/inputgroup.tsx
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/src/components/interface.ts
--rw-r--r--   0        0        0    10224 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/src/components/menu.ts
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/src/components/panelwithtoolbar.ts
--rw-r--r--   0        0        0     4914 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/src/components/search.tsx
--rw-r--r--   0        0        0     4161 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/src/components/sidepanel.ts
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/src/components/spinner.ts
--rw-r--r--   0        0        0     2995 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/src/components/styling.ts
--rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/src/components/switch.ts
--rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/src/components/table.tsx
--rw-r--r--   0        0        0    37219 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/src/components/toolbar.tsx
--rw-r--r--   0        0        0     8376 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/src/components/vdom.ts
--rw-r--r--   0        0        0    59996 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/src/components/windowedlist.ts
--rw-r--r--   0        0        0    17691 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/src/icon/iconimports.ts
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/src/icon/index.ts
--rw-r--r--   0        0        0    28069 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/src/icon/labicon.tsx
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/src/icon/widgets/commandpalettesvg.ts
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/src/icon/widgets/index.ts
--rw-r--r--   0        0        0     5952 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/src/icon/widgets/menusvg.ts
--rw-r--r--   0        0        0     3543 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/src/icon/widgets/tabbarsvg.ts
--rw-r--r--   0        0        0    13354 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/src/style/icon.ts
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/src/style/index.ts
--rw-r--r--   0        0        0     4209 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/base.css
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/collapse.css
--rw-r--r--   0        0        0    13082 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/deprecated.css
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/deprecatedExtra.css
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/hoverbox.css
--rw-r--r--   0        0        0     6108 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons.css
--rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/iconsalt.css
--rw-r--r--   0        0        0     4762 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/iconshover.css
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/iframe.css
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/index.css
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/index.js
--rw-r--r--   0        0        0     5704 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/rjsfTemplates.css
--rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/sidepanel.css
--rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/spinner.css
--rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/styling.css
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/switch.css
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/tabbar.css
--rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/table.css
--rw-r--r--   0        0        0     3401 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/toolbar.css
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/windowedlist.css
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/debug/bad.svg
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/debug/blank.svg
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/deprecated/check-disabled.svg
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/error.svg
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/history.svg
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/info.svg
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/lock.svg
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/arrow/caret-down-empty-thin.svg
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/arrow/caret-down-empty.svg
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/arrow/caret-down.svg
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/arrow/caret-left.svg
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/arrow/caret-right.svg
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/arrow/caret-up-empty-thin.svg
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/arrow/caret-up.svg
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/filetype/console.svg
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/filetype/file.svg
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/filetype/folder-favorite.svg
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/filetype/folder.svg
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/filetype/home.svg
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/filetype/html5.svg
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/filetype/image.svg
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/filetype/inspector.svg
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/filetype/json.svg
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/filetype/julia.svg
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/filetype/keyboard.svg
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/filetype/launcher.svg
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/filetype/markdown.svg
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/filetype/mermaid.svg
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/filetype/notebook.svg
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/filetype/pdf.svg
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/filetype/python.svg
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/filetype/r-kernel.svg
--rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/filetype/react.svg
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/filetype/settings.svg
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/filetype/spreadsheet.svg
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/filetype/text-editor.svg
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/filetype/vega.svg
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/filetype/yaml.svg
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/jupyter/jupyter-favicon.svg
--rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/jupyter/jupyter.svg
--rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/jupyter/jupyterlab-wordmark.svg
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/licenses/copyright.svg
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/lsp/code-check.svg
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/output/collapse.svg
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/output/expand.svg
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/search/case-sensitive.svg
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/search/filter-dot.svg
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/search/filter.svg
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/search/regex.svg
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/search/word.svg
--rw-r--r--   0        0        0     2430 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/sidebar/build.svg
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/sidebar/extension.svg
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/sidebar/palette.svg
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/sidebar/running.svg
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/sidebar/share.svg
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/sidebar/tab.svg
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/sidebar/toc.svg
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/sidebar/user.svg
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/sidebar/users.svg
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/statusbar/bell.svg
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/statusbar/kernel.svg
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/statusbar/line-form.svg
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/statusbar/list.svg
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/statusbar/not-trusted.svg
--rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/statusbar/terminal.svg
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/statusbar/trusted.svg
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/add-above.svg
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/add-below.svg
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/add.svg
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/bug-dot.svg
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/bug.svg
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/check.svg
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/circle-empty.svg
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/circle.svg
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/clear.svg
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/close.svg
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/code.svg
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/collapse-all.svg
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/copy.svg
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/cut.svg
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/delete.svg
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/download.svg
--rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/duplicate.svg
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/edit.svg
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/ellipses.svg
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/expand-all.svg
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/fast-forward.svg
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/file-upload.svg
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/filter-list.svg
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/launch.svg
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/link.svg
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/move-down.svg
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/move-up.svg
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/new-folder.svg
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/numbering.svg
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/offline-bolt.svg
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/paste.svg
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/redo.svg
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/refresh.svg
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/run.svg
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/save.svg
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/search.svg
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/stop.svg
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/table-rows.svg
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/tag.svg
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/tree-view.svg
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/undo.svg
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/unused/home.svg
--rw-r--r--   0        0        0    16859 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/unused/jupyterlab.svg
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/unused/text-editor-alt.svg
--rw-r--r--   0        0        0     3917 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/src/collaboratorspanel.tsx
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/src/components.tsx
--rw-r--r--   0        0        0    11810 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/src/cursors.ts
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/src/index.ts
--rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/src/menu.ts
--rw-r--r--   0        0        0     5638 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/src/sharedlink.ts
--rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/src/tokens.ts
--rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/src/userinfopanel.tsx
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/style/base.css
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/style/index.css
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/style/index.js
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/style/menu.css
--rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration/style/sidepanel.css
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/README.md
--rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/package.json
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/tsconfig.json
--rw-r--r--   0        0        0    98773 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/tsconfig.tsbuildinfo
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/lib/collaboration.d.ts
--rw-r--r--   0        0        0     5657 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/lib/collaboration.js
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/lib/index.d.ts
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/lib/index.js
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/lib/sharedlink.d.ts
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/lib/sharedlink.js
--rw-r--r--   0        0        0    11754 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/README.md
--rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/package.json
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/FormRendererRegistry.d.ts
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/FormRendererRegistry.js
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/FormRendererRegistry.js.map
--rw-r--r--   0        0        0     3991 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/hoverbox.d.ts
--rw-r--r--   0        0        0    10279 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/hoverbox.js
--rw-r--r--   0        0        0     7792 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/hoverbox.js.map
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/index.d.ts
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/index.js
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/index.js.map
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/tokens.d.ts
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/tokens.js
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/tokens.js.map
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/utils.d.ts
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/utils.js
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/utils.js.map
--rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/accordiontoolbar.d.ts
--rw-r--r--   0        0        0     7922 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/accordiontoolbar.js
--rw-r--r--   0        0        0     3750 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/accordiontoolbar.js.map
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/button.d.ts
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/button.js
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/button.js.map
--rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/collapser.d.ts
--rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/collapser.js
--rw-r--r--   0        0        0     3882 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/collapser.js.map
--rw-r--r--   0        0        0     3450 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/form.d.ts
--rw-r--r--   0        0        0    15525 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/form.js
--rw-r--r--   0        0        0    11514 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/form.js.map
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/htmlselect.d.ts
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/htmlselect.js
--rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/htmlselect.js.map
--rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/iframe.d.ts
--rw-r--r--   0        0        0     2749 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/iframe.js
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/iframe.js.map
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/index.d.ts
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/index.js
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/index.js.map
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/inputgroup.d.ts
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/inputgroup.js
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/inputgroup.js.map
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/interface.d.ts
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/interface.js
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/interface.js.map
--rw-r--r--   0        0        0     4385 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/menu.d.ts
--rw-r--r--   0        0        0     8343 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/menu.js
--rw-r--r--   0        0        0     5842 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/menu.js.map
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/panelwithtoolbar.d.ts
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/panelwithtoolbar.js
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/panelwithtoolbar.js.map
--rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/search.d.ts
--rw-r--r--   0        0        0     3780 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/search.js
--rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/search.js.map
--rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/sidepanel.d.ts
--rw-r--r--   0        0        0     3189 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/sidepanel.js
--rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/sidepanel.js.map
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/spinner.d.ts
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/spinner.js
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/spinner.js.map
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/styling.d.ts
--rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/styling.js
--rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/styling.js.map
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/switch.d.ts
--rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/switch.js
--rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/switch.js.map
--rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/table.d.ts
--rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/table.js
--rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/table.js.map
--rw-r--r--   0        0        0    14396 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/toolbar.d.ts
--rw-r--r--   0        0        0    37369 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/toolbar.js
--rw-r--r--   0        0        0    23689 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/toolbar.js.map
--rw-r--r--   0        0        0     5635 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/vdom.d.ts
--rw-r--r--   0        0        0     6383 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/vdom.js
--rw-r--r--   0        0        0     3921 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/vdom.js.map
--rw-r--r--   0        0        0    28402 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/windowedlist.d.ts
--rw-r--r--   0        0        0    53928 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/windowedlist.js
--rw-r--r--   0        0        0    32680 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/windowedlist.js.map
--rw-r--r--   0        0        0     4514 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/icon/iconimports.d.ts
--rw-r--r--   0        0        0    17726 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/icon/iconimports.js
--rw-r--r--   0        0        0    14441 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/icon/iconimports.js.map
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/icon/index.d.ts
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/icon/index.js
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/icon/index.js.map
--rw-r--r--   0        0        0    11503 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/icon/labicon.d.ts
--rw-r--r--   0        0        0    25278 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/icon/labicon.js
--rw-r--r--   0        0        0    14573 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/icon/labicon.js.map
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/icon/widgets/commandpalettesvg.d.ts
--rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/icon/widgets/commandpalettesvg.js
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/icon/widgets/commandpalettesvg.js.map
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/icon/widgets/index.d.ts
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/icon/widgets/index.js
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/icon/widgets/index.js.map
--rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/icon/widgets/menusvg.d.ts
--rw-r--r--   0        0        0     6138 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/icon/widgets/menusvg.js
--rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/icon/widgets/menusvg.js.map
--rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/icon/widgets/tabbarsvg.d.ts
--rw-r--r--   0        0        0     3788 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/icon/widgets/tabbarsvg.js
--rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/icon/widgets/tabbarsvg.js.map
--rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/style/icon.d.ts
--rw-r--r--   0        0        0    11068 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/style/icon.js
--rw-r--r--   0        0        0     7175 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/style/icon.js.map
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/style/index.d.ts
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/style/index.js
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/style/index.js.map
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/README.md
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/package.json
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/lib/activitymonitor.d.ts
--rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/lib/activitymonitor.js
--rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/lib/activitymonitor.js.map
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/lib/index.d.ts
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/lib/index.js
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/lib/index.js.map
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/lib/interfaces.d.ts
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/lib/interfaces.js
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/lib/interfaces.js.map
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/lib/lru.d.ts
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/lib/lru.js
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/lib/lru.js.map
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/lib/markdowncodeblocks.d.ts
--rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/lib/markdowncodeblocks.js
--rw-r--r--   0        0        0     2158 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/lib/markdowncodeblocks.js.map
--rw-r--r--   0        0        0     4590 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/lib/pageconfig.d.ts
--rw-r--r--   0        0        0    10629 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/lib/pageconfig.js
--rw-r--r--   0        0        0     6260 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/lib/pageconfig.js.map
--rw-r--r--   0        0        0     4071 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/lib/path.d.ts
--rw-r--r--   0        0        0     5518 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/lib/path.js
--rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/lib/path.js.map
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/lib/signal.d.ts
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/lib/signal.js
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/lib/signal.js.map
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/lib/testutils.d.ts
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/lib/testutils.js
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/lib/testutils.js.map
--rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/lib/text.d.ts
--rw-r--r--   0        0        0     3929 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/lib/text.js
--rw-r--r--   0        0        0     2208 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/lib/text.js.map
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/lib/time.d.ts
--rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/lib/time.js
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/lib/time.js.map
--rw-r--r--   0        0        0     3399 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/lib/url.d.ts
--rw-r--r--   0        0        0     4717 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/lib/url.js
--rw-r--r--   0        0        0     3272 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/lib/url.js.map
--rw-r--r--   0        0        0     2616 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/src/activitymonitor.ts
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/src/index.ts
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/src/interfaces.ts
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/src/lru.ts
--rw-r--r--   0        0        0     3057 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/src/markdowncodeblocks.ts
--rw-r--r--   0        0        0     9854 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/src/pageconfig.ts
--rw-r--r--   0        0        0     4862 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/src/path.ts
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/src/signal.ts
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/src/testutils.ts
--rw-r--r--   0        0        0     3332 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/src/text.ts
--rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/src/time.ts
--rw-r--r--   0        0        0     5347 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/src/url.ts
--rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/src/FormRendererRegistry.tsx
--rw-r--r--   0        0        0    11700 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/src/hoverbox.ts
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/src/index.ts
--rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/src/svg.d.ts
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/src/tokens.ts
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/src/utils.ts
--rw-r--r--   0        0        0     7363 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/src/components/accordiontoolbar.ts
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/src/components/button.tsx
--rw-r--r--   0        0        0     4821 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/src/components/collapser.ts
--rw-r--r--   0        0        0    18987 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/src/components/form.tsx
--rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/src/components/htmlselect.tsx
--rw-r--r--   0        0        0     4216 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/src/components/iframe.ts
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/src/components/index.ts
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/src/components/inputgroup.tsx
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/src/components/interface.ts
--rw-r--r--   0        0        0    10224 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/src/components/menu.ts
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/src/components/panelwithtoolbar.ts
--rw-r--r--   0        0        0     4914 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/src/components/search.tsx
--rw-r--r--   0        0        0     4161 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/src/components/sidepanel.ts
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/src/components/spinner.ts
--rw-r--r--   0        0        0     2995 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/src/components/styling.ts
--rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/src/components/switch.ts
--rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/src/components/table.tsx
--rw-r--r--   0        0        0    37192 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/src/components/toolbar.tsx
--rw-r--r--   0        0        0     8376 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/src/components/vdom.ts
--rw-r--r--   0        0        0    60687 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/src/components/windowedlist.ts
--rw-r--r--   0        0        0    17691 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/src/icon/iconimports.ts
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/src/icon/index.ts
--rw-r--r--   0        0        0    28069 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/src/icon/labicon.tsx
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/src/icon/widgets/commandpalettesvg.ts
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/src/icon/widgets/index.ts
--rw-r--r--   0        0        0     5952 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/src/icon/widgets/menusvg.ts
--rw-r--r--   0        0        0     3543 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/src/icon/widgets/tabbarsvg.ts
--rw-r--r--   0        0        0    13354 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/src/style/icon.ts
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/src/style/index.ts
--rw-r--r--   0        0        0     4209 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/base.css
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/collapse.css
--rw-r--r--   0        0        0    13082 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/deprecated.css
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/deprecatedExtra.css
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/hoverbox.css
--rw-r--r--   0        0        0     6117 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons.css
--rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/iconsalt.css
--rw-r--r--   0        0        0     4762 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/iconshover.css
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/iframe.css
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/index.css
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/index.js
--rw-r--r--   0        0        0     5722 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/rjsfTemplates.css
--rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/sidepanel.css
--rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/spinner.css
--rw-r--r--   0        0        0     2617 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/styling.css
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/switch.css
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/tabbar.css
--rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/table.css
--rw-r--r--   0        0        0     3401 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/toolbar.css
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/windowedlist.css
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/debug/bad.svg
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/debug/blank.svg
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/deprecated/check-disabled.svg
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/error.svg
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/history.svg
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/info.svg
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/lock.svg
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/arrow/caret-down-empty-thin.svg
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/arrow/caret-down-empty.svg
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/arrow/caret-down.svg
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/arrow/caret-left.svg
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/arrow/caret-right.svg
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/arrow/caret-up-empty-thin.svg
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/arrow/caret-up.svg
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/filetype/console.svg
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/filetype/file.svg
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/filetype/folder-favorite.svg
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/filetype/folder.svg
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/filetype/home.svg
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/filetype/html5.svg
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/filetype/image.svg
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/filetype/inspector.svg
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/filetype/json.svg
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/filetype/julia.svg
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/filetype/keyboard.svg
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/filetype/launcher.svg
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/filetype/markdown.svg
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/filetype/mermaid.svg
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/filetype/notebook.svg
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/filetype/pdf.svg
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/filetype/python.svg
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/filetype/r-kernel.svg
--rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/filetype/react.svg
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/filetype/settings.svg
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/filetype/spreadsheet.svg
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/filetype/text-editor.svg
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/filetype/vega.svg
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/filetype/yaml.svg
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/jupyter/jupyter-favicon.svg
--rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/jupyter/jupyter.svg
--rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/jupyter/jupyterlab-wordmark.svg
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/licenses/copyright.svg
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/lsp/code-check.svg
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/output/collapse.svg
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/output/expand.svg
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/search/case-sensitive.svg
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/search/filter-dot.svg
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/search/filter.svg
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/search/regex.svg
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/search/word.svg
--rw-r--r--   0        0        0     2430 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/sidebar/build.svg
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/sidebar/extension.svg
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/sidebar/palette.svg
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/sidebar/running.svg
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/sidebar/share.svg
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/sidebar/tab.svg
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/sidebar/toc.svg
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/sidebar/user.svg
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/sidebar/users.svg
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/statusbar/bell.svg
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/statusbar/kernel.svg
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/statusbar/line-form.svg
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/statusbar/list.svg
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/statusbar/not-trusted.svg
--rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/statusbar/terminal.svg
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/statusbar/trusted.svg
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/add-above.svg
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/add-below.svg
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/add.svg
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/bug-dot.svg
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/bug.svg
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/check.svg
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/circle-empty.svg
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/circle.svg
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/clear.svg
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/close.svg
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/code.svg
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/collapse-all.svg
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/copy.svg
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/cut.svg
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/delete.svg
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/download.svg
--rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/duplicate.svg
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/edit.svg
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/ellipses.svg
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/expand-all.svg
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/fast-forward.svg
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/file-upload.svg
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/filter-list.svg
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/launch.svg
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/link.svg
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/move-down.svg
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/move-up.svg
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/new-folder.svg
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/numbering.svg
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/offline-bolt.svg
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/paste.svg
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/redo.svg
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/refresh.svg
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/run.svg
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/save.svg
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/search.svg
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/stop.svg
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/table-rows.svg
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/tag.svg
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/tree-view.svg
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/undo.svg
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/unused/home.svg
--rw-r--r--   0        0        0    16859 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/unused/jupyterlab.svg
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/unused/text-editor-alt.svg
--rw-r--r--   0        0        0    10947 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/LICENSE.md
--rw-r--r--   0        0        0     3764 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/README.md
--rw-r--r--   0        0        0     3293 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/package.json
--rw-r--r--   0        0        0   131120 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/dist/core.umd.js
--rw-r--r--   0        0        0   131364 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/dist/index.esm.js
--rw-r--r--   0        0        0   261719 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/dist/index.esm.js.map
--rw-r--r--   0        0        0   138979 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/dist/index.js
--rw-r--r--   0        0        0   259198 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/dist/index.js.map
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/getDefaultRegistry.d.ts
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/getDefaultRegistry.js
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/getDefaultRegistry.js.map
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/index.d.ts
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/index.js
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/index.js.map
--rw-r--r--   0        0        0    72060 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/tsconfig.tsbuildinfo
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/withTheme.d.ts
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/withTheme.js
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/withTheme.js.map
--rw-r--r--   0        0        0    21834 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/Form.d.ts
--rw-r--r--   0        0        0    28563 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/Form.js
--rw-r--r--   0        0        0    16852 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/Form.js.map
--rw-r--r--   0        0        0     9098 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/fields/ArrayField.d.ts
--rw-r--r--   0        0        0    30510 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/fields/ArrayField.js
--rw-r--r--   0        0        0    20629 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/fields/ArrayField.js.map
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/fields/BooleanField.d.ts
--rw-r--r--   0        0        0     3345 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/fields/BooleanField.js
--rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/fields/BooleanField.js.map
--rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/fields/MultiSchemaField.d.ts
--rw-r--r--   0        0        0     9207 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/fields/MultiSchemaField.js
--rw-r--r--   0        0        0     6539 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/fields/MultiSchemaField.js.map
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/fields/NullField.d.ts
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/fields/NullField.js
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/fields/NullField.js.map
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/fields/NumberField.d.ts
--rw-r--r--   0        0        0     3484 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/fields/NumberField.js
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/fields/NumberField.js.map
--rw-r--r--   0        0        0     3898 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/fields/ObjectField.d.ts
--rw-r--r--   0        0        0    11814 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/fields/ObjectField.js
--rw-r--r--   0        0        0     7324 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/fields/ObjectField.js.map
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/fields/SchemaField.d.ts
--rw-r--r--   0        0        0    10578 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/fields/SchemaField.js
--rw-r--r--   0        0        0     8353 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/fields/SchemaField.js.map
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/fields/StringField.d.ts
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/fields/StringField.js
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/fields/StringField.js.map
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/fields/index.d.ts
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/fields/index.js
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/fields/index.js.map
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/ArrayFieldDescriptionTemplate.d.ts
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/ArrayFieldDescriptionTemplate.js
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/ArrayFieldDescriptionTemplate.js.map
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/ArrayFieldItemTemplate.d.ts
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/ArrayFieldItemTemplate.js
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/ArrayFieldItemTemplate.js.map
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/ArrayFieldTemplate.d.ts
--rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/ArrayFieldTemplate.js
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/ArrayFieldTemplate.js.map
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/ArrayFieldTitleTemplate.d.ts
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/ArrayFieldTitleTemplate.js
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/ArrayFieldTitleTemplate.js.map
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/BaseInputTemplate.d.ts
--rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/BaseInputTemplate.js
--rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/BaseInputTemplate.js.map
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/DescriptionField.d.ts
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/DescriptionField.js
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/DescriptionField.js.map
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/ErrorList.d.ts
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/ErrorList.js
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/ErrorList.js.map
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/FieldErrorTemplate.d.ts
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/FieldErrorTemplate.js
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/FieldErrorTemplate.js.map
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/FieldHelpTemplate.d.ts
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/FieldHelpTemplate.js
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/FieldHelpTemplate.js.map
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/ObjectFieldTemplate.d.ts
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/ObjectFieldTemplate.js
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/ObjectFieldTemplate.js.map
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/TitleField.d.ts
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/TitleField.js
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/TitleField.js.map
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/UnsupportedField.d.ts
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/UnsupportedField.js
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/UnsupportedField.js.map
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/WrapIfAdditionalTemplate.d.ts
--rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/WrapIfAdditionalTemplate.js
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/WrapIfAdditionalTemplate.js.map
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/index.d.ts
--rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/index.js
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/index.js.map
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/ButtonTemplates/AddButton.d.ts
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/ButtonTemplates/AddButton.js
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/ButtonTemplates/AddButton.js.map
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/ButtonTemplates/IconButton.d.ts
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/ButtonTemplates/IconButton.js
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/ButtonTemplates/IconButton.js.map
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/ButtonTemplates/SubmitButton.d.ts
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/ButtonTemplates/SubmitButton.js
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/ButtonTemplates/SubmitButton.js.map
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/ButtonTemplates/index.d.ts
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/ButtonTemplates/index.js
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/ButtonTemplates/index.js.map
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/FieldTemplate/FieldTemplate.d.ts
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/FieldTemplate/FieldTemplate.js
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/FieldTemplate/FieldTemplate.js.map
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/FieldTemplate/Label.d.ts
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/FieldTemplate/Label.js
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/FieldTemplate/Label.js.map
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/FieldTemplate/index.d.ts
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/FieldTemplate/index.js
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/FieldTemplate/index.js.map
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/AltDateTimeWidget.d.ts
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/AltDateTimeWidget.js
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/AltDateTimeWidget.js.map
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/AltDateWidget.d.ts
--rw-r--r--   0        0        0     3927 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/AltDateWidget.js
--rw-r--r--   0        0        0     4140 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/AltDateWidget.js.map
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/CheckboxWidget.d.ts
--rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/CheckboxWidget.js
--rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/CheckboxWidget.js.map
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/CheckboxesWidget.d.ts
--rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/CheckboxesWidget.js
--rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/CheckboxesWidget.js.map
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/ColorWidget.d.ts
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/ColorWidget.js
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/ColorWidget.js.map
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/DateTimeWidget.d.ts
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/DateTimeWidget.js
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/DateTimeWidget.js.map
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/DateWidget.d.ts
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/DateWidget.js
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/DateWidget.js.map
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/EmailWidget.d.ts
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/EmailWidget.js
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/EmailWidget.js.map
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/FileWidget.d.ts
--rw-r--r--   0        0        0     5527 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/FileWidget.js
--rw-r--r--   0        0        0     4878 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/FileWidget.js.map
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/HiddenWidget.d.ts
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/HiddenWidget.js
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/HiddenWidget.js.map
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/PasswordWidget.d.ts
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/PasswordWidget.js
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/PasswordWidget.js.map
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/RadioWidget.d.ts
--rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/RadioWidget.js
--rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/RadioWidget.js.map
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/RangeWidget.d.ts
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/RangeWidget.js
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/RangeWidget.js.map
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/SelectWidget.d.ts
--rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/SelectWidget.js
--rw-r--r--   0        0        0     2565 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/SelectWidget.js.map
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/TextWidget.d.ts
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/TextWidget.js
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/TextWidget.js.map
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/TextareaWidget.d.ts
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/TextareaWidget.js
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/TextareaWidget.js.map
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/TimeWidget.d.ts
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/TimeWidget.js
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/TimeWidget.js.map
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/URLWidget.d.ts
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/URLWidget.js
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/URLWidget.js.map
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/UpDownWidget.d.ts
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/UpDownWidget.js
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/UpDownWidget.js.map
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/index.d.ts
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/index.js
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/index.js.map
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/getDefaultRegistry.ts
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/index.ts
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/tsconfig.json
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/withTheme.tsx
--rw-r--r--   0        0        0    39338 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/Form.tsx
--rw-r--r--   0        0        0    30440 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/fields/ArrayField.tsx
--rw-r--r--   0        0        0     3349 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/fields/BooleanField.tsx
--rw-r--r--   0        0        0     9539 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/fields/MultiSchemaField.tsx
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/fields/NullField.tsx
--rw-r--r--   0        0        0     3560 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/fields/NumberField.tsx
--rw-r--r--   0        0        0    11443 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/fields/ObjectField.tsx
--rw-r--r--   0        0        0    12037 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/fields/SchemaField.tsx
--rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/fields/StringField.tsx
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/fields/index.ts
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/templates/ArrayFieldDescriptionTemplate.tsx
--rw-r--r--   0        0        0     2665 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/templates/ArrayFieldItemTemplate.tsx
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/templates/ArrayFieldTemplate.tsx
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/templates/ArrayFieldTitleTemplate.tsx
--rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/templates/BaseInputTemplate.tsx
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/templates/DescriptionField.tsx
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/templates/ErrorList.tsx
--rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/templates/FieldErrorTemplate.tsx
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/templates/FieldHelpTemplate.tsx
--rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/templates/ObjectFieldTemplate.tsx
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/templates/TitleField.tsx
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/templates/UnsupportedField.tsx
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/templates/WrapIfAdditionalTemplate.tsx
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/templates/index.ts
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/templates/ButtonTemplates/AddButton.tsx
--rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/templates/ButtonTemplates/IconButton.tsx
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/templates/ButtonTemplates/SubmitButton.tsx
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/templates/ButtonTemplates/index.ts
--rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/templates/FieldTemplate/FieldTemplate.tsx
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/templates/FieldTemplate/Label.tsx
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/templates/FieldTemplate/index.ts
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/widgets/AltDateTimeWidget.tsx
--rw-r--r--   0        0        0     5070 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/widgets/AltDateWidget.tsx
--rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/widgets/CheckboxWidget.tsx
--rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/widgets/CheckboxesWidget.tsx
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/widgets/ColorWidget.tsx
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/widgets/DateTimeWidget.tsx
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/widgets/DateWidget.tsx
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/widgets/EmailWidget.tsx
--rw-r--r--   0        0        0     6045 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/widgets/FileWidget.tsx
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/widgets/HiddenWidget.tsx
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/widgets/PasswordWidget.tsx
--rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/widgets/RadioWidget.tsx
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/widgets/RangeWidget.tsx
--rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/widgets/SelectWidget.tsx
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/widgets/TextWidget.tsx
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/widgets/TextareaWidget.tsx
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/widgets/TimeWidget.tsx
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/widgets/URLWidget.tsx
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/widgets/UpDownWidget.tsx
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/widgets/index.ts
--rw-r--r--   0        0        0    10947 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/LICENSE.md
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/README.md
--rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/package.json
--rw-r--r--   0        0        0   103957 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/dist/index.js
--rw-r--r--   0        0        0   265256 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/dist/index.js.map
--rw-r--r--   0        0        0    96830 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/dist/utils.esm.js
--rw-r--r--   0        0        0   259446 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/dist/utils.esm.js.map
--rw-r--r--   0        0        0   103426 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/dist/utils.umd.js
--rw-r--r--   0        0        0     3758 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/ErrorSchemaBuilder.d.ts
--rw-r--r--   0        0        0     5254 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/ErrorSchemaBuilder.js
--rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/ErrorSchemaBuilder.js.map
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/allowAdditionalItems.d.ts
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/allowAdditionalItems.js
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/allowAdditionalItems.js.map
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/asNumber.d.ts
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/asNumber.js
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/asNumber.js.map
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/canExpand.d.ts
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/canExpand.js
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/canExpand.js.map
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/constants.d.ts
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/constants.js
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/constants.js.map
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/createErrorHandler.d.ts
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/createErrorHandler.js
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/createErrorHandler.js.map
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/createSchemaUtils.d.ts
--rw-r--r--   0        0        0    13359 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/createSchemaUtils.js
--rw-r--r--   0        0        0     3216 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/createSchemaUtils.js.map
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/dataURItoBlob.d.ts
--rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/dataURItoBlob.js
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/dataURItoBlob.js.map
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/deepEquals.d.ts
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/deepEquals.js
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/deepEquals.js.map
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/englishStringTranslator.d.ts
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/englishStringTranslator.js
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/englishStringTranslator.js.map
--rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/enumOptionsDeselectValue.d.ts
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/enumOptionsDeselectValue.js
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/enumOptionsDeselectValue.js.map
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/enumOptionsIndexForValue.d.ts
--rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/enumOptionsIndexForValue.js
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/enumOptionsIndexForValue.js.map
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/enumOptionsIsSelected.d.ts
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/enumOptionsIsSelected.js
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/enumOptionsIsSelected.js.map
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/enumOptionsSelectValue.d.ts
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/enumOptionsSelectValue.js
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/enumOptionsSelectValue.js.map
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/enumOptionsValueForIndex.d.ts
--rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/enumOptionsValueForIndex.js
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/enumOptionsValueForIndex.js.map
--rw-r--r--   0        0        0     3931 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/enums.d.ts
--rw-r--r--   0        0        0     4801 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/enums.js
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/enums.js.map
--rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/findSchemaDefinition.d.ts
--rw-r--r--   0        0        0     3977 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/findSchemaDefinition.js
--rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/findSchemaDefinition.js.map
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/getDateElementProps.d.ts
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/getDateElementProps.js
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/getDateElementProps.js.map
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/getDiscriminatorFieldFromSchema.d.ts
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/getDiscriminatorFieldFromSchema.js
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/getDiscriminatorFieldFromSchema.js.map
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/getInputProps.d.ts
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/getInputProps.js
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/getInputProps.js.map
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/getOptionMatchingSimpleDiscriminator.d.ts
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/getOptionMatchingSimpleDiscriminator.js
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/getOptionMatchingSimpleDiscriminator.js.map
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/getSchemaType.d.ts
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/getSchemaType.js
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/getSchemaType.js.map
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/getSubmitButtonOptions.d.ts
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/getSubmitButtonOptions.js
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/getSubmitButtonOptions.js.map
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/getTemplate.d.ts
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/getTemplate.js
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/getTemplate.js.map
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/getUiOptions.d.ts
--rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/getUiOptions.js
--rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/getUiOptions.js.map
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/getWidget.d.ts
--rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/getWidget.js
--rw-r--r--   0        0        0     2739 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/getWidget.js.map
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/guessType.d.ts
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/guessType.js
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/guessType.js.map
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/hasWidget.d.ts
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/hasWidget.js
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/hasWidget.js.map
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/hashForSchema.d.ts
--rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/hashForSchema.js
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/hashForSchema.js.map
--rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/idGenerators.d.ts
--rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/idGenerators.js
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/idGenerators.js.map
--rw-r--r--   0        0        0     3881 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/index.d.ts
--rw-r--r--   0        0        0     3867 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/index.js
--rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/index.js.map
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/isConstant.d.ts
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/isConstant.js
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/isConstant.js.map
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/isCustomWidget.d.ts
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/isCustomWidget.js
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/isCustomWidget.js.map
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/isFixedItems.d.ts
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/isFixedItems.js
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/isFixedItems.js.map
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/isObject.d.ts
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/isObject.js
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/isObject.js.map
--rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/labelValue.d.ts
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/labelValue.js
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/labelValue.js.map
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/localToUTC.d.ts
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/localToUTC.js
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/localToUTC.js.map
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/mergeDefaultsWithFormData.d.ts
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/mergeDefaultsWithFormData.js
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/mergeDefaultsWithFormData.js.map
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/mergeObjects.d.ts
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/mergeObjects.js
--rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/mergeObjects.js.map
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/mergeSchemas.d.ts
--rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/mergeSchemas.js
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/mergeSchemas.js.map
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/optionsList.d.ts
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/optionsList.js
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/optionsList.js.map
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/orderProperties.d.ts
--rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/orderProperties.js
--rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/orderProperties.js.map
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/pad.d.ts
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/pad.js
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/pad.js.map
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/parseDateString.d.ts
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/parseDateString.js
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/parseDateString.js.map
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/rangeSpec.d.ts
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/rangeSpec.js
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/rangeSpec.js.map
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/replaceStringParameters.d.ts
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/replaceStringParameters.js
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/replaceStringParameters.js.map
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schemaRequiresTrueValue.d.ts
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schemaRequiresTrueValue.js
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schemaRequiresTrueValue.js.map
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/shouldRender.d.ts
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/shouldRender.js
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/shouldRender.js.map
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/toConstant.d.ts
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/toConstant.js
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/toConstant.js.map
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/toDateString.d.ts
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/toDateString.js
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/toDateString.js.map
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/toErrorList.d.ts
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/toErrorList.js
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/toErrorList.js.map
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/toErrorSchema.d.ts
--rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/toErrorSchema.js
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/toErrorSchema.js.map
--rw-r--r--   0        0        0    67837 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/tsconfig.tsbuildinfo
--rw-r--r--   0        0        0    57219 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/types.d.ts
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/types.js
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/types.js.map
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/unwrapErrorHandler.d.ts
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/unwrapErrorHandler.js
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/unwrapErrorHandler.js.map
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/utcToLocal.d.ts
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/utcToLocal.js
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/utcToLocal.js.map
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/validationDataMerge.d.ts
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/validationDataMerge.js
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/validationDataMerge.js.map
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/withIdRefPrefix.d.ts
--rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/withIdRefPrefix.js
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/withIdRefPrefix.js.map
--rw-r--r--   0        0        0     4257 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/parser/ParserValidator.d.ts
--rw-r--r--   0        0        0     5010 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/parser/ParserValidator.js
--rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/parser/ParserValidator.js.map
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/parser/index.d.ts
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/parser/index.js
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/parser/index.js.map
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/parser/schemaParser.d.ts
--rw-r--r--   0        0        0     2672 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/parser/schemaParser.js
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/parser/schemaParser.js.map
--rw-r--r--   0        0        0     4194 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/getClosestMatchingOption.d.ts
--rw-r--r--   0        0        0     8998 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/getClosestMatchingOption.js
--rw-r--r--   0        0        0     4361 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/getClosestMatchingOption.js.map
--rw-r--r--   0        0        0     5391 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/getDefaultFormState.d.ts
--rw-r--r--   0        0        0    22107 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/getDefaultFormState.js
--rw-r--r--   0        0        0    10811 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/getDefaultFormState.js.map
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/getDisplayLabel.d.ts
--rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/getDisplayLabel.js
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/getDisplayLabel.js.map
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/getFirstMatchingOption.d.ts
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/getFirstMatchingOption.js
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/getFirstMatchingOption.js.map
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/getMatchingOption.d.ts
--rw-r--r--   0        0        0     4231 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/getMatchingOption.js
--rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/getMatchingOption.js.map
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/index.d.ts
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/index.js
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/index.js.map
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/isFilesArray.d.ts
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/isFilesArray.js
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/isFilesArray.js.map
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/isMultiSelect.d.ts
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/isMultiSelect.js
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/isMultiSelect.js.map
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/isSelect.d.ts
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/isSelect.js
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/isSelect.js.map
--rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/mergeValidationData.d.ts
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/mergeValidationData.js
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/mergeValidationData.js.map
--rw-r--r--   0        0        0    15291 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/retrieveSchema.d.ts
--rw-r--r--   0        0        0    28066 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/retrieveSchema.js
--rw-r--r--   0        0        0    13290 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/retrieveSchema.js.map
--rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/sanitizeDataForNewSchema.d.ts
--rw-r--r--   0        0        0    11577 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/sanitizeDataForNewSchema.js
--rw-r--r--   0        0        0     4889 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/sanitizeDataForNewSchema.js.map
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/toIdSchema.d.ts
--rw-r--r--   0        0        0     3499 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/toIdSchema.js
--rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/toIdSchema.js.map
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/toPathSchema.d.ts
--rw-r--r--   0        0        0     4764 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/toPathSchema.js
--rw-r--r--   0        0        0     3182 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/toPathSchema.js.map
--rw-r--r--   0        0        0     5215 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/ErrorSchemaBuilder.ts
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/allowAdditionalItems.ts
--rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/asNumber.ts
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/canExpand.ts
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/constants.ts
--rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/createErrorHandler.ts
--rw-r--r--   0        0        0    14372 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/createSchemaUtils.ts
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/dataURItoBlob.ts
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/deepEquals.ts
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/englishStringTranslator.ts
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/enumOptionsDeselectValue.ts
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/enumOptionsIndexForValue.ts
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/enumOptionsIsSelected.ts
--rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/enumOptionsSelectValue.ts
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/enumOptionsValueForIndex.ts
--rw-r--r--   0        0        0     3914 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/enums.ts
--rw-r--r--   0        0        0     4067 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/findSchemaDefinition.ts
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/getDateElementProps.ts
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/getDiscriminatorFieldFromSchema.ts
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/getInputProps.ts
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/getOptionMatchingSimpleDiscriminator.ts
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/getSchemaType.ts
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/getSubmitButtonOptions.ts
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/getTemplate.ts
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/getUiOptions.ts
--rw-r--r--   0        0        0     4671 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/getWidget.tsx
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/guessType.ts
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/hasWidget.ts
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/hashForSchema.ts
--rw-r--r--   0        0        0     3310 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/idGenerators.ts
--rw-r--r--   0        0        0     4004 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/index.ts
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/isConstant.ts
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/isCustomWidget.ts
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/isFixedItems.ts
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/isObject.ts
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/labelValue.ts
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/localToUTC.ts
--rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/mergeDefaultsWithFormData.ts
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/mergeObjects.ts
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/mergeSchemas.ts
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/optionsList.ts
--rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/orderProperties.ts
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/pad.ts
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/parseDateString.ts
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/rangeSpec.ts
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/replaceStringParameters.ts
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/schemaRequiresTrueValue.ts
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/shouldRender.ts
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/toConstant.ts
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/toDateString.ts
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/toErrorList.ts
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/toErrorSchema.ts
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/tsconfig.json
--rw-r--r--   0        0        0    56287 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/types.ts
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/unwrapErrorHandler.ts
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/utcToLocal.ts
--rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/validationDataMerge.ts
--rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/withIdRefPrefix.ts
--rw-r--r--   0        0        0     5622 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/parser/ParserValidator.ts
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/parser/index.ts
--rw-r--r--   0        0        0     2902 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/parser/schemaParser.ts
--rw-r--r--   0        0        0     9294 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/schema/getClosestMatchingOption.ts
--rw-r--r--   0        0        0    21319 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/schema/getDefaultFormState.ts
--rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/schema/getDisplayLabel.ts
--rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/schema/getFirstMatchingOption.ts
--rw-r--r--   0        0        0     4060 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/schema/getMatchingOption.ts
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/schema/index.ts
--rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/schema/isFilesArray.ts
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/schema/isMultiSelect.ts
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/schema/isSelect.ts
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/schema/mergeValidationData.ts
--rw-r--r--   0        0        0    30469 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/schema/retrieveSchema.ts
--rw-r--r--   0        0        0    11171 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/schema/sanitizeDataForNewSchema.ts
--rw-r--r--   0        0        0     4110 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/schema/toIdSchema.ts
--rw-r--r--   0        0        0     5403 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/schema/toPathSchema.ts
--rwxr-xr-x   0        0        0     1141 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@types/react/LICENSE
--rwxr-xr-x   0        0        0     1916 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@types/react/README.md
--rwxr-xr-x   0        0        0     4743 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@types/react/experimental.d.ts
--rwxr-xr-x   0        0        0     7431 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@types/react/global.d.ts
--rwxr-xr-x   0        0        0   156037 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@types/react/index.d.ts
--rwxr-xr-x   0        0        0       61 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@types/react/jsx-dev-runtime.d.ts
--rwxr-xr-x   0        0        0       61 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@types/react/jsx-runtime.d.ts
--rwxr-xr-x   0        0        0     2929 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@types/react/next.d.ts
--rwxr-xr-x   0        0        0     6002 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@types/react/package.json
--rwxr-xr-x   0        0        0     4613 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@types/react/ts5.0/experimental.d.ts
--rwxr-xr-x   0        0        0     7409 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@types/react/ts5.0/global.d.ts
--rwxr-xr-x   0        0        0   152997 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@types/react/ts5.0/index.d.ts
--rwxr-xr-x   0        0        0       61 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@types/react/ts5.0/jsx-dev-runtime.d.ts
--rwxr-xr-x   0        0        0       61 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@types/react/ts5.0/jsx-runtime.d.ts
--rwxr-xr-x   0        0        0     2929 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@types/react/ts5.0/next.d.ts
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/markdown-to-jsx/LICENSE
--rw-r--r--   0        0        0    19014 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/markdown-to-jsx/README.md
--rw-r--r--   0        0        0     4073 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/markdown-to-jsx/package.json
--rw-r--r--   0        0        0    16150 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/markdown-to-jsx/dist/index.cjs
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/markdown-to-jsx/dist/index.cjs.d.ts
--rw-r--r--   0        0        0    90164 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/markdown-to-jsx/dist/index.cjs.map
--rw-r--r--   0        0        0    13626 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/markdown-to-jsx/dist/index.d.ts
--rw-r--r--   0        0        0    14946 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/markdown-to-jsx/dist/index.modern.js
--rw-r--r--   0        0        0    89358 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/markdown-to-jsx/dist/index.modern.js.map
--rw-r--r--   0        0        0    15880 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/markdown-to-jsx/dist/index.module.js
--rw-r--r--   0        0        0    89921 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/markdown-to-jsx/dist/index.module.js.map
--rw-r--r--   0        0        0    16345 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/markdown-to-jsx/dist/index.umd.js
--rw-r--r--   0        0        0    90167 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/markdown-to-jsx/dist/index.umd.js.map
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/markdown-to-jsx/dist/site.d.ts
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/react-dom/LICENSE
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/react-dom/README.md
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/react-dom/client.js
--rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/react-dom/index.js
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/react-dom/package.json
--rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/react-dom/profiling.js
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/react-dom/server.browser.js
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/react-dom/server.js
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/react-dom/server.node.js
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/react-dom/test-utils.js
--rw-r--r--   0        0        0   243900 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/react-dom/cjs/react-dom-server-legacy.browser.development.js
--rw-r--r--   0        0        0    35019 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/react-dom/cjs/react-dom-server-legacy.browser.production.min.js
--rw-r--r--   0        0        0   245608 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/react-dom/cjs/react-dom-server-legacy.node.development.js
--rw-r--r--   0        0        0    38796 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/react-dom/cjs/react-dom-server-legacy.node.production.min.js
--rw-r--r--   0        0        0   242789 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/react-dom/cjs/react-dom-server.browser.development.js
--rw-r--r--   0        0        0    35597 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/react-dom/cjs/react-dom-server.browser.production.min.js
--rw-r--r--   0        0        0   244170 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/react-dom/cjs/react-dom-server.node.development.js
--rw-r--r--   0        0        0    39058 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/react-dom/cjs/react-dom-server.node.production.min.js
--rw-r--r--   0        0        0    55073 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/react-dom/cjs/react-dom-test-utils.development.js
--rw-r--r--   0        0        0    12616 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/react-dom/cjs/react-dom-test-utils.production.min.js
--rw-r--r--   0        0        0  1026501 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/react-dom/cjs/react-dom.development.js
--rw-r--r--   0        0        0   131737 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/react-dom/cjs/react-dom.production.min.js
--rw-r--r--   0        0        0   141164 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/react-dom/cjs/react-dom.profiling.min.js
--rw-r--r--   0        0        0   255793 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/react-dom/umd/react-dom-server-legacy.browser.development.js
--rw-r--r--   0        0        0    35128 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/react-dom/umd/react-dom-server-legacy.browser.production.min.js
--rw-r--r--   0        0        0   254652 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/react-dom/umd/react-dom-server.browser.development.js
--rw-r--r--   0        0        0    35699 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/react-dom/umd/react-dom-server.browser.production.min.js
--rw-r--r--   0        0        0    58151 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/react-dom/umd/react-dom-test-utils.development.js
--rw-r--r--   0        0        0    12689 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/react-dom/umd/react-dom-test-utils.production.min.js
--rw-r--r--   0        0        0  1077022 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/react-dom/umd/react-dom.development.js
--rw-r--r--   0        0        0   131882 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/react-dom/umd/react-dom.production.min.js
--rw-r--r--   0        0        0   140615 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/react-dom/umd/react-dom.profiling.min.js
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/schema/shared-link.json
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/schema/user-menu-bar.json
--rw-r--r--   0        0        0     5807 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/src/collaboration.ts
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/src/index.ts
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/src/sharedlink.ts
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/style/index.css
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/style/index.js
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider/babel.config.js
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider/jest.config.js
--rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider/package.json
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider/tsconfig.json
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider/tsconfig.test.json
--rw-r--r--   0        0        0    71721 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider/tsconfig.tsbuildinfo
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider/lib/awareness.d.ts
--rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider/lib/awareness.js
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider/lib/index.d.ts
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider/lib/index.js
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider/lib/requests.d.ts
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider/lib/requests.js
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider/lib/tokens.d.ts
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider/lib/tokens.js
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider/lib/utils.d.ts
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider/lib/utils.js
--rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider/lib/ydrive.d.ts
--rw-r--r--   0        0        0     6599 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider/lib/ydrive.js
--rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider/lib/yprovider.d.ts
--rw-r--r--   0        0        0     3906 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider/lib/yprovider.js
--rw-r--r--   0        0        0     3594 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider/src/awareness.ts
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider/src/index.ts
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider/src/requests.ts
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider/src/tokens.ts
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider/src/utils.ts
--rw-r--r--   0        0        0     6975 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider/src/ydrive.ts
--rw-r--r--   0        0        0     5061 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider/src/yprovider.ts
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider/src/__tests__/yprovider.spec.ts
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/README.md
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/package.json
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/tsconfig.json
--rw-r--r--   0        0        0   130558 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/tsconfig.tsbuildinfo
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/lib/executor.d.ts
--rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/lib/executor.js
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/lib/filebrowser.d.ts
--rw-r--r--   0        0        0     9694 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/lib/filebrowser.js
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/lib/index.d.ts
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/lib/index.js
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@jupyterlab/settingregistry/package.json
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@jupyterlab/settingregistry/lib/index.d.ts
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@jupyterlab/settingregistry/lib/index.js
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@jupyterlab/settingregistry/lib/index.js.map
--rw-r--r--   0        0        0    13651 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@jupyterlab/settingregistry/lib/plugin-schema.json
--rw-r--r--   0        0        0    15495 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@jupyterlab/settingregistry/lib/settingregistry.d.ts
--rw-r--r--   0        0        0    43561 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@jupyterlab/settingregistry/lib/settingregistry.js
--rw-r--r--   0        0        0    28805 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@jupyterlab/settingregistry/lib/settingregistry.js.map
--rw-r--r--   0        0        0    20288 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@jupyterlab/settingregistry/lib/tokens.d.ts
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@jupyterlab/settingregistry/lib/tokens.js
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@jupyterlab/settingregistry/lib/tokens.js.map
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@jupyterlab/settingregistry/src/index.ts
--rw-r--r--   0        0        0    10239 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@jupyterlab/settingregistry/src/plugin-schema.json
--rw-r--r--   0        0        0    45173 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@jupyterlab/settingregistry/src/settingregistry.ts
--rw-r--r--   0        0        0    18913 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@jupyterlab/settingregistry/src/tokens.ts
--rw-r--r--   0        0        0    10947 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/LICENSE.md
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/README.md
--rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/package.json
--rw-r--r--   0        0        0   103957 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/dist/index.js
--rw-r--r--   0        0        0   265256 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/dist/index.js.map
--rw-r--r--   0        0        0    96830 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/dist/utils.esm.js
--rw-r--r--   0        0        0   259446 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/dist/utils.esm.js.map
--rw-r--r--   0        0        0   103426 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/dist/utils.umd.js
--rw-r--r--   0        0        0     3758 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/ErrorSchemaBuilder.d.ts
--rw-r--r--   0        0        0     5254 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/ErrorSchemaBuilder.js
--rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/ErrorSchemaBuilder.js.map
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/allowAdditionalItems.d.ts
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/allowAdditionalItems.js
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/allowAdditionalItems.js.map
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/asNumber.d.ts
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/asNumber.js
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/asNumber.js.map
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/canExpand.d.ts
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/canExpand.js
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/canExpand.js.map
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/constants.d.ts
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/constants.js
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/constants.js.map
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/createErrorHandler.d.ts
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/createErrorHandler.js
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/createErrorHandler.js.map
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/createSchemaUtils.d.ts
--rw-r--r--   0        0        0    13359 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/createSchemaUtils.js
--rw-r--r--   0        0        0     3216 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/createSchemaUtils.js.map
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/dataURItoBlob.d.ts
--rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/dataURItoBlob.js
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/dataURItoBlob.js.map
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/deepEquals.d.ts
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/deepEquals.js
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/deepEquals.js.map
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/englishStringTranslator.d.ts
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/englishStringTranslator.js
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/englishStringTranslator.js.map
--rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/enumOptionsDeselectValue.d.ts
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/enumOptionsDeselectValue.js
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/enumOptionsDeselectValue.js.map
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/enumOptionsIndexForValue.d.ts
--rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/enumOptionsIndexForValue.js
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/enumOptionsIndexForValue.js.map
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/enumOptionsIsSelected.d.ts
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/enumOptionsIsSelected.js
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/enumOptionsIsSelected.js.map
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/enumOptionsSelectValue.d.ts
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/enumOptionsSelectValue.js
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/enumOptionsSelectValue.js.map
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/enumOptionsValueForIndex.d.ts
--rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/enumOptionsValueForIndex.js
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/enumOptionsValueForIndex.js.map
--rw-r--r--   0        0        0     3931 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/enums.d.ts
--rw-r--r--   0        0        0     4801 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/enums.js
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/enums.js.map
--rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/findSchemaDefinition.d.ts
--rw-r--r--   0        0        0     3977 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/findSchemaDefinition.js
--rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/findSchemaDefinition.js.map
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/getDateElementProps.d.ts
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/getDateElementProps.js
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/getDateElementProps.js.map
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/getDiscriminatorFieldFromSchema.d.ts
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/getDiscriminatorFieldFromSchema.js
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/getDiscriminatorFieldFromSchema.js.map
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/getInputProps.d.ts
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/getInputProps.js
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/getInputProps.js.map
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/getOptionMatchingSimpleDiscriminator.d.ts
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/getOptionMatchingSimpleDiscriminator.js
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/getOptionMatchingSimpleDiscriminator.js.map
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/getSchemaType.d.ts
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/getSchemaType.js
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/getSchemaType.js.map
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/getSubmitButtonOptions.d.ts
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/getSubmitButtonOptions.js
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/getSubmitButtonOptions.js.map
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/getTemplate.d.ts
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/getTemplate.js
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/getTemplate.js.map
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/getUiOptions.d.ts
--rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/getUiOptions.js
--rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/getUiOptions.js.map
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/getWidget.d.ts
--rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/getWidget.js
--rw-r--r--   0        0        0     2739 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/getWidget.js.map
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/guessType.d.ts
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/guessType.js
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/guessType.js.map
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/hasWidget.d.ts
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/hasWidget.js
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/hasWidget.js.map
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/hashForSchema.d.ts
--rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/hashForSchema.js
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/hashForSchema.js.map
--rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/idGenerators.d.ts
--rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/idGenerators.js
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/idGenerators.js.map
--rw-r--r--   0        0        0     3881 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/index.d.ts
--rw-r--r--   0        0        0     3867 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/index.js
--rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/index.js.map
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/isConstant.d.ts
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/isConstant.js
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/isConstant.js.map
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/isCustomWidget.d.ts
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/isCustomWidget.js
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/isCustomWidget.js.map
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/isFixedItems.d.ts
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/isFixedItems.js
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/isFixedItems.js.map
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/isObject.d.ts
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/isObject.js
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/isObject.js.map
--rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/labelValue.d.ts
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/labelValue.js
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/labelValue.js.map
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/localToUTC.d.ts
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/localToUTC.js
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/localToUTC.js.map
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/mergeDefaultsWithFormData.d.ts
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/mergeDefaultsWithFormData.js
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/mergeDefaultsWithFormData.js.map
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/mergeObjects.d.ts
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/mergeObjects.js
--rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/mergeObjects.js.map
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/mergeSchemas.d.ts
--rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/mergeSchemas.js
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/mergeSchemas.js.map
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/optionsList.d.ts
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/optionsList.js
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/optionsList.js.map
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/orderProperties.d.ts
--rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/orderProperties.js
--rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/orderProperties.js.map
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/pad.d.ts
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/pad.js
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/pad.js.map
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/parseDateString.d.ts
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/parseDateString.js
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/parseDateString.js.map
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/rangeSpec.d.ts
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/rangeSpec.js
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/rangeSpec.js.map
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/replaceStringParameters.d.ts
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/replaceStringParameters.js
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/replaceStringParameters.js.map
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schemaRequiresTrueValue.d.ts
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schemaRequiresTrueValue.js
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schemaRequiresTrueValue.js.map
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/shouldRender.d.ts
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/shouldRender.js
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/shouldRender.js.map
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/toConstant.d.ts
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/toConstant.js
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/toConstant.js.map
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/toDateString.d.ts
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/toDateString.js
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/toDateString.js.map
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/toErrorList.d.ts
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/toErrorList.js
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/toErrorList.js.map
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/toErrorSchema.d.ts
--rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/toErrorSchema.js
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/toErrorSchema.js.map
--rw-r--r--   0        0        0    67837 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/tsconfig.tsbuildinfo
--rw-r--r--   0        0        0    57219 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/types.d.ts
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/types.js
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/types.js.map
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/unwrapErrorHandler.d.ts
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/unwrapErrorHandler.js
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/unwrapErrorHandler.js.map
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/utcToLocal.d.ts
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/utcToLocal.js
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/utcToLocal.js.map
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/validationDataMerge.d.ts
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/validationDataMerge.js
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/validationDataMerge.js.map
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/withIdRefPrefix.d.ts
--rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/withIdRefPrefix.js
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/withIdRefPrefix.js.map
--rw-r--r--   0        0        0     4257 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/parser/ParserValidator.d.ts
--rw-r--r--   0        0        0     5010 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/parser/ParserValidator.js
--rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/parser/ParserValidator.js.map
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/parser/index.d.ts
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/parser/index.js
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/parser/index.js.map
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/parser/schemaParser.d.ts
--rw-r--r--   0        0        0     2672 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/parser/schemaParser.js
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/parser/schemaParser.js.map
--rw-r--r--   0        0        0     4194 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/getClosestMatchingOption.d.ts
--rw-r--r--   0        0        0     8998 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/getClosestMatchingOption.js
--rw-r--r--   0        0        0     4361 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/getClosestMatchingOption.js.map
--rw-r--r--   0        0        0     5391 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/getDefaultFormState.d.ts
--rw-r--r--   0        0        0    22107 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/getDefaultFormState.js
--rw-r--r--   0        0        0    10811 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/getDefaultFormState.js.map
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/getDisplayLabel.d.ts
--rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/getDisplayLabel.js
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/getDisplayLabel.js.map
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/getFirstMatchingOption.d.ts
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/getFirstMatchingOption.js
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/getFirstMatchingOption.js.map
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/getMatchingOption.d.ts
--rw-r--r--   0        0        0     4231 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/getMatchingOption.js
--rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/getMatchingOption.js.map
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/index.d.ts
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/index.js
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/index.js.map
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/isFilesArray.d.ts
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/isFilesArray.js
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/isFilesArray.js.map
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/isMultiSelect.d.ts
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/isMultiSelect.js
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/isMultiSelect.js.map
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/isSelect.d.ts
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/isSelect.js
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/isSelect.js.map
--rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/mergeValidationData.d.ts
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/mergeValidationData.js
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/mergeValidationData.js.map
--rw-r--r--   0        0        0    15291 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/retrieveSchema.d.ts
--rw-r--r--   0        0        0    28066 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/retrieveSchema.js
--rw-r--r--   0        0        0    13290 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/retrieveSchema.js.map
--rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/sanitizeDataForNewSchema.d.ts
--rw-r--r--   0        0        0    11577 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/sanitizeDataForNewSchema.js
--rw-r--r--   0        0        0     4889 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/sanitizeDataForNewSchema.js.map
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/toIdSchema.d.ts
--rw-r--r--   0        0        0     3499 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/toIdSchema.js
--rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/toIdSchema.js.map
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/toPathSchema.d.ts
--rw-r--r--   0        0        0     4764 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/toPathSchema.js
--rw-r--r--   0        0        0     3182 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/toPathSchema.js.map
--rw-r--r--   0        0        0     5215 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/ErrorSchemaBuilder.ts
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/allowAdditionalItems.ts
--rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/asNumber.ts
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/canExpand.ts
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/constants.ts
--rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/createErrorHandler.ts
--rw-r--r--   0        0        0    14372 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/createSchemaUtils.ts
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/dataURItoBlob.ts
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/deepEquals.ts
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/englishStringTranslator.ts
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/enumOptionsDeselectValue.ts
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/enumOptionsIndexForValue.ts
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/enumOptionsIsSelected.ts
--rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/enumOptionsSelectValue.ts
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/enumOptionsValueForIndex.ts
--rw-r--r--   0        0        0     3914 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/enums.ts
--rw-r--r--   0        0        0     4067 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/findSchemaDefinition.ts
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/getDateElementProps.ts
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/getDiscriminatorFieldFromSchema.ts
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/getInputProps.ts
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/getOptionMatchingSimpleDiscriminator.ts
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/getSchemaType.ts
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/getSubmitButtonOptions.ts
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/getTemplate.ts
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/getUiOptions.ts
--rw-r--r--   0        0        0     4671 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/getWidget.tsx
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/guessType.ts
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/hasWidget.ts
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/hashForSchema.ts
--rw-r--r--   0        0        0     3310 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/idGenerators.ts
--rw-r--r--   0        0        0     4004 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/index.ts
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/isConstant.ts
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/isCustomWidget.ts
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/isFixedItems.ts
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/isObject.ts
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/labelValue.ts
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/localToUTC.ts
--rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/mergeDefaultsWithFormData.ts
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/mergeObjects.ts
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/mergeSchemas.ts
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/optionsList.ts
--rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/orderProperties.ts
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/pad.ts
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/parseDateString.ts
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/rangeSpec.ts
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/replaceStringParameters.ts
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/schemaRequiresTrueValue.ts
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/shouldRender.ts
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/toConstant.ts
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/toDateString.ts
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/toErrorList.ts
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/toErrorSchema.ts
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/tsconfig.json
--rw-r--r--   0        0        0    56287 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/types.ts
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/unwrapErrorHandler.ts
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/utcToLocal.ts
--rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/validationDataMerge.ts
--rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/withIdRefPrefix.ts
--rw-r--r--   0        0        0     5622 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/parser/ParserValidator.ts
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/parser/index.ts
--rw-r--r--   0        0        0     2902 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/parser/schemaParser.ts
--rw-r--r--   0        0        0     9294 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/schema/getClosestMatchingOption.ts
--rw-r--r--   0        0        0    21319 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/schema/getDefaultFormState.ts
--rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/schema/getDisplayLabel.ts
--rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/schema/getFirstMatchingOption.ts
--rw-r--r--   0        0        0     4060 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/schema/getMatchingOption.ts
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/schema/index.ts
--rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/schema/isFilesArray.ts
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/schema/isMultiSelect.ts
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/schema/isSelect.ts
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/schema/mergeValidationData.ts
--rw-r--r--   0        0        0    30469 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/schema/retrieveSchema.ts
--rw-r--r--   0        0        0    11171 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/schema/sanitizeDataForNewSchema.ts
--rw-r--r--   0        0        0     4110 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/schema/toIdSchema.ts
--rw-r--r--   0        0        0     5403 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/schema/toPathSchema.ts
--rwxr-xr-x   0        0        0     1141 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@types/react/LICENSE
--rwxr-xr-x   0        0        0     1916 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@types/react/README.md
--rwxr-xr-x   0        0        0     4743 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@types/react/experimental.d.ts
--rwxr-xr-x   0        0        0     7431 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@types/react/global.d.ts
--rwxr-xr-x   0        0        0   156037 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@types/react/index.d.ts
--rwxr-xr-x   0        0        0       61 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@types/react/jsx-dev-runtime.d.ts
--rwxr-xr-x   0        0        0       61 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@types/react/jsx-runtime.d.ts
--rwxr-xr-x   0        0        0     2929 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@types/react/next.d.ts
--rwxr-xr-x   0        0        0     6002 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@types/react/package.json
--rwxr-xr-x   0        0        0     4613 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@types/react/ts5.0/experimental.d.ts
--rwxr-xr-x   0        0        0     7409 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@types/react/ts5.0/global.d.ts
--rwxr-xr-x   0        0        0   152997 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@types/react/ts5.0/index.d.ts
--rwxr-xr-x   0        0        0       61 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@types/react/ts5.0/jsx-dev-runtime.d.ts
--rwxr-xr-x   0        0        0       61 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@types/react/ts5.0/jsx-runtime.d.ts
--rwxr-xr-x   0        0        0     2929 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/node_modules/@types/react/ts5.0/next.d.ts
--rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/src/executor.ts
--rw-r--r--   0        0        0     9449 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/src/filebrowser.ts
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/src/index.ts
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/style/index.css
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/style/index.js
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/.gitignore
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/LICENSE
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/README.md
--rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/pyproject.toml
--rw-r--r--   0        0        0     4703 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a0/PKG-INFO
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/install.json
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/setup.py
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/jupyter_collaboration_ui/__init__.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/jupyter_collaboration_ui/_version.py
+-rw-r--r--   0        0        0     3750 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/jupyter_collaboration_ui/labextension/package.json
+-rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/jupyter_collaboration_ui/labextension/schemas/@jupyter/collaboration-extension/package.json.orig
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/jupyter_collaboration_ui/labextension/schemas/@jupyter/collaboration-extension/shared-link.json
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/jupyter_collaboration_ui/labextension/schemas/@jupyter/collaboration-extension/user-menu-bar.json
+-rw-r--r--   0        0        0     5287 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/jupyter_collaboration_ui/labextension/static/341.2e8e5b6b71bf13a327e4.js
+-rw-r--r--   0        0        0     3255 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/jupyter_collaboration_ui/labextension/static/422.c33fd4bf2f8b13b1f430.js
+-rw-r--r--   0        0        0    11313 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/jupyter_collaboration_ui/labextension/static/44.0ba472088663f425d307.js
+-rw-r--r--   0        0        0     5287 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/jupyter_collaboration_ui/labextension/static/722.542e750613dbd427da59.js
+-rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/jupyter_collaboration_ui/labextension/static/784.1e2f345c812db2777387.js
+-rw-r--r--   0        0        0     3466 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/jupyter_collaboration_ui/labextension/static/842.5f0d12cba5fc800873b2.js
+-rw-r--r--   0        0        0     8224 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/jupyter_collaboration_ui/labextension/static/944.0167e5870ff1c1e28b32.js
+-rw-r--r--   0        0        0     9385 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/jupyter_collaboration_ui/labextension/static/952.e3c8e98af75bf2e2b0f2.js
+-rw-r--r--   0        0        0     9326 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/jupyter_collaboration_ui/labextension/static/remoteEntry.0faaa3f9527c21590e28.js
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/jupyter_collaboration_ui/labextension/static/style.js
+-rw-r--r--   0        0        0     7762 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/jupyter_collaboration_ui/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/collaboration/README.md
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/collaboration/package.json
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/collaboration/tsconfig.json
+-rw-r--r--   0        0        0     3917 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/collaboration/src/collaboratorspanel.tsx
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/collaboration/src/components.tsx
+-rw-r--r--   0        0        0    11810 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/collaboration/src/cursors.ts
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/collaboration/src/index.ts
+-rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/collaboration/src/menu.ts
+-rw-r--r--   0        0        0     5638 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/collaboration/src/sharedlink.ts
+-rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/collaboration/src/tokens.ts
+-rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/collaboration/src/userinfopanel.tsx
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/collaboration/style/base.css
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/collaboration/style/index.css
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/collaboration/style/index.js
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/collaboration/style/menu.css
+-rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/collaboration/style/sidepanel.css
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/collaboration-extension/README.md
+-rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/collaboration-extension/package.json
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/collaboration-extension/tsconfig.json
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/collaboration-extension/schema/shared-link.json
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/collaboration-extension/schema/user-menu-bar.json
+-rw-r--r--   0        0        0     5807 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/collaboration-extension/src/collaboration.ts
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/collaboration-extension/src/index.ts
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/collaboration-extension/src/sharedlink.ts
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/collaboration-extension/style/index.css
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/collaboration-extension/style/index.js
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/docprovider/babel.config.js
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/docprovider/jest.config.js
+-rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/docprovider/package.json
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/docprovider/tsconfig.json
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/docprovider/tsconfig.test.json
+-rw-r--r--   0        0        0     3594 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/docprovider/src/awareness.ts
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/docprovider/src/index.ts
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/docprovider/src/requests.ts
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/docprovider/src/tokens.ts
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/docprovider/src/utils.ts
+-rw-r--r--   0        0        0     6975 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/docprovider/src/ydrive.ts
+-rw-r--r--   0        0        0     5061 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/docprovider/src/yprovider.ts
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/docprovider/src/__tests__/yprovider.spec.ts
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/docprovider-extension/README.md
+-rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/docprovider-extension/package.json
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/docprovider-extension/tsconfig.json
+-rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/docprovider-extension/src/executor.ts
+-rw-r--r--   0        0        0     9449 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/docprovider-extension/src/filebrowser.ts
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/docprovider-extension/src/index.ts
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/docprovider-extension/style/index.css
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/docprovider-extension/style/index.js
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/.gitignore
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/LICENSE
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/README.md
+-rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/pyproject.toml
+-rw-r--r--   0        0        0     4703 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/PKG-INFO
```

### Comparing `jupyter_collaboration_ui-1.0.0a0/jupyter_collaboration_ui/labextension/package.json` & `jupyter_collaboration_ui-1.0.0a1/jupyter_collaboration_ui/labextension/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9753787878787878%*

 * *Differences: {"'dependencies'": "{'@jupyter/collaboration': '^3.0.0-alpha.1', '@jupyter/docprovider': "*

 * *                   "'^3.0.0-alpha.1'}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.0faaa3f9527c21590e28.js'}}",*

 * * "'version'": "'3.0.0-alpha.1'"}*

```diff
@@ -1,15 +1,15 @@
 {
     "author": "Project Jupyter",
     "bugs": {
         "url": "https://github.com/jupyterlab/jupyter-collaboration/issues"
     },
     "dependencies": {
-        "@jupyter/collaboration": "^3.0.0-alpha.0",
-        "@jupyter/docprovider": "^3.0.0-alpha.0",
+        "@jupyter/collaboration": "^3.0.0-alpha.1",
+        "@jupyter/docprovider": "^3.0.0-alpha.1",
         "@jupyter/ydoc": "^1.1.0-a0",
         "@jupyterlab/application": "^4.2.0-beta.0",
         "@jupyterlab/apputils": "^4.2.0-beta.0",
         "@jupyterlab/codemirror": "^4.2.0-beta.0",
         "@jupyterlab/coreutils": "^6.0.5",
         "@jupyterlab/services": "^7.0.5",
         "@jupyterlab/statedb": "^4.2.0-beta.0",
@@ -39,15 +39,15 @@
         "style/*.css",
         "style/index.js"
     ],
     "homepage": "https://github.com/jupyterlab/jupyter-collaboration",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.4f29d48a8c309dadd4a6.js",
+            "load": "static/remoteEntry.0faaa3f9527c21590e28.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "../../projects/jupyter-collaboration-ui/jupyter_collaboration_ui/labextension",
         "schemaDir": "./schema",
         "sharedPackages": {
             "@codemirror/state": {
@@ -120,9 +120,9 @@
     "typedoc": {
         "displayName": "@jupyter/collaboration-extension",
         "entryPoint": "./src/index.ts",
         "readmeFile": "./README.md",
         "tsconfig": "./tsconfig.json"
     },
     "types": "lib/index.d.ts",
-    "version": "3.0.0-alpha.0"
+    "version": "3.0.0-alpha.1"
 }
```

### Comparing `jupyter_collaboration_ui-1.0.0a0/jupyter_collaboration_ui/labextension/schemas/@jupyter/collaboration-extension/package.json.orig` & `jupyter_collaboration_ui-1.0.0a1/jupyter_collaboration_ui/labextension/schemas/@jupyter/collaboration-extension/package.json.orig`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9757575757575757%*

 * *Differences: {"'dependencies'": "{'@jupyter/collaboration': '^3.0.0-alpha.1', '@jupyter/docprovider': "*

 * *                   "'^3.0.0-alpha.1'}",*

 * * "'version'": "'3.0.0-alpha.1'"}*

```diff
@@ -1,15 +1,15 @@
 {
     "author": "Project Jupyter",
     "bugs": {
         "url": "https://github.com/jupyterlab/jupyter-collaboration/issues"
     },
     "dependencies": {
-        "@jupyter/collaboration": "^3.0.0-alpha.0",
-        "@jupyter/docprovider": "^3.0.0-alpha.0",
+        "@jupyter/collaboration": "^3.0.0-alpha.1",
+        "@jupyter/docprovider": "^3.0.0-alpha.1",
         "@jupyter/ydoc": "^1.1.0-a0",
         "@jupyterlab/application": "^4.2.0-beta.0",
         "@jupyterlab/apputils": "^4.2.0-beta.0",
         "@jupyterlab/codemirror": "^4.2.0-beta.0",
         "@jupyterlab/coreutils": "^6.0.5",
         "@jupyterlab/services": "^7.0.5",
         "@jupyterlab/statedb": "^4.2.0-beta.0",
@@ -115,9 +115,9 @@
     "typedoc": {
         "displayName": "@jupyter/collaboration-extension",
         "entryPoint": "./src/index.ts",
         "readmeFile": "./README.md",
         "tsconfig": "./tsconfig.json"
     },
     "types": "lib/index.d.ts",
-    "version": "3.0.0-alpha.0"
+    "version": "3.0.0-alpha.1"
 }
```

### Comparing `jupyter_collaboration_ui-1.0.0a0/jupyter_collaboration_ui/labextension/static/341.f4c7f164b4cd115c5478.js` & `jupyter_collaboration_ui-1.0.0a1/jupyter_collaboration_ui/labextension/static/341.2e8e5b6b71bf13a327e4.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -42,17 +42,17 @@
                         t = i.xv();
                     i.zd(t, o.CHAT), i.Qj(t, JSON.stringify(s)), this.ws.send(i.Fo(t))
                 }
                 _onUserChanged(e) {
                     this._awareness.setLocalStateField("user", e.identity)
                 }
             }
-            var h = t(6597),
-                d = t(2486),
-                l = t(7638),
+            var h = t(7655),
+                d = t(8824),
+                l = t(8440),
                 _ = t(7262);
             class p {
                 constructor(e) {
                     this._onConnectionClosed = e => {
                         1003 === e.code && (console.error("Document provider closed:", e.reason), (0, l.showErrorMessage)(this._trans.__("Document session error"), e.reason, [l.Dialog.okButton()]), this._sharedModel.dispose())
                     }, this._onSync = e => {
                         var s;
```

### Comparing `jupyter_collaboration_ui-1.0.0a0/jupyter_collaboration_ui/labextension/static/422.c33fd4bf2f8b13b1f430.js` & `jupyter_collaboration_ui-1.0.0a1/jupyter_collaboration_ui/labextension/static/422.c33fd4bf2f8b13b1f430.js`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration_ui-1.0.0a0/jupyter_collaboration_ui/labextension/static/44.432895baa828dc568436.js` & `jupyter_collaboration_ui-1.0.0a1/jupyter_collaboration_ui/labextension/static/44.0ba472088663f425d307.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -15,16 +15,16 @@
                 showSharedLinkDialog: () => L
             });
             var r = n(7262);
             const s = new r.Token("@jupyter/collaboration:IUserMenu"),
                 o = new r.Token("@jupyter/collaboration:IGlobalAwareness");
             var a = n(3345),
                 i = n(5256),
-                l = n(7638),
-                c = n(6597);
+                l = n(8440),
+                c = n(7655);
             const d = "jp-Collaborator";
             class u extends i.Panel {
                 constructor(e, t, n) {
                     super({}), this._onAwarenessChanged = () => {
                         const e = this._awareness.getStates(),
                             t = [];
                         e.forEach(((e, n) => {
@@ -249,15 +249,15 @@
                         parent: document.body
                     })]
                 });
 
             function x(e) {
                 return [f.of(e), C]
             }
-            var j = n(7664),
+            var j = n(2126),
                 A = n(4873);
             class I extends i.MenuBar.Renderer {
                 constructor(e) {
                     super(), this._user = e
                 }
                 renderItem(e) {
                     const t = this.createItemClass(e),
@@ -293,15 +293,15 @@
                 }
             }
             class P extends i.Menu {
                 constructor(e) {
                     super(e)
                 }
             }
-            var E = n(7714);
+            var E = n(2844);
             async function L({
                 translator: e
             }) {
                 const t = (null != e ? e : E.nullTranslator).load("collaboration"),
                     n = c.PageConfig.getToken(),
                     r = new URL(c.URLExt.normalize(c.PageConfig.getUrl({
                         workspace: c.PageConfig.defaultWorkspace
```

### Comparing `jupyter_collaboration_ui-1.0.0a0/jupyter_collaboration_ui/labextension/static/722.260709dc491d985c4f31.js` & `jupyter_collaboration_ui-1.0.0a1/jupyter_collaboration_ui/labextension/static/722.542e750613dbd427da59.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -42,17 +42,17 @@
                         t = i.xv();
                     i.zd(t, o.CHAT), i.Qj(t, JSON.stringify(s)), this.ws.send(i.Fo(t))
                 }
                 _onUserChanged(e) {
                     this._awareness.setLocalStateField("user", e.identity)
                 }
             }
-            var h = t(6597),
-                d = t(2486),
-                l = t(7638),
+            var h = t(7655),
+                d = t(8824),
+                l = t(8440),
                 _ = t(7262);
             class p {
                 constructor(e) {
                     this._onConnectionClosed = e => {
                         1003 === e.code && (console.error("Document provider closed:", e.reason), (0, l.showErrorMessage)(this._trans.__("Document session error"), e.reason, [l.Dialog.okButton()]), this._sharedModel.dispose())
                     }, this._onSync = e => {
                         var s;
```

### Comparing `jupyter_collaboration_ui-1.0.0a0/jupyter_collaboration_ui/labextension/static/784.1e2f345c812db2777387.js` & `jupyter_collaboration_ui-1.0.0a1/jupyter_collaboration_ui/labextension/static/784.1e2f345c812db2777387.js`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration_ui-1.0.0a0/jupyter_collaboration_ui/labextension/static/842.b8a53bb7e5d9e0593385.js` & `jupyter_collaboration_ui-1.0.0a1/jupyter_collaboration_ui/labextension/static/842.5f0d12cba5fc800873b2.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,24 +1,24 @@
 "use strict";
 (self.webpackChunk_jupyter_collaboration_extension = self.webpackChunk_jupyter_collaboration_extension || []).push([
     [842], {
         4842: (e, r, a) => {
             a.r(r), a.d(r, {
                 default: () => x
             });
-            var t = a(7638),
-                o = a(6901),
-                n = a(424),
-                s = a(7664),
-                i = a(6597),
-                l = a(2486),
-                c = a(9750),
-                d = a(7714),
+            var t = a(8440),
+                o = a(7623),
+                n = a(9835),
+                s = a(2126),
+                i = a(7655),
+                l = a(8824),
+                c = a(2824),
+                d = a(2844),
                 u = a(5256),
-                p = a(908),
+                p = a(7435),
                 m = a(2206),
                 b = a(7784);
             const y = {
                     id: "@jupyter/collaboration-extension:userMenu",
                     description: "Provide connected user menu.",
                     requires: [],
                     provides: p.IUserMenu,
```

### Comparing `jupyter_collaboration_ui-1.0.0a0/jupyter_collaboration_ui/labextension/static/944.0167e5870ff1c1e28b32.js` & `jupyter_collaboration_ui-1.0.0a1/jupyter_collaboration_ui/labextension/static/944.0167e5870ff1c1e28b32.js`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration_ui-1.0.0a0/jupyter_collaboration_ui/labextension/static/952.e3c8e98af75bf2e2b0f2.js` & `jupyter_collaboration_ui-1.0.0a1/jupyter_collaboration_ui/labextension/static/952.e3c8e98af75bf2e2b0f2.js`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration_ui-1.0.0a0/jupyter_collaboration_ui/labextension/static/remoteEntry.4f29d48a8c309dadd4a6.js` & `jupyter_collaboration_ui-1.0.0a1/jupyter_collaboration_ui/labextension/static/remoteEntry.0faaa3f9527c21590e28.js`

 * *Files 11% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, a, o, n, i, l, u, d, f, s, c, p, h, b, v, m, y, g, j, w = {
-            4819: (e, r, t) => {
+    var e, r, t, a, o, n, i, l, u, d, f, c, s, p, h, b, v, m, y, g, j, w = {
+            1998: (e, r, t) => {
                 var a = {
-                        "./index": () => Promise.all([t.e(422), t.e(784), t.e(206), t.e(254), t.e(30), t.e(486), t.e(842)]).then((() => () => t(4842))),
-                        "./extension": () => Promise.all([t.e(422), t.e(784), t.e(206), t.e(254), t.e(30), t.e(486), t.e(842)]).then((() => () => t(4842))),
+                        "./index": () => Promise.all([t.e(422), t.e(784), t.e(206), t.e(394), t.e(242), t.e(824), t.e(842)]).then((() => () => t(4842))),
+                        "./extension": () => Promise.all([t.e(422), t.e(784), t.e(206), t.e(394), t.e(242), t.e(824), t.e(842)]).then((() => () => t(4842))),
                         "./style": () => t.e(944).then((() => () => t(5944)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     n = (e, r) => {
                         if (t.S) {
@@ -43,41 +43,41 @@
         }), r
     }, S.d = (e, r) => {
         for (var t in r) S.o(r, t) && !S.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, S.f = {}, S.e = e => Promise.all(Object.keys(S.f).reduce(((r, t) => (S.f[t](e, r), r)), [])), S.u = e => e + "." + {
-        30: "611f74066991109f0a62",
-        44: "432895baa828dc568436",
+        44: "0ba472088663f425d307",
         206: "7108eced39c49eb27106",
-        254: "4e54507d87d51091054d",
+        242: "f38d53af901815a08cb5",
         262: "d6f92031996231d96ae8",
-        341: "f4c7f164b4cd115c5478",
+        341: "2e8e5b6b71bf13a327e4",
         349: "e89d95e45f94f06ccdb1",
+        394: "c889587484bcd2ab8dd1",
         422: "c33fd4bf2f8b13b1f430",
-        486: "f1d8694bde9147160492",
-        722: "260709dc491d985c4f31",
+        722: "542e750613dbd427da59",
         784: "1e2f345c812db2777387",
-        842: "b8a53bb7e5d9e0593385",
+        824: "7eeac4763f58845a00cd",
+        842: "5f0d12cba5fc800873b2",
         944: "0167e5870ff1c1e28b32",
         952: "e3c8e98af75bf2e2b0f2"
     } [e] + ".js?v=" + {
-        30: "611f74066991109f0a62",
-        44: "432895baa828dc568436",
+        44: "0ba472088663f425d307",
         206: "7108eced39c49eb27106",
-        254: "4e54507d87d51091054d",
+        242: "f38d53af901815a08cb5",
         262: "d6f92031996231d96ae8",
-        341: "f4c7f164b4cd115c5478",
+        341: "2e8e5b6b71bf13a327e4",
         349: "e89d95e45f94f06ccdb1",
+        394: "c889587484bcd2ab8dd1",
         422: "c33fd4bf2f8b13b1f430",
-        486: "f1d8694bde9147160492",
-        722: "260709dc491d985c4f31",
+        722: "542e750613dbd427da59",
         784: "1e2f345c812db2777387",
-        842: "b8a53bb7e5d9e0593385",
+        824: "7eeac4763f58845a00cd",
+        842: "5f0d12cba5fc800873b2",
         944: "0167e5870ff1c1e28b32",
         952: "e3c8e98af75bf2e2b0f2"
     } [e], S.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
@@ -92,24 +92,24 @@
                     var f = u[d];
                     if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + o) {
                         i = f;
                         break
                     }
                 }
             i || (l = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, S.nc && i.setAttribute("nonce", S.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [a];
-            var s = (r, a) => {
-                    i.onerror = i.onload = null, clearTimeout(c);
+            var c = (r, a) => {
+                    i.onerror = i.onload = null, clearTimeout(s);
                     var o = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(a))), r) return r(a)
                 },
-                c = setTimeout(s.bind(null, void 0, {
+                s = setTimeout(c.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = s.bind(null, i.onerror), i.onload = s.bind(null, i.onload), l && document.head.appendChild(i)
+            i.onerror = c.bind(null, i.onerror), i.onload = c.bind(null, i.onload), l && document.head.appendChild(i)
         }
     }, S.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -131,15 +131,15 @@
                         (!l || !l.loaded && (!a != !l.eager ? a : i > l.from)) && (o[r] = {
                             get: t,
                             from: i,
                             eager: !!a
                         })
                     },
                     u = [];
-                return "default" === t && (l("@jupyter/collaboration-extension", "3.0.0-alpha.0", (() => Promise.all([S.e(422), S.e(784), S.e(206), S.e(254), S.e(30), S.e(486), S.e(842)]).then((() => () => S(4842))))), l("@jupyter/collaboration", "3.0.0-alpha.0", (() => Promise.all([S.e(206), S.e(262), S.e(254), S.e(44), S.e(30)]).then((() => () => S(2044))))), l("@jupyter/docprovider", "3.0.0-alpha.0", (() => Promise.all([S.e(422), S.e(262), S.e(254), S.e(349), S.e(486), S.e(341)]).then((() => () => S(9341))))), l("y-websocket", "1.5.4", (() => Promise.all([S.e(422), S.e(784), S.e(952), S.e(206)]).then((() => () => S(2952)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                return "default" === t && (l("@jupyter/collaboration-extension", "3.0.0-alpha.1", (() => Promise.all([S.e(422), S.e(784), S.e(206), S.e(394), S.e(242), S.e(824), S.e(842)]).then((() => () => S(4842))))), l("@jupyter/collaboration", "3.0.0-alpha.1", (() => Promise.all([S.e(206), S.e(262), S.e(394), S.e(44), S.e(242)]).then((() => () => S(2044))))), l("@jupyter/docprovider", "3.0.0-alpha.1", (() => Promise.all([S.e(422), S.e(262), S.e(394), S.e(349), S.e(824), S.e(341)]).then((() => () => S(9341))))), l("y-websocket", "1.5.4", (() => Promise.all([S.e(422), S.e(784), S.e(952), S.e(206)]).then((() => () => S(2952)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         S.g.importScripts && (e = S.g.location + "");
         var r = S.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -189,91 +189,91 @@
     }, n = (e, r) => {
         if (0 in e) {
             r = t(r);
             var a = e[0],
                 o = a < 0;
             o && (a = -a - 1);
             for (var i = 0, l = 1, u = !0;; l++, i++) {
-                var d, f, s = l < e.length ? (typeof e[l])[0] : "";
-                if (i >= r.length || "o" == (f = (typeof(d = r[i]))[0])) return !u || ("u" == s ? l > a && !o : "" == s != o);
+                var d, f, c = l < e.length ? (typeof e[l])[0] : "";
+                if (i >= r.length || "o" == (f = (typeof(d = r[i]))[0])) return !u || ("u" == c ? l > a && !o : "" == c != o);
                 if ("u" == f) {
-                    if (!u || "u" != s) return !1
+                    if (!u || "u" != c) return !1
                 } else if (u)
-                    if (s == f)
+                    if (c == f)
                         if (l <= a) {
                             if (d != e[l]) return !1
                         } else {
                             if (o ? d > e[l] : d < e[l]) return !1;
                             d != e[l] && (u = !1)
                         }
-                else if ("s" != s && "n" != s) {
+                else if ("s" != c && "n" != c) {
                     if (o || l <= a) return !1;
                     u = !1, l--
                 } else {
-                    if (l <= a || f < s != o) return !1;
+                    if (l <= a || f < c != o) return !1;
                     u = !1
-                } else "s" != s && "n" != s && (u = !1, l--)
+                } else "s" != c && "n" != c && (u = !1, l--)
             }
         }
-        var c = [],
-            p = c.pop.bind(c);
+        var s = [],
+            p = s.pop.bind(s);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
-            c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? n(h, r) : !p())
+            s.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? n(h, r) : !p())
         }
         return !!p()
     }, i = (e, r) => {
         var t = S.S[e];
         if (!t || !S.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, l = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && a(e, r) ? r : e), 0)
     }, u = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(a) + ")", d = (e, r, t, a) => {
         var o = l(e, t);
-        return n(a, o) || s(u(e, t, o, a)), c(e[t][o])
+        return n(a, o) || c(u(e, t, o, a)), s(e[t][o])
     }, f = (e, r, t) => {
         var o = e[r];
         return (r = Object.keys(o).reduce(((e, r) => !n(t, r) || e && !a(e, r) ? e : r), 0)) && o[r]
-    }, s = e => {
+    }, c = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
-    }, c = e => (e.loaded = 1, e.get()), h = (p = e => function(r, t, a, o) {
+    }, s = e => (e.loaded = 1, e.get()), h = (p = e => function(r, t, a, o) {
         var n = S.I(r);
         return n && n.then ? n.then(e.bind(e, r, S.S[r], t, a, o)) : e(r, S.S[r], t, a, o)
     })(((e, r, t, a) => (i(e, t), d(r, 0, t, a)))), b = p(((e, r, t, a, o) => r && S.o(r, t) ? d(r, 0, t, a) : o())), v = p(((e, r, t, a, o) => {
         var n = r && S.o(r, t) && f(r, t, a);
-        return n ? c(n) : o()
+        return n ? s(n) : o()
     })), m = {}, y = {
         2206: () => h("default", "yjs", [1, 13, 5, 40]),
-        6597: () => h("default", "@jupyterlab/coreutils", [1, 6, 1, 6]),
-        7638: () => h("default", "@jupyterlab/apputils", [1, 4, 2, 6]),
+        7655: () => h("default", "@jupyterlab/coreutils", [1, 6, 1, 8]),
+        8440: () => h("default", "@jupyterlab/apputils", [1, 4, 2, 8]),
+        2126: () => h("default", "@jupyterlab/ui-components", [1, 4, 1, 8]),
+        2844: () => h("default", "@jupyterlab/translation", [1, 4, 1, 8]),
         5256: () => h("default", "@lumino/widgets", [1, 2, 3, 1, , "alpha", 0]),
-        7664: () => h("default", "@jupyterlab/ui-components", [1, 4, 1, 6]),
-        7714: () => h("default", "@jupyterlab/translation", [1, 4, 1, 6]),
-        2486: () => h("default", "@jupyterlab/services", [1, 7, 1, 6]),
-        424: () => b("default", "@jupyter/docprovider", [1, 3, 0, 0, , "alpha", 0], (() => Promise.all([S.e(262), S.e(349), S.e(722)]).then((() => () => S(9341))))),
-        908: () => b("default", "@jupyter/collaboration", [1, 3, 0, 0, , "alpha", 0], (() => Promise.all([S.e(262), S.e(44)]).then((() => () => S(2044))))),
-        6901: () => h("default", "@jupyterlab/codemirror", [1, 4, 1, 6]),
-        9750: () => h("default", "@jupyterlab/statedb", [1, 4, 1, 6]),
+        8824: () => h("default", "@jupyterlab/services", [1, 7, 1, 8]),
+        2824: () => h("default", "@jupyterlab/statedb", [1, 4, 1, 8]),
+        7435: () => b("default", "@jupyter/collaboration", [1, 3, 0, 0, , "alpha", 1], (() => Promise.all([S.e(262), S.e(44)]).then((() => () => S(2044))))),
+        7623: () => h("default", "@jupyterlab/codemirror", [1, 4, 1, 8]),
+        9835: () => b("default", "@jupyter/docprovider", [1, 3, 0, 0, , "alpha", 1], (() => Promise.all([S.e(262), S.e(349), S.e(722)]).then((() => () => S(9341))))),
         7262: () => h("default", "@lumino/coreutils", [1, 2, 0, 0]),
         195: () => h("default", "@codemirror/state", [1, 6, 2, 0]),
         3345: () => h("default", "react", [1, 18, 2, 0]),
         4873: () => h("default", "@lumino/virtualdom", [1, 2, 0, 0]),
         5024: () => h("default", "@codemirror/view", [1, 6, 9, 6]),
         3560: () => v("default", "y-websocket", [1, 1, 3, 15], (() => Promise.all([S.e(784), S.e(952), S.e(206)]).then((() => () => S(2952))))),
         4602: () => h("default", "@lumino/signaling", [1, 2, 0, 0])
     }, g = {
-        30: [5256, 7664, 7714],
         44: [195, 3345, 4873, 5024],
         206: [2206],
-        254: [6597, 7638],
+        242: [2126, 2844, 5256],
         262: [7262],
         349: [3560, 4602],
-        486: [2486],
-        842: [424, 908, 6901, 9750]
+        394: [7655, 8440],
+        824: [8824],
+        842: [2824, 7435, 7623, 9835]
     }, j = {}, S.f.consumes = (e, r) => {
         S.o(g, e) && g[e].forEach((e => {
             if (S.o(m, e)) return r.push(m[e]);
             if (!j[e]) {
                 var t = r => {
                     m[e] = 0, S.m[e] = t => {
                         delete S.c[e], t.exports = r()
@@ -297,15 +297,15 @@
         var e = {
             270: 0
         };
         S.f.j = (r, t) => {
             var a = S.o(e, r) ? e[r] : void 0;
             if (0 !== a)
                 if (a) t.push(a[2]);
-                else if (/^(2(06|54|62)|30|349|486)$/.test(r)) e[r] = 0;
+                else if (/^(2(06|42|62)|349|394|824)$/.test(r)) e[r] = 0;
             else {
                 var o = new Promise(((t, o) => a = e[r] = [t, o]));
                 t.push(a[2] = o);
                 var n = S.p + S.u(r),
                     i = new Error;
                 S.l(n, (t => {
                     if (S.o(e, r) && (0 !== (a = e[r]) && (e[r] = void 0), a)) {
@@ -324,10 +324,10 @@
                     l && l(S)
                 }
                 for (r && r(t); u < n.length; u++) o = n[u], S.o(e, o) && e[o] && e[o][0](), e[o] = 0
             },
             t = self.webpackChunk_jupyter_collaboration_extension = self.webpackChunk_jupyter_collaboration_extension || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), S.nc = void 0;
-    var x = S(4819);
+    var x = S(1998);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@jupyter/collaboration-extension"] = x
 })();
```

### Comparing `jupyter_collaboration_ui-1.0.0a0/jupyter_collaboration_ui/labextension/static/third-party-licenses.json` & `jupyter_collaboration_ui-1.0.0a1/jupyter_collaboration_ui/labextension/static/third-party-licenses.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.984375%*

 * *Differences: {"'packages'": "{0: {'versionInfo': '3.0.0-alpha.1'}, 1: {'versionInfo': '3.0.0-alpha.1'}}"}*

```diff
@@ -1,20 +1,20 @@
 {
     "packages": [
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyter/collaboration",
-            "versionInfo": "3.0.0-alpha.0"
+            "versionInfo": "3.0.0-alpha.1"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyter/docprovider",
-            "versionInfo": "3.0.0-alpha.0"
+            "versionInfo": "3.0.0-alpha.1"
         },
         {
             "extractedText": "Copyright JS Foundation and other contributors\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n'Software'), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY\nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,\nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE\nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "css-loader",
             "versionInfo": "6.11.0"
         },
```

### Comparing `jupyter_collaboration_ui-1.0.0a0/packages/collaboration/package.json` & `jupyter_collaboration_ui-1.0.0a1/packages/collaboration/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9740384615384615%*

 * *Differences: {"'dependencies'": "{'@jupyter/docprovider': '^3.0.0-alpha.1'}", "'version'": "'3.0.0-alpha.1'"}*

```diff
@@ -2,15 +2,15 @@
     "author": "Project Jupyter",
     "bugs": {
         "url": "https://github.com/jupyterlab/jupyter-collaboration/issues"
     },
     "dependencies": {
         "@codemirror/state": "^6.2.0",
         "@codemirror/view": "^6.7.0",
-        "@jupyter/docprovider": "^3.0.0-alpha.0",
+        "@jupyter/docprovider": "^3.0.0-alpha.1",
         "@jupyterlab/apputils": "^4.0.5",
         "@jupyterlab/coreutils": "^6.0.5",
         "@jupyterlab/services": "^7.0.5",
         "@jupyterlab/ui-components": "^4.0.5",
         "@lumino/coreutils": "^2.1.0",
         "@lumino/virtualdom": "^2.0.0",
         "@lumino/widgets": "^2.1.0",
@@ -63,9 +63,9 @@
     "typedoc": {
         "displayName": "@jupyter/collaboration",
         "entryPoint": "./src/index.ts",
         "readmeFile": "./README.md",
         "tsconfig": "./tsconfig.json"
     },
     "types": "lib/index.d.ts",
-    "version": "3.0.0-alpha.0"
+    "version": "3.0.0-alpha.1"
 }
```

### Comparing `jupyter_collaboration_ui-1.0.0a0/packages/collaboration/lib/collaboratorspanel.js` & `jupyter_collaboration_ui-1.0.0a1/packages/collaboration/src/collaboratorspanel.tsx`

 * *Files 9% similar despite different names*

```diff
@@ -1,227 +1,245 @@
 00000000: 2f2f 2043 6f70 7972 6967 6874 2028 6329  // Copyright (c)
 00000010: 204a 7570 7974 6572 2044 6576 656c 6f70   Jupyter Develop
 00000020: 6d65 6e74 2054 6561 6d2e 0a2f 2f20 4469  ment Team..// Di
 00000030: 7374 7269 6275 7465 6420 756e 6465 7220  stributed under 
 00000040: 7468 6520 7465 726d 7320 6f66 2074 6865  the terms of the
 00000050: 204d 6f64 6966 6965 6420 4253 4420 4c69   Modified BSD Li
-00000060: 6365 6e73 652e 0a69 6d70 6f72 7420 2a20  cense..import * 
-00000070: 6173 2052 6561 6374 2066 726f 6d20 2772  as React from 'r
-00000080: 6561 6374 273b 0a69 6d70 6f72 7420 7b20  eact';.import { 
-00000090: 5061 6e65 6c20 7d20 6672 6f6d 2027 406c  Panel } from '@l
-000000a0: 756d 696e 6f2f 7769 6467 6574 7327 3b0a  umino/widgets';.
-000000b0: 696d 706f 7274 207b 2052 6561 6374 5769  import { ReactWi
-000000c0: 6467 6574 207d 2066 726f 6d20 2740 6a75  dget } from '@ju
-000000d0: 7079 7465 726c 6162 2f61 7070 7574 696c  pyterlab/apputil
-000000e0: 7327 3b0a 696d 706f 7274 207b 2050 6174  s';.import { Pat
-000000f0: 6845 7874 207d 2066 726f 6d20 2740 6a75  hExt } from '@ju
-00000100: 7079 7465 726c 6162 2f63 6f72 6575 7469  pyterlab/coreuti
-00000110: 6c73 273b 0a2f 2a2a 0a20 2a20 5468 6520  ls';./**. * The 
-00000120: 4353 5320 636c 6173 7320 6164 6465 6420  CSS class added 
-00000130: 746f 2063 6f6c 6c61 626f 7261 746f 7273  to collaborators
-00000140: 2070 616e 656c 2e0a 202a 2f0a 636f 6e73   panel.. */.cons
-00000150: 7420 434f 4c4c 4142 4f52 4154 4f52 535f  t COLLABORATORS_
-00000160: 5041 4e45 4c5f 434c 4153 5320 3d20 276a  PANEL_CLASS = 'j
-00000170: 702d 436f 6c6c 6162 6f72 6174 6f72 7350  p-CollaboratorsP
-00000180: 616e 656c 273b 0a2f 2a2a 0a20 2a20 5468  anel';./**. * Th
-00000190: 6520 4353 5320 636c 6173 7320 6164 6465  e CSS class adde
-000001a0: 6420 746f 2063 6f6c 6c61 626f 7261 746f  d to collaborato
-000001b0: 7273 206c 6973 7420 636f 6e74 6169 6e65  rs list containe
-000001c0: 722e 0a20 2a2f 0a63 6f6e 7374 2043 4f4c  r.. */.const COL
-000001d0: 4c41 424f 5241 544f 5253 5f4c 4953 545f  LABORATORS_LIST_
-000001e0: 434c 4153 5320 3d20 276a 702d 436f 6c6c  CLASS = 'jp-Coll
-000001f0: 6162 6f72 6174 6f72 734c 6973 7427 3b0a  aboratorsList';.
-00000200: 2f2a 2a0a 202a 2054 6865 2043 5353 2063  /**. * The CSS c
-00000210: 6c61 7373 2061 6464 6564 2074 6f20 6561  lass added to ea
-00000220: 6368 2063 6f6c 6c61 626f 7261 746f 7220  ch collaborator 
-00000230: 656c 656d 656e 742e 0a20 2a2f 0a63 6f6e  element.. */.con
-00000240: 7374 2043 4f4c 4c41 424f 5241 544f 525f  st COLLABORATOR_
-00000250: 434c 4153 5320 3d20 276a 702d 436f 6c6c  CLASS = 'jp-Coll
-00000260: 6162 6f72 6174 6f72 273b 0a2f 2a2a 0a20  aborator';./**. 
-00000270: 2a20 5468 6520 4353 5320 636c 6173 7320  * The CSS class 
-00000280: 6164 6465 6420 746f 2065 6163 6820 636f  added to each co
-00000290: 6c6c 6162 6f72 6174 6f72 2065 6c65 6d65  llaborator eleme
-000002a0: 6e74 2e0a 202a 2f0a 636f 6e73 7420 434c  nt.. */.const CL
-000002b0: 4943 4b41 424c 455f 434f 4c4c 4142 4f52  ICKABLE_COLLABOR
-000002c0: 4154 4f52 5f43 4c41 5353 203d 2027 6a70  ATOR_CLASS = 'jp
-000002d0: 2d43 6c69 636b 6162 6c65 436f 6c6c 6162  -ClickableCollab
-000002e0: 6f72 6174 6f72 273b 0a2f 2a2a 0a20 2a20  orator';./**. * 
-000002f0: 5468 6520 4353 5320 636c 6173 7320 6164  The CSS class ad
-00000300: 6465 6420 746f 2065 6163 6820 636f 6c6c  ded to each coll
-00000310: 6162 6f72 6174 6f72 2069 636f 6e2e 0a20  aborator icon.. 
-00000320: 2a2f 0a63 6f6e 7374 2043 4f4c 4c41 424f  */.const COLLABO
-00000330: 5241 544f 525f 4943 4f4e 5f43 4c41 5353  RATOR_ICON_CLASS
-00000340: 203d 2027 6a70 2d43 6f6c 6c61 626f 7261   = 'jp-Collabora
-00000350: 746f 7249 636f 6e27 3b0a 6578 706f 7274  torIcon';.export
-00000360: 2063 6c61 7373 2043 6f6c 6c61 626f 7261   class Collabora
-00000370: 746f 7273 5061 6e65 6c20 6578 7465 6e64  torsPanel extend
-00000380: 7320 5061 6e65 6c20 7b0a 2020 2020 636f  s Panel {.    co
-00000390: 6e73 7472 7563 746f 7228 6375 7272 656e  nstructor(curren
-000003a0: 7455 7365 722c 2061 7761 7265 6e65 7373  tUser, awareness
-000003b0: 2c20 6669 6c65 6f70 656e 6572 2920 7b0a  , fileopener) {.
-000003c0: 2020 2020 2020 2020 7375 7065 7228 7b7d          super({}
-000003d0: 293b 0a20 2020 2020 2020 202f 2a2a 0a20  );.        /**. 
-000003e0: 2020 2020 2020 2020 2a20 4861 6e64 6c65          * Handle
-000003f0: 2063 6f6c 6c61 626f 7261 746f 7220 6368   collaborator ch
-00000400: 616e 6765 2e0a 2020 2020 2020 2020 202a  ange..         *
-00000410: 2f0a 2020 2020 2020 2020 7468 6973 2e5f  /.        this._
-00000420: 6f6e 4177 6172 656e 6573 7343 6861 6e67  onAwarenessChang
-00000430: 6564 203d 2028 2920 3d3e 207b 0a20 2020  ed = () => {.   
-00000440: 2020 2020 2020 2020 2063 6f6e 7374 2073           const s
-00000450: 7461 7465 203d 2074 6869 732e 5f61 7761  tate = this._awa
-00000460: 7265 6e65 7373 2e67 6574 5374 6174 6573  reness.getStates
-00000470: 2829 3b0a 2020 2020 2020 2020 2020 2020  ();.            
-00000480: 636f 6e73 7420 636f 6c6c 6162 6f72 6174  const collaborat
-00000490: 6f72 7320 3d20 5b5d 3b0a 2020 2020 2020  ors = [];.      
-000004a0: 2020 2020 2020 7374 6174 652e 666f 7245        state.forE
-000004b0: 6163 6828 2876 616c 7565 2c20 6b65 7929  ach((value, key)
-000004c0: 203d 3e20 7b0a 2020 2020 2020 2020 2020   => {.          
-000004d0: 2020 2020 2020 6966 2028 7468 6973 2e5f        if (this._
-000004e0: 6375 7272 656e 7455 7365 722e 6973 5265  currentUser.isRe
-000004f0: 6164 7920 2626 0a20 2020 2020 2020 2020  ady &&.         
-00000500: 2020 2020 2020 2020 2020 2076 616c 7565             value
-00000510: 2e75 7365 722e 7573 6572 6e61 6d65 2021  .user.username !
-00000520: 3d3d 2074 6869 732e 5f63 7572 7265 6e74  == this._current
-00000530: 5573 6572 2e69 6465 6e74 6974 792e 7573  User.identity.us
-00000540: 6572 6e61 6d65 2920 7b0a 2020 2020 2020  ername) {.      
-00000550: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00000560: 6c6c 6162 6f72 6174 6f72 732e 7075 7368  llaborators.push
-00000570: 2876 616c 7565 293b 0a20 2020 2020 2020  (value);.       
-00000580: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
-00000590: 2020 2020 2020 207d 293b 0a20 2020 2020         });.     
-000005a0: 2020 2020 2020 2074 6869 732e 5f62 6f64         this._bod
-000005b0: 792e 636f 6c6c 6162 6f72 6174 6f72 7320  y.collaborators 
-000005c0: 3d20 636f 6c6c 6162 6f72 6174 6f72 733b  = collaborators;
-000005d0: 0a20 2020 2020 2020 207d 3b0a 2020 2020  .        };.    
-000005e0: 2020 2020 7468 6973 2e5f 6177 6172 656e      this._awaren
-000005f0: 6573 7320 3d20 6177 6172 656e 6573 733b  ess = awareness;
-00000600: 0a20 2020 2020 2020 2074 6869 732e 5f63  .        this._c
-00000610: 7572 7265 6e74 5573 6572 203d 2063 7572  urrentUser = cur
-00000620: 7265 6e74 5573 6572 3b0a 2020 2020 2020  rentUser;.      
-00000630: 2020 7468 6973 2e61 6464 436c 6173 7328    this.addClass(
-00000640: 434f 4c4c 4142 4f52 4154 4f52 535f 5041  COLLABORATORS_PA
-00000650: 4e45 4c5f 434c 4153 5329 3b0a 2020 2020  NEL_CLASS);.    
-00000660: 2020 2020 7468 6973 2e5f 626f 6479 203d      this._body =
-00000670: 206e 6577 2043 6f6c 6c61 626f 7261 746f   new Collaborato
-00000680: 7273 426f 6479 2866 696c 656f 7065 6e65  rsBody(fileopene
-00000690: 7229 3b0a 2020 2020 2020 2020 7468 6973  r);.        this
-000006a0: 2e61 6464 5769 6467 6574 2874 6869 732e  .addWidget(this.
-000006b0: 5f62 6f64 7929 3b0a 2020 2020 2020 2020  _body);.        
-000006c0: 7468 6973 2e75 7064 6174 6528 293b 0a20  this.update();. 
-000006d0: 2020 2020 2020 2074 6869 732e 5f61 7761         this._awa
-000006e0: 7265 6e65 7373 2e6f 6e28 2763 6861 6e67  reness.on('chang
-000006f0: 6527 2c20 7468 6973 2e5f 6f6e 4177 6172  e', this._onAwar
-00000700: 656e 6573 7343 6861 6e67 6564 293b 0a20  enessChanged);. 
-00000710: 2020 207d 0a7d 0a2f 2a2a 0a20 2a20 5468     }.}./**. * Th
-00000720: 6520 636f 6c6c 6162 6f72 6174 6f72 7320  e collaborators 
-00000730: 6c69 7374 2e0a 202a 2f0a 6578 706f 7274  list.. */.export
-00000740: 2063 6c61 7373 2043 6f6c 6c61 626f 7261   class Collabora
-00000750: 746f 7273 426f 6479 2065 7874 656e 6473  torsBody extends
-00000760: 2052 6561 6374 5769 6467 6574 207b 0a20   ReactWidget {. 
-00000770: 2020 2063 6f6e 7374 7275 6374 6f72 2866     constructor(f
-00000780: 696c 656f 7065 6e65 7229 207b 0a20 2020  ileopener) {.   
-00000790: 2020 2020 2073 7570 6572 2829 3b0a 2020       super();.  
-000007a0: 2020 2020 2020 7468 6973 2e5f 636f 6c6c        this._coll
-000007b0: 6162 6f72 6174 6f72 7320 3d20 5b5d 3b0a  aborators = [];.
-000007c0: 2020 2020 2020 2020 7468 6973 2e5f 6669          this._fi
-000007d0: 6c65 6f70 656e 6572 203d 2066 696c 656f  leopener = fileo
-000007e0: 7065 6e65 723b 0a20 2020 2020 2020 2074  pener;.        t
-000007f0: 6869 732e 6164 6443 6c61 7373 2843 4f4c  his.addClass(COL
-00000800: 4c41 424f 5241 544f 5253 5f4c 4953 545f  LABORATORS_LIST_
-00000810: 434c 4153 5329 3b0a 2020 2020 7d0a 2020  CLASS);.    }.  
-00000820: 2020 6765 7420 636f 6c6c 6162 6f72 6174    get collaborat
-00000830: 6f72 7328 2920 7b0a 2020 2020 2020 2020  ors() {.        
-00000840: 7265 7475 726e 2074 6869 732e 5f63 6f6c  return this._col
-00000850: 6c61 626f 7261 746f 7273 3b0a 2020 2020  laborators;.    
-00000860: 7d0a 2020 2020 7365 7420 636f 6c6c 6162  }.    set collab
-00000870: 6f72 6174 6f72 7328 7661 6c75 6529 207b  orators(value) {
-00000880: 0a20 2020 2020 2020 2074 6869 732e 5f63  .        this._c
-00000890: 6f6c 6c61 626f 7261 746f 7273 203d 2076  ollaborators = v
-000008a0: 616c 7565 3b0a 2020 2020 2020 2020 7468  alue;.        th
-000008b0: 6973 2e75 7064 6174 6528 293b 0a20 2020  is.update();.   
-000008c0: 207d 0a20 2020 2072 656e 6465 7228 2920   }.    render() 
-000008d0: 7b0a 2020 2020 2020 2020 7265 7475 726e  {.        return
-000008e0: 2074 6869 732e 5f63 6f6c 6c61 626f 7261   this._collabora
-000008f0: 746f 7273 2e6d 6170 2828 7661 6c75 652c  tors.map((value,
-00000900: 2069 2920 3d3e 207b 0a20 2020 2020 2020   i) => {.       
-00000910: 2020 2020 206c 6574 2063 616e 4f70 656e       let canOpen
-00000920: 4375 7272 656e 7420 3d20 6661 6c73 653b  Current = false;
-00000930: 0a20 2020 2020 2020 2020 2020 206c 6574  .            let
-00000940: 2063 7572 7265 6e74 203d 2027 273b 0a20   current = '';. 
-00000950: 2020 2020 2020 2020 2020 206c 6574 2073             let s
-00000960: 6570 6172 6174 6f72 203d 2027 273b 0a20  eparator = '';. 
-00000970: 2020 2020 2020 2020 2020 206c 6574 2063             let c
-00000980: 7572 7265 6e74 4669 6c65 4c6f 6361 7469  urrentFileLocati
-00000990: 6f6e 203d 2027 273b 0a20 2020 2020 2020  on = '';.       
-000009a0: 2020 2020 2069 6620 2876 616c 7565 2e63       if (value.c
-000009b0: 7572 7265 6e74 2920 7b0a 2020 2020 2020  urrent) {.      
-000009c0: 2020 2020 2020 2020 2020 6361 6e4f 7065            canOpe
-000009d0: 6e43 7572 7265 6e74 203d 2074 7275 653b  nCurrent = true;
-000009e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000009f0: 2063 6f6e 7374 2070 6174 6820 3d20 7661   const path = va
-00000a00: 6c75 652e 6375 7272 656e 742e 7370 6c69  lue.current.spli
-00000a10: 7428 273a 2729 3b0a 2020 2020 2020 2020  t(':');.        
-00000a20: 2020 2020 2020 2020 6375 7272 656e 7446          currentF
-00000a30: 696c 654c 6f63 6174 696f 6e20 3d20 6024  ileLocation = `$
-00000a40: 7b70 6174 685b 315d 7d3a 247b 7061 7468  {path[1]}:${path
-00000a50: 5b32 5d7d 603b 0a20 2020 2020 2020 2020  [2]}`;.         
-00000a60: 2020 2020 2020 2063 7572 7265 6e74 203d         current =
-00000a70: 2050 6174 6845 7874 2e62 6173 656e 616d   PathExt.basenam
-00000a80: 6528 7061 7468 5b32 5d29 3b0a 2020 2020  e(path[2]);.    
-00000a90: 2020 2020 2020 2020 2020 2020 6375 7272              curr
-00000aa0: 656e 7420 3d0a 2020 2020 2020 2020 2020  ent =.          
-00000ab0: 2020 2020 2020 2020 2020 6375 7272 656e            curren
-00000ac0: 742e 6c65 6e67 7468 203e 2032 3520 3f20  t.length > 25 ? 
-00000ad0: 6375 7272 656e 742e 736c 6963 6528 302c  current.slice(0,
-00000ae0: 2031 3229 2e63 6f6e 6361 7428 27e2 80a6   12).concat('...
-00000af0: 2729 203a 2063 7572 7265 6e74 3b0a 2020  ') : current;.  
-00000b00: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00000b10: 7061 7261 746f 7220 3d20 27e2 80a2 273b  parator = '...';
-00000b20: 0a20 2020 2020 2020 2020 2020 207d 0a20  .            }. 
-00000b30: 2020 2020 2020 2020 2020 2063 6f6e 7374             const
-00000b40: 206f 6e43 6c69 636b 203d 2028 2920 3d3e   onClick = () =>
-00000b50: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-00000b60: 2020 2069 6620 2863 616e 4f70 656e 4375     if (canOpenCu
-00000b70: 7272 656e 7429 207b 0a20 2020 2020 2020  rrent) {.       
-00000b80: 2020 2020 2020 2020 2020 2020 2074 6869               thi
-00000b90: 732e 5f66 696c 656f 7065 6e65 7228 6375  s._fileopener(cu
-00000ba0: 7272 656e 7446 696c 654c 6f63 6174 696f  rrentFileLocatio
-00000bb0: 6e29 3b0a 2020 2020 2020 2020 2020 2020  n);.            
-00000bc0: 2020 2020 7d0a 2020 2020 2020 2020 2020      }.          
-00000bd0: 2020 7d3b 0a20 2020 2020 2020 2020 2020    };.           
-00000be0: 2063 6f6e 7374 2064 6973 706c 6179 4e61   const displayNa
-00000bf0: 6d65 203d 2060 247b 7661 6c75 652e 7573  me = `${value.us
-00000c00: 6572 2e64 6973 706c 6179 5f6e 616d 657d  er.display_name}
-00000c10: 2024 7b73 6570 6172 6174 6f72 7d20 247b   ${separator} ${
-00000c20: 6375 7272 656e 747d 603b 0a20 2020 2020  current}`;.     
-00000c30: 2020 2020 2020 2072 6574 7572 6e20 2852         return (R
-00000c40: 6561 6374 2e63 7265 6174 6545 6c65 6d65  eact.createEleme
-00000c50: 6e74 2822 6469 7622 2c20 7b20 636c 6173  nt("div", { clas
-00000c60: 734e 616d 653a 2063 616e 4f70 656e 4375  sName: canOpenCu
-00000c70: 7272 656e 740a 2020 2020 2020 2020 2020  rrent.          
-00000c80: 2020 2020 2020 2020 2020 3f20 6024 7b43            ? `${C
-00000c90: 4c49 434b 4142 4c45 5f43 4f4c 4c41 424f  LICKABLE_COLLABO
-00000ca0: 5241 544f 525f 434c 4153 537d 2024 7b43  RATOR_CLASS} ${C
-00000cb0: 4f4c 4c41 424f 5241 544f 525f 434c 4153  OLLABORATOR_CLAS
-00000cc0: 537d 600a 2020 2020 2020 2020 2020 2020  S}`.            
-00000cd0: 2020 2020 2020 2020 3a20 434f 4c4c 4142          : COLLAB
-00000ce0: 4f52 4154 4f52 5f43 4c41 5353 2c20 6b65  ORATOR_CLASS, ke
-00000cf0: 793a 2069 2c20 6f6e 436c 6963 6b3a 206f  y: i, onClick: o
-00000d00: 6e43 6c69 636b 207d 2c0a 2020 2020 2020  nClick },.      
-00000d10: 2020 2020 2020 2020 2020 5265 6163 742e            React.
-00000d20: 6372 6561 7465 456c 656d 656e 7428 2264  createElement("d
-00000d30: 6976 222c 207b 2063 6c61 7373 4e61 6d65  iv", { className
-00000d40: 3a20 434f 4c4c 4142 4f52 4154 4f52 5f49  : COLLABORATOR_I
-00000d50: 434f 4e5f 434c 4153 532c 2073 7479 6c65  CON_CLASS, style
-00000d60: 3a20 7b20 6261 636b 6772 6f75 6e64 436f  : { backgroundCo
-00000d70: 6c6f 723a 2076 616c 7565 2e75 7365 722e  lor: value.user.
-00000d80: 636f 6c6f 7220 7d20 7d2c 0a20 2020 2020  color } },.     
-00000d90: 2020 2020 2020 2020 2020 2020 2020 2052                 R
-00000da0: 6561 6374 2e63 7265 6174 6545 6c65 6d65  eact.createEleme
-00000db0: 6e74 2822 7370 616e 222c 206e 756c 6c2c  nt("span", null,
-00000dc0: 2076 616c 7565 2e75 7365 722e 696e 6974   value.user.init
-00000dd0: 6961 6c73 2929 2c0a 2020 2020 2020 2020  ials)),.        
-00000de0: 2020 2020 2020 2020 5265 6163 742e 6372          React.cr
-00000df0: 6561 7465 456c 656d 656e 7428 2273 7061  eateElement("spa
-00000e00: 6e22 2c20 6e75 6c6c 2c20 6469 7370 6c61  n", null, displa
-00000e10: 794e 616d 6529 2929 3b0a 2020 2020 2020  yName)));.      
-00000e20: 2020 7d29 3b0a 2020 2020 7d0a 7d0a         });.    }.}.
+00000060: 6365 6e73 652e 0a0a 696d 706f 7274 202a  cense...import *
+00000070: 2061 7320 5265 6163 7420 6672 6f6d 2027   as React from '
+00000080: 7265 6163 7427 3b0a 0a69 6d70 6f72 7420  react';..import 
+00000090: 7b20 4177 6172 656e 6573 7320 7d20 6672  { Awareness } fr
+000000a0: 6f6d 2027 792d 7072 6f74 6f63 6f6c 732f  om 'y-protocols/
+000000b0: 6177 6172 656e 6573 7327 3b0a 0a69 6d70  awareness';..imp
+000000c0: 6f72 7420 7b20 5061 6e65 6c20 7d20 6672  ort { Panel } fr
+000000d0: 6f6d 2027 406c 756d 696e 6f2f 7769 6467  om '@lumino/widg
+000000e0: 6574 7327 3b0a 0a69 6d70 6f72 7420 7b20  ets';..import { 
+000000f0: 5265 6163 7457 6964 6765 7420 7d20 6672  ReactWidget } fr
+00000100: 6f6d 2027 406a 7570 7974 6572 6c61 622f  om '@jupyterlab/
+00000110: 6170 7075 7469 6c73 273b 0a0a 696d 706f  apputils';..impo
+00000120: 7274 207b 2055 7365 7220 7d20 6672 6f6d  rt { User } from
+00000130: 2027 406a 7570 7974 6572 6c61 622f 7365   '@jupyterlab/se
+00000140: 7276 6963 6573 273b 0a0a 696d 706f 7274  rvices';..import
+00000150: 207b 2050 6174 6845 7874 207d 2066 726f   { PathExt } fro
+00000160: 6d20 2740 6a75 7079 7465 726c 6162 2f63  m '@jupyterlab/c
+00000170: 6f72 6575 7469 6c73 273b 0a0a 696d 706f  oreutils';..impo
+00000180: 7274 207b 2049 436f 6c6c 6162 6f72 6174  rt { ICollaborat
+00000190: 6f72 4177 6172 656e 6573 7320 7d20 6672  orAwareness } fr
+000001a0: 6f6d 2027 2e2f 746f 6b65 6e73 273b 0a0a  om './tokens';..
+000001b0: 2f2a 2a0a 202a 2054 6865 2043 5353 2063  /**. * The CSS c
+000001c0: 6c61 7373 2061 6464 6564 2074 6f20 636f  lass added to co
+000001d0: 6c6c 6162 6f72 6174 6f72 7320 7061 6e65  llaborators pane
+000001e0: 6c2e 0a20 2a2f 0a63 6f6e 7374 2043 4f4c  l.. */.const COL
+000001f0: 4c41 424f 5241 544f 5253 5f50 414e 454c  LABORATORS_PANEL
+00000200: 5f43 4c41 5353 203d 2027 6a70 2d43 6f6c  _CLASS = 'jp-Col
+00000210: 6c61 626f 7261 746f 7273 5061 6e65 6c27  laboratorsPanel'
+00000220: 3b0a 0a2f 2a2a 0a20 2a20 5468 6520 4353  ;../**. * The CS
+00000230: 5320 636c 6173 7320 6164 6465 6420 746f  S class added to
+00000240: 2063 6f6c 6c61 626f 7261 746f 7273 206c   collaborators l
+00000250: 6973 7420 636f 6e74 6169 6e65 722e 0a20  ist container.. 
+00000260: 2a2f 0a63 6f6e 7374 2043 4f4c 4c41 424f  */.const COLLABO
+00000270: 5241 544f 5253 5f4c 4953 545f 434c 4153  RATORS_LIST_CLAS
+00000280: 5320 3d20 276a 702d 436f 6c6c 6162 6f72  S = 'jp-Collabor
+00000290: 6174 6f72 734c 6973 7427 3b0a 0a2f 2a2a  atorsList';../**
+000002a0: 0a20 2a20 5468 6520 4353 5320 636c 6173  . * The CSS clas
+000002b0: 7320 6164 6465 6420 746f 2065 6163 6820  s added to each 
+000002c0: 636f 6c6c 6162 6f72 6174 6f72 2065 6c65  collaborator ele
+000002d0: 6d65 6e74 2e0a 202a 2f0a 636f 6e73 7420  ment.. */.const 
+000002e0: 434f 4c4c 4142 4f52 4154 4f52 5f43 4c41  COLLABORATOR_CLA
+000002f0: 5353 203d 2027 6a70 2d43 6f6c 6c61 626f  SS = 'jp-Collabo
+00000300: 7261 746f 7227 3b0a 0a2f 2a2a 0a20 2a20  rator';../**. * 
+00000310: 5468 6520 4353 5320 636c 6173 7320 6164  The CSS class ad
+00000320: 6465 6420 746f 2065 6163 6820 636f 6c6c  ded to each coll
+00000330: 6162 6f72 6174 6f72 2065 6c65 6d65 6e74  aborator element
+00000340: 2e0a 202a 2f0a 636f 6e73 7420 434c 4943  .. */.const CLIC
+00000350: 4b41 424c 455f 434f 4c4c 4142 4f52 4154  KABLE_COLLABORAT
+00000360: 4f52 5f43 4c41 5353 203d 2027 6a70 2d43  OR_CLASS = 'jp-C
+00000370: 6c69 636b 6162 6c65 436f 6c6c 6162 6f72  lickableCollabor
+00000380: 6174 6f72 273b 0a0a 2f2a 2a0a 202a 2054  ator';../**. * T
+00000390: 6865 2043 5353 2063 6c61 7373 2061 6464  he CSS class add
+000003a0: 6564 2074 6f20 6561 6368 2063 6f6c 6c61  ed to each colla
+000003b0: 626f 7261 746f 7220 6963 6f6e 2e0a 202a  borator icon.. *
+000003c0: 2f0a 636f 6e73 7420 434f 4c4c 4142 4f52  /.const COLLABOR
+000003d0: 4154 4f52 5f49 434f 4e5f 434c 4153 5320  ATOR_ICON_CLASS 
+000003e0: 3d20 276a 702d 436f 6c6c 6162 6f72 6174  = 'jp-Collaborat
+000003f0: 6f72 4963 6f6e 273b 0a0a 6578 706f 7274  orIcon';..export
+00000400: 2063 6c61 7373 2043 6f6c 6c61 626f 7261   class Collabora
+00000410: 746f 7273 5061 6e65 6c20 6578 7465 6e64  torsPanel extend
+00000420: 7320 5061 6e65 6c20 7b0a 2020 7072 6976  s Panel {.  priv
+00000430: 6174 6520 5f63 7572 7265 6e74 5573 6572  ate _currentUser
+00000440: 3a20 5573 6572 2e49 4d61 6e61 6765 723b  : User.IManager;
+00000450: 0a20 2070 7269 7661 7465 205f 6177 6172  .  private _awar
+00000460: 656e 6573 733a 2041 7761 7265 6e65 7373  eness: Awareness
+00000470: 3b0a 2020 7072 6976 6174 6520 5f62 6f64  ;.  private _bod
+00000480: 793a 2043 6f6c 6c61 626f 7261 746f 7273  y: Collaborators
+00000490: 426f 6479 3b0a 0a20 2063 6f6e 7374 7275  Body;..  constru
+000004a0: 6374 6f72 280a 2020 2020 6375 7272 656e  ctor(.    curren
+000004b0: 7455 7365 723a 2055 7365 722e 494d 616e  tUser: User.IMan
+000004c0: 6167 6572 2c0a 2020 2020 6177 6172 656e  ager,.    awaren
+000004d0: 6573 733a 2041 7761 7265 6e65 7373 2c0a  ess: Awareness,.
+000004e0: 2020 2020 6669 6c65 6f70 656e 6572 3a20      fileopener: 
+000004f0: 2870 6174 683a 2073 7472 696e 6729 203d  (path: string) =
+00000500: 3e20 766f 6964 0a20 2029 207b 0a20 2020  > void.  ) {.   
+00000510: 2073 7570 6572 287b 7d29 3b0a 0a20 2020   super({});..   
+00000520: 2074 6869 732e 5f61 7761 7265 6e65 7373   this._awareness
+00000530: 203d 2061 7761 7265 6e65 7373 3b0a 0a20   = awareness;.. 
+00000540: 2020 2074 6869 732e 5f63 7572 7265 6e74     this._current
+00000550: 5573 6572 203d 2063 7572 7265 6e74 5573  User = currentUs
+00000560: 6572 3b0a 0a20 2020 2074 6869 732e 6164  er;..    this.ad
+00000570: 6443 6c61 7373 2843 4f4c 4c41 424f 5241  dClass(COLLABORA
+00000580: 544f 5253 5f50 414e 454c 5f43 4c41 5353  TORS_PANEL_CLASS
+00000590: 293b 0a0a 2020 2020 7468 6973 2e5f 626f  );..    this._bo
+000005a0: 6479 203d 206e 6577 2043 6f6c 6c61 626f  dy = new Collabo
+000005b0: 7261 746f 7273 426f 6479 2866 696c 656f  ratorsBody(fileo
+000005c0: 7065 6e65 7229 3b0a 2020 2020 7468 6973  pener);.    this
+000005d0: 2e61 6464 5769 6467 6574 2874 6869 732e  .addWidget(this.
+000005e0: 5f62 6f64 7929 3b0a 2020 2020 7468 6973  _body);.    this
+000005f0: 2e75 7064 6174 6528 293b 0a0a 2020 2020  .update();..    
+00000600: 7468 6973 2e5f 6177 6172 656e 6573 732e  this._awareness.
+00000610: 6f6e 2827 6368 616e 6765 272c 2074 6869  on('change', thi
+00000620: 732e 5f6f 6e41 7761 7265 6e65 7373 4368  s._onAwarenessCh
+00000630: 616e 6765 6429 3b0a 2020 7d0a 0a20 202f  anged);.  }..  /
+00000640: 2a2a 0a20 2020 2a20 4861 6e64 6c65 2063  **.   * Handle c
+00000650: 6f6c 6c61 626f 7261 746f 7220 6368 616e  ollaborator chan
+00000660: 6765 2e0a 2020 202a 2f0a 2020 7072 6976  ge..   */.  priv
+00000670: 6174 6520 5f6f 6e41 7761 7265 6e65 7373  ate _onAwareness
+00000680: 4368 616e 6765 6420 3d20 2829 203d 3e20  Changed = () => 
+00000690: 7b0a 2020 2020 636f 6e73 7420 7374 6174  {.    const stat
+000006a0: 6520 3d20 7468 6973 2e5f 6177 6172 656e  e = this._awaren
+000006b0: 6573 732e 6765 7453 7461 7465 7328 2920  ess.getStates() 
+000006c0: 6173 2061 6e79 3b0a 2020 2020 636f 6e73  as any;.    cons
+000006d0: 7420 636f 6c6c 6162 6f72 6174 6f72 733a  t collaborators:
+000006e0: 2049 436f 6c6c 6162 6f72 6174 6f72 4177   ICollaboratorAw
+000006f0: 6172 656e 6573 735b 5d20 3d20 5b5d 3b0a  areness[] = [];.
+00000700: 0a20 2020 2073 7461 7465 2e66 6f72 4561  .    state.forEa
+00000710: 6368 2828 7661 6c75 653a 2049 436f 6c6c  ch((value: IColl
+00000720: 6162 6f72 6174 6f72 4177 6172 656e 6573  aboratorAwarenes
+00000730: 732c 206b 6579 3a20 616e 7929 203d 3e20  s, key: any) => 
+00000740: 7b0a 2020 2020 2020 6966 2028 0a20 2020  {.      if (.   
+00000750: 2020 2020 2074 6869 732e 5f63 7572 7265       this._curre
+00000760: 6e74 5573 6572 2e69 7352 6561 6479 2026  ntUser.isReady &
+00000770: 260a 2020 2020 2020 2020 7661 6c75 652e  &.        value.
+00000780: 7573 6572 2e75 7365 726e 616d 6520 213d  user.username !=
+00000790: 3d20 7468 6973 2e5f 6375 7272 656e 7455  = this._currentU
+000007a0: 7365 722e 6964 656e 7469 7479 212e 7573  ser.identity!.us
+000007b0: 6572 6e61 6d65 0a20 2020 2020 2029 207b  ername.      ) {
+000007c0: 0a20 2020 2020 2020 2063 6f6c 6c61 626f  .        collabo
+000007d0: 7261 746f 7273 2e70 7573 6828 7661 6c75  rators.push(valu
+000007e0: 6529 3b0a 2020 2020 2020 7d0a 2020 2020  e);.      }.    
+000007f0: 7d29 3b0a 0a20 2020 2074 6869 732e 5f62  });..    this._b
+00000800: 6f64 792e 636f 6c6c 6162 6f72 6174 6f72  ody.collaborator
+00000810: 7320 3d20 636f 6c6c 6162 6f72 6174 6f72  s = collaborator
+00000820: 733b 0a20 207d 3b0a 7d0a 0a2f 2a2a 0a20  s;.  };.}../**. 
+00000830: 2a20 5468 6520 636f 6c6c 6162 6f72 6174  * The collaborat
+00000840: 6f72 7320 6c69 7374 2e0a 202a 2f0a 6578  ors list.. */.ex
+00000850: 706f 7274 2063 6c61 7373 2043 6f6c 6c61  port class Colla
+00000860: 626f 7261 746f 7273 426f 6479 2065 7874  boratorsBody ext
+00000870: 656e 6473 2052 6561 6374 5769 6467 6574  ends ReactWidget
+00000880: 207b 0a20 2070 7269 7661 7465 205f 636f   {.  private _co
+00000890: 6c6c 6162 6f72 6174 6f72 733a 2049 436f  llaborators: ICo
+000008a0: 6c6c 6162 6f72 6174 6f72 4177 6172 656e  llaboratorAwaren
+000008b0: 6573 735b 5d20 3d20 5b5d 3b0a 2020 7072  ess[] = [];.  pr
+000008c0: 6976 6174 6520 5f66 696c 656f 7065 6e65  ivate _fileopene
+000008d0: 723a 2028 7061 7468 3a20 7374 7269 6e67  r: (path: string
+000008e0: 2920 3d3e 2076 6f69 643b 0a0a 2020 636f  ) => void;..  co
+000008f0: 6e73 7472 7563 746f 7228 6669 6c65 6f70  nstructor(fileop
+00000900: 656e 6572 3a20 2870 6174 683a 2073 7472  ener: (path: str
+00000910: 696e 6729 203d 3e20 766f 6964 2920 7b0a  ing) => void) {.
+00000920: 2020 2020 7375 7065 7228 293b 0a20 2020      super();.   
+00000930: 2074 6869 732e 5f66 696c 656f 7065 6e65   this._fileopene
+00000940: 7220 3d20 6669 6c65 6f70 656e 6572 3b0a  r = fileopener;.
+00000950: 2020 2020 7468 6973 2e61 6464 436c 6173      this.addClas
+00000960: 7328 434f 4c4c 4142 4f52 4154 4f52 535f  s(COLLABORATORS_
+00000970: 4c49 5354 5f43 4c41 5353 293b 0a20 207d  LIST_CLASS);.  }
+00000980: 0a0a 2020 6765 7420 636f 6c6c 6162 6f72  ..  get collabor
+00000990: 6174 6f72 7328 293a 2049 436f 6c6c 6162  ators(): ICollab
+000009a0: 6f72 6174 6f72 4177 6172 656e 6573 735b  oratorAwareness[
+000009b0: 5d20 7b0a 2020 2020 7265 7475 726e 2074  ] {.    return t
+000009c0: 6869 732e 5f63 6f6c 6c61 626f 7261 746f  his._collaborato
+000009d0: 7273 3b0a 2020 7d0a 0a20 2073 6574 2063  rs;.  }..  set c
+000009e0: 6f6c 6c61 626f 7261 746f 7273 2876 616c  ollaborators(val
+000009f0: 7565 3a20 4943 6f6c 6c61 626f 7261 746f  ue: ICollaborato
+00000a00: 7241 7761 7265 6e65 7373 5b5d 2920 7b0a  rAwareness[]) {.
+00000a10: 2020 2020 7468 6973 2e5f 636f 6c6c 6162      this._collab
+00000a20: 6f72 6174 6f72 7320 3d20 7661 6c75 653b  orators = value;
+00000a30: 0a20 2020 2074 6869 732e 7570 6461 7465  .    this.update
+00000a40: 2829 3b0a 2020 7d0a 0a20 2072 656e 6465  ();.  }..  rende
+00000a50: 7228 293a 2052 6561 6374 2e52 6561 6374  r(): React.React
+00000a60: 456c 656d 656e 743c 616e 793e 5b5d 207b  Element<any>[] {
+00000a70: 0a20 2020 2072 6574 7572 6e20 7468 6973  .    return this
+00000a80: 2e5f 636f 6c6c 6162 6f72 6174 6f72 732e  ._collaborators.
+00000a90: 6d61 7028 2876 616c 7565 2c20 6929 203d  map((value, i) =
+00000aa0: 3e20 7b0a 2020 2020 2020 6c65 7420 6361  > {.      let ca
+00000ab0: 6e4f 7065 6e43 7572 7265 6e74 203d 2066  nOpenCurrent = f
+00000ac0: 616c 7365 3b0a 2020 2020 2020 6c65 7420  alse;.      let 
+00000ad0: 6375 7272 656e 7420 3d20 2727 3b0a 2020  current = '';.  
+00000ae0: 2020 2020 6c65 7420 7365 7061 7261 746f      let separato
+00000af0: 7220 3d20 2727 3b0a 2020 2020 2020 6c65  r = '';.      le
+00000b00: 7420 6375 7272 656e 7446 696c 654c 6f63  t currentFileLoc
+00000b10: 6174 696f 6e20 3d20 2727 3b0a 0a20 2020  ation = '';..   
+00000b20: 2020 2069 6620 2876 616c 7565 2e63 7572     if (value.cur
+00000b30: 7265 6e74 2920 7b0a 2020 2020 2020 2020  rent) {.        
+00000b40: 6361 6e4f 7065 6e43 7572 7265 6e74 203d  canOpenCurrent =
+00000b50: 2074 7275 653b 0a20 2020 2020 2020 2063   true;.        c
+00000b60: 6f6e 7374 2070 6174 6820 3d20 7661 6c75  onst path = valu
+00000b70: 652e 6375 7272 656e 742e 7370 6c69 7428  e.current.split(
+00000b80: 273a 2729 3b0a 2020 2020 2020 2020 6375  ':');.        cu
+00000b90: 7272 656e 7446 696c 654c 6f63 6174 696f  rrentFileLocatio
+00000ba0: 6e20 3d20 6024 7b70 6174 685b 315d 7d3a  n = `${path[1]}:
+00000bb0: 247b 7061 7468 5b32 5d7d 603b 0a0a 2020  ${path[2]}`;..  
+00000bc0: 2020 2020 2020 6375 7272 656e 7420 3d20        current = 
+00000bd0: 5061 7468 4578 742e 6261 7365 6e61 6d65  PathExt.basename
+00000be0: 2870 6174 685b 325d 293b 0a20 2020 2020  (path[2]);.     
+00000bf0: 2020 2063 7572 7265 6e74 203d 0a20 2020     current =.   
+00000c00: 2020 2020 2020 2063 7572 7265 6e74 2e6c         current.l
+00000c10: 656e 6774 6820 3e20 3235 203f 2063 7572  ength > 25 ? cur
+00000c20: 7265 6e74 2e73 6c69 6365 2830 2c20 3132  rent.slice(0, 12
+00000c30: 292e 636f 6e63 6174 2827 e280 a627 2920  ).concat('...') 
+00000c40: 3a20 6375 7272 656e 743b 0a20 2020 2020  : current;.     
+00000c50: 2020 2073 6570 6172 6174 6f72 203d 2027     separator = '
+00000c60: e280 a227 3b0a 2020 2020 2020 7d0a 0a20  ...';.      }.. 
+00000c70: 2020 2020 2063 6f6e 7374 206f 6e43 6c69       const onCli
+00000c80: 636b 203d 2028 2920 3d3e 207b 0a20 2020  ck = () => {.   
+00000c90: 2020 2020 2069 6620 2863 616e 4f70 656e       if (canOpen
+00000ca0: 4375 7272 656e 7429 207b 0a20 2020 2020  Current) {.     
+00000cb0: 2020 2020 2074 6869 732e 5f66 696c 656f       this._fileo
+00000cc0: 7065 6e65 7228 6375 7272 656e 7446 696c  pener(currentFil
+00000cd0: 654c 6f63 6174 696f 6e29 3b0a 2020 2020  eLocation);.    
+00000ce0: 2020 2020 7d0a 2020 2020 2020 7d3b 0a0a      }.      };..
+00000cf0: 2020 2020 2020 636f 6e73 7420 6469 7370        const disp
+00000d00: 6c61 794e 616d 6520 3d20 6024 7b76 616c  layName = `${val
+00000d10: 7565 2e75 7365 722e 6469 7370 6c61 795f  ue.user.display_
+00000d20: 6e61 6d65 7d20 247b 7365 7061 7261 746f  name} ${separato
+00000d30: 727d 2024 7b63 7572 7265 6e74 7d60 3b0a  r} ${current}`;.
+00000d40: 0a20 2020 2020 2072 6574 7572 6e20 280a  .      return (.
+00000d50: 2020 2020 2020 2020 3c64 6976 0a20 2020          <div.   
+00000d60: 2020 2020 2020 2063 6c61 7373 4e61 6d65         className
+00000d70: 3d7b 0a20 2020 2020 2020 2020 2020 2063  ={.            c
+00000d80: 616e 4f70 656e 4375 7272 656e 740a 2020  anOpenCurrent.  
+00000d90: 2020 2020 2020 2020 2020 2020 3f20 6024              ? `$
+00000da0: 7b43 4c49 434b 4142 4c45 5f43 4f4c 4c41  {CLICKABLE_COLLA
+00000db0: 424f 5241 544f 525f 434c 4153 537d 2024  BORATOR_CLASS} $
+00000dc0: 7b43 4f4c 4c41 424f 5241 544f 525f 434c  {COLLABORATOR_CL
+00000dd0: 4153 537d 600a 2020 2020 2020 2020 2020  ASS}`.          
+00000de0: 2020 2020 3a20 434f 4c4c 4142 4f52 4154      : COLLABORAT
+00000df0: 4f52 5f43 4c41 5353 0a20 2020 2020 2020  OR_CLASS.       
+00000e00: 2020 207d 0a20 2020 2020 2020 2020 206b     }.          k
+00000e10: 6579 3d7b 697d 0a20 2020 2020 2020 2020  ey={i}.         
+00000e20: 206f 6e43 6c69 636b 3d7b 6f6e 436c 6963   onClick={onClic
+00000e30: 6b7d 0a20 2020 2020 2020 203e 0a20 2020  k}.        >.   
+00000e40: 2020 2020 2020 203c 6469 760a 2020 2020         <div.    
+00000e50: 2020 2020 2020 2020 636c 6173 734e 616d          classNam
+00000e60: 653d 7b43 4f4c 4c41 424f 5241 544f 525f  e={COLLABORATOR_
+00000e70: 4943 4f4e 5f43 4c41 5353 7d0a 2020 2020  ICON_CLASS}.    
+00000e80: 2020 2020 2020 2020 7374 796c 653d 7b7b          style={{
+00000e90: 2062 6163 6b67 726f 756e 6443 6f6c 6f72   backgroundColor
+00000ea0: 3a20 7661 6c75 652e 7573 6572 2e63 6f6c  : value.user.col
+00000eb0: 6f72 207d 7d0a 2020 2020 2020 2020 2020  or }}.          
+00000ec0: 3e0a 2020 2020 2020 2020 2020 2020 3c73  >.            <s
+00000ed0: 7061 6e3e 7b76 616c 7565 2e75 7365 722e  pan>{value.user.
+00000ee0: 696e 6974 6961 6c73 7d3c 2f73 7061 6e3e  initials}</span>
+00000ef0: 0a20 2020 2020 2020 2020 203c 2f64 6976  .          </div
+00000f00: 3e0a 2020 2020 2020 2020 2020 3c73 7061  >.          <spa
+00000f10: 6e3e 7b64 6973 706c 6179 4e61 6d65 7d3c  n>{displayName}<
+00000f20: 2f73 7061 6e3e 0a20 2020 2020 2020 203c  /span>.        <
+00000f30: 2f64 6976 3e0a 2020 2020 2020 293b 0a20  /div>.      );. 
+00000f40: 2020 207d 293b 0a20 207d 0a7d 0a            });.  }.}.
```

### Comparing `jupyter_collaboration_ui-1.0.0a0/packages/collaboration/lib/cursors.js` & `jupyter_collaboration_ui-1.0.0a1/packages/collaboration/src/cursors.ts`

 * *Files 18% similar despite different names*

```diff
@@ -1,738 +1,739 @@
 00000000: 2f2f 2043 6f70 7972 6967 6874 2028 6329  // Copyright (c)
 00000010: 204a 7570 7974 6572 2044 6576 656c 6f70   Jupyter Develop
 00000020: 6d65 6e74 2054 6561 6d2e 0a2f 2f20 4469  ment Team..// Di
 00000030: 7374 7269 6275 7465 6420 756e 6465 7220  stributed under 
 00000040: 7468 6520 7465 726d 7320 6f66 2074 6865  the terms of the
 00000050: 204d 6f64 6966 6965 6420 4253 4420 4c69   Modified BSD Li
-00000060: 6365 6e73 652e 0a69 6d70 6f72 7420 7b20  cense..import { 
-00000070: 416e 6e6f 7461 7469 6f6e 2c20 4564 6974  Annotation, Edit
-00000080: 6f72 5365 6c65 6374 696f 6e2c 2046 6163  orSelection, Fac
-00000090: 6574 207d 2066 726f 6d20 2740 636f 6465  et } from '@code
-000000a0: 6d69 7272 6f72 2f73 7461 7465 273b 0a69  mirror/state';.i
-000000b0: 6d70 6f72 7420 7b20 4564 6974 6f72 5669  mport { EditorVi
-000000c0: 6577 2c20 686f 7665 7254 6f6f 6c74 6970  ew, hoverTooltip
-000000d0: 2c20 6c61 7965 722c 2052 6563 7461 6e67  , layer, Rectang
-000000e0: 6c65 4d61 726b 6572 2c20 746f 6f6c 7469  leMarker, toolti
-000000f0: 7073 2c20 5669 6577 506c 7567 696e 207d  ps, ViewPlugin }
-00000100: 2066 726f 6d20 2740 636f 6465 6d69 7272   from '@codemirr
-00000110: 6f72 2f76 6965 7727 3b0a 696d 706f 7274  or/view';.import
-00000120: 207b 204a 534f 4e45 7874 207d 2066 726f   { JSONExt } fro
-00000130: 6d20 2740 6c75 6d69 6e6f 2f63 6f72 6575  m '@lumino/coreu
-00000140: 7469 6c73 273b 0a69 6d70 6f72 7420 7b20  tils';.import { 
-00000150: 6372 6561 7465 4162 736f 6c75 7465 506f  createAbsolutePo
-00000160: 7369 7469 6f6e 4672 6f6d 5265 6c61 7469  sitionFromRelati
-00000170: 7665 506f 7369 7469 6f6e 2c20 6372 6561  vePosition, crea
-00000180: 7465 5265 6c61 7469 7665 506f 7369 7469  teRelativePositi
-00000190: 6f6e 4672 6f6d 4a53 4f4e 2c20 6372 6561  onFromJSON, crea
-000001a0: 7465 5265 6c61 7469 7665 506f 7369 7469  teRelativePositi
-000001b0: 6f6e 4672 6f6d 5479 7065 496e 6465 7820  onFromTypeIndex 
-000001c0: 7d20 6672 6f6d 2027 796a 7327 3b0a 2f2a  } from 'yjs';./*
-000001d0: 2a0a 202a 2046 6163 6574 2073 746f 7269  *. * Facet stori
-000001e0: 6e67 2074 6865 2059 6a73 2064 6f63 756d  ng the Yjs docum
-000001f0: 656e 7420 6f62 6a65 6374 730a 202a 2f0a  ent objects. */.
-00000200: 636f 6e73 7420 6564 6974 6f72 4177 6172  const editorAwar
-00000210: 656e 6573 7346 6163 6574 203d 2046 6163  enessFacet = Fac
-00000220: 6574 2e64 6566 696e 6528 7b0a 2020 2020  et.define({.    
-00000230: 636f 6d62 696e 6528 636f 6e66 6967 7329  combine(configs)
-00000240: 207b 0a20 2020 2020 2020 2072 6574 7572   {.        retur
-00000250: 6e20 636f 6e66 6967 735b 636f 6e66 6967  n configs[config
-00000260: 732e 6c65 6e67 7468 202d 2031 5d3b 0a20  s.length - 1];. 
-00000270: 2020 207d 0a7d 293b 0a2f 2a2a 0a20 2a20     }.});./**. * 
-00000280: 5265 6d6f 7465 2073 656c 6563 7469 6f6e  Remote selection
-00000290: 2074 6865 6d65 0a20 2a2f 0a63 6f6e 7374   theme. */.const
-000002a0: 2072 656d 6f74 6553 656c 6563 7469 6f6e   remoteSelection
-000002b0: 5468 656d 6520 3d20 4564 6974 6f72 5669  Theme = EditorVi
-000002c0: 6577 2e62 6173 6554 6865 6d65 287b 0a20  ew.baseTheme({. 
-000002d0: 2020 2027 2e6a 702d 7265 6d6f 7465 2d63     '.jp-remote-c
-000002e0: 7572 736f 7227 3a20 7b0a 2020 2020 2020  ursor': {.      
-000002f0: 2020 626f 7264 6572 4c65 6674 3a20 2731    borderLeft: '1
-00000300: 7078 2073 6f6c 6964 2062 6c61 636b 272c  px solid black',
-00000310: 0a20 2020 2020 2020 206d 6172 6769 6e4c  .        marginL
-00000320: 6566 743a 2027 2d31 7078 270a 2020 2020  eft: '-1px'.    
-00000330: 7d2c 0a20 2020 2027 2e6a 702d 7265 6d6f  },.    '.jp-remo
-00000340: 7465 2d63 7572 736f 722e 6a70 2d6d 6f64  te-cursor.jp-mod
-00000350: 2d70 7269 6d61 7279 273a 207b 0a20 2020  -primary': {.   
-00000360: 2020 2020 2062 6f72 6465 724c 6566 7457       borderLeftW
-00000370: 6964 7468 3a20 2732 7078 270a 2020 2020  idth: '2px'.    
-00000380: 7d2c 0a20 2020 2027 2e6a 702d 7265 6d6f  },.    '.jp-remo
-00000390: 7465 2d73 656c 6563 7469 6f6e 273a 207b  te-selection': {
-000003a0: 0a20 2020 2020 2020 206f 7061 6369 7479  .        opacity
-000003b0: 3a20 302e 350a 2020 2020 7d2c 0a20 2020  : 0.5.    },.   
-000003c0: 2027 2e63 6d2d 746f 6f6c 7469 7027 3a20   '.cm-tooltip': 
-000003d0: 7b0a 2020 2020 2020 2020 626f 7264 6572  {.        border
-000003e0: 3a20 276e 6f6e 6527 0a20 2020 207d 2c0a  : 'none'.    },.
-000003f0: 2020 2020 272e 636d 2d74 6f6f 6c74 6970      '.cm-tooltip
-00000400: 202e 6a70 2d72 656d 6f74 652d 7573 6572   .jp-remote-user
-00000410: 496e 666f 273a 207b 0a20 2020 2020 2020  Info': {.       
-00000420: 2063 6f6c 6f72 3a20 2776 6172 282d 2d6a   color: 'var(--j
-00000430: 702d 7569 2d69 6e76 6572 7365 2d66 6f6e  p-ui-inverse-fon
-00000440: 742d 636f 6c6f 7230 2927 2c0a 2020 2020  t-color0)',.    
-00000450: 2020 2020 7061 6464 696e 673a 2027 3070      padding: '0p
-00000460: 7820 3270 7827 0a20 2020 207d 0a7d 293b  x 2px'.    }.});
-00000470: 0a2f 2f20 544f 444f 2066 6978 2077 6869  .// TODO fix whi
-00000480: 6368 2075 7365 7220 6e65 6564 7320 7570  ch user needs up
-00000490: 6461 7465 0a63 6f6e 7374 2072 656d 6f74  date.const remot
-000004a0: 6553 656c 6563 7469 6f6e 7341 6e6e 6f74  eSelectionsAnnot
-000004b0: 6174 696f 6e20 3d20 416e 6e6f 7461 7469  ation = Annotati
-000004c0: 6f6e 2e64 6566 696e 6528 293b 0a2f 2a2a  on.define();./**
-000004d0: 0a20 2a20 5772 6170 7065 7220 6172 6f75  . * Wrapper arou
-000004e0: 6e64 2052 6563 7461 6e67 6c65 4d61 726b  nd RectangleMark
-000004f0: 6572 2074 6f20 6265 2061 626c 6520 746f  er to be able to
-00000500: 2073 6574 2074 6865 2075 7365 7220 636f   set the user co
-00000510: 6c6f 7220 666f 7220 7468 6520 7265 6d6f  lor for the remo
-00000520: 7465 2063 7572 736f 7220 616e 6420 7365  te cursor and se
-00000530: 6c65 6374 696f 6e20 7261 6e67 6573 2e0a  lection ranges..
-00000540: 202a 2f0a 636c 6173 7320 5265 6d6f 7465   */.class Remote
-00000550: 4d61 726b 6572 207b 0a20 2020 202f 2a2a  Marker {.    /**
-00000560: 0a20 2020 2020 2a20 436f 6e73 7472 7563  .     * Construc
-00000570: 746f 720a 2020 2020 202a 0a20 2020 2020  tor.     *.     
-00000580: 2a20 4070 6172 616d 2073 7479 6c65 2053  * @param style S
-00000590: 7065 6369 6669 6320 7573 6572 2073 7479  pecific user sty
-000005a0: 6c65 2074 6f20 6265 2061 7070 6c69 6564  le to be applied
-000005b0: 206f 6e20 7468 6520 6d61 726b 6572 2065   on the marker e
-000005c0: 6c65 6d65 6e74 0a20 2020 2020 2a20 4070  lement.     * @p
-000005d0: 6172 616d 206d 6172 6b65 7220 7b40 6c69  aram marker {@li
-000005e0: 6e6b 2052 6563 7461 6e67 6c65 4d61 726b  nk RectangleMark
-000005f0: 6572 7d20 746f 2077 7261 700a 2020 2020  er} to wrap.    
-00000600: 202a 2f0a 2020 2020 636f 6e73 7472 7563   */.    construc
-00000610: 746f 7228 7374 796c 652c 206d 6172 6b65  tor(style, marke
-00000620: 7229 207b 0a20 2020 2020 2020 2074 6869  r) {.        thi
-00000630: 732e 7374 796c 6520 3d20 7374 796c 653b  s.style = style;
-00000640: 0a20 2020 2020 2020 2074 6869 732e 6d61  .        this.ma
-00000650: 726b 6572 203d 206d 6172 6b65 723b 0a20  rker = marker;. 
-00000660: 2020 207d 0a20 2020 2064 7261 7728 2920     }.    draw() 
-00000670: 7b0a 2020 2020 2020 2020 636f 6e73 7420  {.        const 
-00000680: 656c 7420 3d20 7468 6973 2e6d 6172 6b65  elt = this.marke
-00000690: 722e 6472 6177 2829 3b0a 2020 2020 2020  r.draw();.      
-000006a0: 2020 666f 7220 2863 6f6e 7374 205b 6b65    for (const [ke
-000006b0: 792c 2076 616c 7565 5d20 6f66 204f 626a  y, value] of Obj
-000006c0: 6563 742e 656e 7472 6965 7328 7468 6973  ect.entries(this
-000006d0: 2e73 7479 6c65 2929 207b 0a20 2020 2020  .style)) {.     
-000006e0: 2020 2020 2020 202f 2f20 4074 732d 6578         // @ts-ex
-000006f0: 7065 6374 2d65 7272 6f72 2055 6e6b 6e6f  pect-error Unkno
-00000700: 776e 206b 6579 0a20 2020 2020 2020 2020  wn key.         
-00000710: 2020 2065 6c74 2e73 7479 6c65 5b6b 6579     elt.style[key
-00000720: 5d20 3d20 7661 6c75 653b 0a20 2020 2020  ] = value;.     
-00000730: 2020 207d 0a20 2020 2020 2020 2072 6574     }.        ret
-00000740: 7572 6e20 656c 743b 0a20 2020 207d 0a20  urn elt;.    }. 
-00000750: 2020 2065 7128 6f74 6865 7229 207b 0a20     eq(other) {. 
-00000760: 2020 2020 2020 2072 6574 7572 6e20 2874         return (t
-00000770: 6869 732e 6d61 726b 6572 2e65 7128 6f74  his.marker.eq(ot
-00000780: 6865 722e 6d61 726b 6572 2920 2626 204a  her.marker) && J
-00000790: 534f 4e45 7874 2e64 6565 7045 7175 616c  SONExt.deepEqual
-000007a0: 2874 6869 732e 7374 796c 652c 206f 7468  (this.style, oth
-000007b0: 6572 2e73 7479 6c65 2929 3b0a 2020 2020  er.style));.    
-000007c0: 7d0a 2020 2020 7570 6461 7465 2864 6f6d  }.    update(dom
-000007d0: 2c20 6f6c 644d 6172 6b65 7229 207b 0a20  , oldMarker) {. 
-000007e0: 2020 2020 2020 2066 6f72 2028 636f 6e73         for (cons
-000007f0: 7420 5b6b 6579 2c20 7661 6c75 655d 206f  t [key, value] o
-00000800: 6620 4f62 6a65 6374 2e65 6e74 7269 6573  f Object.entries
-00000810: 2874 6869 732e 7374 796c 6529 2920 7b0a  (this.style)) {.
-00000820: 2020 2020 2020 2020 2020 2020 2f2f 2040              // @
-00000830: 7473 2d65 7870 6563 742d 6572 726f 7220  ts-expect-error 
-00000840: 556e 6b6e 6f77 6e20 6b65 790a 2020 2020  Unknown key.    
-00000850: 2020 2020 2020 2020 646f 6d2e 7374 796c          dom.styl
-00000860: 655b 6b65 795d 203d 2076 616c 7565 3b0a  e[key] = value;.
-00000870: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-00000880: 2020 7265 7475 726e 2074 6869 732e 6d61    return this.ma
-00000890: 726b 6572 2e75 7064 6174 6528 646f 6d2c  rker.update(dom,
-000008a0: 206f 6c64 4d61 726b 6572 2e6d 6172 6b65   oldMarker.marke
-000008b0: 7229 3b0a 2020 2020 7d0a 7d0a 2f2a 2a0a  r);.    }.}./**.
-000008c0: 202a 2045 7874 656e 7369 6f6e 2064 6566   * Extension def
-000008d0: 696e 696e 6720 6120 6e65 7720 6564 6974  ining a new edit
-000008e0: 6f72 206c 6179 6572 2073 746f 7269 6e67  or layer storing
-000008f0: 2074 6865 2072 656d 6f74 6520 7573 6572   the remote user
-00000900: 2063 7572 736f 7273 0a20 2a2f 0a63 6f6e   cursors. */.con
-00000910: 7374 2072 656d 6f74 6543 7572 736f 7273  st remoteCursors
-00000920: 4c61 7965 7220 3d20 6c61 7965 7228 7b0a  Layer = layer({.
-00000930: 2020 2020 6162 6f76 653a 2074 7275 652c      above: true,
-00000940: 0a20 2020 206d 6172 6b65 7273 2876 6965  .    markers(vie
-00000950: 7729 207b 0a20 2020 2020 2020 2063 6f6e  w) {.        con
-00000960: 7374 207b 2061 7761 7265 6e65 7373 2c20  st { awareness, 
-00000970: 7974 6578 7420 7d20 3d20 7669 6577 2e73  ytext } = view.s
-00000980: 7461 7465 2e66 6163 6574 2865 6469 746f  tate.facet(edito
-00000990: 7241 7761 7265 6e65 7373 4661 6365 7429  rAwarenessFacet)
-000009a0: 3b0a 2020 2020 2020 2020 636f 6e73 7420  ;.        const 
-000009b0: 7964 6f63 203d 2079 7465 7874 2e64 6f63  ydoc = ytext.doc
-000009c0: 3b0a 2020 2020 2020 2020 636f 6e73 7420  ;.        const 
-000009d0: 6375 7273 6f72 7320 3d20 5b5d 3b0a 2020  cursors = [];.  
-000009e0: 2020 2020 2020 6177 6172 656e 6573 732e        awareness.
-000009f0: 6765 7453 7461 7465 7328 292e 666f 7245  getStates().forE
-00000a00: 6163 6828 2873 7461 7465 2c20 636c 6965  ach((state, clie
-00000a10: 6e74 4944 2920 3d3e 207b 0a20 2020 2020  ntID) => {.     
-00000a20: 2020 2020 2020 2076 6172 205f 612c 205f         var _a, _
-00000a30: 622c 205f 633b 0a20 2020 2020 2020 2020  b, _c;.         
-00000a40: 2020 2069 6620 2863 6c69 656e 7449 4420     if (clientID 
-00000a50: 3d3d 3d20 6177 6172 656e 6573 732e 646f  === awareness.do
-00000a60: 632e 636c 6965 6e74 4944 2920 7b0a 2020  c.clientID) {.  
-00000a70: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00000a80: 7475 726e 3b0a 2020 2020 2020 2020 2020  turn;.          
-00000a90: 2020 7d0a 2020 2020 2020 2020 2020 2020    }.            
-00000aa0: 636f 6e73 7420 6375 7273 6f72 735f 203d  const cursors_ =
-00000ab0: 2073 7461 7465 2e63 7572 736f 7273 3b0a   state.cursors;.
-00000ac0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00000ad0: 2863 6f6e 7374 2063 7572 736f 7220 6f66  (const cursor of
-00000ae0: 2063 7572 736f 7273 5f20 213d 3d20 6e75   cursors_ !== nu
-00000af0: 6c6c 2026 2620 6375 7273 6f72 735f 2021  ll && cursors_ !
-00000b00: 3d3d 2076 6f69 6420 3020 3f20 6375 7273  == void 0 ? curs
-00000b10: 6f72 735f 203a 205b 5d29 207b 0a20 2020  ors_ : []) {.   
-00000b20: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00000b30: 2821 2863 7572 736f 7220 3d3d 3d20 6e75  (!(cursor === nu
-00000b40: 6c6c 207c 7c20 6375 7273 6f72 203d 3d3d  ll || cursor ===
-00000b50: 2076 6f69 6420 3020 3f20 766f 6964 2030   void 0 ? void 0
-00000b60: 203a 2063 7572 736f 722e 616e 6368 6f72   : cursor.anchor
-00000b70: 2920 7c7c 2021 2863 7572 736f 7220 3d3d  ) || !(cursor ==
-00000b80: 3d20 6e75 6c6c 207c 7c20 6375 7273 6f72  = null || cursor
-00000b90: 203d 3d3d 2076 6f69 6420 3020 3f20 766f   === void 0 ? vo
-00000ba0: 6964 2030 203a 2063 7572 736f 722e 6865  id 0 : cursor.he
-00000bb0: 6164 2929 207b 0a20 2020 2020 2020 2020  ad)) {.         
-00000bc0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00000bd0: 6e3b 0a20 2020 2020 2020 2020 2020 2020  n;.             
-00000be0: 2020 207d 0a20 2020 2020 2020 2020 2020     }.           
-00000bf0: 2020 2020 2063 6f6e 7374 2061 6e63 686f       const ancho
-00000c00: 7220 3d20 6372 6561 7465 4162 736f 6c75  r = createAbsolu
-00000c10: 7465 506f 7369 7469 6f6e 4672 6f6d 5265  tePositionFromRe
-00000c20: 6c61 7469 7665 506f 7369 7469 6f6e 2863  lativePosition(c
-00000c30: 7572 736f 722e 616e 6368 6f72 2c20 7964  ursor.anchor, yd
-00000c40: 6f63 293b 0a20 2020 2020 2020 2020 2020  oc);.           
-00000c50: 2020 2020 2063 6f6e 7374 2068 6561 6420       const head 
-00000c60: 3d20 6372 6561 7465 4162 736f 6c75 7465  = createAbsolute
-00000c70: 506f 7369 7469 6f6e 4672 6f6d 5265 6c61  PositionFromRela
-00000c80: 7469 7665 506f 7369 7469 6f6e 2863 7572  tivePosition(cur
-00000c90: 736f 722e 6865 6164 2c20 7964 6f63 293b  sor.head, ydoc);
-00000ca0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000cb0: 2069 6620 2828 616e 6368 6f72 203d 3d3d   if ((anchor ===
-00000cc0: 206e 756c 6c20 7c7c 2061 6e63 686f 7220   null || anchor 
-00000cd0: 3d3d 3d20 766f 6964 2030 203f 2076 6f69  === void 0 ? voi
-00000ce0: 6420 3020 3a20 616e 6368 6f72 2e74 7970  d 0 : anchor.typ
-00000cf0: 6529 2021 3d3d 2079 7465 7874 207c 7c20  e) !== ytext || 
-00000d00: 2868 6561 6420 3d3d 3d20 6e75 6c6c 207c  (head === null |
-00000d10: 7c20 6865 6164 203d 3d3d 2076 6f69 6420  | head === void 
-00000d20: 3020 3f20 766f 6964 2030 203a 2068 6561  0 ? void 0 : hea
-00000d30: 642e 7479 7065 2920 213d 3d20 7974 6578  d.type) !== ytex
-00000d40: 7429 207b 0a20 2020 2020 2020 2020 2020  t) {.           
-00000d50: 2020 2020 2020 2020 2072 6574 7572 6e3b           return;
-00000d60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000d70: 207d 0a20 2020 2020 2020 2020 2020 2020   }.             
-00000d80: 2020 2063 6f6e 7374 2063 6c61 7373 4e61     const classNa
-00000d90: 6d65 203d 2028 285f 6120 3d20 6375 7273  me = ((_a = curs
-00000da0: 6f72 2e70 7269 6d61 7279 2920 213d 3d20  or.primary) !== 
-00000db0: 6e75 6c6c 2026 2620 5f61 2021 3d3d 2076  null && _a !== v
-00000dc0: 6f69 6420 3020 3f20 5f61 203a 2074 7275  oid 0 ? _a : tru
-00000dd0: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
-00000de0: 2020 2020 2020 203f 2027 6a70 2d72 656d         ? 'jp-rem
-00000df0: 6f74 652d 6375 7273 6f72 206a 702d 6d6f  ote-cursor jp-mo
-00000e00: 642d 7072 696d 6172 7927 0a20 2020 2020  d-primary'.     
-00000e10: 2020 2020 2020 2020 2020 2020 2020 203a                 :
-00000e20: 2027 6a70 2d72 656d 6f74 652d 6375 7273   'jp-remote-curs
-00000e30: 6f72 273b 0a20 2020 2020 2020 2020 2020  or';.           
-00000e40: 2020 2020 2063 6f6e 7374 2063 7572 736f       const curso
-00000e50: 725f 203d 2045 6469 746f 7253 656c 6563  r_ = EditorSelec
-00000e60: 7469 6f6e 2e63 7572 736f 7228 6865 6164  tion.cursor(head
-00000e70: 2e69 6e64 6578 2c20 6865 6164 2e69 6e64  .index, head.ind
-00000e80: 6578 203e 2061 6e63 686f 722e 696e 6465  ex > anchor.inde
-00000e90: 7820 3f20 2d31 203a 2031 293b 0a20 2020  x ? -1 : 1);.   
-00000ea0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-00000eb0: 2028 636f 6e73 7420 7069 6563 6520 6f66   (const piece of
-00000ec0: 2052 6563 7461 6e67 6c65 4d61 726b 6572   RectangleMarker
-00000ed0: 2e66 6f72 5261 6e67 6528 7669 6577 2c20  .forRange(view, 
-00000ee0: 636c 6173 734e 616d 652c 2063 7572 736f  className, curso
-00000ef0: 725f 2929 207b 0a20 2020 2020 2020 2020  r_)) {.         
-00000f00: 2020 2020 2020 2020 2020 202f 2f20 5772             // Wr
-00000f10: 6170 2074 6865 2072 6563 7461 6e67 6c65  ap the rectangle
-00000f20: 206d 6172 6b65 7220 746f 2073 6574 2074   marker to set t
-00000f30: 6865 2075 7365 7220 636f 6c6f 720a 2020  he user color.  
-00000f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f50: 2020 6375 7273 6f72 732e 7075 7368 286e    cursors.push(n
-00000f60: 6577 2052 656d 6f74 654d 6172 6b65 7228  ew RemoteMarker(
-00000f70: 7b20 626f 7264 6572 4c65 6674 436f 6c6f  { borderLeftColo
-00000f80: 723a 2028 5f63 203d 2028 5f62 203d 2073  r: (_c = (_b = s
-00000f90: 7461 7465 2e75 7365 7229 203d 3d3d 206e  tate.user) === n
-00000fa0: 756c 6c20 7c7c 205f 6220 3d3d 3d20 766f  ull || _b === vo
-00000fb0: 6964 2030 203f 2076 6f69 6420 3020 3a20  id 0 ? void 0 : 
-00000fc0: 5f62 2e63 6f6c 6f72 2920 213d 3d20 6e75  _b.color) !== nu
-00000fd0: 6c6c 2026 2620 5f63 2021 3d3d 2076 6f69  ll && _c !== voi
-00000fe0: 6420 3020 3f20 5f63 203a 2027 626c 6163  d 0 ? _c : 'blac
-00000ff0: 6b27 207d 2c20 7069 6563 6529 293b 0a20  k' }, piece));. 
-00001000: 2020 2020 2020 2020 2020 2020 2020 207d                 }
-00001010: 0a20 2020 2020 2020 2020 2020 207d 0a20  .            }. 
-00001020: 2020 2020 2020 207d 293b 0a20 2020 2020         });.     
-00001030: 2020 2072 6574 7572 6e20 6375 7273 6f72     return cursor
-00001040: 733b 0a20 2020 207d 2c0a 2020 2020 7570  s;.    },.    up
-00001050: 6461 7465 2875 7064 6174 652c 206c 6179  date(update, lay
-00001060: 6572 2920 7b0a 2020 2020 2020 2020 7265  er) {.        re
-00001070: 7475 726e 2021 2175 7064 6174 652e 7472  turn !!update.tr
-00001080: 616e 7361 6374 696f 6e73 2e66 696e 6428  ansactions.find(
-00001090: 7420 3d3e 2074 2e61 6e6e 6f74 6174 696f  t => t.annotatio
-000010a0: 6e28 7265 6d6f 7465 5365 6c65 6374 696f  n(remoteSelectio
-000010b0: 6e73 416e 6e6f 7461 7469 6f6e 2929 3b0a  nsAnnotation));.
-000010c0: 2020 2020 7d2c 0a20 2020 2063 6c61 7373      },.    class
-000010d0: 3a20 276a 702d 7265 6d6f 7465 2d63 7572  : 'jp-remote-cur
-000010e0: 736f 7273 270a 7d29 3b0a 2f2a 2a0a 202a  sors'.});./**. *
-000010f0: 2054 6f6f 6c74 6970 2065 7874 656e 7369   Tooltip extensi
-00001100: 6f6e 2074 6f20 6469 7370 6c61 7920 7573  on to display us
-00001110: 6572 2064 6973 706c 6179 206e 616d 6520  er display name 
-00001120: 6174 2063 7572 736f 7220 706f 7369 7469  at cursor positi
-00001130: 6f6e 0a20 2a2f 0a63 6f6e 7374 2075 7365  on. */.const use
-00001140: 7248 6f76 6572 203d 2068 6f76 6572 546f  rHover = hoverTo
-00001150: 6f6c 7469 7028 2876 6965 772c 2070 6f73  oltip((view, pos
-00001160: 2920 3d3e 207b 0a20 2020 2076 6172 205f  ) => {.    var _
-00001170: 613b 0a20 2020 2063 6f6e 7374 207b 2061  a;.    const { a
-00001180: 7761 7265 6e65 7373 2c20 7974 6578 7420  wareness, ytext 
-00001190: 7d20 3d20 7669 6577 2e73 7461 7465 2e66  } = view.state.f
-000011a0: 6163 6574 2865 6469 746f 7241 7761 7265  acet(editorAware
-000011b0: 6e65 7373 4661 6365 7429 3b0a 2020 2020  nessFacet);.    
-000011c0: 636f 6e73 7420 7964 6f63 203d 2079 7465  const ydoc = yte
-000011d0: 7874 2e64 6f63 3b0a 2020 2020 666f 7220  xt.doc;.    for 
-000011e0: 2863 6f6e 7374 205b 636c 6965 6e74 4944  (const [clientID
-000011f0: 2c20 7374 6174 655d 206f 6620 6177 6172  , state] of awar
-00001200: 656e 6573 732e 6765 7453 7461 7465 7328  eness.getStates(
-00001210: 2929 207b 0a20 2020 2020 2020 2069 6620  )) {.        if 
-00001220: 2863 6c69 656e 7449 4420 3d3d 3d20 6177  (clientID === aw
-00001230: 6172 656e 6573 732e 646f 632e 636c 6965  areness.doc.clie
-00001240: 6e74 4944 2920 7b0a 2020 2020 2020 2020  ntID) {.        
-00001250: 2020 2020 636f 6e74 696e 7565 3b0a 2020      continue;.  
-00001260: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-00001270: 666f 7220 2863 6f6e 7374 2063 7572 736f  for (const curso
-00001280: 7220 6f66 2028 5f61 203d 2073 7461 7465  r of (_a = state
-00001290: 2e63 7572 736f 7273 2920 213d 3d20 6e75  .cursors) !== nu
-000012a0: 6c6c 2026 2620 5f61 2021 3d3d 2076 6f69  ll && _a !== voi
-000012b0: 6420 3020 3f20 5f61 203a 205b 5d29 207b  d 0 ? _a : []) {
-000012c0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-000012d0: 2821 2863 7572 736f 7220 3d3d 3d20 6e75  (!(cursor === nu
-000012e0: 6c6c 207c 7c20 6375 7273 6f72 203d 3d3d  ll || cursor ===
-000012f0: 2076 6f69 6420 3020 3f20 766f 6964 2030   void 0 ? void 0
-00001300: 203a 2063 7572 736f 722e 6865 6164 2929   : cursor.head))
-00001310: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-00001320: 2020 2063 6f6e 7469 6e75 653b 0a20 2020     continue;.   
-00001330: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
-00001340: 2020 2020 2020 2063 6f6e 7374 2068 6561         const hea
-00001350: 6420 3d20 6372 6561 7465 4162 736f 6c75  d = createAbsolu
-00001360: 7465 506f 7369 7469 6f6e 4672 6f6d 5265  tePositionFromRe
-00001370: 6c61 7469 7665 506f 7369 7469 6f6e 2863  lativePosition(c
-00001380: 7572 736f 722e 6865 6164 2c20 7964 6f63  ursor.head, ydoc
-00001390: 293b 0a20 2020 2020 2020 2020 2020 2069  );.            i
-000013a0: 6620 2828 6865 6164 203d 3d3d 206e 756c  f ((head === nul
-000013b0: 6c20 7c7c 2068 6561 6420 3d3d 3d20 766f  l || head === vo
-000013c0: 6964 2030 203f 2076 6f69 6420 3020 3a20  id 0 ? void 0 : 
-000013d0: 6865 6164 2e74 7970 6529 2021 3d3d 2079  head.type) !== y
-000013e0: 7465 7874 2920 7b0a 2020 2020 2020 2020  text) {.        
-000013f0: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
-00001400: 3b0a 2020 2020 2020 2020 2020 2020 7d0a  ;.            }.
-00001410: 2020 2020 2020 2020 2020 2020 2f2f 2055              // U
-00001420: 7365 2073 6f6d 6520 6d61 7267 696e 2061  se some margin a
-00001430: 726f 756e 6420 7468 6520 6375 7273 6f72  round the cursor
-00001440: 2074 6f20 6469 7370 6c61 7920 7468 6520   to display the 
-00001450: 7573 6572 2e0a 2020 2020 2020 2020 2020  user..          
-00001460: 2020 6966 2028 6865 6164 2e69 6e64 6578    if (head.index
-00001470: 202d 2033 203c 3d20 706f 7320 2626 2070   - 3 <= pos && p
-00001480: 6f73 203c 3d20 6865 6164 2e69 6e64 6578  os <= head.index
-00001490: 202b 2033 2920 7b0a 2020 2020 2020 2020   + 3) {.        
-000014a0: 2020 2020 2020 2020 7265 7475 726e 207b          return {
-000014b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000014c0: 2020 2020 2070 6f73 3a20 6865 6164 2e69       pos: head.i
-000014d0: 6e64 6578 2c0a 2020 2020 2020 2020 2020  ndex,.          
-000014e0: 2020 2020 2020 2020 2020 6162 6f76 653a            above:
-000014f0: 2074 7275 652c 0a20 2020 2020 2020 2020   true,.         
-00001500: 2020 2020 2020 2020 2020 2063 7265 6174             creat
-00001510: 653a 2028 2920 3d3e 207b 0a20 2020 2020  e: () => {.     
-00001520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001530: 2020 2076 6172 205f 612c 205f 622c 205f     var _a, _b, _
-00001540: 632c 205f 643b 0a20 2020 2020 2020 2020  c, _d;.         
-00001550: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00001560: 6f6e 7374 2064 6f6d 203d 2064 6f63 756d  onst dom = docum
-00001570: 656e 742e 6372 6561 7465 456c 656d 656e  ent.createElemen
-00001580: 7428 2764 6976 2729 3b0a 2020 2020 2020  t('div');.      
-00001590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000015a0: 2020 646f 6d2e 636c 6173 734c 6973 742e    dom.classList.
-000015b0: 6164 6428 276a 702d 7265 6d6f 7465 2d75  add('jp-remote-u
-000015c0: 7365 7249 6e66 6f27 293b 0a20 2020 2020  serInfo');.     
-000015d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000015e0: 2020 2064 6f6d 2e73 7479 6c65 2e62 6163     dom.style.bac
-000015f0: 6b67 726f 756e 6443 6f6c 6f72 203d 2028  kgroundColor = (
-00001600: 5f62 203d 2028 5f61 203d 2073 7461 7465  _b = (_a = state
-00001610: 2e75 7365 7229 203d 3d3d 206e 756c 6c20  .user) === null 
-00001620: 7c7c 205f 6120 3d3d 3d20 766f 6964 2030  || _a === void 0
-00001630: 203f 2076 6f69 6420 3020 3a20 5f61 2e63   ? void 0 : _a.c
-00001640: 6f6c 6f72 2920 213d 3d20 6e75 6c6c 2026  olor) !== null &
-00001650: 2620 5f62 2021 3d3d 2076 6f69 6420 3020  & _b !== void 0 
-00001660: 3f20 5f62 203a 2027 6461 726b 6772 6579  ? _b : 'darkgrey
-00001670: 273b 0a20 2020 2020 2020 2020 2020 2020  ';.             
-00001680: 2020 2020 2020 2020 2020 2064 6f6d 2e74             dom.t
-00001690: 6578 7443 6f6e 7465 6e74 203d 0a20 2020  extContent =.   
-000016a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000016b0: 2020 2020 2020 2020 2028 5f64 203d 2028           (_d = (
-000016c0: 5f63 203d 2073 7461 7465 2e75 7365 7229  _c = state.user)
-000016d0: 203d 3d3d 206e 756c 6c20 7c7c 205f 6320   === null || _c 
-000016e0: 3d3d 3d20 766f 6964 2030 203f 2076 6f69  === void 0 ? voi
-000016f0: 6420 3020 3a20 5f63 2e64 6973 706c 6179  d 0 : _c.display
-00001700: 5f6e 616d 6529 2021 3d3d 206e 756c 6c20  _name) !== null 
-00001710: 2626 205f 6420 213d 3d20 766f 6964 2030  && _d !== void 0
-00001720: 203f 205f 6420 3a20 2741 6e6f 6e79 6d6f   ? _d : 'Anonymo
-00001730: 7573 273b 0a20 2020 2020 2020 2020 2020  us';.           
-00001740: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-00001750: 7572 6e20 7b20 646f 6d20 7d3b 0a20 2020  urn { dom };.   
-00001760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001770: 207d 0a20 2020 2020 2020 2020 2020 2020   }.             
-00001780: 2020 207d 3b0a 2020 2020 2020 2020 2020     };.          
-00001790: 2020 7d0a 2020 2020 2020 2020 7d0a 2020    }.        }.  
-000017a0: 2020 7d0a 2020 2020 7265 7475 726e 206e    }.    return n
-000017b0: 756c 6c3b 0a7d 2c20 7b0a 2020 2020 6869  ull;.}, {.    hi
-000017c0: 6465 4f6e 3a20 2874 722c 2074 6f6f 6c74  deOn: (tr, toolt
-000017d0: 6970 2920 3d3e 2021 2174 722e 616e 6e6f  ip) => !!tr.anno
-000017e0: 7461 7469 6f6e 2872 656d 6f74 6553 656c  tation(remoteSel
-000017f0: 6563 7469 6f6e 7341 6e6e 6f74 6174 696f  ectionsAnnotatio
-00001800: 6e29 2c0a 2020 2020 686f 7665 7254 696d  n),.    hoverTim
-00001810: 653a 2030 0a7d 293b 0a2f 2a2a 0a20 2a20  e: 0.});./**. * 
-00001820: 4578 7465 6e73 696f 6e20 6465 6669 6e69  Extension defini
-00001830: 6e67 2061 206e 6577 2065 6469 746f 7220  ng a new editor 
-00001840: 6c61 7965 7220 7374 6f72 696e 6720 7468  layer storing th
-00001850: 6520 7265 6d6f 7465 2073 656c 6563 7469  e remote selecti
-00001860: 6f6e 730a 202a 2f0a 636f 6e73 7420 7265  ons. */.const re
-00001870: 6d6f 7465 5365 6c65 6374 696f 6e4c 6179  moteSelectionLay
-00001880: 6572 203d 206c 6179 6572 287b 0a20 2020  er = layer({.   
-00001890: 2061 626f 7665 3a20 6661 6c73 652c 0a20   above: false,. 
-000018a0: 2020 206d 6172 6b65 7273 2876 6965 7729     markers(view)
-000018b0: 207b 0a20 2020 2020 2020 2063 6f6e 7374   {.        const
-000018c0: 207b 2061 7761 7265 6e65 7373 2c20 7974   { awareness, yt
-000018d0: 6578 7420 7d20 3d20 7669 6577 2e73 7461  ext } = view.sta
-000018e0: 7465 2e66 6163 6574 2865 6469 746f 7241  te.facet(editorA
-000018f0: 7761 7265 6e65 7373 4661 6365 7429 3b0a  warenessFacet);.
-00001900: 2020 2020 2020 2020 636f 6e73 7420 7964          const yd
-00001910: 6f63 203d 2079 7465 7874 2e64 6f63 3b0a  oc = ytext.doc;.
-00001920: 2020 2020 2020 2020 636f 6e73 7420 6375          const cu
-00001930: 7273 6f72 7320 3d20 5b5d 3b0a 2020 2020  rsors = [];.    
-00001940: 2020 2020 6177 6172 656e 6573 732e 6765      awareness.ge
-00001950: 7453 7461 7465 7328 292e 666f 7245 6163  tStates().forEac
-00001960: 6828 2873 7461 7465 2c20 636c 6965 6e74  h((state, client
-00001970: 4944 2920 3d3e 207b 0a20 2020 2020 2020  ID) => {.       
-00001980: 2020 2020 2076 6172 205f 612c 205f 622c       var _a, _b,
-00001990: 205f 633b 0a20 2020 2020 2020 2020 2020   _c;.           
-000019a0: 2069 6620 2863 6c69 656e 7449 4420 3d3d   if (clientID ==
-000019b0: 3d20 6177 6172 656e 6573 732e 646f 632e  = awareness.doc.
-000019c0: 636c 6965 6e74 4944 2920 7b0a 2020 2020  clientID) {.    
-000019d0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-000019e0: 726e 3b0a 2020 2020 2020 2020 2020 2020  rn;.            
-000019f0: 7d0a 2020 2020 2020 2020 2020 2020 636f  }.            co
-00001a00: 6e73 7420 6375 7273 6f72 735f 203d 2073  nst cursors_ = s
-00001a10: 7461 7465 2e63 7572 736f 7273 3b0a 2020  tate.cursors;.  
-00001a20: 2020 2020 2020 2020 2020 666f 7220 2863            for (c
-00001a30: 6f6e 7374 2063 7572 736f 7220 6f66 2063  onst cursor of c
-00001a40: 7572 736f 7273 5f20 213d 3d20 6e75 6c6c  ursors_ !== null
-00001a50: 2026 2620 6375 7273 6f72 735f 2021 3d3d   && cursors_ !==
-00001a60: 2076 6f69 6420 3020 3f20 6375 7273 6f72   void 0 ? cursor
-00001a70: 735f 203a 205b 5d29 207b 0a20 2020 2020  s_ : []) {.     
-00001a80: 2020 2020 2020 2020 2020 2069 6620 2828             if ((
-00001a90: 285f 6120 3d20 6375 7273 6f72 2e65 6d70  (_a = cursor.emp
-00001aa0: 7479 2920 213d 3d20 6e75 6c6c 2026 2620  ty) !== null && 
-00001ab0: 5f61 2021 3d3d 2076 6f69 6420 3020 3f20  _a !== void 0 ? 
-00001ac0: 5f61 203a 2074 7275 6529 207c 7c20 2128  _a : true) || !(
-00001ad0: 6375 7273 6f72 203d 3d3d 206e 756c 6c20  cursor === null 
-00001ae0: 7c7c 2063 7572 736f 7220 3d3d 3d20 766f  || cursor === vo
-00001af0: 6964 2030 203f 2076 6f69 6420 3020 3a20  id 0 ? void 0 : 
-00001b00: 6375 7273 6f72 2e61 6e63 686f 7229 207c  cursor.anchor) |
-00001b10: 7c20 2128 6375 7273 6f72 203d 3d3d 206e  | !(cursor === n
-00001b20: 756c 6c20 7c7c 2063 7572 736f 7220 3d3d  ull || cursor ==
-00001b30: 3d20 766f 6964 2030 203f 2076 6f69 6420  = void 0 ? void 
-00001b40: 3020 3a20 6375 7273 6f72 2e68 6561 6429  0 : cursor.head)
-00001b50: 2920 7b0a 2020 2020 2020 2020 2020 2020  ) {.            
-00001b60: 2020 2020 2020 2020 7265 7475 726e 3b0a          return;.
-00001b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b80: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
-00001b90: 2020 636f 6e73 7420 616e 6368 6f72 203d    const anchor =
-00001ba0: 2063 7265 6174 6541 6273 6f6c 7574 6550   createAbsoluteP
-00001bb0: 6f73 6974 696f 6e46 726f 6d52 656c 6174  ositionFromRelat
-00001bc0: 6976 6550 6f73 6974 696f 6e28 6375 7273  ivePosition(curs
-00001bd0: 6f72 2e61 6e63 686f 722c 2079 646f 6329  or.anchor, ydoc)
-00001be0: 3b0a 2020 2020 2020 2020 2020 2020 2020  ;.              
-00001bf0: 2020 636f 6e73 7420 6865 6164 203d 2063    const head = c
-00001c00: 7265 6174 6541 6273 6f6c 7574 6550 6f73  reateAbsolutePos
-00001c10: 6974 696f 6e46 726f 6d52 656c 6174 6976  itionFromRelativ
-00001c20: 6550 6f73 6974 696f 6e28 6375 7273 6f72  ePosition(cursor
-00001c30: 2e68 6561 642c 2079 646f 6329 3b0a 2020  .head, ydoc);.  
-00001c40: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00001c50: 2028 2861 6e63 686f 7220 3d3d 3d20 6e75   ((anchor === nu
-00001c60: 6c6c 207c 7c20 616e 6368 6f72 203d 3d3d  ll || anchor ===
-00001c70: 2076 6f69 6420 3020 3f20 766f 6964 2030   void 0 ? void 0
-00001c80: 203a 2061 6e63 686f 722e 7479 7065 2920   : anchor.type) 
-00001c90: 213d 3d20 7974 6578 7420 7c7c 2028 6865  !== ytext || (he
-00001ca0: 6164 203d 3d3d 206e 756c 6c20 7c7c 2068  ad === null || h
-00001cb0: 6561 6420 3d3d 3d20 766f 6964 2030 203f  ead === void 0 ?
-00001cc0: 2076 6f69 6420 3020 3a20 6865 6164 2e74   void 0 : head.t
-00001cd0: 7970 6529 2021 3d3d 2079 7465 7874 2920  ype) !== ytext) 
-00001ce0: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-00001cf0: 2020 2020 2020 7265 7475 726e 3b0a 2020        return;.  
-00001d00: 2020 2020 2020 2020 2020 2020 2020 7d0a                }.
-00001d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d20: 636f 6e73 7420 636c 6173 734e 616d 6520  const className 
-00001d30: 3d20 276a 702d 7265 6d6f 7465 2d73 656c  = 'jp-remote-sel
-00001d40: 6563 7469 6f6e 273b 0a20 2020 2020 2020  ection';.       
-00001d50: 2020 2020 2020 2020 2066 6f72 2028 636f           for (co
-00001d60: 6e73 7420 7069 6563 6520 6f66 2052 6563  nst piece of Rec
-00001d70: 7461 6e67 6c65 4d61 726b 6572 2e66 6f72  tangleMarker.for
-00001d80: 5261 6e67 6528 7669 6577 2c20 636c 6173  Range(view, clas
-00001d90: 734e 616d 652c 2045 6469 746f 7253 656c  sName, EditorSel
-00001da0: 6563 7469 6f6e 2e72 616e 6765 2861 6e63  ection.range(anc
-00001db0: 686f 722e 696e 6465 782c 2068 6561 642e  hor.index, head.
-00001dc0: 696e 6465 7829 2929 207b 0a20 2020 2020  index))) {.     
-00001dd0: 2020 2020 2020 2020 2020 2020 2020 202f                 /
-00001de0: 2f20 5772 6170 2074 6865 2072 6563 7461  / Wrap the recta
-00001df0: 6e67 6c65 206d 6172 6b65 7220 746f 2073  ngle marker to s
-00001e00: 6574 2074 6865 2075 7365 7220 636f 6c6f  et the user colo
-00001e10: 720a 2020 2020 2020 2020 2020 2020 2020  r.              
-00001e20: 2020 2020 2020 6375 7273 6f72 732e 7075        cursors.pu
-00001e30: 7368 286e 6577 2052 656d 6f74 654d 6172  sh(new RemoteMar
-00001e40: 6b65 7228 7b20 6261 636b 6772 6f75 6e64  ker({ background
-00001e50: 436f 6c6f 723a 2028 5f63 203d 2028 5f62  Color: (_c = (_b
-00001e60: 203d 2073 7461 7465 2e75 7365 7229 203d   = state.user) =
-00001e70: 3d3d 206e 756c 6c20 7c7c 205f 6220 3d3d  == null || _b ==
-00001e80: 3d20 766f 6964 2030 203f 2076 6f69 6420  = void 0 ? void 
-00001e90: 3020 3a20 5f62 2e63 6f6c 6f72 2920 213d  0 : _b.color) !=
-00001ea0: 3d20 6e75 6c6c 2026 2620 5f63 2021 3d3d  = null && _c !==
-00001eb0: 2076 6f69 6420 3020 3f20 5f63 203a 2027   void 0 ? _c : '
-00001ec0: 626c 6163 6b27 207d 2c20 7069 6563 6529  black' }, piece)
-00001ed0: 293b 0a20 2020 2020 2020 2020 2020 2020  );.             
-00001ee0: 2020 207d 0a20 2020 2020 2020 2020 2020     }.           
-00001ef0: 207d 0a20 2020 2020 2020 207d 293b 0a20   }.        });. 
-00001f00: 2020 2020 2020 2072 6574 7572 6e20 6375         return cu
-00001f10: 7273 6f72 733b 0a20 2020 207d 2c0a 2020  rsors;.    },.  
-00001f20: 2020 7570 6461 7465 2875 7064 6174 652c    update(update,
-00001f30: 206c 6179 6572 2920 7b0a 2020 2020 2020   layer) {.      
-00001f40: 2020 7265 7475 726e 2021 2175 7064 6174    return !!updat
-00001f50: 652e 7472 616e 7361 6374 696f 6e73 2e66  e.transactions.f
-00001f60: 696e 6428 7420 3d3e 2074 2e61 6e6e 6f74  ind(t => t.annot
-00001f70: 6174 696f 6e28 7265 6d6f 7465 5365 6c65  ation(remoteSele
-00001f80: 6374 696f 6e73 416e 6e6f 7461 7469 6f6e  ctionsAnnotation
-00001f90: 2929 3b0a 2020 2020 7d2c 0a20 2020 2063  ));.    },.    c
-00001fa0: 6c61 7373 3a20 276a 702d 7265 6d6f 7465  lass: 'jp-remote
-00001fb0: 2d73 656c 6563 7469 6f6e 7327 0a7d 293b  -selections'.});
-00001fc0: 0a2f 2a2a 0a20 2a20 436f 6465 4d69 7272  ./**. * CodeMirr
-00001fd0: 6f72 2065 7874 656e 7369 6f6e 2065 7863  or extension exc
-00001fe0: 6861 6e67 696e 6720 616e 6420 6469 7370  hanging and disp
-00001ff0: 6c61 7969 6e67 2072 656d 6f74 6520 7573  laying remote us
-00002000: 6572 2073 656c 6563 7469 6f6e 2072 616e  er selection ran
-00002010: 6765 7320 2869 6e63 6c75 6469 6e67 2063  ges (including c
-00002020: 7572 736f 7273 290a 202a 2f0a 636f 6e73  ursors). */.cons
-00002030: 7420 7368 6f77 436f 6c6c 6162 6f72 6174  t showCollaborat
-00002040: 6f72 7320 3d20 5669 6577 506c 7567 696e  ors = ViewPlugin
-00002050: 2e66 726f 6d43 6c61 7373 2863 6c61 7373  .fromClass(class
-00002060: 207b 0a20 2020 2063 6f6e 7374 7275 6374   {.    construct
-00002070: 6f72 2876 6965 7729 207b 0a20 2020 2020  or(view) {.     
-00002080: 2020 2074 6869 732e 6564 6974 6f72 4177     this.editorAw
-00002090: 6172 656e 6573 7320 3d20 7669 6577 2e73  areness = view.s
-000020a0: 7461 7465 2e66 6163 6574 2865 6469 746f  tate.facet(edito
-000020b0: 7241 7761 7265 6e65 7373 4661 6365 7429  rAwarenessFacet)
-000020c0: 3b0a 2020 2020 2020 2020 7468 6973 2e5f  ;.        this._
-000020d0: 6c69 7374 656e 6572 203d 2028 7b20 6164  listener = ({ ad
-000020e0: 6465 642c 2075 7064 6174 6564 2c20 7265  ded, updated, re
-000020f0: 6d6f 7665 6420 7d29 203d 3e20 7b0a 2020  moved }) => {.  
-00002100: 2020 2020 2020 2020 2020 636f 6e73 7420            const 
-00002110: 636c 6965 6e74 7320 3d20 6164 6465 642e  clients = added.
-00002120: 636f 6e63 6174 2875 7064 6174 6564 292e  concat(updated).
-00002130: 636f 6e63 6174 2872 656d 6f76 6564 293b  concat(removed);
-00002140: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00002150: 2863 6c69 656e 7473 2e66 696e 6449 6e64  (clients.findInd
-00002160: 6578 2869 6420 3d3e 2069 6420 213d 3d20  ex(id => id !== 
-00002170: 7468 6973 2e65 6469 746f 7241 7761 7265  this.editorAware
-00002180: 6e65 7373 2e61 7761 7265 6e65 7373 2e64  ness.awareness.d
-00002190: 6f63 2e63 6c69 656e 7449 4429 203e 3d20  oc.clientID) >= 
-000021a0: 3029 207b 0a20 2020 2020 2020 2020 2020  0) {.           
-000021b0: 2020 2020 202f 2f20 5472 6963 6b20 746f       // Trick to
-000021c0: 2067 6574 2074 6865 2072 656d 6f74 6543   get the remoteC
-000021d0: 7572 736f 724c 6179 6572 7320 746f 2062  ursorLayers to b
-000021e0: 6520 7570 6461 7465 640a 2020 2020 2020  e updated.      
-000021f0: 2020 2020 2020 2020 2020 7669 6577 2e64            view.d
-00002200: 6973 7061 7463 6828 7b20 616e 6e6f 7461  ispatch({ annota
-00002210: 7469 6f6e 733a 205b 7265 6d6f 7465 5365  tions: [remoteSe
-00002220: 6c65 6374 696f 6e73 416e 6e6f 7461 7469  lectionsAnnotati
-00002230: 6f6e 2e6f 6628 5b5d 295d 207d 293b 0a20  on.of([])] });. 
-00002240: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
-00002250: 2020 2020 207d 3b0a 2020 2020 2020 2020       };.        
-00002260: 7468 6973 2e65 6469 746f 7241 7761 7265  this.editorAware
-00002270: 6e65 7373 2e61 7761 7265 6e65 7373 2e6f  ness.awareness.o
-00002280: 6e28 2763 6861 6e67 6527 2c20 7468 6973  n('change', this
-00002290: 2e5f 6c69 7374 656e 6572 293b 0a20 2020  ._listener);.   
-000022a0: 207d 0a20 2020 2064 6573 7472 6f79 2829   }.    destroy()
-000022b0: 207b 0a20 2020 2020 2020 2074 6869 732e   {.        this.
-000022c0: 6564 6974 6f72 4177 6172 656e 6573 732e  editorAwareness.
-000022d0: 6177 6172 656e 6573 732e 6f66 6628 2763  awareness.off('c
-000022e0: 6861 6e67 6527 2c20 7468 6973 2e5f 6c69  hange', this._li
-000022f0: 7374 656e 6572 293b 0a20 2020 207d 0a20  stener);.    }. 
-00002300: 2020 202f 2a2a 0a20 2020 2020 2a20 436f     /**.     * Co
-00002310: 6d6d 756e 6963 6174 6520 7468 6520 6375  mmunicate the cu
-00002320: 7272 656e 7420 7573 6572 2063 7572 736f  rrent user curso
-00002330: 7220 706f 7369 7469 6f6e 2074 6f20 616c  r position to al
-00002340: 6c20 7265 6d6f 7465 730a 2020 2020 202a  l remotes.     *
-00002350: 2f0a 2020 2020 7570 6461 7465 2875 7064  /.    update(upd
-00002360: 6174 6529 207b 0a20 2020 2020 2020 2076  ate) {.        v
-00002370: 6172 205f 613b 0a20 2020 2020 2020 2069  ar _a;.        i
-00002380: 6620 2821 7570 6461 7465 2e64 6f63 4368  f (!update.docCh
-00002390: 616e 6765 6420 2626 2021 7570 6461 7465  anged && !update
-000023a0: 2e73 656c 6563 7469 6f6e 5365 7429 207b  .selectionSet) {
-000023b0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-000023c0: 7572 6e3b 0a20 2020 2020 2020 207d 0a20  urn;.        }. 
-000023d0: 2020 2020 2020 2063 6f6e 7374 207b 2061         const { a
-000023e0: 7761 7265 6e65 7373 2c20 7974 6578 7420  wareness, ytext 
-000023f0: 7d20 3d20 7468 6973 2e65 6469 746f 7241  } = this.editorA
-00002400: 7761 7265 6e65 7373 3b0a 2020 2020 2020  wareness;.      
-00002410: 2020 636f 6e73 7420 6c6f 6361 6c41 7761    const localAwa
-00002420: 7265 6e65 7373 5374 6174 6520 3d20 6177  renessState = aw
-00002430: 6172 656e 6573 732e 6765 744c 6f63 616c  areness.getLocal
-00002440: 5374 6174 6528 293b 0a20 2020 2020 2020  State();.       
-00002450: 202f 2f20 7365 7420 6c6f 6361 6c20 6177   // set local aw
-00002460: 6172 656e 6573 7320 7374 6174 6520 2875  areness state (u
-00002470: 7064 6174 6520 6375 7273 6f72 7329 0a20  pdate cursors). 
-00002480: 2020 2020 2020 2069 6620 286c 6f63 616c         if (local
-00002490: 4177 6172 656e 6573 7353 7461 7465 2920  AwarenessState) 
-000024a0: 7b0a 2020 2020 2020 2020 2020 2020 636f  {.            co
-000024b0: 6e73 7420 6861 7346 6f63 7573 203d 2075  nst hasFocus = u
-000024c0: 7064 6174 652e 7669 6577 2e68 6173 466f  pdate.view.hasFo
-000024d0: 6375 7320 2626 2075 7064 6174 652e 7669  cus && update.vi
-000024e0: 6577 2e64 6f6d 2e6f 776e 6572 446f 6375  ew.dom.ownerDocu
-000024f0: 6d65 6e74 2e68 6173 466f 6375 7328 293b  ment.hasFocus();
-00002500: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
-00002510: 7374 2073 656c 6563 7469 6f6e 203d 2075  st selection = u
-00002520: 7064 6174 652e 7374 6174 652e 7365 6c65  pdate.state.sele
-00002530: 6374 696f 6e3b 0a20 2020 2020 2020 2020  ction;.         
-00002540: 2020 2063 6f6e 7374 2063 7572 736f 7273     const cursors
-00002550: 203d 206e 6577 2041 7272 6179 2829 3b0a   = new Array();.
-00002560: 2020 2020 2020 2020 2020 2020 6966 2028              if (
-00002570: 6861 7346 6f63 7573 2026 2620 7365 6c65  hasFocus && sele
-00002580: 6374 696f 6e29 207b 0a20 2020 2020 2020  ction) {.       
-00002590: 2020 2020 2020 2020 2066 6f72 2028 636f           for (co
-000025a0: 6e73 7420 7220 6f66 2073 656c 6563 7469  nst r of selecti
-000025b0: 6f6e 2e72 616e 6765 7329 207b 0a20 2020  on.ranges) {.   
-000025c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000025d0: 2063 6f6e 7374 2070 7269 6d61 7279 203d   const primary =
-000025e0: 2072 203d 3d3d 2073 656c 6563 7469 6f6e   r === selection
-000025f0: 2e6d 6169 6e3b 0a20 2020 2020 2020 2020  .main;.         
-00002600: 2020 2020 2020 2020 2020 2063 6f6e 7374             const
-00002610: 2061 6e63 686f 7220 3d20 6372 6561 7465   anchor = create
-00002620: 5265 6c61 7469 7665 506f 7369 7469 6f6e  RelativePosition
-00002630: 4672 6f6d 5479 7065 496e 6465 7828 7974  FromTypeIndex(yt
-00002640: 6578 742c 2072 2e61 6e63 686f 7229 3b0a  ext, r.anchor);.
-00002650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002660: 2020 2020 636f 6e73 7420 6865 6164 203d      const head =
-00002670: 2063 7265 6174 6552 656c 6174 6976 6550   createRelativeP
-00002680: 6f73 6974 696f 6e46 726f 6d54 7970 6549  ositionFromTypeI
-00002690: 6e64 6578 2879 7465 7874 2c20 722e 6865  ndex(ytext, r.he
-000026a0: 6164 293b 0a20 2020 2020 2020 2020 2020  ad);.           
-000026b0: 2020 2020 2020 2020 2063 7572 736f 7273           cursors
-000026c0: 2e70 7573 6828 7b0a 2020 2020 2020 2020  .push({.        
-000026d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000026e0: 616e 6368 6f72 2c0a 2020 2020 2020 2020  anchor,.        
-000026f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002700: 6865 6164 2c0a 2020 2020 2020 2020 2020  head,.          
-00002710: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-00002720: 696d 6172 792c 0a20 2020 2020 2020 2020  imary,.         
-00002730: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00002740: 6d70 7479 3a20 722e 656d 7074 790a 2020  mpty: r.empty.  
-00002750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002760: 2020 7d29 3b0a 2020 2020 2020 2020 2020    });.          
-00002770: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-00002780: 2020 2020 2020 2020 6966 2028 216c 6f63          if (!loc
-00002790: 616c 4177 6172 656e 6573 7353 7461 7465  alAwarenessState
-000027a0: 2e63 7572 736f 7273 207c 7c20 6375 7273  .cursors || curs
-000027b0: 6f72 732e 6c65 6e67 7468 203e 2030 2920  ors.length > 0) 
-000027c0: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-000027d0: 2020 2020 2020 636f 6e73 7420 6f6c 6443        const oldC
-000027e0: 7572 736f 7273 203d 2028 5f61 203d 206c  ursors = (_a = l
-000027f0: 6f63 616c 4177 6172 656e 6573 7353 7461  ocalAwarenessSta
-00002800: 7465 2e63 7572 736f 7273 2920 3d3d 3d20  te.cursors) === 
-00002810: 6e75 6c6c 207c 7c20 5f61 203d 3d3d 2076  null || _a === v
-00002820: 6f69 6420 3020 3f20 766f 6964 2030 203a  oid 0 ? void 0 :
-00002830: 205f 612e 6d61 7028 6375 7273 6f72 203d   _a.map(cursor =
-00002840: 3e20 7b0a 2020 2020 2020 2020 2020 2020  > {.            
-00002850: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00002860: 726e 207b 0a20 2020 2020 2020 2020 2020  rn {.           
-00002870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002880: 202e 2e2e 6375 7273 6f72 2c0a 2020 2020   ...cursor,.    
-00002890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000028a0: 2020 2020 2020 2020 616e 6368 6f72 3a20          anchor: 
-000028b0: 2863 7572 736f 7220 3d3d 3d20 6e75 6c6c  (cursor === null
-000028c0: 207c 7c20 6375 7273 6f72 203d 3d3d 2076   || cursor === v
-000028d0: 6f69 6420 3020 3f20 766f 6964 2030 203a  oid 0 ? void 0 :
-000028e0: 2063 7572 736f 722e 616e 6368 6f72 290a   cursor.anchor).
-000028f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002910: 3f20 6372 6561 7465 5265 6c61 7469 7665  ? createRelative
-00002920: 506f 7369 7469 6f6e 4672 6f6d 4a53 4f4e  PositionFromJSON
-00002930: 2863 7572 736f 722e 616e 6368 6f72 290a  (cursor.anchor).
-00002940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002960: 3a20 6e75 6c6c 2c0a 2020 2020 2020 2020  : null,.        
-00002970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002980: 2020 2020 6865 6164 3a20 2863 7572 736f      head: (curso
-00002990: 7220 3d3d 3d20 6e75 6c6c 207c 7c20 6375  r === null || cu
-000029a0: 7273 6f72 203d 3d3d 2076 6f69 6420 3020  rsor === void 0 
-000029b0: 3f20 766f 6964 2030 203a 2063 7572 736f  ? void 0 : curso
-000029c0: 722e 6865 6164 290a 2020 2020 2020 2020  r.head).        
-000029d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000029e0: 2020 2020 2020 2020 3f20 6372 6561 7465          ? create
-000029f0: 5265 6c61 7469 7665 506f 7369 7469 6f6e  RelativePosition
-00002a00: 4672 6f6d 4a53 4f4e 2863 7572 736f 722e  FromJSON(cursor.
-00002a10: 6865 6164 290a 2020 2020 2020 2020 2020  head).          
-00002a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a30: 2020 2020 2020 3a20 6e75 6c6c 0a20 2020        : null.   
-00002a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a50: 2020 2020 207d 3b0a 2020 2020 2020 2020       };.        
-00002a60: 2020 2020 2020 2020 2020 2020 7d29 3b0a              });.
-00002a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a80: 2020 2020 6966 2028 214a 534f 4e45 7874      if (!JSONExt
-00002a90: 2e64 6565 7045 7175 616c 2863 7572 736f  .deepEqual(curso
-00002aa0: 7273 2c20 6f6c 6443 7572 736f 7273 2929  rs, oldCursors))
-00002ab0: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-00002ac0: 2020 2020 2020 2020 2020 202f 2f20 5570             // Up
-00002ad0: 6461 7465 2063 7572 736f 7273 0a20 2020  date cursors.   
-00002ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002af0: 2020 2020 2061 7761 7265 6e65 7373 2e73       awareness.s
-00002b00: 6574 4c6f 6361 6c53 7461 7465 4669 656c  etLocalStateFiel
-00002b10: 6428 2763 7572 736f 7273 272c 2063 7572  d('cursors', cur
-00002b20: 736f 7273 293b 0a20 2020 2020 2020 2020  sors);.         
-00002b30: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
-00002b40: 2020 2020 2020 2020 2020 2020 207d 0a20               }. 
-00002b50: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
-00002b60: 2020 2020 207d 0a20 2020 207d 0a7d 2c20       }.    }.}, 
-00002b70: 7b0a 2020 2020 7072 6f76 6964 653a 2028  {.    provide: (
-00002b80: 2920 3d3e 207b 0a20 2020 2020 2020 2072  ) => {.        r
-00002b90: 6574 7572 6e20 5b0a 2020 2020 2020 2020  eturn [.        
+00000060: 6365 6e73 652e 0a0a 696d 706f 7274 207b  cense...import {
+00000070: 0a20 2041 6e6e 6f74 6174 696f 6e2c 0a20  .  Annotation,. 
+00000080: 2045 6469 746f 7253 656c 6563 7469 6f6e   EditorSelection
+00000090: 2c0a 2020 4578 7465 6e73 696f 6e2c 0a20  ,.  Extension,. 
+000000a0: 2046 6163 6574 0a7d 2066 726f 6d20 2740   Facet.} from '@
+000000b0: 636f 6465 6d69 7272 6f72 2f73 7461 7465  codemirror/state
+000000c0: 273b 0a69 6d70 6f72 7420 7b0a 2020 4564  ';.import {.  Ed
+000000d0: 6974 6f72 5669 6577 2c0a 2020 686f 7665  itorView,.  hove
+000000e0: 7254 6f6f 6c74 6970 2c0a 2020 6c61 7965  rTooltip,.  laye
+000000f0: 722c 0a20 204c 6179 6572 4d61 726b 6572  r,.  LayerMarker
+00000100: 2c0a 2020 5265 6374 616e 676c 654d 6172  ,.  RectangleMar
+00000110: 6b65 722c 0a20 2074 6f6f 6c74 6970 732c  ker,.  tooltips,
+00000120: 0a20 2056 6965 7750 6c75 6769 6e2c 0a20  .  ViewPlugin,. 
+00000130: 2056 6965 7755 7064 6174 650a 7d20 6672   ViewUpdate.} fr
+00000140: 6f6d 2027 4063 6f64 656d 6972 726f 722f  om '@codemirror/
+00000150: 7669 6577 273b 0a69 6d70 6f72 7420 7b20  view';.import { 
+00000160: 5573 6572 207d 2066 726f 6d20 2740 6a75  User } from '@ju
+00000170: 7079 7465 726c 6162 2f73 6572 7669 6365  pyterlab/service
+00000180: 7327 3b0a 696d 706f 7274 207b 204a 534f  s';.import { JSO
+00000190: 4e45 7874 207d 2066 726f 6d20 2740 6c75  NExt } from '@lu
+000001a0: 6d69 6e6f 2f63 6f72 6575 7469 6c73 273b  mino/coreutils';
+000001b0: 0a69 6d70 6f72 7420 7b20 4177 6172 656e  .import { Awaren
+000001c0: 6573 7320 7d20 6672 6f6d 2027 792d 7072  ess } from 'y-pr
+000001d0: 6f74 6f63 6f6c 732f 6177 6172 656e 6573  otocols/awarenes
+000001e0: 7327 3b0a 696d 706f 7274 207b 0a20 2063  s';.import {.  c
+000001f0: 7265 6174 6541 6273 6f6c 7574 6550 6f73  reateAbsolutePos
+00000200: 6974 696f 6e46 726f 6d52 656c 6174 6976  itionFromRelativ
+00000210: 6550 6f73 6974 696f 6e2c 0a20 2063 7265  ePosition,.  cre
+00000220: 6174 6552 656c 6174 6976 6550 6f73 6974  ateRelativePosit
+00000230: 696f 6e46 726f 6d4a 534f 4e2c 0a20 2063  ionFromJSON,.  c
+00000240: 7265 6174 6552 656c 6174 6976 6550 6f73  reateRelativePos
+00000250: 6974 696f 6e46 726f 6d54 7970 6549 6e64  itionFromTypeInd
+00000260: 6578 2c0a 2020 5265 6c61 7469 7665 506f  ex,.  RelativePo
+00000270: 7369 7469 6f6e 2c0a 2020 5465 7874 0a7d  sition,.  Text.}
+00000280: 2066 726f 6d20 2779 6a73 273b 0a0a 2f2a   from 'yjs';../*
+00000290: 0a20 2041 6464 2077 6964 6765 7420 746f  .  Add widget to
+000002a0: 2063 6f64 656d 6972 726f 7220 3620 6564   codemirror 6 ed
+000002b0: 6974 6f72 7320 6469 7370 6c61 7969 6e67  itors displaying
+000002c0: 2063 6f6c 6c61 626f 7261 746f 7273 2e0a   collaborators..
+000002d0: 0a20 2054 6869 7320 636f 6465 2069 7320  .  This code is 
+000002e0: 696e 7370 6972 6564 2062 7920 6874 7470  inspired by http
+000002f0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f79  s://github.com/y
+00000300: 6a73 2f79 2d63 6f64 656d 6972 726f 722e  js/y-codemirror.
+00000310: 6e65 7874 2f62 6c6f 622f 6d61 696e 2f73  next/blob/main/s
+00000320: 7263 2f79 2d72 656d 6f74 652d 7365 6c65  rc/y-remote-sele
+00000330: 6374 696f 6e73 2e6a 7320 6c69 6365 6e73  ctions.js licens
+00000340: 6564 2075 6e64 6572 204d 4954 204c 6963  ed under MIT Lic
+00000350: 656e 7365 2062 7920 4b65 7669 6e20 4a61  ense by Kevin Ja
+00000360: 686e 730a 0a20 2042 7574 2069 7420 7573  hns..  But it us
+00000370: 6573 2061 6e20 6170 7072 6f61 6368 2073  es an approach s
+00000380: 696d 696c 6172 2074 6f20 7468 6520 6472  imilar to the dr
+00000390: 6177 2073 656c 6563 7469 6f6e 2065 7874  aw selection ext
+000003a0: 656e 7369 6f6e 206f 6620 636f 7265 2043  ension of core C
+000003b0: 6f64 654d 6972 726f 7220 746f 2064 6973  odeMirror to dis
+000003c0: 706c 6179 2063 7572 736f 7273 2061 6e64  play cursors and
+000003d0: 2073 656c 6563 7469 6f6e 732e 0a20 2a2f   selections.. */
+000003e0: 0a0a 2f2a 2a0a 202a 2059 6a73 2064 6f63  ../**. * Yjs doc
+000003f0: 756d 656e 7420 6f62 6a65 6374 730a 202a  ument objects. *
+00000400: 2f0a 6578 706f 7274 2074 7970 6520 4564  /.export type Ed
+00000410: 6974 6f72 4177 6172 656e 6573 7320 3d20  itorAwareness = 
+00000420: 7b0a 2020 2f2a 2a0a 2020 202a 2055 7365  {.  /**.   * Use
+00000430: 7220 7265 6c61 7465 6420 696e 666f 726d  r related inform
+00000440: 6174 696f 6e0a 2020 202a 2f0a 2020 6177  ation.   */.  aw
+00000450: 6172 656e 6573 733a 2041 7761 7265 6e65  areness: Awarene
+00000460: 7373 3b0a 2020 2f2a 2a0a 2020 202a 2053  ss;.  /**.   * S
+00000470: 6861 7265 6420 6564 6974 6f72 2073 6f75  hared editor sou
+00000480: 7263 650a 2020 202a 2f0a 2020 7974 6578  rce.   */.  ytex
+00000490: 743a 2054 6578 743b 0a7d 3b0a 0a69 6e74  t: Text;.};..int
+000004a0: 6572 6661 6365 2049 4375 7273 6f72 5374  erface ICursorSt
+000004b0: 6174 6520 7b0a 2020 2f2a 2a0a 2020 202a  ate {.  /**.   *
+000004c0: 2043 7572 736f 7220 616e 6368 6f72 0a20   Cursor anchor. 
+000004d0: 2020 2a2f 0a20 2061 6e63 686f 723a 2052    */.  anchor: R
+000004e0: 656c 6174 6976 6550 6f73 6974 696f 6e3b  elativePosition;
+000004f0: 0a20 202f 2a2a 0a20 2020 2a20 4375 7273  .  /**.   * Curs
+00000500: 6f72 2068 6561 640a 2020 202a 2f0a 2020  or head.   */.  
+00000510: 6865 6164 3a20 5265 6c61 7469 7665 506f  head: RelativePo
+00000520: 7369 7469 6f6e 3b0a 2020 2f2a 2a0a 2020  sition;.  /**.  
+00000530: 202a 2057 6865 7468 6572 2074 6865 2063   * Whether the c
+00000540: 7572 736f 7220 6973 2061 6e20 656d 7074  ursor is an empt
+00000550: 7920 7261 6e67 6520 6f72 206e 6f74 2e0a  y range or not..
+00000560: 2020 202a 0a20 2020 2a20 4465 6661 756c     *.   * Defaul
+00000570: 7420 6074 7275 6560 0a20 2020 2a2f 0a20  t `true`.   */. 
+00000580: 2065 6d70 7479 3f3a 2062 6f6f 6c65 616e   empty?: boolean
+00000590: 3b0a 2020 2f2a 2a0a 2020 202a 2057 6865  ;.  /**.   * Whe
+000005a0: 7468 6572 2074 6865 2063 7572 736f 7220  ther the cursor 
+000005b0: 6973 2074 6865 2070 7269 6d61 7279 206f  is the primary o
+000005c0: 6e65 206f 7220 6e6f 742e 0a20 2020 2a0a  ne or not..   *.
+000005d0: 2020 202a 2044 6566 6175 6c74 2060 6661     * Default `fa
+000005e0: 6c73 6560 0a20 2020 2a2f 0a20 2070 7269  lse`.   */.  pri
+000005f0: 6d61 7279 3f3a 2062 6f6f 6c65 616e 3b0a  mary?: boolean;.
+00000600: 7d0a 0a2f 2a2a 0a20 2a20 4177 6172 656e  }../**. * Awaren
+00000610: 6573 7320 7374 6174 6520 6465 6669 6e69  ess state defini
+00000620: 7469 6f6e 0a20 2a2f 0a69 6e74 6572 6661  tion. */.interfa
+00000630: 6365 2049 4177 6172 656e 6573 7353 7461  ce IAwarenessSta
+00000640: 7465 2065 7874 656e 6473 2052 6563 6f72  te extends Recor
+00000650: 643c 7374 7269 6e67 2c20 616e 793e 207b  d<string, any> {
+00000660: 0a20 202f 2a2a 0a20 2020 2a20 5573 6572  .  /**.   * User
+00000670: 2069 6465 6e74 6974 790a 2020 202a 2f0a   identity.   */.
+00000680: 2020 7573 6572 3f3a 2055 7365 722e 4949    user?: User.II
+00000690: 6465 6e74 6974 793b 0a20 202f 2a2a 0a20  dentity;.  /**. 
+000006a0: 2020 2a20 5573 6572 2063 7572 736f 7273    * User cursors
+000006b0: 0a20 2020 2a2f 0a20 2063 7572 736f 7273  .   */.  cursors
+000006c0: 3f3a 2049 4375 7273 6f72 5374 6174 655b  ?: ICursorState[
+000006d0: 5d3b 0a7d 0a0a 2f2a 2a0a 202a 2046 6163  ];.}../**. * Fac
+000006e0: 6574 2073 746f 7269 6e67 2074 6865 2059  et storing the Y
+000006f0: 6a73 2064 6f63 756d 656e 7420 6f62 6a65  js document obje
+00000700: 6374 730a 202a 2f0a 636f 6e73 7420 6564  cts. */.const ed
+00000710: 6974 6f72 4177 6172 656e 6573 7346 6163  itorAwarenessFac
+00000720: 6574 203d 2046 6163 6574 2e64 6566 696e  et = Facet.defin
+00000730: 653c 4564 6974 6f72 4177 6172 656e 6573  e<EditorAwarenes
+00000740: 732c 2045 6469 746f 7241 7761 7265 6e65  s, EditorAwarene
+00000750: 7373 3e28 7b0a 2020 636f 6d62 696e 6528  ss>({.  combine(
+00000760: 636f 6e66 6967 733a 2072 6561 646f 6e6c  configs: readonl
+00000770: 7920 4564 6974 6f72 4177 6172 656e 6573  y EditorAwarenes
+00000780: 735b 5d29 207b 0a20 2020 2072 6574 7572  s[]) {.    retur
+00000790: 6e20 636f 6e66 6967 735b 636f 6e66 6967  n configs[config
+000007a0: 732e 6c65 6e67 7468 202d 2031 5d3b 0a20  s.length - 1];. 
+000007b0: 207d 0a7d 293b 0a0a 2f2a 2a0a 202a 2052   }.});../**. * R
+000007c0: 656d 6f74 6520 7365 6c65 6374 696f 6e20  emote selection 
+000007d0: 7468 656d 650a 202a 2f0a 636f 6e73 7420  theme. */.const 
+000007e0: 7265 6d6f 7465 5365 6c65 6374 696f 6e54  remoteSelectionT
+000007f0: 6865 6d65 203d 2045 6469 746f 7256 6965  heme = EditorVie
+00000800: 772e 6261 7365 5468 656d 6528 7b0a 2020  w.baseTheme({.  
+00000810: 272e 6a70 2d72 656d 6f74 652d 6375 7273  '.jp-remote-curs
+00000820: 6f72 273a 207b 0a20 2020 2062 6f72 6465  or': {.    borde
+00000830: 724c 6566 743a 2027 3170 7820 736f 6c69  rLeft: '1px soli
+00000840: 6420 626c 6163 6b27 2c0a 2020 2020 6d61  d black',.    ma
+00000850: 7267 696e 4c65 6674 3a20 272d 3170 7827  rginLeft: '-1px'
+00000860: 0a20 207d 2c0a 2020 272e 6a70 2d72 656d  .  },.  '.jp-rem
+00000870: 6f74 652d 6375 7273 6f72 2e6a 702d 6d6f  ote-cursor.jp-mo
+00000880: 642d 7072 696d 6172 7927 3a20 7b0a 2020  d-primary': {.  
+00000890: 2020 626f 7264 6572 4c65 6674 5769 6474    borderLeftWidt
+000008a0: 683a 2027 3270 7827 0a20 207d 2c0a 2020  h: '2px'.  },.  
+000008b0: 272e 6a70 2d72 656d 6f74 652d 7365 6c65  '.jp-remote-sele
+000008c0: 6374 696f 6e27 3a20 7b0a 2020 2020 6f70  ction': {.    op
+000008d0: 6163 6974 793a 2030 2e35 0a20 207d 2c0a  acity: 0.5.  },.
+000008e0: 2020 272e 636d 2d74 6f6f 6c74 6970 273a    '.cm-tooltip':
+000008f0: 207b 0a20 2020 2062 6f72 6465 723a 2027   {.    border: '
+00000900: 6e6f 6e65 270a 2020 7d2c 0a20 2027 2e63  none'.  },.  '.c
+00000910: 6d2d 746f 6f6c 7469 7020 2e6a 702d 7265  m-tooltip .jp-re
+00000920: 6d6f 7465 2d75 7365 7249 6e66 6f27 3a20  mote-userInfo': 
+00000930: 7b0a 2020 2020 636f 6c6f 723a 2027 7661  {.    color: 'va
+00000940: 7228 2d2d 6a70 2d75 692d 696e 7665 7273  r(--jp-ui-invers
+00000950: 652d 666f 6e74 2d63 6f6c 6f72 3029 272c  e-font-color0)',
+00000960: 0a20 2020 2070 6164 6469 6e67 3a20 2730  .    padding: '0
+00000970: 7078 2032 7078 270a 2020 7d0a 7d29 3b0a  px 2px'.  }.});.
+00000980: 0a2f 2f20 544f 444f 2066 6978 2077 6869  .// TODO fix whi
+00000990: 6368 2075 7365 7220 6e65 6564 7320 7570  ch user needs up
+000009a0: 6461 7465 0a63 6f6e 7374 2072 656d 6f74  date.const remot
+000009b0: 6553 656c 6563 7469 6f6e 7341 6e6e 6f74  eSelectionsAnnot
+000009c0: 6174 696f 6e20 3d20 416e 6e6f 7461 7469  ation = Annotati
+000009d0: 6f6e 2e64 6566 696e 6528 293b 0a0a 2f2a  on.define();../*
+000009e0: 2a0a 202a 2057 7261 7070 6572 2061 726f  *. * Wrapper aro
+000009f0: 756e 6420 5265 6374 616e 676c 654d 6172  und RectangleMar
+00000a00: 6b65 7220 746f 2062 6520 6162 6c65 2074  ker to be able t
+00000a10: 6f20 7365 7420 7468 6520 7573 6572 2063  o set the user c
+00000a20: 6f6c 6f72 2066 6f72 2074 6865 2072 656d  olor for the rem
+00000a30: 6f74 6520 6375 7273 6f72 2061 6e64 2073  ote cursor and s
+00000a40: 656c 6563 7469 6f6e 2072 616e 6765 732e  election ranges.
+00000a50: 0a20 2a2f 0a63 6c61 7373 2052 656d 6f74  . */.class Remot
+00000a60: 654d 6172 6b65 7220 696d 706c 656d 656e  eMarker implemen
+00000a70: 7473 204c 6179 6572 4d61 726b 6572 207b  ts LayerMarker {
+00000a80: 0a20 202f 2a2a 0a20 2020 2a20 436f 6e73  .  /**.   * Cons
+00000a90: 7472 7563 746f 720a 2020 202a 0a20 2020  tructor.   *.   
+00000aa0: 2a20 4070 6172 616d 2073 7479 6c65 2053  * @param style S
+00000ab0: 7065 6369 6669 6320 7573 6572 2073 7479  pecific user sty
+00000ac0: 6c65 2074 6f20 6265 2061 7070 6c69 6564  le to be applied
+00000ad0: 206f 6e20 7468 6520 6d61 726b 6572 2065   on the marker e
+00000ae0: 6c65 6d65 6e74 0a20 2020 2a20 4070 6172  lement.   * @par
+00000af0: 616d 206d 6172 6b65 7220 7b40 6c69 6e6b  am marker {@link
+00000b00: 2052 6563 7461 6e67 6c65 4d61 726b 6572   RectangleMarker
+00000b10: 7d20 746f 2077 7261 700a 2020 202a 2f0a  } to wrap.   */.
+00000b20: 2020 636f 6e73 7472 7563 746f 7228 0a20    constructor(. 
+00000b30: 2020 2070 7269 7661 7465 2073 7479 6c65     private style
+00000b40: 3a20 5265 636f 7264 3c73 7472 696e 672c  : Record<string,
+00000b50: 2073 7472 696e 673e 2c0a 2020 2020 7072   string>,.    pr
+00000b60: 6976 6174 6520 6d61 726b 6572 3a20 5265  ivate marker: Re
+00000b70: 6374 616e 676c 654d 6172 6b65 720a 2020  ctangleMarker.  
+00000b80: 2920 7b7d 0a0a 2020 6472 6177 2829 3a20  ) {}..  draw(): 
+00000b90: 4854 4d4c 4469 7645 6c65 6d65 6e74 207b  HTMLDivElement {
+00000ba0: 0a20 2020 2063 6f6e 7374 2065 6c74 203d  .    const elt =
+00000bb0: 2074 6869 732e 6d61 726b 6572 2e64 7261   this.marker.dra
+00000bc0: 7728 293b 0a20 2020 2066 6f72 2028 636f  w();.    for (co
+00000bd0: 6e73 7420 5b6b 6579 2c20 7661 6c75 655d  nst [key, value]
+00000be0: 206f 6620 4f62 6a65 6374 2e65 6e74 7269   of Object.entri
+00000bf0: 6573 2874 6869 732e 7374 796c 6529 2920  es(this.style)) 
+00000c00: 7b0a 2020 2020 2020 2f2f 2040 7473 2d65  {.      // @ts-e
+00000c10: 7870 6563 742d 6572 726f 7220 556e 6b6e  xpect-error Unkn
+00000c20: 6f77 6e20 6b65 790a 2020 2020 2020 656c  own key.      el
+00000c30: 742e 7374 796c 655b 6b65 795d 203d 2076  t.style[key] = v
+00000c40: 616c 7565 3b0a 2020 2020 7d0a 2020 2020  alue;.    }.    
+00000c50: 7265 7475 726e 2065 6c74 3b0a 2020 7d0a  return elt;.  }.
+00000c60: 0a20 2065 7128 6f74 6865 723a 2052 656d  .  eq(other: Rem
+00000c70: 6f74 654d 6172 6b65 7229 3a20 626f 6f6c  oteMarker): bool
+00000c80: 6561 6e20 7b0a 2020 2020 7265 7475 726e  ean {.    return
+00000c90: 2028 0a20 2020 2020 2074 6869 732e 6d61   (.      this.ma
+00000ca0: 726b 6572 2e65 7128 6f74 6865 722e 6d61  rker.eq(other.ma
+00000cb0: 726b 6572 2920 2626 204a 534f 4e45 7874  rker) && JSONExt
+00000cc0: 2e64 6565 7045 7175 616c 2874 6869 732e  .deepEqual(this.
+00000cd0: 7374 796c 652c 206f 7468 6572 2e73 7479  style, other.sty
+00000ce0: 6c65 290a 2020 2020 293b 0a20 207d 0a0a  le).    );.  }..
+00000cf0: 2020 7570 6461 7465 2864 6f6d 3a20 4854    update(dom: HT
+00000d00: 4d4c 456c 656d 656e 742c 206f 6c64 4d61  MLElement, oldMa
+00000d10: 726b 6572 3a20 5265 6d6f 7465 4d61 726b  rker: RemoteMark
+00000d20: 6572 293a 2062 6f6f 6c65 616e 207b 0a20  er): boolean {. 
+00000d30: 2020 2066 6f72 2028 636f 6e73 7420 5b6b     for (const [k
+00000d40: 6579 2c20 7661 6c75 655d 206f 6620 4f62  ey, value] of Ob
+00000d50: 6a65 6374 2e65 6e74 7269 6573 2874 6869  ject.entries(thi
+00000d60: 732e 7374 796c 6529 2920 7b0a 2020 2020  s.style)) {.    
+00000d70: 2020 2f2f 2040 7473 2d65 7870 6563 742d    // @ts-expect-
+00000d80: 6572 726f 7220 556e 6b6e 6f77 6e20 6b65  error Unknown ke
+00000d90: 790a 2020 2020 2020 646f 6d2e 7374 796c  y.      dom.styl
+00000da0: 655b 6b65 795d 203d 2076 616c 7565 3b0a  e[key] = value;.
+00000db0: 2020 2020 7d0a 2020 2020 7265 7475 726e      }.    return
+00000dc0: 2074 6869 732e 6d61 726b 6572 2e75 7064   this.marker.upd
+00000dd0: 6174 6528 646f 6d2c 206f 6c64 4d61 726b  ate(dom, oldMark
+00000de0: 6572 2e6d 6172 6b65 7229 3b0a 2020 7d0a  er.marker);.  }.
+00000df0: 7d0a 0a2f 2a2a 0a20 2a20 4578 7465 6e73  }../**. * Extens
+00000e00: 696f 6e20 6465 6669 6e69 6e67 2061 206e  ion defining a n
+00000e10: 6577 2065 6469 746f 7220 6c61 7965 7220  ew editor layer 
+00000e20: 7374 6f72 696e 6720 7468 6520 7265 6d6f  storing the remo
+00000e30: 7465 2075 7365 7220 6375 7273 6f72 730a  te user cursors.
+00000e40: 202a 2f0a 636f 6e73 7420 7265 6d6f 7465   */.const remote
+00000e50: 4375 7273 6f72 734c 6179 6572 203d 206c  CursorsLayer = l
+00000e60: 6179 6572 287b 0a20 2061 626f 7665 3a20  ayer({.  above: 
+00000e70: 7472 7565 2c0a 2020 6d61 726b 6572 7328  true,.  markers(
+00000e80: 7669 6577 2920 7b0a 2020 2020 636f 6e73  view) {.    cons
+00000e90: 7420 7b20 6177 6172 656e 6573 732c 2079  t { awareness, y
+00000ea0: 7465 7874 207d 203d 2076 6965 772e 7374  text } = view.st
+00000eb0: 6174 652e 6661 6365 7428 6564 6974 6f72  ate.facet(editor
+00000ec0: 4177 6172 656e 6573 7346 6163 6574 293b  AwarenessFacet);
+00000ed0: 0a20 2020 2063 6f6e 7374 2079 646f 6320  .    const ydoc 
+00000ee0: 3d20 7974 6578 742e 646f 6321 3b0a 2020  = ytext.doc!;.  
+00000ef0: 2020 636f 6e73 7420 6375 7273 6f72 733a    const cursors:
+00000f00: 204c 6179 6572 4d61 726b 6572 5b5d 203d   LayerMarker[] =
+00000f10: 205b 5d3b 0a20 2020 2061 7761 7265 6e65   [];.    awarene
+00000f20: 7373 2e67 6574 5374 6174 6573 2829 2e66  ss.getStates().f
+00000f30: 6f72 4561 6368 2828 7374 6174 653a 2049  orEach((state: I
+00000f40: 4177 6172 656e 6573 7353 7461 7465 2c20  AwarenessState, 
+00000f50: 636c 6965 6e74 4944 2920 3d3e 207b 0a20  clientID) => {. 
+00000f60: 2020 2020 2069 6620 2863 6c69 656e 7449       if (clientI
+00000f70: 4420 3d3d 3d20 6177 6172 656e 6573 732e  D === awareness.
+00000f80: 646f 632e 636c 6965 6e74 4944 2920 7b0a  doc.clientID) {.
+00000f90: 2020 2020 2020 2020 7265 7475 726e 3b0a          return;.
+00000fa0: 2020 2020 2020 7d0a 0a20 2020 2020 2063        }..      c
+00000fb0: 6f6e 7374 2063 7572 736f 7273 5f20 3d20  onst cursors_ = 
+00000fc0: 7374 6174 652e 6375 7273 6f72 733b 0a20  state.cursors;. 
+00000fd0: 2020 2020 2066 6f72 2028 636f 6e73 7420       for (const 
+00000fe0: 6375 7273 6f72 206f 6620 6375 7273 6f72  cursor of cursor
+00000ff0: 735f 203f 3f20 5b5d 2920 7b0a 2020 2020  s_ ?? []) {.    
+00001000: 2020 2020 6966 2028 2163 7572 736f 723f      if (!cursor?
+00001010: 2e61 6e63 686f 7220 7c7c 2021 6375 7273  .anchor || !curs
+00001020: 6f72 3f2e 6865 6164 2920 7b0a 2020 2020  or?.head) {.    
+00001030: 2020 2020 2020 7265 7475 726e 3b0a 2020        return;.  
+00001040: 2020 2020 2020 7d0a 0a20 2020 2020 2020        }..       
+00001050: 2063 6f6e 7374 2061 6e63 686f 7220 3d20   const anchor = 
+00001060: 6372 6561 7465 4162 736f 6c75 7465 506f  createAbsolutePo
+00001070: 7369 7469 6f6e 4672 6f6d 5265 6c61 7469  sitionFromRelati
+00001080: 7665 506f 7369 7469 6f6e 280a 2020 2020  vePosition(.    
+00001090: 2020 2020 2020 6375 7273 6f72 2e61 6e63        cursor.anc
+000010a0: 686f 722c 0a20 2020 2020 2020 2020 2079  hor,.          y
+000010b0: 646f 630a 2020 2020 2020 2020 293b 0a20  doc.        );. 
+000010c0: 2020 2020 2020 2063 6f6e 7374 2068 6561         const hea
+000010d0: 6420 3d20 6372 6561 7465 4162 736f 6c75  d = createAbsolu
+000010e0: 7465 506f 7369 7469 6f6e 4672 6f6d 5265  tePositionFromRe
+000010f0: 6c61 7469 7665 506f 7369 7469 6f6e 280a  lativePosition(.
+00001100: 2020 2020 2020 2020 2020 6375 7273 6f72            cursor
+00001110: 2e68 6561 642c 0a20 2020 2020 2020 2020  .head,.         
+00001120: 2079 646f 630a 2020 2020 2020 2020 293b   ydoc.        );
+00001130: 0a20 2020 2020 2020 2069 6620 2861 6e63  .        if (anc
+00001140: 686f 723f 2e74 7970 6520 213d 3d20 7974  hor?.type !== yt
+00001150: 6578 7420 7c7c 2068 6561 643f 2e74 7970  ext || head?.typ
+00001160: 6520 213d 3d20 7974 6578 7429 207b 0a20  e !== ytext) {. 
+00001170: 2020 2020 2020 2020 2072 6574 7572 6e3b           return;
+00001180: 0a20 2020 2020 2020 207d 0a0a 2020 2020  .        }..    
+00001190: 2020 2020 636f 6e73 7420 636c 6173 734e      const classN
+000011a0: 616d 6520 3d0a 2020 2020 2020 2020 2020  ame =.          
+000011b0: 6375 7273 6f72 2e70 7269 6d61 7279 203f  cursor.primary ?
+000011c0: 3f20 7472 7565 0a20 2020 2020 2020 2020  ? true.         
+000011d0: 2020 203f 2027 6a70 2d72 656d 6f74 652d     ? 'jp-remote-
+000011e0: 6375 7273 6f72 206a 702d 6d6f 642d 7072  cursor jp-mod-pr
+000011f0: 696d 6172 7927 0a20 2020 2020 2020 2020  imary'.         
+00001200: 2020 203a 2027 6a70 2d72 656d 6f74 652d     : 'jp-remote-
+00001210: 6375 7273 6f72 273b 0a20 2020 2020 2020  cursor';.       
+00001220: 2063 6f6e 7374 2063 7572 736f 725f 203d   const cursor_ =
+00001230: 2045 6469 746f 7253 656c 6563 7469 6f6e   EditorSelection
+00001240: 2e63 7572 736f 7228 0a20 2020 2020 2020  .cursor(.       
+00001250: 2020 2068 6561 642e 696e 6465 782c 0a20     head.index,. 
+00001260: 2020 2020 2020 2020 2068 6561 642e 696e           head.in
+00001270: 6465 7820 3e20 616e 6368 6f72 2e69 6e64  dex > anchor.ind
+00001280: 6578 203f 202d 3120 3a20 310a 2020 2020  ex ? -1 : 1.    
+00001290: 2020 2020 293b 0a20 2020 2020 2020 2066      );.        f
+000012a0: 6f72 2028 636f 6e73 7420 7069 6563 6520  or (const piece 
+000012b0: 6f66 2052 6563 7461 6e67 6c65 4d61 726b  of RectangleMark
+000012c0: 6572 2e66 6f72 5261 6e67 6528 0a20 2020  er.forRange(.   
+000012d0: 2020 2020 2020 2076 6965 772c 0a20 2020         view,.   
+000012e0: 2020 2020 2020 2063 6c61 7373 4e61 6d65         className
+000012f0: 2c0a 2020 2020 2020 2020 2020 6375 7273  ,.          curs
+00001300: 6f72 5f0a 2020 2020 2020 2020 2929 207b  or_.        )) {
+00001310: 0a20 2020 2020 2020 2020 202f 2f20 5772  .          // Wr
+00001320: 6170 2074 6865 2072 6563 7461 6e67 6c65  ap the rectangle
+00001330: 206d 6172 6b65 7220 746f 2073 6574 2074   marker to set t
+00001340: 6865 2075 7365 7220 636f 6c6f 720a 2020  he user color.  
+00001350: 2020 2020 2020 2020 6375 7273 6f72 732e          cursors.
+00001360: 7075 7368 280a 2020 2020 2020 2020 2020  push(.          
+00001370: 2020 6e65 7720 5265 6d6f 7465 4d61 726b    new RemoteMark
+00001380: 6572 280a 2020 2020 2020 2020 2020 2020  er(.            
+00001390: 2020 7b20 626f 7264 6572 4c65 6674 436f    { borderLeftCo
+000013a0: 6c6f 723a 2073 7461 7465 2e75 7365 723f  lor: state.user?
+000013b0: 2e63 6f6c 6f72 203f 3f20 2762 6c61 636b  .color ?? 'black
+000013c0: 2720 7d2c 0a20 2020 2020 2020 2020 2020  ' },.           
+000013d0: 2020 2070 6965 6365 0a20 2020 2020 2020     piece.       
+000013e0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+000013f0: 2029 3b0a 2020 2020 2020 2020 7d0a 2020   );.        }.  
+00001400: 2020 2020 7d0a 2020 2020 7d29 3b0a 2020      }.    });.  
+00001410: 2020 7265 7475 726e 2063 7572 736f 7273    return cursors
+00001420: 3b0a 2020 7d2c 0a20 2075 7064 6174 6528  ;.  },.  update(
+00001430: 7570 6461 7465 2c20 6c61 7965 7229 207b  update, layer) {
+00001440: 0a20 2020 2072 6574 7572 6e20 2121 7570  .    return !!up
+00001450: 6461 7465 2e74 7261 6e73 6163 7469 6f6e  date.transaction
+00001460: 732e 6669 6e64 2874 203d 3e0a 2020 2020  s.find(t =>.    
+00001470: 2020 742e 616e 6e6f 7461 7469 6f6e 2872    t.annotation(r
+00001480: 656d 6f74 6553 656c 6563 7469 6f6e 7341  emoteSelectionsA
+00001490: 6e6e 6f74 6174 696f 6e29 0a20 2020 2029  nnotation).    )
+000014a0: 3b0a 2020 7d2c 0a20 2063 6c61 7373 3a20  ;.  },.  class: 
+000014b0: 276a 702d 7265 6d6f 7465 2d63 7572 736f  'jp-remote-curso
+000014c0: 7273 270a 7d29 3b0a 0a2f 2a2a 0a20 2a20  rs'.});../**. * 
+000014d0: 546f 6f6c 7469 7020 6578 7465 6e73 696f  Tooltip extensio
+000014e0: 6e20 746f 2064 6973 706c 6179 2075 7365  n to display use
+000014f0: 7220 6469 7370 6c61 7920 6e61 6d65 2061  r display name a
+00001500: 7420 6375 7273 6f72 2070 6f73 6974 696f  t cursor positio
+00001510: 6e0a 202a 2f0a 636f 6e73 7420 7573 6572  n. */.const user
+00001520: 486f 7665 7220 3d20 686f 7665 7254 6f6f  Hover = hoverToo
+00001530: 6c74 6970 280a 2020 2876 6965 772c 2070  ltip(.  (view, p
+00001540: 6f73 2920 3d3e 207b 0a20 2020 2063 6f6e  os) => {.    con
+00001550: 7374 207b 2061 7761 7265 6e65 7373 2c20  st { awareness, 
+00001560: 7974 6578 7420 7d20 3d20 7669 6577 2e73  ytext } = view.s
+00001570: 7461 7465 2e66 6163 6574 2865 6469 746f  tate.facet(edito
+00001580: 7241 7761 7265 6e65 7373 4661 6365 7429  rAwarenessFacet)
+00001590: 3b0a 2020 2020 636f 6e73 7420 7964 6f63  ;.    const ydoc
+000015a0: 203d 2079 7465 7874 2e64 6f63 213b 0a0a   = ytext.doc!;..
+000015b0: 2020 2020 666f 7220 2863 6f6e 7374 205b      for (const [
+000015c0: 636c 6965 6e74 4944 2c20 7374 6174 655d  clientID, state]
+000015d0: 206f 6620 6177 6172 656e 6573 732e 6765   of awareness.ge
+000015e0: 7453 7461 7465 7328 2929 207b 0a20 2020  tStates()) {.   
+000015f0: 2020 2069 6620 2863 6c69 656e 7449 4420     if (clientID 
+00001600: 3d3d 3d20 6177 6172 656e 6573 732e 646f  === awareness.do
+00001610: 632e 636c 6965 6e74 4944 2920 7b0a 2020  c.clientID) {.  
+00001620: 2020 2020 2020 636f 6e74 696e 7565 3b0a        continue;.
+00001630: 2020 2020 2020 7d0a 0a20 2020 2020 2066        }..      f
+00001640: 6f72 2028 636f 6e73 7420 6375 7273 6f72  or (const cursor
+00001650: 206f 6620 7374 6174 652e 6375 7273 6f72   of state.cursor
+00001660: 7320 3f3f 205b 5d29 207b 0a20 2020 2020  s ?? []) {.     
+00001670: 2020 2069 6620 2821 6375 7273 6f72 3f2e     if (!cursor?.
+00001680: 6865 6164 2920 7b0a 2020 2020 2020 2020  head) {.        
+00001690: 2020 636f 6e74 696e 7565 3b0a 2020 2020    continue;.    
+000016a0: 2020 2020 7d0a 2020 2020 2020 2020 636f      }.        co
+000016b0: 6e73 7420 6865 6164 203d 2063 7265 6174  nst head = creat
+000016c0: 6541 6273 6f6c 7574 6550 6f73 6974 696f  eAbsolutePositio
+000016d0: 6e46 726f 6d52 656c 6174 6976 6550 6f73  nFromRelativePos
+000016e0: 6974 696f 6e28 0a20 2020 2020 2020 2020  ition(.         
+000016f0: 2063 7572 736f 722e 6865 6164 2c0a 2020   cursor.head,.  
+00001700: 2020 2020 2020 2020 7964 6f63 0a20 2020          ydoc.   
+00001710: 2020 2020 2029 3b0a 2020 2020 2020 2020       );.        
+00001720: 6966 2028 6865 6164 3f2e 7479 7065 2021  if (head?.type !
+00001730: 3d3d 2079 7465 7874 2920 7b0a 2020 2020  == ytext) {.    
+00001740: 2020 2020 2020 636f 6e74 696e 7565 3b0a        continue;.
+00001750: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+00001760: 2020 2f2f 2055 7365 2073 6f6d 6520 6d61    // Use some ma
+00001770: 7267 696e 2061 726f 756e 6420 7468 6520  rgin around the 
+00001780: 6375 7273 6f72 2074 6f20 6469 7370 6c61  cursor to displa
+00001790: 7920 7468 6520 7573 6572 2e0a 2020 2020  y the user..    
+000017a0: 2020 2020 6966 2028 6865 6164 2e69 6e64      if (head.ind
+000017b0: 6578 202d 2033 203c 3d20 706f 7320 2626  ex - 3 <= pos &&
+000017c0: 2070 6f73 203c 3d20 6865 6164 2e69 6e64   pos <= head.ind
+000017d0: 6578 202b 2033 2920 7b0a 2020 2020 2020  ex + 3) {.      
+000017e0: 2020 2020 7265 7475 726e 207b 0a20 2020      return {.   
+000017f0: 2020 2020 2020 2020 2070 6f73 3a20 6865           pos: he
+00001800: 6164 2e69 6e64 6578 2c0a 2020 2020 2020  ad.index,.      
+00001810: 2020 2020 2020 6162 6f76 653a 2074 7275        above: tru
+00001820: 652c 0a20 2020 2020 2020 2020 2020 2063  e,.            c
+00001830: 7265 6174 653a 2028 2920 3d3e 207b 0a20  reate: () => {. 
+00001840: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
+00001850: 7374 2064 6f6d 203d 2064 6f63 756d 656e  st dom = documen
+00001860: 742e 6372 6561 7465 456c 656d 656e 7428  t.createElement(
+00001870: 2764 6976 2729 3b0a 2020 2020 2020 2020  'div');.        
+00001880: 2020 2020 2020 646f 6d2e 636c 6173 734c        dom.classL
+00001890: 6973 742e 6164 6428 276a 702d 7265 6d6f  ist.add('jp-remo
+000018a0: 7465 2d75 7365 7249 6e66 6f27 293b 0a20  te-userInfo');. 
+000018b0: 2020 2020 2020 2020 2020 2020 2064 6f6d               dom
+000018c0: 2e73 7479 6c65 2e62 6163 6b67 726f 756e  .style.backgroun
+000018d0: 6443 6f6c 6f72 203d 2073 7461 7465 2e75  dColor = state.u
+000018e0: 7365 723f 2e63 6f6c 6f72 203f 3f20 2764  ser?.color ?? 'd
+000018f0: 6172 6b67 7265 7927 3b0a 2020 2020 2020  arkgrey';.      
+00001900: 2020 2020 2020 2020 646f 6d2e 7465 7874          dom.text
+00001910: 436f 6e74 656e 7420 3d0a 2020 2020 2020  Content =.      
+00001920: 2020 2020 2020 2020 2020 2873 7461 7465            (state
+00001930: 2061 7320 4941 7761 7265 6e65 7373 5374   as IAwarenessSt
+00001940: 6174 6529 2e75 7365 723f 2e64 6973 706c  ate).user?.displ
+00001950: 6179 5f6e 616d 6520 3f3f 2027 416e 6f6e  ay_name ?? 'Anon
+00001960: 796d 6f75 7327 3b0a 2020 2020 2020 2020  ymous';.        
+00001970: 2020 2020 2020 7265 7475 726e 207b 2064        return { d
+00001980: 6f6d 207d 3b0a 2020 2020 2020 2020 2020  om };.          
+00001990: 2020 7d0a 2020 2020 2020 2020 2020 7d3b    }.          };
+000019a0: 0a20 2020 2020 2020 207d 0a20 2020 2020  .        }.     
+000019b0: 207d 0a20 2020 207d 0a0a 2020 2020 7265   }.    }..    re
+000019c0: 7475 726e 206e 756c 6c3b 0a20 207d 2c0a  turn null;.  },.
+000019d0: 2020 7b0a 2020 2020 6869 6465 4f6e 3a20    {.    hideOn: 
+000019e0: 2874 722c 2074 6f6f 6c74 6970 2920 3d3e  (tr, tooltip) =>
+000019f0: 2021 2174 722e 616e 6e6f 7461 7469 6f6e   !!tr.annotation
+00001a00: 2872 656d 6f74 6553 656c 6563 7469 6f6e  (remoteSelection
+00001a10: 7341 6e6e 6f74 6174 696f 6e29 2c0a 2020  sAnnotation),.  
+00001a20: 2020 686f 7665 7254 696d 653a 2030 0a20    hoverTime: 0. 
+00001a30: 207d 0a29 3b0a 0a2f 2a2a 0a20 2a20 4578   }.);../**. * Ex
+00001a40: 7465 6e73 696f 6e20 6465 6669 6e69 6e67  tension defining
+00001a50: 2061 206e 6577 2065 6469 746f 7220 6c61   a new editor la
+00001a60: 7965 7220 7374 6f72 696e 6720 7468 6520  yer storing the 
+00001a70: 7265 6d6f 7465 2073 656c 6563 7469 6f6e  remote selection
+00001a80: 730a 202a 2f0a 636f 6e73 7420 7265 6d6f  s. */.const remo
+00001a90: 7465 5365 6c65 6374 696f 6e4c 6179 6572  teSelectionLayer
+00001aa0: 203d 206c 6179 6572 287b 0a20 2061 626f   = layer({.  abo
+00001ab0: 7665 3a20 6661 6c73 652c 0a20 206d 6172  ve: false,.  mar
+00001ac0: 6b65 7273 2876 6965 7729 207b 0a20 2020  kers(view) {.   
+00001ad0: 2063 6f6e 7374 207b 2061 7761 7265 6e65   const { awarene
+00001ae0: 7373 2c20 7974 6578 7420 7d20 3d20 7669  ss, ytext } = vi
+00001af0: 6577 2e73 7461 7465 2e66 6163 6574 2865  ew.state.facet(e
+00001b00: 6469 746f 7241 7761 7265 6e65 7373 4661  ditorAwarenessFa
+00001b10: 6365 7429 3b0a 2020 2020 636f 6e73 7420  cet);.    const 
+00001b20: 7964 6f63 203d 2079 7465 7874 2e64 6f63  ydoc = ytext.doc
+00001b30: 213b 0a20 2020 2063 6f6e 7374 2063 7572  !;.    const cur
+00001b40: 736f 7273 3a20 4c61 7965 724d 6172 6b65  sors: LayerMarke
+00001b50: 725b 5d20 3d20 5b5d 3b0a 2020 2020 6177  r[] = [];.    aw
+00001b60: 6172 656e 6573 732e 6765 7453 7461 7465  areness.getState
+00001b70: 7328 292e 666f 7245 6163 6828 2873 7461  s().forEach((sta
+00001b80: 7465 3a20 4941 7761 7265 6e65 7373 5374  te: IAwarenessSt
+00001b90: 6174 652c 2063 6c69 656e 7449 4429 203d  ate, clientID) =
+00001ba0: 3e20 7b0a 2020 2020 2020 6966 2028 636c  > {.      if (cl
+00001bb0: 6965 6e74 4944 203d 3d3d 2061 7761 7265  ientID === aware
+00001bc0: 6e65 7373 2e64 6f63 2e63 6c69 656e 7449  ness.doc.clientI
+00001bd0: 4429 207b 0a20 2020 2020 2020 2072 6574  D) {.        ret
+00001be0: 7572 6e3b 0a20 2020 2020 207d 0a0a 2020  urn;.      }..  
+00001bf0: 2020 2020 636f 6e73 7420 6375 7273 6f72      const cursor
+00001c00: 735f 203d 2073 7461 7465 2e63 7572 736f  s_ = state.curso
+00001c10: 7273 3b0a 2020 2020 2020 666f 7220 2863  rs;.      for (c
+00001c20: 6f6e 7374 2063 7572 736f 7220 6f66 2063  onst cursor of c
+00001c30: 7572 736f 7273 5f20 3f3f 205b 5d29 207b  ursors_ ?? []) {
+00001c40: 0a20 2020 2020 2020 2069 6620 2828 6375  .        if ((cu
+00001c50: 7273 6f72 2e65 6d70 7479 203f 3f20 7472  rsor.empty ?? tr
+00001c60: 7565 2920 7c7c 2021 6375 7273 6f72 3f2e  ue) || !cursor?.
+00001c70: 616e 6368 6f72 207c 7c20 2163 7572 736f  anchor || !curso
+00001c80: 723f 2e68 6561 6429 207b 0a20 2020 2020  r?.head) {.     
+00001c90: 2020 2020 2072 6574 7572 6e3b 0a20 2020       return;.   
+00001ca0: 2020 2020 207d 0a0a 2020 2020 2020 2020       }..        
+00001cb0: 636f 6e73 7420 616e 6368 6f72 203d 2063  const anchor = c
+00001cc0: 7265 6174 6541 6273 6f6c 7574 6550 6f73  reateAbsolutePos
+00001cd0: 6974 696f 6e46 726f 6d52 656c 6174 6976  itionFromRelativ
+00001ce0: 6550 6f73 6974 696f 6e28 0a20 2020 2020  ePosition(.     
+00001cf0: 2020 2020 2063 7572 736f 722e 616e 6368       cursor.anch
+00001d00: 6f72 2c0a 2020 2020 2020 2020 2020 7964  or,.          yd
+00001d10: 6f63 0a20 2020 2020 2020 2029 3b0a 2020  oc.        );.  
+00001d20: 2020 2020 2020 636f 6e73 7420 6865 6164        const head
+00001d30: 203d 2063 7265 6174 6541 6273 6f6c 7574   = createAbsolut
+00001d40: 6550 6f73 6974 696f 6e46 726f 6d52 656c  ePositionFromRel
+00001d50: 6174 6976 6550 6f73 6974 696f 6e28 0a20  ativePosition(. 
+00001d60: 2020 2020 2020 2020 2063 7572 736f 722e           cursor.
+00001d70: 6865 6164 2c0a 2020 2020 2020 2020 2020  head,.          
+00001d80: 7964 6f63 0a20 2020 2020 2020 2029 3b0a  ydoc.        );.
+00001d90: 2020 2020 2020 2020 6966 2028 616e 6368          if (anch
+00001da0: 6f72 3f2e 7479 7065 2021 3d3d 2079 7465  or?.type !== yte
+00001db0: 7874 207c 7c20 6865 6164 3f2e 7479 7065  xt || head?.type
+00001dc0: 2021 3d3d 2079 7465 7874 2920 7b0a 2020   !== ytext) {.  
+00001dd0: 2020 2020 2020 2020 7265 7475 726e 3b0a          return;.
+00001de0: 2020 2020 2020 2020 7d0a 0a20 2020 2020          }..     
+00001df0: 2020 2063 6f6e 7374 2063 6c61 7373 4e61     const classNa
+00001e00: 6d65 203d 2027 6a70 2d72 656d 6f74 652d  me = 'jp-remote-
+00001e10: 7365 6c65 6374 696f 6e27 3b0a 2020 2020  selection';.    
+00001e20: 2020 2020 666f 7220 2863 6f6e 7374 2070      for (const p
+00001e30: 6965 6365 206f 6620 5265 6374 616e 676c  iece of Rectangl
+00001e40: 654d 6172 6b65 722e 666f 7252 616e 6765  eMarker.forRange
+00001e50: 280a 2020 2020 2020 2020 2020 7669 6577  (.          view
+00001e60: 2c0a 2020 2020 2020 2020 2020 636c 6173  ,.          clas
+00001e70: 734e 616d 652c 0a20 2020 2020 2020 2020  sName,.         
+00001e80: 2045 6469 746f 7253 656c 6563 7469 6f6e   EditorSelection
+00001e90: 2e72 616e 6765 2861 6e63 686f 722e 696e  .range(anchor.in
+00001ea0: 6465 782c 2068 6561 642e 696e 6465 7829  dex, head.index)
+00001eb0: 0a20 2020 2020 2020 2029 2920 7b0a 2020  .        )) {.  
+00001ec0: 2020 2020 2020 2020 2f2f 2057 7261 7020          // Wrap 
+00001ed0: 7468 6520 7265 6374 616e 676c 6520 6d61  the rectangle ma
+00001ee0: 726b 6572 2074 6f20 7365 7420 7468 6520  rker to set the 
+00001ef0: 7573 6572 2063 6f6c 6f72 0a20 2020 2020  user color.     
+00001f00: 2020 2020 2063 7572 736f 7273 2e70 7573       cursors.pus
+00001f10: 6828 0a20 2020 2020 2020 2020 2020 206e  h(.            n
+00001f20: 6577 2052 656d 6f74 654d 6172 6b65 7228  ew RemoteMarker(
+00001f30: 0a20 2020 2020 2020 2020 2020 2020 207b  .              {
+00001f40: 2062 6163 6b67 726f 756e 6443 6f6c 6f72   backgroundColor
+00001f50: 3a20 7374 6174 652e 7573 6572 3f2e 636f  : state.user?.co
+00001f60: 6c6f 7220 3f3f 2027 626c 6163 6b27 207d  lor ?? 'black' }
+00001f70: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00001f80: 7069 6563 650a 2020 2020 2020 2020 2020  piece.          
+00001f90: 2020 290a 2020 2020 2020 2020 2020 293b    ).          );
+00001fa0: 0a20 2020 2020 2020 207d 0a20 2020 2020  .        }.     
+00001fb0: 207d 0a20 2020 207d 293b 0a20 2020 2072   }.    });.    r
+00001fc0: 6574 7572 6e20 6375 7273 6f72 733b 0a20  eturn cursors;. 
+00001fd0: 207d 2c0a 2020 7570 6461 7465 2875 7064   },.  update(upd
+00001fe0: 6174 652c 206c 6179 6572 2920 7b0a 2020  ate, layer) {.  
+00001ff0: 2020 7265 7475 726e 2021 2175 7064 6174    return !!updat
+00002000: 652e 7472 616e 7361 6374 696f 6e73 2e66  e.transactions.f
+00002010: 696e 6428 7420 3d3e 0a20 2020 2020 2074  ind(t =>.      t
+00002020: 2e61 6e6e 6f74 6174 696f 6e28 7265 6d6f  .annotation(remo
+00002030: 7465 5365 6c65 6374 696f 6e73 416e 6e6f  teSelectionsAnno
+00002040: 7461 7469 6f6e 290a 2020 2020 293b 0a20  tation).    );. 
+00002050: 207d 2c0a 2020 636c 6173 733a 2027 6a70   },.  class: 'jp
+00002060: 2d72 656d 6f74 652d 7365 6c65 6374 696f  -remote-selectio
+00002070: 6e73 270a 7d29 3b0a 0a2f 2a2a 0a20 2a20  ns'.});../**. * 
+00002080: 436f 6465 4d69 7272 6f72 2065 7874 656e  CodeMirror exten
+00002090: 7369 6f6e 2065 7863 6861 6e67 696e 6720  sion exchanging 
+000020a0: 616e 6420 6469 7370 6c61 7969 6e67 2072  and displaying r
+000020b0: 656d 6f74 6520 7573 6572 2073 656c 6563  emote user selec
+000020c0: 7469 6f6e 2072 616e 6765 7320 2869 6e63  tion ranges (inc
+000020d0: 6c75 6469 6e67 2063 7572 736f 7273 290a  luding cursors).
+000020e0: 202a 2f0a 636f 6e73 7420 7368 6f77 436f   */.const showCo
+000020f0: 6c6c 6162 6f72 6174 6f72 7320 3d20 5669  llaborators = Vi
+00002100: 6577 506c 7567 696e 2e66 726f 6d43 6c61  ewPlugin.fromCla
+00002110: 7373 280a 2020 636c 6173 7320 7b0a 2020  ss(.  class {.  
+00002120: 2020 6564 6974 6f72 4177 6172 656e 6573    editorAwarenes
+00002130: 733a 2045 6469 746f 7241 7761 7265 6e65  s: EditorAwarene
+00002140: 7373 3b0a 2020 2020 5f6c 6973 7465 6e65  ss;.    _listene
+00002150: 723a 2028 743a 207b 0a20 2020 2020 2061  r: (t: {.      a
+00002160: 6464 6564 3a20 4172 7261 793c 616e 793e  dded: Array<any>
+00002170: 3b0a 2020 2020 2020 7570 6461 7465 643a  ;.      updated:
+00002180: 2041 7272 6179 3c61 6e79 3e3b 0a20 2020   Array<any>;.   
+00002190: 2020 2072 656d 6f76 6564 3a20 4172 7261     removed: Arra
+000021a0: 793c 616e 793e 3b0a 2020 2020 7d29 203d  y<any>;.    }) =
+000021b0: 3e20 766f 6964 3b0a 0a20 2020 2063 6f6e  > void;..    con
+000021c0: 7374 7275 6374 6f72 2876 6965 773a 2045  structor(view: E
+000021d0: 6469 746f 7256 6965 7729 207b 0a20 2020  ditorView) {.   
+000021e0: 2020 2074 6869 732e 6564 6974 6f72 4177     this.editorAw
+000021f0: 6172 656e 6573 7320 3d20 7669 6577 2e73  areness = view.s
+00002200: 7461 7465 2e66 6163 6574 2865 6469 746f  tate.facet(edito
+00002210: 7241 7761 7265 6e65 7373 4661 6365 7429  rAwarenessFacet)
+00002220: 3b0a 2020 2020 2020 7468 6973 2e5f 6c69  ;.      this._li
+00002230: 7374 656e 6572 203d 2028 7b20 6164 6465  stener = ({ adde
+00002240: 642c 2075 7064 6174 6564 2c20 7265 6d6f  d, updated, remo
+00002250: 7665 6420 7d29 203d 3e20 7b0a 2020 2020  ved }) => {.    
+00002260: 2020 2020 636f 6e73 7420 636c 6965 6e74      const client
+00002270: 7320 3d20 6164 6465 642e 636f 6e63 6174  s = added.concat
+00002280: 2875 7064 6174 6564 292e 636f 6e63 6174  (updated).concat
+00002290: 2872 656d 6f76 6564 293b 0a20 2020 2020  (removed);.     
+000022a0: 2020 2069 6620 280a 2020 2020 2020 2020     if (.        
+000022b0: 2020 636c 6965 6e74 732e 6669 6e64 496e    clients.findIn
+000022c0: 6465 7828 0a20 2020 2020 2020 2020 2020  dex(.           
+000022d0: 2069 6420 3d3e 2069 6420 213d 3d20 7468   id => id !== th
+000022e0: 6973 2e65 6469 746f 7241 7761 7265 6e65  is.editorAwarene
+000022f0: 7373 2e61 7761 7265 6e65 7373 2e64 6f63  ss.awareness.doc
+00002300: 2e63 6c69 656e 7449 440a 2020 2020 2020  .clientID.      
+00002310: 2020 2020 2920 3e3d 2030 0a20 2020 2020      ) >= 0.     
+00002320: 2020 2029 207b 0a20 2020 2020 2020 2020     ) {.         
+00002330: 202f 2f20 5472 6963 6b20 746f 2067 6574   // Trick to get
+00002340: 2074 6865 2072 656d 6f74 6543 7572 736f   the remoteCurso
+00002350: 724c 6179 6572 7320 746f 2062 6520 7570  rLayers to be up
+00002360: 6461 7465 640a 2020 2020 2020 2020 2020  dated.          
+00002370: 7669 6577 2e64 6973 7061 7463 6828 7b20  view.dispatch({ 
+00002380: 616e 6e6f 7461 7469 6f6e 733a 205b 7265  annotations: [re
+00002390: 6d6f 7465 5365 6c65 6374 696f 6e73 416e  moteSelectionsAn
+000023a0: 6e6f 7461 7469 6f6e 2e6f 6628 5b5d 295d  notation.of([])]
+000023b0: 207d 293b 0a20 2020 2020 2020 207d 0a20   });.        }. 
+000023c0: 2020 2020 207d 3b0a 0a20 2020 2020 2074       };..      t
+000023d0: 6869 732e 6564 6974 6f72 4177 6172 656e  his.editorAwaren
+000023e0: 6573 732e 6177 6172 656e 6573 732e 6f6e  ess.awareness.on
+000023f0: 2827 6368 616e 6765 272c 2074 6869 732e  ('change', this.
+00002400: 5f6c 6973 7465 6e65 7229 3b0a 2020 2020  _listener);.    
+00002410: 7d0a 0a20 2020 2064 6573 7472 6f79 2829  }..    destroy()
+00002420: 3a20 766f 6964 207b 0a20 2020 2020 2074  : void {.      t
+00002430: 6869 732e 6564 6974 6f72 4177 6172 656e  his.editorAwaren
+00002440: 6573 732e 6177 6172 656e 6573 732e 6f66  ess.awareness.of
+00002450: 6628 2763 6861 6e67 6527 2c20 7468 6973  f('change', this
+00002460: 2e5f 6c69 7374 656e 6572 293b 0a20 2020  ._listener);.   
+00002470: 207d 0a0a 2020 2020 2f2a 2a0a 2020 2020   }..    /**.    
+00002480: 202a 2043 6f6d 6d75 6e69 6361 7465 2074   * Communicate t
+00002490: 6865 2063 7572 7265 6e74 2075 7365 7220  he current user 
+000024a0: 6375 7273 6f72 2070 6f73 6974 696f 6e20  cursor position 
+000024b0: 746f 2061 6c6c 2072 656d 6f74 6573 0a20  to all remotes. 
+000024c0: 2020 2020 2a2f 0a20 2020 2075 7064 6174      */.    updat
+000024d0: 6528 7570 6461 7465 3a20 5669 6577 5570  e(update: ViewUp
+000024e0: 6461 7465 293a 2076 6f69 6420 7b0a 2020  date): void {.  
+000024f0: 2020 2020 6966 2028 2175 7064 6174 652e      if (!update.
+00002500: 646f 6343 6861 6e67 6564 2026 2620 2175  docChanged && !u
+00002510: 7064 6174 652e 7365 6c65 6374 696f 6e53  pdate.selectionS
+00002520: 6574 2920 7b0a 2020 2020 2020 2020 7265  et) {.        re
+00002530: 7475 726e 3b0a 2020 2020 2020 7d0a 0a20  turn;.      }.. 
+00002540: 2020 2020 2063 6f6e 7374 207b 2061 7761       const { awa
+00002550: 7265 6e65 7373 2c20 7974 6578 7420 7d20  reness, ytext } 
+00002560: 3d20 7468 6973 2e65 6469 746f 7241 7761  = this.editorAwa
+00002570: 7265 6e65 7373 3b0a 2020 2020 2020 636f  reness;.      co
+00002580: 6e73 7420 6c6f 6361 6c41 7761 7265 6e65  nst localAwarene
+00002590: 7373 5374 6174 6520 3d0a 2020 2020 2020  ssState =.      
+000025a0: 2020 6177 6172 656e 6573 732e 6765 744c    awareness.getL
+000025b0: 6f63 616c 5374 6174 6528 2920 6173 2049  ocalState() as I
+000025c0: 4177 6172 656e 6573 7353 7461 7465 207c  AwarenessState |
+000025d0: 206e 756c 6c3b 0a0a 2020 2020 2020 2f2f   null;..      //
+000025e0: 2073 6574 206c 6f63 616c 2061 7761 7265   set local aware
+000025f0: 6e65 7373 2073 7461 7465 2028 7570 6461  ness state (upda
+00002600: 7465 2063 7572 736f 7273 290a 2020 2020  te cursors).    
+00002610: 2020 6966 2028 6c6f 6361 6c41 7761 7265    if (localAware
+00002620: 6e65 7373 5374 6174 6529 207b 0a20 2020  nessState) {.   
+00002630: 2020 2020 2063 6f6e 7374 2068 6173 466f       const hasFo
+00002640: 6375 7320 3d0a 2020 2020 2020 2020 2020  cus =.          
+00002650: 7570 6461 7465 2e76 6965 772e 6861 7346  update.view.hasF
+00002660: 6f63 7573 2026 2620 7570 6461 7465 2e76  ocus && update.v
+00002670: 6965 772e 646f 6d2e 6f77 6e65 7244 6f63  iew.dom.ownerDoc
+00002680: 756d 656e 742e 6861 7346 6f63 7573 2829  ument.hasFocus()
+00002690: 3b0a 2020 2020 2020 2020 636f 6e73 7420  ;.        const 
+000026a0: 7365 6c65 6374 696f 6e20 3d20 7570 6461  selection = upda
+000026b0: 7465 2e73 7461 7465 2e73 656c 6563 7469  te.state.selecti
+000026c0: 6f6e 3b0a 2020 2020 2020 2020 636f 6e73  on;.        cons
+000026d0: 7420 6375 7273 6f72 7320 3d20 6e65 7720  t cursors = new 
+000026e0: 4172 7261 793c 4943 7572 736f 7253 7461  Array<ICursorSta
+000026f0: 7465 3e28 293b 0a0a 2020 2020 2020 2020  te>();..        
+00002700: 6966 2028 6861 7346 6f63 7573 2026 2620  if (hasFocus && 
+00002710: 7365 6c65 6374 696f 6e29 207b 0a20 2020  selection) {.   
+00002720: 2020 2020 2020 2066 6f72 2028 636f 6e73         for (cons
+00002730: 7420 7220 6f66 2073 656c 6563 7469 6f6e  t r of selection
+00002740: 2e72 616e 6765 7329 207b 0a20 2020 2020  .ranges) {.     
+00002750: 2020 2020 2020 2063 6f6e 7374 2070 7269         const pri
+00002760: 6d61 7279 203d 2072 203d 3d3d 2073 656c  mary = r === sel
+00002770: 6563 7469 6f6e 2e6d 6169 6e3b 0a20 2020  ection.main;.   
+00002780: 2020 2020 2020 2020 2063 6f6e 7374 2061           const a
+00002790: 6e63 686f 7220 3d20 6372 6561 7465 5265  nchor = createRe
+000027a0: 6c61 7469 7665 506f 7369 7469 6f6e 4672  lativePositionFr
+000027b0: 6f6d 5479 7065 496e 6465 7828 7974 6578  omTypeIndex(ytex
+000027c0: 742c 2072 2e61 6e63 686f 7229 3b0a 2020  t, r.anchor);.  
+000027d0: 2020 2020 2020 2020 2020 636f 6e73 7420            const 
+000027e0: 6865 6164 203d 2063 7265 6174 6552 656c  head = createRel
+000027f0: 6174 6976 6550 6f73 6974 696f 6e46 726f  ativePositionFro
+00002800: 6d54 7970 6549 6e64 6578 2879 7465 7874  mTypeIndex(ytext
+00002810: 2c20 722e 6865 6164 293b 0a0a 2020 2020  , r.head);..    
+00002820: 2020 2020 2020 2020 6375 7273 6f72 732e          cursors.
+00002830: 7075 7368 287b 0a20 2020 2020 2020 2020  push({.         
+00002840: 2020 2020 2061 6e63 686f 722c 0a20 2020       anchor,.   
+00002850: 2020 2020 2020 2020 2020 2068 6561 642c             head,
+00002860: 0a20 2020 2020 2020 2020 2020 2020 2070  .              p
+00002870: 7269 6d61 7279 2c0a 2020 2020 2020 2020  rimary,.        
+00002880: 2020 2020 2020 656d 7074 793a 2072 2e65        empty: r.e
+00002890: 6d70 7479 0a20 2020 2020 2020 2020 2020  mpty.           
+000028a0: 207d 293b 0a20 2020 2020 2020 2020 207d   });.          }
+000028b0: 0a0a 2020 2020 2020 2020 2020 6966 2028  ..          if (
+000028c0: 216c 6f63 616c 4177 6172 656e 6573 7353  !localAwarenessS
+000028d0: 7461 7465 2e63 7572 736f 7273 207c 7c20  tate.cursors || 
+000028e0: 6375 7273 6f72 732e 6c65 6e67 7468 203e  cursors.length >
+000028f0: 2030 2920 7b0a 2020 2020 2020 2020 2020   0) {.          
+00002900: 2020 636f 6e73 7420 6f6c 6443 7572 736f    const oldCurso
+00002910: 7273 203d 206c 6f63 616c 4177 6172 656e  rs = localAwaren
+00002920: 6573 7353 7461 7465 2e63 7572 736f 7273  essState.cursors
+00002930: 3f2e 6d61 7028 6375 7273 6f72 203d 3e20  ?.map(cursor => 
+00002940: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00002950: 7265 7475 726e 207b 0a20 2020 2020 2020  return {.       
+00002960: 2020 2020 2020 2020 202e 2e2e 6375 7273           ...curs
+00002970: 6f72 2c0a 2020 2020 2020 2020 2020 2020  or,.            
+00002980: 2020 2020 616e 6368 6f72 3a20 6375 7273      anchor: curs
+00002990: 6f72 3f2e 616e 6368 6f72 0a20 2020 2020  or?.anchor.     
+000029a0: 2020 2020 2020 2020 2020 2020 203f 2063               ? c
+000029b0: 7265 6174 6552 656c 6174 6976 6550 6f73  reateRelativePos
+000029c0: 6974 696f 6e46 726f 6d4a 534f 4e28 6375  itionFromJSON(cu
+000029d0: 7273 6f72 2e61 6e63 686f 7229 0a20 2020  rsor.anchor).   
+000029e0: 2020 2020 2020 2020 2020 2020 2020 203a                 :
+000029f0: 206e 756c 6c2c 0a20 2020 2020 2020 2020   null,.         
+00002a00: 2020 2020 2020 2068 6561 643a 2063 7572         head: cur
+00002a10: 736f 723f 2e68 6561 640a 2020 2020 2020  sor?.head.      
+00002a20: 2020 2020 2020 2020 2020 2020 3f20 6372              ? cr
+00002a30: 6561 7465 5265 6c61 7469 7665 506f 7369  eateRelativePosi
+00002a40: 7469 6f6e 4672 6f6d 4a53 4f4e 2863 7572  tionFromJSON(cur
+00002a50: 736f 722e 6865 6164 290a 2020 2020 2020  sor.head).      
+00002a60: 2020 2020 2020 2020 2020 2020 3a20 6e75              : nu
+00002a70: 6c6c 0a20 2020 2020 2020 2020 2020 2020  ll.             
+00002a80: 207d 3b0a 2020 2020 2020 2020 2020 2020   };.            
+00002a90: 7d29 3b0a 2020 2020 2020 2020 2020 2020  });.            
+00002aa0: 6966 2028 214a 534f 4e45 7874 2e64 6565  if (!JSONExt.dee
+00002ab0: 7045 7175 616c 2863 7572 736f 7273 2061  pEqual(cursors a
+00002ac0: 7320 616e 792c 206f 6c64 4375 7273 6f72  s any, oldCursor
+00002ad0: 7320 6173 2061 6e79 2929 207b 0a20 2020  s as any)) {.   
+00002ae0: 2020 2020 2020 2020 2020 202f 2f20 5570             // Up
+00002af0: 6461 7465 2063 7572 736f 7273 0a20 2020  date cursors.   
+00002b00: 2020 2020 2020 2020 2020 2061 7761 7265             aware
+00002b10: 6e65 7373 2e73 6574 4c6f 6361 6c53 7461  ness.setLocalSta
+00002b20: 7465 4669 656c 6428 2763 7572 736f 7273  teField('cursors
+00002b30: 272c 2063 7572 736f 7273 293b 0a20 2020  ', cursors);.   
+00002b40: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
+00002b50: 2020 2020 207d 0a20 2020 2020 2020 207d       }.        }
+00002b60: 0a20 2020 2020 207d 0a20 2020 207d 0a20  .      }.    }. 
+00002b70: 207d 2c0a 2020 7b0a 2020 2020 7072 6f76   },.  {.    prov
+00002b80: 6964 653a 2028 2920 3d3e 207b 0a20 2020  ide: () => {.   
+00002b90: 2020 2072 6574 7572 6e20 5b0a 2020 2020     return [.    
 00002ba0: 2020 2020 7265 6d6f 7465 5365 6c65 6374      remoteSelect
 00002bb0: 696f 6e54 6865 6d65 2c0a 2020 2020 2020  ionTheme,.      
-00002bc0: 2020 2020 2020 7265 6d6f 7465 4375 7273        remoteCurs
-00002bd0: 6f72 734c 6179 6572 2c0a 2020 2020 2020  orsLayer,.      
-00002be0: 2020 2020 2020 7265 6d6f 7465 5365 6c65        remoteSele
-00002bf0: 6374 696f 6e4c 6179 6572 2c0a 2020 2020  ctionLayer,.    
-00002c00: 2020 2020 2020 2020 7573 6572 486f 7665          userHove
-00002c10: 722c 0a20 2020 2020 2020 2020 2020 202f  r,.            /
-00002c20: 2f20 4173 2077 6520 7573 6520 7265 6c61  / As we use rela
-00002c30: 7469 7665 2070 6f73 6974 696f 6e69 6e67  tive positioning
-00002c40: 206f 6620 7769 6467 6574 2c20 7468 6520   of widget, the 
-00002c50: 746f 6f6c 7469 7020 6d75 7374 2062 6520  tooltip must be 
-00002c60: 706f 7369 7469 6f6e 6564 2061 6273 6f6c  positioned absol
-00002c70: 7574 656c 790a 2020 2020 2020 2020 2020  utely.          
-00002c80: 2020 2f2f 2041 6e64 2077 6520 6174 7461    // And we atta
-00002c90: 6368 2074 6865 2074 6f6f 6c74 6970 2074  ch the tooltip t
-00002ca0: 6f20 7468 6520 626f 6479 2074 6f20 6176  o the body to av
-00002cb0: 6f69 6420 6f76 6572 666c 6f77 2072 756c  oid overflow rul
-00002cc0: 6573 0a20 2020 2020 2020 2020 2020 2074  es.            t
-00002cd0: 6f6f 6c74 6970 7328 7b20 706f 7369 7469  ooltips({ positi
-00002ce0: 6f6e 3a20 2761 6273 6f6c 7574 6527 2c20  on: 'absolute', 
-00002cf0: 7061 7265 6e74 3a20 646f 6375 6d65 6e74  parent: document
-00002d00: 2e62 6f64 7920 7d29 0a20 2020 2020 2020  .body }).       
-00002d10: 205d 3b0a 2020 2020 7d0a 7d29 3b0a 2f2a   ];.    }.});./*
-00002d20: 2a0a 202a 2043 6f64 654d 6972 726f 7220  *. * CodeMirror 
-00002d30: 6578 7465 6e73 696f 6e20 746f 2064 6973  extension to dis
-00002d40: 706c 6179 2072 656d 6f74 6520 7573 6572  play remote user
-00002d50: 7320 6375 7273 6f72 730a 202a 0a20 2a20  s cursors. *. * 
-00002d60: 4070 6172 616d 2063 6f6e 6669 6720 4564  @param config Ed
-00002d70: 6974 6f72 2073 6f75 7263 6520 616e 6420  itor source and 
-00002d80: 6177 6172 656e 6573 730a 202a 2040 7265  awareness. * @re
-00002d90: 7475 726e 7320 436f 6465 4d69 7272 6f72  turns CodeMirror
-00002da0: 2065 7874 656e 7369 6f6e 0a20 2a2f 0a65   extension. */.e
-00002db0: 7870 6f72 7420 6675 6e63 7469 6f6e 2072  xport function r
-00002dc0: 656d 6f74 6555 7365 7243 7572 736f 7273  emoteUserCursors
-00002dd0: 2863 6f6e 6669 6729 207b 0a20 2020 2072  (config) {.    r
-00002de0: 6574 7572 6e20 5b65 6469 746f 7241 7761  eturn [editorAwa
-00002df0: 7265 6e65 7373 4661 6365 742e 6f66 2863  renessFacet.of(c
-00002e00: 6f6e 6669 6729 2c20 7368 6f77 436f 6c6c  onfig), showColl
-00002e10: 6162 6f72 6174 6f72 735d 3b0a 7d0a       aborators];.}.
+00002bc0: 2020 7265 6d6f 7465 4375 7273 6f72 734c    remoteCursorsL
+00002bd0: 6179 6572 2c0a 2020 2020 2020 2020 7265  ayer,.        re
+00002be0: 6d6f 7465 5365 6c65 6374 696f 6e4c 6179  moteSelectionLay
+00002bf0: 6572 2c0a 2020 2020 2020 2020 7573 6572  er,.        user
+00002c00: 486f 7665 722c 0a20 2020 2020 2020 202f  Hover,.        /
+00002c10: 2f20 4173 2077 6520 7573 6520 7265 6c61  / As we use rela
+00002c20: 7469 7665 2070 6f73 6974 696f 6e69 6e67  tive positioning
+00002c30: 206f 6620 7769 6467 6574 2c20 7468 6520   of widget, the 
+00002c40: 746f 6f6c 7469 7020 6d75 7374 2062 6520  tooltip must be 
+00002c50: 706f 7369 7469 6f6e 6564 2061 6273 6f6c  positioned absol
+00002c60: 7574 656c 790a 2020 2020 2020 2020 2f2f  utely.        //
+00002c70: 2041 6e64 2077 6520 6174 7461 6368 2074   And we attach t
+00002c80: 6865 2074 6f6f 6c74 6970 2074 6f20 7468  he tooltip to th
+00002c90: 6520 626f 6479 2074 6f20 6176 6f69 6420  e body to avoid 
+00002ca0: 6f76 6572 666c 6f77 2072 756c 6573 0a20  overflow rules. 
+00002cb0: 2020 2020 2020 2074 6f6f 6c74 6970 7328         tooltips(
+00002cc0: 7b20 706f 7369 7469 6f6e 3a20 2761 6273  { position: 'abs
+00002cd0: 6f6c 7574 6527 2c20 7061 7265 6e74 3a20  olute', parent: 
+00002ce0: 646f 6375 6d65 6e74 2e62 6f64 7920 7d29  document.body })
+00002cf0: 0a20 2020 2020 205d 3b0a 2020 2020 7d0a  .      ];.    }.
+00002d00: 2020 7d0a 293b 0a0a 2f2a 2a0a 202a 2043    }.);../**. * C
+00002d10: 6f64 654d 6972 726f 7220 6578 7465 6e73  odeMirror extens
+00002d20: 696f 6e20 746f 2064 6973 706c 6179 2072  ion to display r
+00002d30: 656d 6f74 6520 7573 6572 7320 6375 7273  emote users curs
+00002d40: 6f72 730a 202a 0a20 2a20 4070 6172 616d  ors. *. * @param
+00002d50: 2063 6f6e 6669 6720 4564 6974 6f72 2073   config Editor s
+00002d60: 6f75 7263 6520 616e 6420 6177 6172 656e  ource and awaren
+00002d70: 6573 730a 202a 2040 7265 7475 726e 7320  ess. * @returns 
+00002d80: 436f 6465 4d69 7272 6f72 2065 7874 656e  CodeMirror exten
+00002d90: 7369 6f6e 0a20 2a2f 0a65 7870 6f72 7420  sion. */.export 
+00002da0: 6675 6e63 7469 6f6e 2072 656d 6f74 6555  function remoteU
+00002db0: 7365 7243 7572 736f 7273 2863 6f6e 6669  serCursors(confi
+00002dc0: 673a 2045 6469 746f 7241 7761 7265 6e65  g: EditorAwarene
+00002dd0: 7373 293a 2045 7874 656e 7369 6f6e 207b  ss): Extension {
+00002de0: 0a20 2072 6574 7572 6e20 5b65 6469 746f  .  return [edito
+00002df0: 7241 7761 7265 6e65 7373 4661 6365 742e  rAwarenessFacet.
+00002e00: 6f66 2863 6f6e 6669 6729 2c20 7368 6f77  of(config), show
+00002e10: 436f 6c6c 6162 6f72 6174 6f72 735d 3b0a  Collaborators];.
+00002e20: 7d0a                                     }.
```

### Comparing `jupyter_collaboration_ui-1.0.0a0/packages/collaboration/lib/menu.d.ts` & `jupyter_collaboration_ui-1.0.0a1/packages/collaboration/src/tokens.ts`

 * *Files 26% similar despite different names*

```diff
@@ -1,58 +1,93 @@
-import { User } from '@jupyterlab/services';
-import { Menu, MenuBar } from '@lumino/widgets';
-import { VirtualElement } from '@lumino/virtualdom';
+// Copyright (c) Jupyter Development Team.
+// Distributed under the terms of the Modified BSD License.
+
+import type { Menu } from '@lumino/widgets';
+import { Token } from '@lumino/coreutils';
+import type { User } from '@jupyterlab/services';
+
+import { IAwareness } from '@jupyter/ydoc';
+
 /**
- * Custom renderer for the user menu.
+ * The user menu token.
+ *
+ * NOTE: Require this token in your extension to access the user menu
+ * (top-right menu in JupyterLab's interface).
  */
-export declare class RendererUserMenu extends MenuBar.Renderer {
-    private _user;
-    /**
-     * Constructor of the class RendererUserMenu.
-     *
-     * @argument user Current user object.
-     */
-    constructor(user: User.IManager);
-    /**
-     * Render the virtual element for a menu bar item.
-     *
-     * @param data - The data to use for rendering the item.
-     *
-     * @returns A virtual element representing the item.
-     */
-    renderItem(data: MenuBar.IRenderData): VirtualElement;
-    /**
-     * Render the label element for a menu item.
-     *
-     * @param data - The data to use for rendering the label.
-     *
-     * @returns A virtual element representing the item label.
-     */
-    renderLabel(data: MenuBar.IRenderData): VirtualElement;
-    /**
-     * Render the user icon element for a menu item.
-     *
-     * @returns A virtual element representing the item label.
-     */
-    private _createUserIcon;
-}
+export const IUserMenu = new Token<IUserMenu>(
+  '@jupyter/collaboration:IUserMenu'
+);
+
+/**
+ * The global awareness token.
+ */
+export const IGlobalAwareness = new Token<IAwareness>(
+  '@jupyter/collaboration:IGlobalAwareness'
+);
+
 /**
- * This menu does not contain anything but we keep it around in case someone uses it.
- * Custom lumino Menu for the user menu.
+ * An interface describing the user menu.
  */
-export declare class UserMenu extends Menu {
-    constructor(options: UserMenu.IOptions);
+export interface IUserMenu {
+  /**
+   * Dispose of the resources held by the menu.
+   */
+  dispose(): void;
+
+  /**
+   * Test whether the widget has been disposed.
+   */
+  readonly isDisposed: boolean;
+
+  /**
+   * A read-only array of the menu items in the menu.
+   */
+  readonly items: ReadonlyArray<Menu.IItem>;
+
+  /**
+   * Add a menu item to the end of the menu.
+   *
+   * @param options - The options for creating the menu item.
+   *
+   * @returns The menu item added to the menu.
+   */
+  addItem(options: Menu.IItemOptions): Menu.IItem;
+
+  /**
+   * Insert a menu item into the menu at the specified index.
+   *
+   * @param index - The index at which to insert the item.
+   *
+   * @param options - The options for creating the menu item.
+   *
+   * @returns The menu item added to the menu.
+   *
+   * #### Notes
+   * The index will be clamped to the bounds of the items.
+   */
+  insertItem(index: number, options: Menu.IItemOptions): Menu.IItem;
+
+  /**
+   * Remove an item from the menu.
+   *
+   * @param item - The item to remove from the menu.
+   *
+   * #### Notes
+   * This is a no-op if the item is not in the menu.
+   */
+  removeItem(item: Menu.IItem): void;
 }
+
 /**
- * Namespace of the UserMenu class.
+ * Global awareness for JupyterLab scopped shared data.
  */
-export declare namespace UserMenu {
-    /**
-     * User menu options interface
-     */
-    interface IOptions extends Menu.IOptions {
-        /**
-         * Current user manager.
-         */
-        user: User.IManager;
-    }
+export interface ICollaboratorAwareness {
+  /**
+   * The User owning theses data.
+   */
+  user: User.IIdentity;
+
+  /**
+   * The current file/context the user is working on.
+   */
+  current?: string;
 }
```

### Comparing `jupyter_collaboration_ui-1.0.0a0/packages/collaboration/lib/sharedlink.js` & `jupyter_collaboration_ui-1.0.0a1/packages/collaboration/src/sharedlink.ts`

 * *Files 24% similar despite different names*

```diff
@@ -1,342 +1,353 @@
 00000000: 2f2f 2043 6f70 7972 6967 6874 2028 6329  // Copyright (c)
 00000010: 204a 7570 7974 6572 2044 6576 656c 6f70   Jupyter Develop
 00000020: 6d65 6e74 2054 6561 6d2e 0a2f 2f20 4469  ment Team..// Di
 00000030: 7374 7269 6275 7465 6420 756e 6465 7220  stributed under 
 00000040: 7468 6520 7465 726d 7320 6f66 2074 6865  the terms of the
 00000050: 204d 6f64 6966 6965 6420 4253 4420 4c69   Modified BSD Li
-00000060: 6365 6e73 652e 0a69 6d70 6f72 7420 7b20  cense..import { 
-00000070: 4469 616c 6f67 2c20 7368 6f77 4469 616c  Dialog, showDial
-00000080: 6f67 207d 2066 726f 6d20 2740 6a75 7079  og } from '@jupy
-00000090: 7465 726c 6162 2f61 7070 7574 696c 7327  terlab/apputils'
-000000a0: 3b0a 696d 706f 7274 207b 2050 6167 6543  ;.import { PageC
-000000b0: 6f6e 6669 672c 2055 524c 4578 7420 7d20  onfig, URLExt } 
-000000c0: 6672 6f6d 2027 406a 7570 7974 6572 6c61  from '@jupyterla
-000000d0: 622f 636f 7265 7574 696c 7327 3b0a 696d  b/coreutils';.im
-000000e0: 706f 7274 207b 206e 756c 6c54 7261 6e73  port { nullTrans
-000000f0: 6c61 746f 7220 7d20 6672 6f6d 2027 406a  lator } from '@j
-00000100: 7570 7974 6572 6c61 622f 7472 616e 736c  upyterlab/transl
-00000110: 6174 696f 6e27 3b0a 696d 706f 7274 207b  ation';.import {
-00000120: 2057 6964 6765 7420 7d20 6672 6f6d 2027   Widget } from '
-00000130: 406c 756d 696e 6f2f 7769 6467 6574 7327  @lumino/widgets'
-00000140: 3b0a 2f2a 2a0a 202a 2053 686f 7720 7468  ;./**. * Show th
-00000150: 6520 7368 6172 6564 206c 696e 6b20 6469  e shared link di
-00000160: 616c 6f67 0a20 2a0a 202a 2040 7061 7261  alog. *. * @para
-00000170: 6d20 6f70 7469 6f6e 7320 5368 6172 6564  m options Shared
-00000180: 206c 696e 6b20 6469 616c 6f67 206f 7074   link dialog opt
-00000190: 696f 6e73 0a20 2a20 4072 6574 7572 6e73  ions. * @returns
-000001a0: 2044 6961 6c6f 6720 7265 7375 6c74 0a20   Dialog result. 
-000001b0: 2a2f 0a65 7870 6f72 7420 6173 796e 6320  */.export async 
-000001c0: 6675 6e63 7469 6f6e 2073 686f 7753 6861  function showSha
-000001d0: 7265 644c 696e 6b44 6961 6c6f 6728 7b20  redLinkDialog({ 
-000001e0: 7472 616e 736c 6174 6f72 207d 2920 7b0a  translator }) {.
-000001f0: 2020 2020 636f 6e73 7420 7472 616e 7320      const trans 
-00000200: 3d20 2874 7261 6e73 6c61 746f 7220 213d  = (translator !=
-00000210: 3d20 6e75 6c6c 2026 2620 7472 616e 736c  = null && transl
-00000220: 6174 6f72 2021 3d3d 2076 6f69 6420 3020  ator !== void 0 
-00000230: 3f20 7472 616e 736c 6174 6f72 203a 206e  ? translator : n
-00000240: 756c 6c54 7261 6e73 6c61 746f 7229 2e6c  ullTranslator).l
-00000250: 6f61 6428 2763 6f6c 6c61 626f 7261 7469  oad('collaborati
-00000260: 6f6e 2729 3b0a 2020 2020 636f 6e73 7420  on');.    const 
-00000270: 746f 6b65 6e20 3d20 5061 6765 436f 6e66  token = PageConf
-00000280: 6967 2e67 6574 546f 6b65 6e28 293b 0a20  ig.getToken();. 
-00000290: 2020 2063 6f6e 7374 2075 726c 203d 206e     const url = n
-000002a0: 6577 2055 524c 2855 524c 4578 742e 6e6f  ew URL(URLExt.no
-000002b0: 726d 616c 697a 6528 5061 6765 436f 6e66  rmalize(PageConf
-000002c0: 6967 2e67 6574 5572 6c28 7b0a 2020 2020  ig.getUrl({.    
-000002d0: 2020 2020 776f 726b 7370 6163 653a 2050      workspace: P
-000002e0: 6167 6543 6f6e 6669 672e 6465 6661 756c  ageConfig.defaul
-000002f0: 7457 6f72 6b73 7061 6365 0a20 2020 207d  tWorkspace.    }
-00000300: 2929 293b 0a20 2020 2072 6574 7572 6e20  )));.    return 
-00000310: 7368 6f77 4469 616c 6f67 287b 0a20 2020  showDialog({.   
-00000320: 2020 2020 2074 6974 6c65 3a20 7472 616e       title: tran
-00000330: 732e 5f5f 2827 5368 6172 6520 4a75 7079  s.__('Share Jupy
-00000340: 7465 7220 5365 7276 6572 204c 696e 6b27  ter Server Link'
-00000350: 292c 0a20 2020 2020 2020 2062 6f64 793a  ),.        body:
-00000360: 206e 6577 2053 6861 7265 644c 696e 6b42   new SharedLinkB
-00000370: 6f64 7928 7572 6c2e 746f 5374 7269 6e67  ody(url.toString
-00000380: 2829 2c20 746f 6b65 6e2c 2050 6167 6543  (), token, PageC
-00000390: 6f6e 6669 672e 6765 744f 7074 696f 6e28  onfig.getOption(
-000003a0: 2768 7562 5573 6572 2729 2021 3d3d 2027  'hubUser') !== '
-000003b0: 272c 2074 7261 6e73 292c 0a20 2020 2020  ', trans),.     
-000003c0: 2020 2062 7574 746f 6e73 3a20 5b0a 2020     buttons: [.  
-000003d0: 2020 2020 2020 2020 2020 4469 616c 6f67            Dialog
-000003e0: 2e63 616e 6365 6c42 7574 746f 6e28 292c  .cancelButton(),
-000003f0: 0a20 2020 2020 2020 2020 2020 2044 6961  .            Dia
-00000400: 6c6f 672e 6f6b 4275 7474 6f6e 287b 0a20  log.okButton({. 
-00000410: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-00000420: 6162 656c 3a20 7472 616e 732e 5f5f 2827  abel: trans.__('
-00000430: 436f 7079 204c 696e 6b27 292c 0a20 2020  Copy Link'),.   
-00000440: 2020 2020 2020 2020 2020 2020 2063 6170               cap
-00000450: 7469 6f6e 3a20 7472 616e 732e 5f5f 2827  tion: trans.__('
-00000460: 436f 7079 2074 6865 206c 696e 6b20 746f  Copy the link to
-00000470: 2074 6865 204a 7570 7974 6572 2053 6572   the Jupyter Ser
-00000480: 7665 7227 290a 2020 2020 2020 2020 2020  ver').          
-00000490: 2020 7d29 0a20 2020 2020 2020 205d 0a20    }).        ]. 
-000004a0: 2020 207d 293b 0a7d 0a63 6c61 7373 2053     });.}.class S
-000004b0: 6861 7265 644c 696e 6b42 6f64 7920 6578  haredLinkBody ex
-000004c0: 7465 6e64 7320 5769 6467 6574 207b 0a20  tends Widget {. 
-000004d0: 2020 2063 6f6e 7374 7275 6374 6f72 285f     constructor(_
-000004e0: 7572 6c2c 205f 746f 6b65 6e2c 205f 6265  url, _token, _be
-000004f0: 6869 6e64 4875 622c 205f 7472 616e 7329  hindHub, _trans)
-00000500: 207b 0a20 2020 2020 2020 2073 7570 6572   {.        super
-00000510: 2829 3b0a 2020 2020 2020 2020 7468 6973  ();.        this
-00000520: 2e5f 7572 6c20 3d20 5f75 726c 3b0a 2020  ._url = _url;.  
-00000530: 2020 2020 2020 7468 6973 2e5f 746f 6b65        this._toke
-00000540: 6e20 3d20 5f74 6f6b 656e 3b0a 2020 2020  n = _token;.    
-00000550: 2020 2020 7468 6973 2e5f 6265 6869 6e64      this._behind
-00000560: 4875 6220 3d20 5f62 6568 696e 6448 7562  Hub = _behindHub
-00000570: 3b0a 2020 2020 2020 2020 7468 6973 2e5f  ;.        this._
-00000580: 7472 616e 7320 3d20 5f74 7261 6e73 3b0a  trans = _trans;.
-00000590: 2020 2020 2020 2020 7468 6973 2e5f 746f          this._to
-000005a0: 6b65 6e43 6865 636b 626f 7820 3d20 6e75  kenCheckbox = nu
-000005b0: 6c6c 3b0a 2020 2020 2020 2020 7468 6973  ll;.        this
-000005c0: 2e6f 6e54 6f6b 656e 4368 616e 6765 203d  .onTokenChange =
-000005d0: 2028 6529 203d 3e20 7b0a 2020 2020 2020   (e) => {.      
-000005e0: 2020 2020 2020 636f 6e73 7420 7461 7267        const targ
-000005f0: 6574 203d 2065 2e74 6172 6765 743b 0a20  et = e.target;. 
-00000600: 2020 2020 2020 2020 2020 2074 6869 732e             this.
-00000610: 7570 6461 7465 436f 6e74 656e 7428 7461  updateContent(ta
-00000620: 7267 6574 203d 3d3d 206e 756c 6c20 7c7c  rget === null ||
-00000630: 2074 6172 6765 7420 3d3d 3d20 766f 6964   target === void
-00000640: 2030 203f 2076 6f69 6420 3020 3a20 7461   0 ? void 0 : ta
-00000650: 7267 6574 2e63 6865 636b 6564 293b 0a20  rget.checked);. 
-00000660: 2020 2020 2020 207d 3b0a 2020 2020 2020         };.      
-00000670: 2020 7468 6973 2e5f 7761 726e 696e 6720    this._warning 
-00000680: 3d20 646f 6375 6d65 6e74 2e63 7265 6174  = document.creat
-00000690: 6545 6c65 6d65 6e74 2827 6469 7627 293b  eElement('div');
-000006a0: 0a20 2020 2020 2020 2074 6869 732e 706f  .        this.po
-000006b0: 7075 6c61 7465 426f 6479 2874 6869 732e  pulateBody(this.
-000006c0: 6e6f 6465 293b 0a20 2020 2020 2020 2074  node);.        t
-000006d0: 6869 732e 6164 6443 6c61 7373 2827 6a70  his.addClass('jp
-000006e0: 2d73 6861 7265 642d 6c69 6e6b 2d62 6f64  -shared-link-bod
-000006f0: 7927 293b 0a20 2020 207d 0a20 2020 202f  y');.    }.    /
-00000700: 2a2a 0a20 2020 2020 2a20 5265 7475 726e  **.     * Return
-00000710: 7320 7468 6520 696e 7075 7420 7661 6c75  s the input valu
-00000720: 652e 0a20 2020 2020 2a2f 0a20 2020 2067  e..     */.    g
-00000730: 6574 5661 6c75 6528 2920 7b0a 2020 2020  etValue() {.    
-00000740: 2020 2020 7661 7220 5f61 3b0a 2020 2020      var _a;.    
-00000750: 2020 2020 636f 6e73 7420 7769 7468 546f      const withTo
-00000760: 6b65 6e20 3d20 2828 5f61 203d 2074 6869  ken = ((_a = thi
-00000770: 732e 5f74 6f6b 656e 4368 6563 6b62 6f78  s._tokenCheckbox
-00000780: 2920 3d3d 3d20 6e75 6c6c 207c 7c20 5f61  ) === null || _a
-00000790: 203d 3d3d 2076 6f69 6420 3020 3f20 766f   === void 0 ? vo
-000007a0: 6964 2030 203a 205f 612e 6368 6563 6b65  id 0 : _a.checke
-000007b0: 6429 203d 3d3d 2074 7275 653b 0a20 2020  d) === true;.   
-000007c0: 2020 2020 2069 6620 2877 6974 6854 6f6b       if (withTok
-000007d0: 656e 2920 7b0a 2020 2020 2020 2020 2020  en) {.          
-000007e0: 2020 636f 6e73 7420 7572 6c5f 203d 206e    const url_ = n
-000007f0: 6577 2055 524c 2874 6869 732e 5f75 726c  ew URL(this._url
-00000800: 293b 0a20 2020 2020 2020 2020 2020 2075  );.            u
-00000810: 726c 5f2e 7365 6172 6368 5061 7261 6d73  rl_.searchParams
-00000820: 2e73 6574 2827 746f 6b65 6e27 2c20 7468  .set('token', th
-00000830: 6973 2e5f 746f 6b65 6e29 3b0a 2020 2020  is._token);.    
-00000840: 2020 2020 2020 2020 7265 7475 726e 2075          return u
-00000850: 726c 5f2e 746f 5374 7269 6e67 2829 3b0a  rl_.toString();.
-00000860: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-00000870: 2020 656c 7365 207b 0a20 2020 2020 2020    else {.       
-00000880: 2020 2020 2072 6574 7572 6e20 7468 6973       return this
-00000890: 2e5f 7572 6c3b 0a20 2020 2020 2020 207d  ._url;.        }
-000008a0: 0a20 2020 207d 0a20 2020 206f 6e41 6674  .    }.    onAft
-000008b0: 6572 4174 7461 6368 286d 7367 2920 7b0a  erAttach(msg) {.
-000008c0: 2020 2020 2020 2020 7661 7220 5f61 3b0a          var _a;.
-000008d0: 2020 2020 2020 2020 7375 7065 722e 6f6e          super.on
-000008e0: 4166 7465 7241 7474 6163 6828 6d73 6729  AfterAttach(msg)
-000008f0: 3b0a 2020 2020 2020 2020 285f 6120 3d20  ;.        (_a = 
-00000900: 7468 6973 2e5f 746f 6b65 6e43 6865 636b  this._tokenCheck
-00000910: 626f 7829 203d 3d3d 206e 756c 6c20 7c7c  box) === null ||
-00000920: 205f 6120 3d3d 3d20 766f 6964 2030 203f   _a === void 0 ?
-00000930: 2076 6f69 6420 3020 3a20 5f61 2e61 6464   void 0 : _a.add
-00000940: 4576 656e 744c 6973 7465 6e65 7228 2763  EventListener('c
-00000950: 6861 6e67 6527 2c20 7468 6973 2e6f 6e54  hange', this.onT
-00000960: 6f6b 656e 4368 616e 6765 293b 0a20 2020  okenChange);.   
-00000970: 207d 0a20 2020 206f 6e42 6566 6f72 6544   }.    onBeforeD
-00000980: 6574 6163 6828 6d73 6729 207b 0a20 2020  etach(msg) {.   
-00000990: 2020 2020 2076 6172 205f 613b 0a20 2020       var _a;.   
-000009a0: 2020 2020 2028 5f61 203d 2074 6869 732e       (_a = this.
-000009b0: 5f74 6f6b 656e 4368 6563 6b62 6f78 2920  _tokenCheckbox) 
-000009c0: 3d3d 3d20 6e75 6c6c 207c 7c20 5f61 203d  === null || _a =
-000009d0: 3d3d 2076 6f69 6420 3020 3f20 766f 6964  == void 0 ? void
-000009e0: 2030 203a 205f 612e 7265 6d6f 7665 4576   0 : _a.removeEv
-000009f0: 656e 744c 6973 7465 6e65 7228 2763 6861  entListener('cha
-00000a00: 6e67 6527 2c20 7468 6973 2e6f 6e54 6f6b  nge', this.onTok
-00000a10: 656e 4368 616e 6765 293b 0a20 2020 2020  enChange);.     
-00000a20: 2020 2073 7570 6572 2e6f 6e42 6566 6f72     super.onBefor
-00000a30: 6544 6574 6163 6828 6d73 6729 3b0a 2020  eDetach(msg);.  
-00000a40: 2020 7d0a 2020 2020 7570 6461 7465 436f    }.    updateCo
-00000a50: 6e74 656e 7428 7769 7468 546f 6b65 6e29  ntent(withToken)
-00000a60: 207b 0a20 2020 2020 2020 2074 6869 732e   {.        this.
-00000a70: 5f77 6172 6e69 6e67 2e69 6e6e 6572 4854  _warning.innerHT
-00000a80: 4d4c 203d 2027 273b 0a20 2020 2020 2020  ML = '';.       
-00000a90: 2063 6f6e 7374 2075 726c 496e 7075 7420   const urlInput 
-00000aa0: 3d20 7468 6973 2e6e 6f64 652e 7175 6572  = this.node.quer
-00000ab0: 7953 656c 6563 746f 7228 2769 6e70 7574  ySelector('input
-00000ac0: 5b72 6561 646f 6e6c 795d 2729 3b0a 2020  [readonly]');.  
-00000ad0: 2020 2020 2020 6966 2028 7769 7468 546f        if (withTo
-00000ae0: 6b65 6e29 207b 0a20 2020 2020 2020 2020  ken) {.         
-00000af0: 2020 2069 6620 2875 726c 496e 7075 7429     if (urlInput)
-00000b00: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-00000b10: 2020 2063 6f6e 7374 2075 726c 5f20 3d20     const url_ = 
-00000b20: 6e65 7720 5552 4c28 7468 6973 2e5f 7572  new URL(this._ur
-00000b30: 6c29 3b0a 2020 2020 2020 2020 2020 2020  l);.            
-00000b40: 2020 2020 7572 6c5f 2e73 6561 7263 6850      url_.searchP
-00000b50: 6172 616d 732e 7365 7428 2774 6f6b 656e  arams.set('token
-00000b60: 272c 2074 6869 732e 5f74 6f6b 656e 2e73  ', this._token.s
-00000b70: 6c69 6365 2830 2c20 3529 293b 0a20 2020  lice(0, 5));.   
-00000b80: 2020 2020 2020 2020 2020 2020 2075 726c               url
-00000b90: 496e 7075 742e 7661 6c75 6520 3d20 7572  Input.value = ur
-00000ba0: 6c5f 2e74 6f53 7472 696e 6728 2920 2b20  l_.toString() + 
-00000bb0: 27e2 80a6 273b 0a20 2020 2020 2020 2020  '...';.         
-00000bc0: 2020 207d 0a20 2020 2020 2020 2020 2020     }.           
-00000bd0: 2074 6869 732e 5f77 6172 6e69 6e67 2e61   this._warning.a
-00000be0: 7070 656e 6443 6869 6c64 2864 6f63 756d  ppendChild(docum
-00000bf0: 656e 742e 6372 6561 7465 456c 656d 656e  ent.createElemen
-00000c00: 7428 2768 3327 2929 2e74 6578 7443 6f6e  t('h3')).textCon
-00000c10: 7465 6e74 203d 0a20 2020 2020 2020 2020  tent =.         
-00000c20: 2020 2020 2020 2074 6869 732e 5f74 7261         this._tra
-00000c30: 6e73 2e5f 5f28 2753 6563 7572 6974 7920  ns.__('Security 
-00000c40: 7761 726e 696e 6721 2729 3b0a 2020 2020  warning!');.    
-00000c50: 2020 2020 2020 2020 7468 6973 2e5f 7761          this._wa
-00000c60: 726e 696e 672e 696e 7365 7274 4164 6a61  rning.insertAdja
-00000c70: 6365 6e74 5465 7874 2827 6265 666f 7265  centText('before
-00000c80: 656e 6427 2c20 7468 6973 2e5f 7472 616e  end', this._tran
-00000c90: 732e 5f5f 2827 416e 796f 6e65 2077 6974  s.__('Anyone wit
-00000ca0: 6820 7468 6973 206c 696e 6b20 6861 7320  h this link has 
-00000cb0: 6675 6c6c 2061 6363 6573 7320 746f 2079  full access to y
-00000cc0: 6f75 7220 6e6f 7465 626f 6f6b 2073 6572  our notebook ser
-00000cd0: 7665 722c 2069 6e63 6c75 6469 6e67 2061  ver, including a
-00000ce0: 6c6c 2079 6f75 7220 6669 6c65 7321 2729  ll your files!')
-00000cf0: 293b 0a20 2020 2020 2020 2020 2020 2074  );.            t
-00000d00: 6869 732e 5f77 6172 6e69 6e67 2e69 6e73  his._warning.ins
-00000d10: 6572 7441 646a 6163 656e 7448 544d 4c28  ertAdjacentHTML(
-00000d20: 2762 6566 6f72 6565 6e64 272c 2027 3c62  'beforeend', '<b
-00000d30: 723e 2729 3b0a 2020 2020 2020 2020 2020  r>');.          
-00000d40: 2020 7468 6973 2e5f 7761 726e 696e 672e    this._warning.
-00000d50: 696e 7365 7274 4164 6a61 6365 6e74 5465  insertAdjacentTe
-00000d60: 7874 2827 6265 666f 7265 656e 6427 2c20  xt('beforeend', 
-00000d70: 7468 6973 2e5f 7472 616e 732e 5f5f 2827  this._trans.__('
-00000d80: 506c 6561 7365 2062 6520 6361 7265 6675  Please be carefu
-00000d90: 6c20 7768 6f20 796f 7520 7368 6172 6520  l who you share 
-00000da0: 6974 2077 6974 682e 2729 293b 0a20 2020  it with.'));.   
-00000db0: 2020 2020 2020 2020 2074 6869 732e 5f77           this._w
-00000dc0: 6172 6e69 6e67 2e69 6e73 6572 7441 646a  arning.insertAdj
-00000dd0: 6163 656e 7448 544d 4c28 2762 6566 6f72  acentHTML('befor
-00000de0: 6565 6e64 272c 2027 3c62 723e 2729 3b0a  eend', '<br>');.
-00000df0: 2020 2020 2020 2020 2020 2020 6966 2028              if (
-00000e00: 7468 6973 2e5f 6265 6869 6e64 4875 6229  this._behindHub)
-00000e10: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-00000e20: 2020 2074 6869 732e 5f77 6172 6e69 6e67     this._warning
-00000e30: 2e69 6e73 6572 7441 646a 6163 656e 7454  .insertAdjacentT
-00000e40: 6578 7428 2762 6566 6f72 6565 6e64 272c  ext('beforeend',
-00000e50: 202f 2f20 596f 7520 6361 6e20 7265 7374   // You can rest
-00000e60: 6172 7420 7468 6520 7365 7276 6572 2074  art the server t
-00000e70: 6f20 7265 766f 6b65 2074 6865 2074 6f6b  o revoke the tok
-00000e80: 656e 2069 6e20 6120 4a75 7079 7465 7248  en in a JupyterH
-00000e90: 7562 0a20 2020 2020 2020 2020 2020 2020  ub.             
-00000ea0: 2020 2074 6869 732e 5f74 7261 6e73 2e5f     this._trans._
-00000eb0: 5f28 2754 6865 7920 7769 6c6c 2062 6520  _('They will be 
-00000ec0: 6162 6c65 2074 6f20 6163 6365 7373 2074  able to access t
-00000ed0: 6869 7320 7365 7276 6572 2041 5320 594f  his server AS YO
-00000ee0: 552e 2729 293b 0a20 2020 2020 2020 2020  U.'));.         
-00000ef0: 2020 2020 2020 2074 6869 732e 5f77 6172         this._war
-00000f00: 6e69 6e67 2e69 6e73 6572 7441 646a 6163  ning.insertAdjac
-00000f10: 656e 7448 544d 4c28 2762 6566 6f72 6565  entHTML('beforee
-00000f20: 6e64 272c 2027 3c62 723e 2729 3b0a 2020  nd', '<br>');.  
-00000f30: 2020 2020 2020 2020 2020 2020 2020 7468                th
-00000f40: 6973 2e5f 7761 726e 696e 672e 696e 7365  is._warning.inse
-00000f50: 7274 4164 6a61 6365 6e74 5465 7874 2827  rtAdjacentText('
-00000f60: 6265 666f 7265 656e 6427 2c20 7468 6973  beforeend', this
-00000f70: 2e5f 7472 616e 732e 5f5f 2827 546f 2072  ._trans.__('To r
-00000f80: 6576 6f6b 6520 6163 6365 7373 2c20 676f  evoke access, go
-00000f90: 2074 6f20 4669 6c65 202d 3e20 4875 6220   to File -> Hub 
-00000fa0: 436f 6e74 726f 6c20 5061 6e65 6c2c 2061  Control Panel, a
-00000fb0: 6e64 2072 6573 7461 7274 2079 6f75 7220  nd restart your 
-00000fc0: 7365 7276 6572 2e27 2929 3b0a 2020 2020  server.'));.    
-00000fd0: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-00000fe0: 2020 2020 2020 656c 7365 207b 0a20 2020        else {.   
-00000ff0: 2020 2020 2020 2020 2020 2020 2074 6869               thi
-00001000: 732e 5f77 6172 6e69 6e67 2e69 6e73 6572  s._warning.inser
-00001010: 7441 646a 6163 656e 7454 6578 7428 2762  tAdjacentText('b
-00001020: 6566 6f72 6565 6e64 272c 200a 2020 2020  eforeend', .    
-00001030: 2020 2020 2020 2020 2020 2020 2f2f 2045              // E
-00001040: 6c73 6577 6865 7265 2c20 796f 7520 2a6d  lsewhere, you *m
-00001050: 7573 742a 2073 6875 7420 646f 776e 2079  ust* shut down y
-00001060: 6f75 7220 7365 7276 6572 202d 206e 6f20  our server - no 
-00001070: 7761 7920 746f 2072 6576 6f6b 6520 6974  way to revoke it
-00001080: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001090: 2074 6869 732e 5f74 7261 6e73 2e5f 5f28   this._trans.__(
-000010a0: 2743 7572 7265 6e74 6c79 2c20 7468 6572  'Currently, ther
-000010b0: 6520 6973 206e 6f20 7761 7920 746f 2072  e is no way to r
-000010c0: 6576 6f6b 6520 6163 6365 7373 206f 7468  evoke access oth
-000010d0: 6572 2074 6861 6e20 7368 7574 7469 6e67  er than shutting
-000010e0: 2064 6f77 6e20 796f 7572 2073 6572 7665   down your serve
-000010f0: 722e 2729 293b 0a20 2020 2020 2020 2020  r.'));.         
-00001100: 2020 207d 0a20 2020 2020 2020 207d 0a20     }.        }. 
-00001110: 2020 2020 2020 2065 6c73 6520 7b0a 2020         else {.  
-00001120: 2020 2020 2020 2020 2020 6966 2028 7572            if (ur
-00001130: 6c49 6e70 7574 2920 7b0a 2020 2020 2020  lInput) {.      
-00001140: 2020 2020 2020 2020 2020 7572 6c49 6e70            urlInp
-00001150: 7574 2e76 616c 7565 203d 2074 6869 732e  ut.value = this.
-00001160: 5f75 726c 3b0a 2020 2020 2020 2020 2020  _url;.          
-00001170: 2020 7d0a 2020 2020 2020 2020 2020 2020    }.            
-00001180: 6966 2028 7468 6973 2e5f 6265 6869 6e64  if (this._behind
-00001190: 4875 6229 207b 0a20 2020 2020 2020 2020  Hub) {.         
-000011a0: 2020 2020 2020 2074 6869 732e 5f77 6172         this._war
-000011b0: 6e69 6e67 2e69 6e73 6572 7441 646a 6163  ning.insertAdjac
-000011c0: 656e 7454 6578 7428 2762 6566 6f72 6565  entText('beforee
-000011d0: 6e64 272c 2074 6869 732e 5f74 7261 6e73  nd', this._trans
-000011e0: 2e5f 5f28 274f 6e6c 7920 7573 6572 7320  .__('Only users 
-000011f0: 7769 7468 2060 6163 6365 7373 3a73 6572  with `access:ser
-00001200: 7665 7273 6020 7065 726d 6973 7369 6f6e  vers` permission
-00001210: 7320 666f 7220 7468 6973 2073 6572 7665  s for this serve
-00001220: 7220 7769 6c6c 2062 6520 6162 6c65 2074  r will be able t
-00001230: 6f20 7573 6520 7468 6973 206c 696e 6b2e  o use this link.
-00001240: 2729 293b 0a20 2020 2020 2020 2020 2020  '));.           
-00001250: 207d 0a20 2020 2020 2020 2020 2020 2065   }.            e
-00001260: 6c73 6520 7b0a 2020 2020 2020 2020 2020  lse {.          
-00001270: 2020 2020 2020 7468 6973 2e5f 7761 726e        this._warn
-00001280: 696e 672e 696e 7365 7274 4164 6a61 6365  ing.insertAdjace
-00001290: 6e74 5465 7874 2827 6265 666f 7265 656e  ntText('beforeen
-000012a0: 6427 2c20 7468 6973 2e5f 7472 616e 732e  d', this._trans.
-000012b0: 5f5f 2827 4f6e 6c79 2061 7574 6865 6e74  __('Only authent
-000012c0: 6963 6174 6564 2075 7365 7273 2077 696c  icated users wil
-000012d0: 6c20 6265 2061 626c 6520 746f 2075 7365  l be able to use
-000012e0: 2074 6869 7320 6c69 6e6b 2e27 2929 3b0a   this link.'));.
-000012f0: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
-00001300: 2020 2020 2020 7d0a 2020 2020 7d0a 2020        }.    }.  
-00001310: 2020 706f 7075 6c61 7465 426f 6479 2864    populateBody(d
-00001320: 6961 6c6f 6742 6f64 7929 207b 0a20 2020  ialogBody) {.   
-00001330: 2020 2020 2064 6961 6c6f 6742 6f64 792e       dialogBody.
-00001340: 696e 7365 7274 4164 6a61 6365 6e74 4854  insertAdjacentHT
-00001350: 4d4c 2827 6166 7465 7262 6567 696e 272c  ML('afterbegin',
-00001360: 2060 3c69 6e70 7574 2072 6561 646f 6e6c   `<input readonl
-00001370: 7920 7661 6c75 653d 2224 7b74 6869 732e  y value="${this.
-00001380: 5f75 726c 7d22 3e60 293b 0a20 2020 2020  _url}">`);.     
-00001390: 2020 2069 6620 2874 6869 732e 5f74 6f6b     if (this._tok
-000013a0: 656e 2920 7b0a 2020 2020 2020 2020 2020  en) {.          
-000013b0: 2020 636f 6e73 7420 6c61 6265 6c20 3d20    const label = 
-000013c0: 6469 616c 6f67 426f 6479 2e61 7070 656e  dialogBody.appen
-000013d0: 6443 6869 6c64 2864 6f63 756d 656e 742e  dChild(document.
-000013e0: 6372 6561 7465 456c 656d 656e 7428 276c  createElement('l
-000013f0: 6162 656c 2729 293b 0a20 2020 2020 2020  abel'));.       
-00001400: 2020 2020 206c 6162 656c 2e69 6e73 6572       label.inser
-00001410: 7441 646a 6163 656e 7448 544d 4c28 2762  tAdjacentHTML('b
-00001420: 6566 6f72 6565 6e64 272c 2027 3c69 6e70  eforeend', '<inp
-00001430: 7574 2074 7970 653d 2263 6865 636b 626f  ut type="checkbo
-00001440: 7822 3e27 293b 0a20 2020 2020 2020 2020  x">');.         
-00001450: 2020 2074 6869 732e 5f74 6f6b 656e 4368     this._tokenCh
-00001460: 6563 6b62 6f78 203d 206c 6162 656c 2e66  eckbox = label.f
-00001470: 6972 7374 4368 696c 643b 0a20 2020 2020  irstChild;.     
-00001480: 2020 2020 2020 206c 6162 656c 2e69 6e73         label.ins
-00001490: 6572 7441 646a 6163 656e 7454 6578 7428  ertAdjacentText(
-000014a0: 2762 6566 6f72 6565 6e64 272c 2074 6869  'beforeend', thi
-000014b0: 732e 5f74 7261 6e73 2e5f 5f28 2749 6e63  s._trans.__('Inc
-000014c0: 6c75 6465 2074 6f6b 656e 2069 6e20 5552  lude token in UR
-000014d0: 4c27 2929 3b0a 2020 2020 2020 2020 2020  L'));.          
-000014e0: 2020 6469 616c 6f67 426f 6479 2e69 6e73    dialogBody.ins
-000014f0: 6572 7441 646a 6163 656e 7445 6c65 6d65  ertAdjacentEleme
-00001500: 6e74 2827 6265 666f 7265 656e 6427 2c20  nt('beforeend', 
-00001510: 7468 6973 2e5f 7761 726e 696e 6729 3b0a  this._warning);.
-00001520: 2020 2020 2020 2020 2020 2020 7468 6973              this
-00001530: 2e75 7064 6174 6543 6f6e 7465 6e74 2866  .updateContent(f
-00001540: 616c 7365 293b 0a20 2020 2020 2020 207d  alse);.        }
-00001550: 0a20 2020 207d 0a7d 0a                   .    }.}.
+00000060: 6365 6e73 652e 0a0a 696d 706f 7274 207b  cense...import {
+00000070: 2044 6961 6c6f 672c 2073 686f 7744 6961   Dialog, showDia
+00000080: 6c6f 6720 7d20 6672 6f6d 2027 406a 7570  log } from '@jup
+00000090: 7974 6572 6c61 622f 6170 7075 7469 6c73  yterlab/apputils
+000000a0: 273b 0a0a 696d 706f 7274 207b 2050 6167  ';..import { Pag
+000000b0: 6543 6f6e 6669 672c 2055 524c 4578 7420  eConfig, URLExt 
+000000c0: 7d20 6672 6f6d 2027 406a 7570 7974 6572  } from '@jupyter
+000000d0: 6c61 622f 636f 7265 7574 696c 7327 3b0a  lab/coreutils';.
+000000e0: 0a69 6d70 6f72 7420 7b0a 2020 4954 7261  .import {.  ITra
+000000f0: 6e73 6c61 746f 722c 0a20 2054 7261 6e73  nslator,.  Trans
+00000100: 6c61 7469 6f6e 4275 6e64 6c65 2c0a 2020  lationBundle,.  
+00000110: 6e75 6c6c 5472 616e 736c 6174 6f72 0a7d  nullTranslator.}
+00000120: 2066 726f 6d20 2740 6a75 7079 7465 726c   from '@jupyterl
+00000130: 6162 2f74 7261 6e73 6c61 7469 6f6e 273b  ab/translation';
+00000140: 0a0a 696d 706f 7274 207b 2057 6964 6765  ..import { Widge
+00000150: 7420 7d20 6672 6f6d 2027 406c 756d 696e  t } from '@lumin
+00000160: 6f2f 7769 6467 6574 7327 3b0a 0a69 6d70  o/widgets';..imp
+00000170: 6f72 7420 7b20 4d65 7373 6167 6520 7d20  ort { Message } 
+00000180: 6672 6f6d 2027 406c 756d 696e 6f2f 6d65  from '@lumino/me
+00000190: 7373 6167 696e 6727 3b0a 0a2f 2a2a 0a20  ssaging';../**. 
+000001a0: 2a20 5368 6172 6564 206c 696e 6b20 6469  * Shared link di
+000001b0: 616c 6f67 206f 7074 696f 6e73 0a20 2a2f  alog options. */
+000001c0: 0a65 7870 6f72 7420 696e 7465 7266 6163  .export interfac
+000001d0: 6520 4953 6861 7265 644c 696e 6b44 6961  e ISharedLinkDia
+000001e0: 6c6f 674f 7074 696f 6e73 207b 0a20 202f  logOptions {.  /
+000001f0: 2a2a 0a20 2020 2a20 5472 616e 736c 6174  **.   * Translat
+00000200: 696f 6e20 6f62 6a65 6374 2e0a 2020 202a  ion object..   *
+00000210: 2f0a 2020 7472 616e 736c 6174 6f72 3f3a  /.  translator?:
+00000220: 2049 5472 616e 736c 6174 6f72 207c 206e   ITranslator | n
+00000230: 756c 6c3b 0a7d 0a0a 2f2a 2a0a 202a 2053  ull;.}../**. * S
+00000240: 686f 7720 7468 6520 7368 6172 6564 206c  how the shared l
+00000250: 696e 6b20 6469 616c 6f67 0a20 2a0a 202a  ink dialog. *. *
+00000260: 2040 7061 7261 6d20 6f70 7469 6f6e 7320   @param options 
+00000270: 5368 6172 6564 206c 696e 6b20 6469 616c  Shared link dial
+00000280: 6f67 206f 7074 696f 6e73 0a20 2a20 4072  og options. * @r
+00000290: 6574 7572 6e73 2044 6961 6c6f 6720 7265  eturns Dialog re
+000002a0: 7375 6c74 0a20 2a2f 0a65 7870 6f72 7420  sult. */.export 
+000002b0: 6173 796e 6320 6675 6e63 7469 6f6e 2073  async function s
+000002c0: 686f 7753 6861 7265 644c 696e 6b44 6961  howSharedLinkDia
+000002d0: 6c6f 6728 7b0a 2020 7472 616e 736c 6174  log({.  translat
+000002e0: 6f72 0a7d 3a20 4953 6861 7265 644c 696e  or.}: ISharedLin
+000002f0: 6b44 6961 6c6f 674f 7074 696f 6e73 293a  kDialogOptions):
+00000300: 2050 726f 6d69 7365 3c44 6961 6c6f 672e   Promise<Dialog.
+00000310: 4952 6573 756c 743c 7374 7269 6e67 3e3e  IResult<string>>
+00000320: 207b 0a20 2063 6f6e 7374 2074 7261 6e73   {.  const trans
+00000330: 203d 2028 7472 616e 736c 6174 6f72 203f   = (translator ?
+00000340: 3f20 6e75 6c6c 5472 616e 736c 6174 6f72  ? nullTranslator
+00000350: 292e 6c6f 6164 2827 636f 6c6c 6162 6f72  ).load('collabor
+00000360: 6174 696f 6e27 293b 0a0a 2020 636f 6e73  ation');..  cons
+00000370: 7420 746f 6b65 6e20 3d20 5061 6765 436f  t token = PageCo
+00000380: 6e66 6967 2e67 6574 546f 6b65 6e28 293b  nfig.getToken();
+00000390: 0a20 2063 6f6e 7374 2075 726c 203d 206e  .  const url = n
+000003a0: 6577 2055 524c 280a 2020 2020 5552 4c45  ew URL(.    URLE
+000003b0: 7874 2e6e 6f72 6d61 6c69 7a65 280a 2020  xt.normalize(.  
+000003c0: 2020 2020 5061 6765 436f 6e66 6967 2e67      PageConfig.g
+000003d0: 6574 5572 6c28 7b0a 2020 2020 2020 2020  etUrl({.        
+000003e0: 776f 726b 7370 6163 653a 2050 6167 6543  workspace: PageC
+000003f0: 6f6e 6669 672e 6465 6661 756c 7457 6f72  onfig.defaultWor
+00000400: 6b73 7061 6365 0a20 2020 2020 207d 290a  kspace.      }).
+00000410: 2020 2020 290a 2020 293b 0a0a 2020 7265      ).  );..  re
+00000420: 7475 726e 2073 686f 7744 6961 6c6f 6728  turn showDialog(
+00000430: 7b0a 2020 2020 7469 746c 653a 2074 7261  {.    title: tra
+00000440: 6e73 2e5f 5f28 2753 6861 7265 204a 7570  ns.__('Share Jup
+00000450: 7974 6572 2053 6572 7665 7220 4c69 6e6b  yter Server Link
+00000460: 2729 2c0a 2020 2020 626f 6479 3a20 6e65  '),.    body: ne
+00000470: 7720 5368 6172 6564 4c69 6e6b 426f 6479  w SharedLinkBody
+00000480: 280a 2020 2020 2020 7572 6c2e 746f 5374  (.      url.toSt
+00000490: 7269 6e67 2829 2c0a 2020 2020 2020 746f  ring(),.      to
+000004a0: 6b65 6e2c 0a20 2020 2020 2050 6167 6543  ken,.      PageC
+000004b0: 6f6e 6669 672e 6765 744f 7074 696f 6e28  onfig.getOption(
+000004c0: 2768 7562 5573 6572 2729 2021 3d3d 2027  'hubUser') !== '
+000004d0: 272c 0a20 2020 2020 2074 7261 6e73 0a20  ',.      trans. 
+000004e0: 2020 2029 2c0a 2020 2020 6275 7474 6f6e     ),.    button
+000004f0: 733a 205b 0a20 2020 2020 2044 6961 6c6f  s: [.      Dialo
+00000500: 672e 6361 6e63 656c 4275 7474 6f6e 2829  g.cancelButton()
+00000510: 2c0a 2020 2020 2020 4469 616c 6f67 2e6f  ,.      Dialog.o
+00000520: 6b42 7574 746f 6e28 7b0a 2020 2020 2020  kButton({.      
+00000530: 2020 6c61 6265 6c3a 2074 7261 6e73 2e5f    label: trans._
+00000540: 5f28 2743 6f70 7920 4c69 6e6b 2729 2c0a  _('Copy Link'),.
+00000550: 2020 2020 2020 2020 6361 7074 696f 6e3a          caption:
+00000560: 2074 7261 6e73 2e5f 5f28 2743 6f70 7920   trans.__('Copy 
+00000570: 7468 6520 6c69 6e6b 2074 6f20 7468 6520  the link to the 
+00000580: 4a75 7079 7465 7220 5365 7276 6572 2729  Jupyter Server')
+00000590: 0a20 2020 2020 207d 290a 2020 2020 5d0a  .      }).    ].
+000005a0: 2020 7d29 3b0a 7d0a 0a63 6c61 7373 2053    });.}..class S
+000005b0: 6861 7265 644c 696e 6b42 6f64 7920 6578  haredLinkBody ex
+000005c0: 7465 6e64 7320 5769 6467 6574 2069 6d70  tends Widget imp
+000005d0: 6c65 6d65 6e74 7320 4469 616c 6f67 2e49  lements Dialog.I
+000005e0: 426f 6479 5769 6467 6574 207b 0a20 2070  BodyWidget {.  p
+000005f0: 7269 7661 7465 205f 746f 6b65 6e43 6865  rivate _tokenChe
+00000600: 636b 626f 783a 2048 544d 4c49 6e70 7574  ckbox: HTMLInput
+00000610: 456c 656d 656e 7420 7c20 6e75 6c6c 203d  Element | null =
+00000620: 206e 756c 6c3b 0a20 2070 7269 7661 7465   null;.  private
+00000630: 205f 7761 726e 696e 673a 2048 544d 4c44   _warning: HTMLD
+00000640: 6976 456c 656d 656e 743b 0a0a 2020 636f  ivElement;..  co
+00000650: 6e73 7472 7563 746f 7228 0a20 2020 2070  nstructor(.    p
+00000660: 7269 7661 7465 205f 7572 6c3a 2073 7472  rivate _url: str
+00000670: 696e 672c 0a20 2020 2070 7269 7661 7465  ing,.    private
+00000680: 205f 746f 6b65 6e3a 2073 7472 696e 672c   _token: string,
+00000690: 0a20 2020 2070 7269 7661 7465 205f 6265  .    private _be
+000006a0: 6869 6e64 4875 623a 2062 6f6f 6c65 616e  hindHub: boolean
+000006b0: 2c0a 2020 2020 7072 6976 6174 6520 5f74  ,.    private _t
+000006c0: 7261 6e73 3a20 5472 616e 736c 6174 696f  rans: Translatio
+000006d0: 6e42 756e 646c 650a 2020 2920 7b0a 2020  nBundle.  ) {.  
+000006e0: 2020 7375 7065 7228 293b 0a20 2020 2074    super();.    t
+000006f0: 6869 732e 5f77 6172 6e69 6e67 203d 2064  his._warning = d
+00000700: 6f63 756d 656e 742e 6372 6561 7465 456c  ocument.createEl
+00000710: 656d 656e 7428 2764 6976 2729 3b0a 2020  ement('div');.  
+00000720: 2020 7468 6973 2e70 6f70 756c 6174 6542    this.populateB
+00000730: 6f64 7928 7468 6973 2e6e 6f64 6529 3b0a  ody(this.node);.
+00000740: 2020 2020 7468 6973 2e61 6464 436c 6173      this.addClas
+00000750: 7328 276a 702d 7368 6172 6564 2d6c 696e  s('jp-shared-lin
+00000760: 6b2d 626f 6479 2729 3b0a 2020 7d0a 0a20  k-body');.  }.. 
+00000770: 202f 2a2a 0a20 2020 2a20 5265 7475 726e   /**.   * Return
+00000780: 7320 7468 6520 696e 7075 7420 7661 6c75  s the input valu
+00000790: 652e 0a20 2020 2a2f 0a20 2067 6574 5661  e..   */.  getVa
+000007a0: 6c75 6528 293a 2073 7472 696e 6720 7b0a  lue(): string {.
+000007b0: 2020 2020 636f 6e73 7420 7769 7468 546f      const withTo
+000007c0: 6b65 6e20 3d20 7468 6973 2e5f 746f 6b65  ken = this._toke
+000007d0: 6e43 6865 636b 626f 783f 2e63 6865 636b  nCheckbox?.check
+000007e0: 6564 203d 3d3d 2074 7275 653b 0a0a 2020  ed === true;..  
+000007f0: 2020 6966 2028 7769 7468 546f 6b65 6e29    if (withToken)
+00000800: 207b 0a20 2020 2020 2063 6f6e 7374 2075   {.      const u
+00000810: 726c 5f20 3d20 6e65 7720 5552 4c28 7468  rl_ = new URL(th
+00000820: 6973 2e5f 7572 6c29 3b0a 2020 2020 2020  is._url);.      
+00000830: 7572 6c5f 2e73 6561 7263 6850 6172 616d  url_.searchParam
+00000840: 732e 7365 7428 2774 6f6b 656e 272c 2074  s.set('token', t
+00000850: 6869 732e 5f74 6f6b 656e 293b 0a20 2020  his._token);.   
+00000860: 2020 2072 6574 7572 6e20 7572 6c5f 2e74     return url_.t
+00000870: 6f53 7472 696e 6728 293b 0a20 2020 207d  oString();.    }
+00000880: 2065 6c73 6520 7b0a 2020 2020 2020 7265   else {.      re
+00000890: 7475 726e 2074 6869 732e 5f75 726c 3b0a  turn this._url;.
+000008a0: 2020 2020 7d0a 2020 7d0a 0a20 2070 726f      }.  }..  pro
+000008b0: 7465 6374 6564 206f 6e41 6674 6572 4174  tected onAfterAt
+000008c0: 7461 6368 286d 7367 3a20 4d65 7373 6167  tach(msg: Messag
+000008d0: 6529 3a20 766f 6964 207b 0a20 2020 2073  e): void {.    s
+000008e0: 7570 6572 2e6f 6e41 6674 6572 4174 7461  uper.onAfterAtta
+000008f0: 6368 286d 7367 293b 0a20 2020 2074 6869  ch(msg);.    thi
+00000900: 732e 5f74 6f6b 656e 4368 6563 6b62 6f78  s._tokenCheckbox
+00000910: 3f2e 6164 6445 7665 6e74 4c69 7374 656e  ?.addEventListen
+00000920: 6572 2827 6368 616e 6765 272c 2074 6869  er('change', thi
+00000930: 732e 6f6e 546f 6b65 6e43 6861 6e67 6529  s.onTokenChange)
+00000940: 3b0a 2020 7d0a 0a20 2070 726f 7465 6374  ;.  }..  protect
+00000950: 6564 206f 6e42 6566 6f72 6544 6574 6163  ed onBeforeDetac
+00000960: 6828 6d73 673a 204d 6573 7361 6765 293a  h(msg: Message):
+00000970: 2076 6f69 6420 7b0a 2020 2020 7468 6973   void {.    this
+00000980: 2e5f 746f 6b65 6e43 6865 636b 626f 783f  ._tokenCheckbox?
+00000990: 2e72 656d 6f76 6545 7665 6e74 4c69 7374  .removeEventList
+000009a0: 656e 6572 2827 6368 616e 6765 272c 2074  ener('change', t
+000009b0: 6869 732e 6f6e 546f 6b65 6e43 6861 6e67  his.onTokenChang
+000009c0: 6529 3b0a 2020 2020 7375 7065 722e 6f6e  e);.    super.on
+000009d0: 4265 666f 7265 4465 7461 6368 286d 7367  BeforeDetach(msg
+000009e0: 293b 0a20 207d 0a0a 2020 7072 6976 6174  );.  }..  privat
+000009f0: 6520 7570 6461 7465 436f 6e74 656e 7428  e updateContent(
+00000a00: 7769 7468 546f 6b65 6e3a 2062 6f6f 6c65  withToken: boole
+00000a10: 616e 293a 2076 6f69 6420 7b0a 2020 2020  an): void {.    
+00000a20: 7468 6973 2e5f 7761 726e 696e 672e 696e  this._warning.in
+00000a30: 6e65 7248 544d 4c20 3d20 2727 3b0a 2020  nerHTML = '';.  
+00000a40: 2020 636f 6e73 7420 7572 6c49 6e70 7574    const urlInput
+00000a50: 203d 0a20 2020 2020 2074 6869 732e 6e6f   =.      this.no
+00000a60: 6465 2e71 7565 7279 5365 6c65 6374 6f72  de.querySelector
+00000a70: 3c48 544d 4c49 6e70 7574 456c 656d 656e  <HTMLInputElemen
+00000a80: 743e 2827 696e 7075 745b 7265 6164 6f6e  t>('input[readon
+00000a90: 6c79 5d27 293b 0a20 2020 2069 6620 2877  ly]');.    if (w
+00000aa0: 6974 6854 6f6b 656e 2920 7b0a 2020 2020  ithToken) {.    
+00000ab0: 2020 6966 2028 7572 6c49 6e70 7574 2920    if (urlInput) 
+00000ac0: 7b0a 2020 2020 2020 2020 636f 6e73 7420  {.        const 
+00000ad0: 7572 6c5f 203d 206e 6577 2055 524c 2874  url_ = new URL(t
+00000ae0: 6869 732e 5f75 726c 293b 0a20 2020 2020  his._url);.     
+00000af0: 2020 2075 726c 5f2e 7365 6172 6368 5061     url_.searchPa
+00000b00: 7261 6d73 2e73 6574 2827 746f 6b65 6e27  rams.set('token'
+00000b10: 2c20 7468 6973 2e5f 746f 6b65 6e2e 736c  , this._token.sl
+00000b20: 6963 6528 302c 2035 2929 3b0a 2020 2020  ice(0, 5));.    
+00000b30: 2020 2020 7572 6c49 6e70 7574 2e76 616c      urlInput.val
+00000b40: 7565 203d 2075 726c 5f2e 746f 5374 7269  ue = url_.toStri
+00000b50: 6e67 2829 202b 2027 e280 a627 3b0a 2020  ng() + '...';.  
+00000b60: 2020 2020 7d0a 2020 2020 2020 7468 6973      }.      this
+00000b70: 2e5f 7761 726e 696e 672e 6170 7065 6e64  ._warning.append
+00000b80: 4368 696c 6428 646f 6375 6d65 6e74 2e63  Child(document.c
+00000b90: 7265 6174 6545 6c65 6d65 6e74 2827 6833  reateElement('h3
+00000ba0: 2729 292e 7465 7874 436f 6e74 656e 7420  ')).textContent 
+00000bb0: 3d0a 2020 2020 2020 2020 7468 6973 2e5f  =.        this._
+00000bc0: 7472 616e 732e 5f5f 2827 5365 6375 7269  trans.__('Securi
+00000bd0: 7479 2077 6172 6e69 6e67 2127 293b 0a20  ty warning!');. 
+00000be0: 2020 2020 2074 6869 732e 5f77 6172 6e69       this._warni
+00000bf0: 6e67 2e69 6e73 6572 7441 646a 6163 656e  ng.insertAdjacen
+00000c00: 7454 6578 7428 0a20 2020 2020 2020 2027  tText(.        '
+00000c10: 6265 666f 7265 656e 6427 2c0a 2020 2020  beforeend',.    
+00000c20: 2020 2020 7468 6973 2e5f 7472 616e 732e      this._trans.
+00000c30: 5f5f 280a 2020 2020 2020 2020 2020 2741  __(.          'A
+00000c40: 6e79 6f6e 6520 7769 7468 2074 6869 7320  nyone with this 
+00000c50: 6c69 6e6b 2068 6173 2066 756c 6c20 6163  link has full ac
+00000c60: 6365 7373 2074 6f20 796f 7572 206e 6f74  cess to your not
+00000c70: 6562 6f6f 6b20 7365 7276 6572 2c20 696e  ebook server, in
+00000c80: 636c 7564 696e 6720 616c 6c20 796f 7572  cluding all your
+00000c90: 2066 696c 6573 2127 0a20 2020 2020 2020   files!'.       
+00000ca0: 2029 0a20 2020 2020 2029 3b0a 2020 2020   ).      );.    
+00000cb0: 2020 7468 6973 2e5f 7761 726e 696e 672e    this._warning.
+00000cc0: 696e 7365 7274 4164 6a61 6365 6e74 4854  insertAdjacentHT
+00000cd0: 4d4c 2827 6265 666f 7265 656e 6427 2c20  ML('beforeend', 
+00000ce0: 273c 6272 3e27 293b 0a20 2020 2020 2074  '<br>');.      t
+00000cf0: 6869 732e 5f77 6172 6e69 6e67 2e69 6e73  his._warning.ins
+00000d00: 6572 7441 646a 6163 656e 7454 6578 7428  ertAdjacentText(
+00000d10: 0a20 2020 2020 2020 2027 6265 666f 7265  .        'before
+00000d20: 656e 6427 2c0a 2020 2020 2020 2020 7468  end',.        th
+00000d30: 6973 2e5f 7472 616e 732e 5f5f 2827 506c  is._trans.__('Pl
+00000d40: 6561 7365 2062 6520 6361 7265 6675 6c20  ease be careful 
+00000d50: 7768 6f20 796f 7520 7368 6172 6520 6974  who you share it
+00000d60: 2077 6974 682e 2729 0a20 2020 2020 2029   with.').      )
+00000d70: 3b0a 2020 2020 2020 7468 6973 2e5f 7761  ;.      this._wa
+00000d80: 726e 696e 672e 696e 7365 7274 4164 6a61  rning.insertAdja
+00000d90: 6365 6e74 4854 4d4c 2827 6265 666f 7265  centHTML('before
+00000da0: 656e 6427 2c20 273c 6272 3e27 293b 0a20  end', '<br>');. 
+00000db0: 2020 2020 2069 6620 2874 6869 732e 5f62       if (this._b
+00000dc0: 6568 696e 6448 7562 2920 7b0a 2020 2020  ehindHub) {.    
+00000dd0: 2020 2020 7468 6973 2e5f 7761 726e 696e      this._warnin
+00000de0: 672e 696e 7365 7274 4164 6a61 6365 6e74  g.insertAdjacent
+00000df0: 5465 7874 280a 2020 2020 2020 2020 2020  Text(.          
+00000e00: 2762 6566 6f72 6565 6e64 272c 202f 2f20  'beforeend', // 
+00000e10: 596f 7520 6361 6e20 7265 7374 6172 7420  You can restart 
+00000e20: 7468 6520 7365 7276 6572 2074 6f20 7265  the server to re
+00000e30: 766f 6b65 2074 6865 2074 6f6b 656e 2069  voke the token i
+00000e40: 6e20 6120 4a75 7079 7465 7248 7562 0a20  n a JupyterHub. 
+00000e50: 2020 2020 2020 2020 2074 6869 732e 5f74           this._t
+00000e60: 7261 6e73 2e5f 5f28 2754 6865 7920 7769  rans.__('They wi
+00000e70: 6c6c 2062 6520 6162 6c65 2074 6f20 6163  ll be able to ac
+00000e80: 6365 7373 2074 6869 7320 7365 7276 6572  cess this server
+00000e90: 2041 5320 594f 552e 2729 0a20 2020 2020   AS YOU.').     
+00000ea0: 2020 2029 3b0a 2020 2020 2020 2020 7468     );.        th
+00000eb0: 6973 2e5f 7761 726e 696e 672e 696e 7365  is._warning.inse
+00000ec0: 7274 4164 6a61 6365 6e74 4854 4d4c 2827  rtAdjacentHTML('
+00000ed0: 6265 666f 7265 656e 6427 2c20 273c 6272  beforeend', '<br
+00000ee0: 3e27 293b 0a20 2020 2020 2020 2074 6869  >');.        thi
+00000ef0: 732e 5f77 6172 6e69 6e67 2e69 6e73 6572  s._warning.inser
+00000f00: 7441 646a 6163 656e 7454 6578 7428 0a20  tAdjacentText(. 
+00000f10: 2020 2020 2020 2020 2027 6265 666f 7265           'before
+00000f20: 656e 6427 2c0a 2020 2020 2020 2020 2020  end',.          
+00000f30: 7468 6973 2e5f 7472 616e 732e 5f5f 280a  this._trans.__(.
+00000f40: 2020 2020 2020 2020 2020 2020 2754 6f20              'To 
+00000f50: 7265 766f 6b65 2061 6363 6573 732c 2067  revoke access, g
+00000f60: 6f20 746f 2046 696c 6520 2d3e 2048 7562  o to File -> Hub
+00000f70: 2043 6f6e 7472 6f6c 2050 616e 656c 2c20   Control Panel, 
+00000f80: 616e 6420 7265 7374 6172 7420 796f 7572  and restart your
+00000f90: 2073 6572 7665 722e 270a 2020 2020 2020   server.'.      
+00000fa0: 2020 2020 290a 2020 2020 2020 2020 293b      ).        );
+00000fb0: 0a20 2020 2020 207d 2065 6c73 6520 7b0a  .      } else {.
+00000fc0: 2020 2020 2020 2020 7468 6973 2e5f 7761          this._wa
+00000fd0: 726e 696e 672e 696e 7365 7274 4164 6a61  rning.insertAdja
+00000fe0: 6365 6e74 5465 7874 280a 2020 2020 2020  centText(.      
+00000ff0: 2020 2020 2762 6566 6f72 6565 6e64 272c      'beforeend',
+00001000: 0a20 2020 2020 2020 2020 202f 2f20 456c  .          // El
+00001010: 7365 7768 6572 652c 2079 6f75 202a 6d75  sewhere, you *mu
+00001020: 7374 2a20 7368 7574 2064 6f77 6e20 796f  st* shut down yo
+00001030: 7572 2073 6572 7665 7220 2d20 6e6f 2077  ur server - no w
+00001040: 6179 2074 6f20 7265 766f 6b65 2069 740a  ay to revoke it.
+00001050: 2020 2020 2020 2020 2020 7468 6973 2e5f            this._
+00001060: 7472 616e 732e 5f5f 280a 2020 2020 2020  trans.__(.      
+00001070: 2020 2020 2020 2743 7572 7265 6e74 6c79        'Currently
+00001080: 2c20 7468 6572 6520 6973 206e 6f20 7761  , there is no wa
+00001090: 7920 746f 2072 6576 6f6b 6520 6163 6365  y to revoke acce
+000010a0: 7373 206f 7468 6572 2074 6861 6e20 7368  ss other than sh
+000010b0: 7574 7469 6e67 2064 6f77 6e20 796f 7572  utting down your
+000010c0: 2073 6572 7665 722e 270a 2020 2020 2020   server.'.      
+000010d0: 2020 2020 290a 2020 2020 2020 2020 293b      ).        );
+000010e0: 0a20 2020 2020 207d 0a20 2020 207d 2065  .      }.    } e
+000010f0: 6c73 6520 7b0a 2020 2020 2020 6966 2028  lse {.      if (
+00001100: 7572 6c49 6e70 7574 2920 7b0a 2020 2020  urlInput) {.    
+00001110: 2020 2020 7572 6c49 6e70 7574 2e76 616c      urlInput.val
+00001120: 7565 203d 2074 6869 732e 5f75 726c 3b0a  ue = this._url;.
+00001130: 2020 2020 2020 7d0a 2020 2020 2020 6966        }.      if
+00001140: 2028 7468 6973 2e5f 6265 6869 6e64 4875   (this._behindHu
+00001150: 6229 207b 0a20 2020 2020 2020 2074 6869  b) {.        thi
+00001160: 732e 5f77 6172 6e69 6e67 2e69 6e73 6572  s._warning.inser
+00001170: 7441 646a 6163 656e 7454 6578 7428 0a20  tAdjacentText(. 
+00001180: 2020 2020 2020 2020 2027 6265 666f 7265           'before
+00001190: 656e 6427 2c0a 2020 2020 2020 2020 2020  end',.          
+000011a0: 7468 6973 2e5f 7472 616e 732e 5f5f 280a  this._trans.__(.
+000011b0: 2020 2020 2020 2020 2020 2020 274f 6e6c              'Onl
+000011c0: 7920 7573 6572 7320 7769 7468 2060 6163  y users with `ac
+000011d0: 6365 7373 3a73 6572 7665 7273 6020 7065  cess:servers` pe
+000011e0: 726d 6973 7369 6f6e 7320 666f 7220 7468  rmissions for th
+000011f0: 6973 2073 6572 7665 7220 7769 6c6c 2062  is server will b
+00001200: 6520 6162 6c65 2074 6f20 7573 6520 7468  e able to use th
+00001210: 6973 206c 696e 6b2e 270a 2020 2020 2020  is link.'.      
+00001220: 2020 2020 290a 2020 2020 2020 2020 293b      ).        );
+00001230: 0a20 2020 2020 207d 2065 6c73 6520 7b0a  .      } else {.
+00001240: 2020 2020 2020 2020 7468 6973 2e5f 7761          this._wa
+00001250: 726e 696e 672e 696e 7365 7274 4164 6a61  rning.insertAdja
+00001260: 6365 6e74 5465 7874 280a 2020 2020 2020  centText(.      
+00001270: 2020 2020 2762 6566 6f72 6565 6e64 272c      'beforeend',
+00001280: 0a20 2020 2020 2020 2020 2074 6869 732e  .          this.
+00001290: 5f74 7261 6e73 2e5f 5f28 0a20 2020 2020  _trans.__(.     
+000012a0: 2020 2020 2020 2027 4f6e 6c79 2061 7574         'Only aut
+000012b0: 6865 6e74 6963 6174 6564 2075 7365 7273  henticated users
+000012c0: 2077 696c 6c20 6265 2061 626c 6520 746f   will be able to
+000012d0: 2075 7365 2074 6869 7320 6c69 6e6b 2e27   use this link.'
+000012e0: 0a20 2020 2020 2020 2020 2029 0a20 2020  .          ).   
+000012f0: 2020 2020 2029 3b0a 2020 2020 2020 7d0a       );.      }.
+00001300: 2020 2020 7d0a 2020 7d0a 0a20 2070 7269      }.  }..  pri
+00001310: 7661 7465 206f 6e54 6f6b 656e 4368 616e  vate onTokenChan
+00001320: 6765 203d 2028 653a 2045 7665 6e74 2920  ge = (e: Event) 
+00001330: 3d3e 207b 0a20 2020 2063 6f6e 7374 2074  => {.    const t
+00001340: 6172 6765 7420 3d20 652e 7461 7267 6574  arget = e.target
+00001350: 2061 7320 4854 4d4c 496e 7075 7445 6c65   as HTMLInputEle
+00001360: 6d65 6e74 3b0a 2020 2020 7468 6973 2e75  ment;.    this.u
+00001370: 7064 6174 6543 6f6e 7465 6e74 2874 6172  pdateContent(tar
+00001380: 6765 743f 2e63 6865 636b 6564 293b 0a20  get?.checked);. 
+00001390: 207d 3b0a 0a20 2070 7269 7661 7465 2070   };..  private p
+000013a0: 6f70 756c 6174 6542 6f64 7928 6469 616c  opulateBody(dial
+000013b0: 6f67 426f 6479 3a20 4854 4d4c 456c 656d  ogBody: HTMLElem
+000013c0: 656e 7429 3a20 766f 6964 207b 0a20 2020  ent): void {.   
+000013d0: 2064 6961 6c6f 6742 6f64 792e 696e 7365   dialogBody.inse
+000013e0: 7274 4164 6a61 6365 6e74 4854 4d4c 280a  rtAdjacentHTML(.
+000013f0: 2020 2020 2020 2761 6674 6572 6265 6769        'afterbegi
+00001400: 6e27 2c0a 2020 2020 2020 603c 696e 7075  n',.      `<inpu
+00001410: 7420 7265 6164 6f6e 6c79 2076 616c 7565  t readonly value
+00001420: 3d22 247b 7468 6973 2e5f 7572 6c7d 223e  ="${this._url}">
+00001430: 600a 2020 2020 293b 0a0a 2020 2020 6966  `.    );..    if
+00001440: 2028 7468 6973 2e5f 746f 6b65 6e29 207b   (this._token) {
+00001450: 0a20 2020 2020 2063 6f6e 7374 206c 6162  .      const lab
+00001460: 656c 203d 2064 6961 6c6f 6742 6f64 792e  el = dialogBody.
+00001470: 6170 7065 6e64 4368 696c 6428 646f 6375  appendChild(docu
+00001480: 6d65 6e74 2e63 7265 6174 6545 6c65 6d65  ment.createEleme
+00001490: 6e74 2827 6c61 6265 6c27 2929 3b0a 2020  nt('label'));.  
+000014a0: 2020 2020 6c61 6265 6c2e 696e 7365 7274      label.insert
+000014b0: 4164 6a61 6365 6e74 4854 4d4c 2827 6265  AdjacentHTML('be
+000014c0: 666f 7265 656e 6427 2c20 273c 696e 7075  foreend', '<inpu
+000014d0: 7420 7479 7065 3d22 6368 6563 6b62 6f78  t type="checkbox
+000014e0: 223e 2729 3b0a 2020 2020 2020 7468 6973  ">');.      this
+000014f0: 2e5f 746f 6b65 6e43 6865 636b 626f 7820  ._tokenCheckbox 
+00001500: 3d20 6c61 6265 6c2e 6669 7273 7443 6869  = label.firstChi
+00001510: 6c64 2061 7320 4854 4d4c 496e 7075 7445  ld as HTMLInputE
+00001520: 6c65 6d65 6e74 3b0a 2020 2020 2020 6c61  lement;.      la
+00001530: 6265 6c2e 696e 7365 7274 4164 6a61 6365  bel.insertAdjace
+00001540: 6e74 5465 7874 280a 2020 2020 2020 2020  ntText(.        
+00001550: 2762 6566 6f72 6565 6e64 272c 0a20 2020  'beforeend',.   
+00001560: 2020 2020 2074 6869 732e 5f74 7261 6e73       this._trans
+00001570: 2e5f 5f28 2749 6e63 6c75 6465 2074 6f6b  .__('Include tok
+00001580: 656e 2069 6e20 5552 4c27 290a 2020 2020  en in URL').    
+00001590: 2020 293b 0a20 2020 2020 2064 6961 6c6f    );.      dialo
+000015a0: 6742 6f64 792e 696e 7365 7274 4164 6a61  gBody.insertAdja
+000015b0: 6365 6e74 456c 656d 656e 7428 2762 6566  centElement('bef
+000015c0: 6f72 6565 6e64 272c 2074 6869 732e 5f77  oreend', this._w
+000015d0: 6172 6e69 6e67 293b 0a20 2020 2020 2074  arning);.      t
+000015e0: 6869 732e 7570 6461 7465 436f 6e74 656e  his.updateConten
+000015f0: 7428 6661 6c73 6529 3b0a 2020 2020 7d0a  t(false);.    }.
+00001600: 2020 7d0a 7d0a                             }.}.
```

### Comparing `jupyter_collaboration_ui-1.0.0a0/packages/collaboration/lib/userinfopanel.js` & `jupyter_collaboration_ui-1.0.0a1/packages/collaboration/src/userinfopanel.tsx`

 * *Files 11% similar despite different names*

```diff
@@ -1,88 +1,92 @@
 00000000: 2f2f 2043 6f70 7972 6967 6874 2028 6329  // Copyright (c)
 00000010: 204a 7570 7974 6572 2044 6576 656c 6f70   Jupyter Develop
 00000020: 6d65 6e74 2054 6561 6d2e 0a2f 2f20 4469  ment Team..// Di
 00000030: 7374 7269 6275 7465 6420 756e 6465 7220  stributed under 
 00000040: 7468 6520 7465 726d 7320 6f66 2074 6865  the terms of the
 00000050: 204d 6f64 6966 6965 6420 4253 4420 4c69   Modified BSD Li
-00000060: 6365 6e73 652e 0a69 6d70 6f72 7420 7b20  cense..import { 
-00000070: 5265 6163 7457 6964 6765 7420 7d20 6672  ReactWidget } fr
-00000080: 6f6d 2027 406a 7570 7974 6572 6c61 622f  om '@jupyterlab/
-00000090: 6170 7075 7469 6c73 273b 0a69 6d70 6f72  apputils';.impor
-000000a0: 7420 7b20 5061 6e65 6c20 7d20 6672 6f6d  t { Panel } from
-000000b0: 2027 406c 756d 696e 6f2f 7769 6467 6574   '@lumino/widget
-000000c0: 7327 3b0a 696d 706f 7274 202a 2061 7320  s';.import * as 
-000000d0: 5265 6163 7420 6672 6f6d 2027 7265 6163  React from 'reac
-000000e0: 7427 3b0a 696d 706f 7274 207b 2055 7365  t';.import { Use
-000000f0: 7249 636f 6e43 6f6d 706f 6e65 6e74 207d  rIconComponent }
-00000100: 2066 726f 6d20 272e 2f63 6f6d 706f 6e65   from './compone
-00000110: 6e74 7327 3b0a 6578 706f 7274 2063 6c61  nts';.export cla
-00000120: 7373 2055 7365 7249 6e66 6f50 616e 656c  ss UserInfoPanel
-00000130: 2065 7874 656e 6473 2050 616e 656c 207b   extends Panel {
-00000140: 0a20 2020 2063 6f6e 7374 7275 6374 6f72  .    constructor
-00000150: 2875 7365 7229 207b 0a20 2020 2020 2020  (user) {.       
-00000160: 2073 7570 6572 287b 7d29 3b0a 2020 2020   super({});.    
-00000170: 2020 2020 7468 6973 2e61 6464 436c 6173      this.addClas
-00000180: 7328 276a 702d 5573 6572 496e 666f 5061  s('jp-UserInfoPa
-00000190: 6e65 6c27 293b 0a20 2020 2020 2020 2074  nel');.        t
-000001a0: 6869 732e 5f70 726f 6669 6c65 203d 2075  his._profile = u
-000001b0: 7365 723b 0a20 2020 2020 2020 2074 6869  ser;.        thi
-000001c0: 732e 5f62 6f64 7920 3d20 6e75 6c6c 3b0a  s._body = null;.
-000001d0: 2020 2020 2020 2020 6966 2028 7468 6973          if (this
-000001e0: 2e5f 7072 6f66 696c 652e 6973 5265 6164  ._profile.isRead
-000001f0: 7929 207b 0a20 2020 2020 2020 2020 2020  y) {.           
-00000200: 2074 6869 732e 5f62 6f64 7920 3d20 6e65   this._body = ne
-00000210: 7720 5573 6572 496e 666f 426f 6479 2874  w UserInfoBody(t
-00000220: 6869 732e 5f70 726f 6669 6c65 2e69 6465  his._profile.ide
-00000230: 6e74 6974 7929 3b0a 2020 2020 2020 2020  ntity);.        
-00000240: 2020 2020 7468 6973 2e61 6464 5769 6467      this.addWidg
-00000250: 6574 2874 6869 732e 5f62 6f64 7929 3b0a  et(this._body);.
-00000260: 2020 2020 2020 2020 2020 2020 7468 6973              this
-00000270: 2e75 7064 6174 6528 293b 0a20 2020 2020  .update();.     
-00000280: 2020 207d 0a20 2020 2020 2020 2065 6c73     }.        els
-00000290: 6520 7b0a 2020 2020 2020 2020 2020 2020  e {.            
-000002a0: 7468 6973 2e5f 7072 6f66 696c 652e 7265  this._profile.re
-000002b0: 6164 790a 2020 2020 2020 2020 2020 2020  ady.            
-000002c0: 2020 2020 2e74 6865 6e28 2829 203d 3e20      .then(() => 
-000002d0: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-000002e0: 2020 7468 6973 2e5f 626f 6479 203d 206e    this._body = n
-000002f0: 6577 2055 7365 7249 6e66 6f42 6f64 7928  ew UserInfoBody(
-00000300: 7468 6973 2e5f 7072 6f66 696c 652e 6964  this._profile.id
-00000310: 656e 7469 7479 293b 0a20 2020 2020 2020  entity);.       
-00000320: 2020 2020 2020 2020 2074 6869 732e 6164           this.ad
-00000330: 6457 6964 6765 7428 7468 6973 2e5f 626f  dWidget(this._bo
-00000340: 6479 293b 0a20 2020 2020 2020 2020 2020  dy);.           
-00000350: 2020 2020 2074 6869 732e 7570 6461 7465       this.update
-00000360: 2829 3b0a 2020 2020 2020 2020 2020 2020  ();.            
-00000370: 7d29 0a20 2020 2020 2020 2020 2020 2020  }).             
-00000380: 2020 202e 6361 7463 6828 6520 3d3e 2063     .catch(e => c
-00000390: 6f6e 736f 6c65 2e65 7272 6f72 2865 2929  onsole.error(e))
-000003a0: 3b0a 2020 2020 2020 2020 7d0a 2020 2020  ;.        }.    
-000003b0: 7d0a 7d0a 2f2a 2a0a 202a 2041 2053 6574  }.}./**. * A Set
-000003c0: 7469 6e67 7357 6964 6765 7420 666f 7220  tingsWidget for 
-000003d0: 7468 6520 7573 6572 2e0a 202a 2f0a 6578  the user.. */.ex
-000003e0: 706f 7274 2063 6c61 7373 2055 7365 7249  port class UserI
-000003f0: 6e66 6f42 6f64 7920 6578 7465 6e64 7320  nfoBody extends 
-00000400: 5265 6163 7457 6964 6765 7420 7b0a 2020  ReactWidget {.  
-00000410: 2020 2f2a 2a0a 2020 2020 202a 2043 6f6e    /**.     * Con
-00000420: 7374 7275 6374 7320 6120 6e65 7720 7365  structs a new se
-00000430: 7474 696e 6773 2077 6964 6765 742e 0a20  ttings widget.. 
-00000440: 2020 2020 2a2f 0a20 2020 2063 6f6e 7374      */.    const
-00000450: 7275 6374 6f72 2875 7365 7229 207b 0a20  ructor(user) {. 
-00000460: 2020 2020 2020 2073 7570 6572 2829 3b0a         super();.
-00000470: 2020 2020 2020 2020 7468 6973 2e5f 7573          this._us
-00000480: 6572 203d 2075 7365 723b 0a20 2020 207d  er = user;.    }
-00000490: 0a20 2020 2067 6574 2075 7365 7228 2920  .    get user() 
-000004a0: 7b0a 2020 2020 2020 2020 7265 7475 726e  {.        return
-000004b0: 2074 6869 732e 5f75 7365 723b 0a20 2020   this._user;.   
-000004c0: 207d 0a20 2020 2073 6574 2075 7365 7228   }.    set user(
-000004d0: 7573 6572 2920 7b0a 2020 2020 2020 2020  user) {.        
-000004e0: 7468 6973 2e5f 7573 6572 203d 2075 7365  this._user = use
-000004f0: 723b 0a20 2020 2020 2020 2074 6869 732e  r;.        this.
-00000500: 7570 6461 7465 2829 3b0a 2020 2020 7d0a  update();.    }.
-00000510: 2020 2020 7265 6e64 6572 2829 207b 0a20      render() {. 
-00000520: 2020 2020 2020 2072 6574 7572 6e20 5265         return Re
-00000530: 6163 742e 6372 6561 7465 456c 656d 656e  act.createElemen
-00000540: 7428 5573 6572 4963 6f6e 436f 6d70 6f6e  t(UserIconCompon
-00000550: 656e 742c 207b 2075 7365 723a 2074 6869  ent, { user: thi
-00000560: 732e 5f75 7365 7220 7d29 3b0a 2020 2020  s._user });.    
-00000570: 7d0a 7d0a                                }.}.
+00000060: 6365 6e73 652e 0a0a 696d 706f 7274 207b  cense...import {
+00000070: 2052 6561 6374 5769 6467 6574 207d 2066   ReactWidget } f
+00000080: 726f 6d20 2740 6a75 7079 7465 726c 6162  rom '@jupyterlab
+00000090: 2f61 7070 7574 696c 7327 3b0a 0a69 6d70  /apputils';..imp
+000000a0: 6f72 7420 7b20 5573 6572 207d 2066 726f  ort { User } fro
+000000b0: 6d20 2740 6a75 7079 7465 726c 6162 2f73  m '@jupyterlab/s
+000000c0: 6572 7669 6365 7327 3b0a 0a69 6d70 6f72  ervices';..impor
+000000d0: 7420 7b20 5061 6e65 6c20 7d20 6672 6f6d  t { Panel } from
+000000e0: 2027 406c 756d 696e 6f2f 7769 6467 6574   '@lumino/widget
+000000f0: 7327 3b0a 0a69 6d70 6f72 7420 2a20 6173  s';..import * as
+00000100: 2052 6561 6374 2066 726f 6d20 2772 6561   React from 'rea
+00000110: 6374 273b 0a0a 696d 706f 7274 207b 2055  ct';..import { U
+00000120: 7365 7249 636f 6e43 6f6d 706f 6e65 6e74  serIconComponent
+00000130: 207d 2066 726f 6d20 272e 2f63 6f6d 706f   } from './compo
+00000140: 6e65 6e74 7327 3b0a 0a65 7870 6f72 7420  nents';..export 
+00000150: 636c 6173 7320 5573 6572 496e 666f 5061  class UserInfoPa
+00000160: 6e65 6c20 6578 7465 6e64 7320 5061 6e65  nel extends Pane
+00000170: 6c20 7b0a 2020 7072 6976 6174 6520 5f70  l {.  private _p
+00000180: 726f 6669 6c65 3a20 5573 6572 2e49 4d61  rofile: User.IMa
+00000190: 6e61 6765 723b 0a20 2070 7269 7661 7465  nager;.  private
+000001a0: 205f 626f 6479 3a20 5573 6572 496e 666f   _body: UserInfo
+000001b0: 426f 6479 207c 206e 756c 6c3b 0a0a 2020  Body | null;..  
+000001c0: 636f 6e73 7472 7563 746f 7228 7573 6572  constructor(user
+000001d0: 3a20 5573 6572 2e49 4d61 6e61 6765 7229  : User.IManager)
+000001e0: 207b 0a20 2020 2073 7570 6572 287b 7d29   {.    super({})
+000001f0: 3b0a 2020 2020 7468 6973 2e61 6464 436c  ;.    this.addCl
+00000200: 6173 7328 276a 702d 5573 6572 496e 666f  ass('jp-UserInfo
+00000210: 5061 6e65 6c27 293b 0a0a 2020 2020 7468  Panel');..    th
+00000220: 6973 2e5f 7072 6f66 696c 6520 3d20 7573  is._profile = us
+00000230: 6572 3b0a 2020 2020 7468 6973 2e5f 626f  er;.    this._bo
+00000240: 6479 203d 206e 756c 6c3b 0a0a 2020 2020  dy = null;..    
+00000250: 6966 2028 7468 6973 2e5f 7072 6f66 696c  if (this._profil
+00000260: 652e 6973 5265 6164 7929 207b 0a20 2020  e.isReady) {.   
+00000270: 2020 2074 6869 732e 5f62 6f64 7920 3d20     this._body = 
+00000280: 6e65 7720 5573 6572 496e 666f 426f 6479  new UserInfoBody
+00000290: 2874 6869 732e 5f70 726f 6669 6c65 2e69  (this._profile.i
+000002a0: 6465 6e74 6974 7921 293b 0a20 2020 2020  dentity!);.     
+000002b0: 2074 6869 732e 6164 6457 6964 6765 7428   this.addWidget(
+000002c0: 7468 6973 2e5f 626f 6479 293b 0a20 2020  this._body);.   
+000002d0: 2020 2074 6869 732e 7570 6461 7465 2829     this.update()
+000002e0: 3b0a 2020 2020 7d20 656c 7365 207b 0a20  ;.    } else {. 
+000002f0: 2020 2020 2074 6869 732e 5f70 726f 6669       this._profi
+00000300: 6c65 2e72 6561 6479 0a20 2020 2020 2020  le.ready.       
+00000310: 202e 7468 656e 2828 2920 3d3e 207b 0a20   .then(() => {. 
+00000320: 2020 2020 2020 2020 2074 6869 732e 5f62           this._b
+00000330: 6f64 7920 3d20 6e65 7720 5573 6572 496e  ody = new UserIn
+00000340: 666f 426f 6479 2874 6869 732e 5f70 726f  foBody(this._pro
+00000350: 6669 6c65 2e69 6465 6e74 6974 7921 293b  file.identity!);
+00000360: 0a20 2020 2020 2020 2020 2074 6869 732e  .          this.
+00000370: 6164 6457 6964 6765 7428 7468 6973 2e5f  addWidget(this._
+00000380: 626f 6479 293b 0a20 2020 2020 2020 2020  body);.         
+00000390: 2074 6869 732e 7570 6461 7465 2829 3b0a   this.update();.
+000003a0: 2020 2020 2020 2020 7d29 0a20 2020 2020          }).     
+000003b0: 2020 202e 6361 7463 6828 6520 3d3e 2063     .catch(e => c
+000003c0: 6f6e 736f 6c65 2e65 7272 6f72 2865 2929  onsole.error(e))
+000003d0: 3b0a 2020 2020 7d0a 2020 7d0a 7d0a 0a2f  ;.    }.  }.}../
+000003e0: 2a2a 0a20 2a20 4120 5365 7474 696e 6773  **. * A Settings
+000003f0: 5769 6467 6574 2066 6f72 2074 6865 2075  Widget for the u
+00000400: 7365 722e 0a20 2a2f 0a65 7870 6f72 7420  ser.. */.export 
+00000410: 636c 6173 7320 5573 6572 496e 666f 426f  class UserInfoBo
+00000420: 6479 2065 7874 656e 6473 2052 6561 6374  dy extends React
+00000430: 5769 6467 6574 207b 0a20 2070 7269 7661  Widget {.  priva
+00000440: 7465 205f 7573 6572 3a20 5573 6572 2e49  te _user: User.I
+00000450: 4964 656e 7469 7479 3b0a 0a20 202f 2a2a  Identity;..  /**
+00000460: 0a20 2020 2a20 436f 6e73 7472 7563 7473  .   * Constructs
+00000470: 2061 206e 6577 2073 6574 7469 6e67 7320   a new settings 
+00000480: 7769 6467 6574 2e0a 2020 202a 2f0a 2020  widget..   */.  
+00000490: 636f 6e73 7472 7563 746f 7228 7573 6572  constructor(user
+000004a0: 3a20 5573 6572 2e49 4964 656e 7469 7479  : User.IIdentity
+000004b0: 2920 7b0a 2020 2020 7375 7065 7228 293b  ) {.    super();
+000004c0: 0a20 2020 2074 6869 732e 5f75 7365 7220  .    this._user 
+000004d0: 3d20 7573 6572 3b0a 2020 7d0a 0a20 2067  = user;.  }..  g
+000004e0: 6574 2075 7365 7228 293a 2055 7365 722e  et user(): User.
+000004f0: 4949 6465 6e74 6974 7920 7b0a 2020 2020  IIdentity {.    
+00000500: 7265 7475 726e 2074 6869 732e 5f75 7365  return this._use
+00000510: 723b 0a20 207d 0a0a 2020 7365 7420 7573  r;.  }..  set us
+00000520: 6572 2875 7365 723a 2055 7365 722e 4949  er(user: User.II
+00000530: 6465 6e74 6974 7929 207b 0a20 2020 2074  dentity) {.    t
+00000540: 6869 732e 5f75 7365 7220 3d20 7573 6572  his._user = user
+00000550: 3b0a 2020 2020 7468 6973 2e75 7064 6174  ;.    this.updat
+00000560: 6528 293b 0a20 207d 0a0a 2020 7265 6e64  e();.  }..  rend
+00000570: 6572 2829 3a20 4a53 582e 456c 656d 656e  er(): JSX.Elemen
+00000580: 7420 7b0a 2020 2020 7265 7475 726e 203c  t {.    return <
+00000590: 5573 6572 4963 6f6e 436f 6d70 6f6e 656e  UserIconComponen
+000005a0: 7420 7573 6572 3d7b 7468 6973 2e5f 7573  t user={this._us
+000005b0: 6572 7d20 2f3e 3b0a 2020 7d0a 7d0a       er} />;.  }.}.
```

### Comparing `jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/observables/package.json` & `jupyter_collaboration_ui-1.0.0a1/packages/docprovider/package.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7440656565656565%*

 * *Differences: {"'bugs'": "{'url': 'https://github.com/jupyterlab/jupyter-collaboration/issues'}",*

 * * "'dependencies'": "{'@lumino/coreutils': '^2.1.0', '@lumino/disposable': '^2.1.0', "*

 * *                   "'@lumino/signaling': '^2.1.0', '@jupyter/ydoc': '^1.1.0-a0', "*

 * *                   "'@jupyterlab/coreutils': '^6.0.5', '@jupyterlab/services': '^7.0.5', "*

 * *                   "'y-protocols': '^1.0.5', 'y-websocket': '^1.3.15', 'yjs': '^13.5.40', delete: "*

 * *                   "['@lumino/algorithm', '@lumino/messaging']}",*

 * * " […]*

```diff
@@ -1,57 +1,69 @@
 {
     "author": "Project Jupyter",
     "bugs": {
-        "url": "https://github.com/jupyterlab/jupyterlab/issues"
+        "url": "https://github.com/jupyterlab/jupyter-collaboration/issues"
     },
     "dependencies": {
-        "@lumino/algorithm": "^2.0.1",
-        "@lumino/coreutils": "^2.1.2",
-        "@lumino/disposable": "^2.1.2",
-        "@lumino/messaging": "^2.0.1",
-        "@lumino/signaling": "^2.1.2"
+        "@jupyter/ydoc": "^1.1.0-a0",
+        "@jupyterlab/coreutils": "^6.0.5",
+        "@jupyterlab/services": "^7.0.5",
+        "@lumino/coreutils": "^2.1.0",
+        "@lumino/disposable": "^2.1.0",
+        "@lumino/signaling": "^2.1.0",
+        "y-protocols": "^1.0.5",
+        "y-websocket": "^1.3.15",
+        "yjs": "^13.5.40"
     },
-    "description": "Data structures which may be observed for changes.",
+    "description": "JupyterLab - Document Provider",
     "devDependencies": {
-        "@jupyterlab/testing": "^4.1.6",
+        "@jupyterlab/testing": "^4.0.5",
         "@types/jest": "^29.2.0",
-        "jest": "^29.2.0",
-        "rimraf": "~5.0.5",
-        "typedoc": "~0.24.7",
-        "typescript": "~5.1.6"
+        "jest": "^29.5.0",
+        "rimraf": "^4.1.2",
+        "typescript": "~5.0.4"
     },
     "directories": {
         "lib": "lib/"
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
+        "schema/*.json",
         "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
-        "src/**/*.{ts,tsx}"
+        "style/index.js"
     ],
-    "homepage": "https://github.com/jupyterlab/jupyterlab",
+    "homepage": "https://github.com/jupyterlab/jupyter-collaboration",
     "license": "BSD-3-Clause",
     "main": "lib/index.js",
-    "name": "@jupyterlab/observables",
+    "name": "@jupyter/docprovider",
     "publishConfig": {
         "access": "public"
     },
     "repository": {
         "type": "git",
-        "url": "https://github.com/jupyterlab/jupyterlab.git"
+        "url": "https://github.com/jupyterlab/jupyter-collaboration.git"
     },
     "scripts": {
         "build": "tsc -b",
+        "build:prod": "jlpm run build",
         "build:test": "tsc --build tsconfig.test.json",
-        "clean": "rimraf lib && rimraf tsconfig.tsbuildinfo",
-        "docs": "typedoc src",
+        "clean": "rimraf lib tsconfig.tsbuildinfo",
+        "clean:all": "rimraf lib tsconfig.tsbuildinfo node_modules",
+        "clean:lib": "jlpm run clean:all",
+        "install:extension": "jlpm run build",
         "test": "jest",
         "test:cov": "jest --collect-coverage",
-        "test:debug": "node --inspect-brk ../../node_modules/.bin/jest --runInBand",
-        "test:debug:watch": "node --inspect-brk ../../node_modules/.bin/jest --runInBand --watch",
+        "test:debug": "node --inspect-brk node_modules/.bin/jest --runInBand",
+        "test:debug:watch": "node --inspect-brk node_modules/.bin/jest --runInBand --watch",
         "watch": "tsc -b --watch"
     },
     "sideEffects": [
         "style/**/*"
     ],
+    "typedoc": {
+        "displayName": "@jupyter/docprovider",
+        "entryPoint": "./src/index.ts",
+        "tsconfig": "./tsconfig.json"
+    },
     "types": "lib/index.d.ts",
-    "version": "5.1.6"
+    "version": "3.0.0-alpha.1"
 }
```

### Comparing `jupyter_collaboration_ui-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/collapse.css` & `jupyter_collaboration_ui-1.0.0a1/packages/collaboration/style/menu.css`

 * *Files 27% similar despite different names*

```diff
@@ -1,44 +1,41 @@
-/*-----------------------------------------------------------------------------
+/* -----------------------------------------------------------------------------
 | Copyright (c) Jupyter Development Team.
 | Distributed under the terms of the Modified BSD License.
-|----------------------------------------------------------------------------*/
+|---------------------------------------------------------------------------- */
 
-.jp-Collapse {
-  display: flex;
-  flex-direction: column;
-  align-items: stretch;
+.jp-MenuBar-label {
+  margin-left: 25px;
 }
 
-.jp-Collapse-header {
-  padding: 1px 12px;
-  background-color: var(--jp-layout-color1);
-  border-bottom: solid var(--jp-border-width) var(--jp-border-color2);
+.jp-MenuBar-anonymousIcon span {
+  width: 24px;
+  text-align: center;
+  fill: var(--jp-ui-font-color1);
   color: var(--jp-ui-font-color1);
-  cursor: pointer;
-  display: flex;
-  align-items: center;
-  font-size: var(--jp-ui-font-size0);
-  font-weight: 600;
-  text-transform: uppercase;
-  user-select: none;
-}
-
-.jp-Collapser-icon {
-  height: 16px;
 }
 
-.jp-Collapse-header-collapsed .jp-Collapser-icon {
-  transform: rotate(-90deg);
-  margin: auto 0;
+.jp-MenuBar-anonymousIcon,
+.jp-MenuBar-imageIcon {
+  position: absolute;
+  top: 1px;
+  left: 8px;
+  width: 24px;
+  height: 24px;
+  display: flex;
+  align-items: center;
+  vertical-align: middle;
+  border-radius: 100%;
 }
 
-.jp-Collapser-title {
-  line-height: 25px;
+.jp-MenuBar-imageIcon img {
+  width: 24px;
+  border-radius: 100%;
+  fill: var(--jp-ui-font-color1);
+  color: var(--jp-ui-font-color1);
 }
 
-.jp-Collapse-contents {
-  padding: 0 12px;
-  background-color: var(--jp-layout-color1);
-  color: var(--jp-ui-font-color1);
-  overflow: auto;
+.jp-UserMenu-caretDownIcon {
+  height: 22px;
+  position: relative;
+  top: 15%;
 }
```

### Comparing `jupyter_collaboration_ui-1.0.0a0/packages/collaboration/src/components.tsx` & `jupyter_collaboration_ui-1.0.0a1/packages/collaboration/src/components.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration_ui-1.0.0a0/packages/collaboration/src/menu.ts` & `jupyter_collaboration_ui-1.0.0a1/packages/collaboration/src/menu.ts`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration_ui-1.0.0a0/packages/collaboration/style/sidepanel.css` & `jupyter_collaboration_ui-1.0.0a1/packages/collaboration/style/sidepanel.css`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/package.json` & `jupyter_collaboration_ui-1.0.0a1/packages/collaboration-extension/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9757575757575757%*

 * *Differences: {"'dependencies'": "{'@jupyter/collaboration': '^3.0.0-alpha.1', '@jupyter/docprovider': "*

 * *                   "'^3.0.0-alpha.1'}",*

 * * "'version'": "'3.0.0-alpha.1'"}*

```diff
@@ -1,15 +1,15 @@
 {
     "author": "Project Jupyter",
     "bugs": {
         "url": "https://github.com/jupyterlab/jupyter-collaboration/issues"
     },
     "dependencies": {
-        "@jupyter/collaboration": "^3.0.0-alpha.0",
-        "@jupyter/docprovider": "^3.0.0-alpha.0",
+        "@jupyter/collaboration": "^3.0.0-alpha.1",
+        "@jupyter/docprovider": "^3.0.0-alpha.1",
         "@jupyter/ydoc": "^1.1.0-a0",
         "@jupyterlab/application": "^4.2.0-beta.0",
         "@jupyterlab/apputils": "^4.2.0-beta.0",
         "@jupyterlab/codemirror": "^4.2.0-beta.0",
         "@jupyterlab/coreutils": "^6.0.5",
         "@jupyterlab/services": "^7.0.5",
         "@jupyterlab/statedb": "^4.2.0-beta.0",
@@ -115,9 +115,9 @@
     "typedoc": {
         "displayName": "@jupyter/collaboration-extension",
         "entryPoint": "./src/index.ts",
         "readmeFile": "./README.md",
         "tsconfig": "./tsconfig.json"
     },
     "types": "lib/index.d.ts",
-    "version": "3.0.0-alpha.0"
+    "version": "3.0.0-alpha.1"
 }
```

### Comparing `jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/lib/collaboration.js` & `jupyter_collaboration_ui-1.0.0a1/packages/collaboration-extension/src/collaboration.ts`

 * *Files 8% similar despite different names*

```diff
@@ -4,351 +4,360 @@
 00000030: 7374 7269 6275 7465 6420 756e 6465 7220  stributed under 
 00000040: 7468 6520 7465 726d 7320 6f66 2074 6865  the terms of the
 00000050: 204d 6f64 6966 6965 6420 4253 4420 4c69   Modified BSD Li
 00000060: 6365 6e73 652e 0a2f 2a2a 0a20 2a20 4070  cense../**. * @p
 00000070: 6163 6b61 6765 446f 6375 6d65 6e74 6174  ackageDocumentat
 00000080: 696f 6e0a 202a 2040 6d6f 6475 6c65 2063  ion. * @module c
 00000090: 6f6c 6c61 626f 7261 7469 6f6e 2d65 7874  ollaboration-ext
-000000a0: 656e 7369 6f6e 0a20 2a2f 0a69 6d70 6f72  ension. */.impor
-000000b0: 7420 7b20 4954 6f6f 6c62 6172 5769 6467  t { IToolbarWidg
-000000c0: 6574 5265 6769 7374 7279 207d 2066 726f  etRegistry } fro
-000000d0: 6d20 2740 6a75 7079 7465 726c 6162 2f61  m '@jupyterlab/a
-000000e0: 7070 7574 696c 7327 3b0a 696d 706f 7274  pputils';.import
-000000f0: 207b 2045 6469 746f 7245 7874 656e 7369   { EditorExtensi
-00000100: 6f6e 5265 6769 7374 7279 2c20 4945 6469  onRegistry, IEdi
-00000110: 746f 7245 7874 656e 7369 6f6e 5265 6769  torExtensionRegi
-00000120: 7374 7279 207d 2066 726f 6d20 2740 6a75  stry } from '@ju
-00000130: 7079 7465 726c 6162 2f63 6f64 656d 6972  pyterlab/codemir
-00000140: 726f 7227 3b0a 696d 706f 7274 207b 2057  ror';.import { W
-00000150: 6562 536f 636b 6574 4177 6172 656e 6573  ebSocketAwarenes
-00000160: 7350 726f 7669 6465 7220 7d20 6672 6f6d  sProvider } from
-00000170: 2027 406a 7570 7974 6572 2f64 6f63 7072   '@jupyter/docpr
-00000180: 6f76 6964 6572 273b 0a69 6d70 6f72 7420  ovider';.import 
-00000190: 7b20 5369 6465 5061 6e65 6c2c 2075 7365  { SidePanel, use
-000001a0: 7273 4963 6f6e 207d 2066 726f 6d20 2740  rsIcon } from '@
-000001b0: 6a75 7079 7465 726c 6162 2f75 692d 636f  jupyterlab/ui-co
-000001c0: 6d70 6f6e 656e 7473 273b 0a69 6d70 6f72  mponents';.impor
-000001d0: 7420 7b20 5552 4c45 7874 207d 2066 726f  t { URLExt } fro
-000001e0: 6d20 2740 6a75 7079 7465 726c 6162 2f63  m '@jupyterlab/c
-000001f0: 6f72 6575 7469 6c73 273b 0a69 6d70 6f72  oreutils';.impor
-00000200: 7420 7b20 5365 7276 6572 436f 6e6e 6563  t { ServerConnec
-00000210: 7469 6f6e 207d 2066 726f 6d20 2740 6a75  tion } from '@ju
-00000220: 7079 7465 726c 6162 2f73 6572 7669 6365  pyterlab/service
-00000230: 7327 3b0a 696d 706f 7274 207b 2049 5374  s';.import { ISt
-00000240: 6174 6544 4220 7d20 6672 6f6d 2027 406a  ateDB } from '@j
-00000250: 7570 7974 6572 6c61 622f 7374 6174 6564  upyterlab/stated
-00000260: 6227 3b0a 696d 706f 7274 207b 2049 5472  b';.import { ITr
-00000270: 616e 736c 6174 6f72 2c20 6e75 6c6c 5472  anslator, nullTr
-00000280: 616e 736c 6174 6f72 207d 2066 726f 6d20  anslator } from 
-00000290: 2740 6a75 7079 7465 726c 6162 2f74 7261  '@jupyterlab/tra
-000002a0: 6e73 6c61 7469 6f6e 273b 0a69 6d70 6f72  nslation';.impor
-000002b0: 7420 7b20 4d65 6e75 4261 7220 7d20 6672  t { MenuBar } fr
-000002c0: 6f6d 2027 406c 756d 696e 6f2f 7769 6467  om '@lumino/widg
-000002d0: 6574 7327 3b0a 696d 706f 7274 207b 2043  ets';.import { C
-000002e0: 6f6c 6c61 626f 7261 746f 7273 5061 6e65  ollaboratorsPane
-000002f0: 6c2c 2049 476c 6f62 616c 4177 6172 656e  l, IGlobalAwaren
-00000300: 6573 732c 2049 5573 6572 4d65 6e75 2c20  ess, IUserMenu, 
-00000310: 7265 6d6f 7465 5573 6572 4375 7273 6f72  remoteUserCursor
-00000320: 732c 2052 656e 6465 7265 7255 7365 724d  s, RendererUserM
-00000330: 656e 752c 2055 7365 7249 6e66 6f50 616e  enu, UserInfoPan
-00000340: 656c 2c20 5573 6572 4d65 6e75 207d 2066  el, UserMenu } f
-00000350: 726f 6d20 2740 6a75 7079 7465 722f 636f  rom '@jupyter/co
-00000360: 6c6c 6162 6f72 6174 696f 6e27 3b0a 696d  llaboration';.im
-00000370: 706f 7274 202a 2061 7320 5920 6672 6f6d  port * as Y from
-00000380: 2027 796a 7327 3b0a 696d 706f 7274 207b   'yjs';.import {
-00000390: 2041 7761 7265 6e65 7373 207d 2066 726f   Awareness } fro
-000003a0: 6d20 2779 2d70 726f 746f 636f 6c73 2f61  m 'y-protocols/a
-000003b0: 7761 7265 6e65 7373 273b 0a2f 2a2a 0a20  wareness';./**. 
-000003c0: 2a20 4a75 7079 7465 7220 706c 7567 696e  * Jupyter plugin
-000003d0: 2070 726f 7669 6469 6e67 2074 6865 2049   providing the I
-000003e0: 5573 6572 4d65 6e75 2e0a 202a 2f0a 6578  UserMenu.. */.ex
-000003f0: 706f 7274 2063 6f6e 7374 2075 7365 724d  port const userM
-00000400: 656e 7550 6c75 6769 6e20 3d20 7b0a 2020  enuPlugin = {.  
-00000410: 2020 6964 3a20 2740 6a75 7079 7465 722f    id: '@jupyter/
-00000420: 636f 6c6c 6162 6f72 6174 696f 6e2d 6578  collaboration-ex
-00000430: 7465 6e73 696f 6e3a 7573 6572 4d65 6e75  tension:userMenu
-00000440: 272c 0a20 2020 2064 6573 6372 6970 7469  ',.    descripti
-00000450: 6f6e 3a20 2750 726f 7669 6465 2063 6f6e  on: 'Provide con
-00000460: 6e65 6374 6564 2075 7365 7220 6d65 6e75  nected user menu
-00000470: 2e27 2c0a 2020 2020 7265 7175 6972 6573  .',.    requires
-00000480: 3a20 5b5d 2c0a 2020 2020 7072 6f76 6964  : [],.    provid
-00000490: 6573 3a20 4955 7365 724d 656e 752c 0a20  es: IUserMenu,. 
-000004a0: 2020 2061 6374 6976 6174 653a 2028 6170     activate: (ap
-000004b0: 7029 203d 3e20 7b0a 2020 2020 2020 2020  p) => {.        
-000004c0: 636f 6e73 7420 7b20 636f 6d6d 616e 6473  const { commands
-000004d0: 207d 203d 2061 7070 3b0a 2020 2020 2020   } = app;.      
-000004e0: 2020 636f 6e73 7420 7b20 7573 6572 207d    const { user }
-000004f0: 203d 2061 7070 2e73 6572 7669 6365 4d61   = app.serviceMa
-00000500: 6e61 6765 723b 0a20 2020 2020 2020 2072  nager;.        r
-00000510: 6574 7572 6e20 6e65 7720 5573 6572 4d65  eturn new UserMe
-00000520: 6e75 287b 2063 6f6d 6d61 6e64 732c 2075  nu({ commands, u
-00000530: 7365 7220 7d29 3b0a 2020 2020 7d0a 7d3b  ser });.    }.};
-00000540: 0a2f 2a2a 0a20 2a20 4a75 7079 7465 7220  ./**. * Jupyter 
-00000550: 706c 7567 696e 2061 6464 696e 6720 7468  plugin adding th
-00000560: 6520 4955 7365 724d 656e 7520 746f 2074  e IUserMenu to t
-00000570: 6865 206d 656e 7520 6261 7220 6966 2063  he menu bar if c
-00000580: 6f6c 6c61 626f 7261 7469 7665 2066 6c61  ollaborative fla
-00000590: 6720 656e 6162 6c65 642e 0a20 2a2f 0a65  g enabled.. */.e
-000005a0: 7870 6f72 7420 636f 6e73 7420 6d65 6e75  xport const menu
-000005b0: 4261 7250 6c75 6769 6e20 3d20 7b0a 2020  BarPlugin = {.  
-000005c0: 2020 6964 3a20 2740 6a75 7079 7465 722f    id: '@jupyter/
-000005d0: 636f 6c6c 6162 6f72 6174 696f 6e2d 6578  collaboration-ex
-000005e0: 7465 6e73 696f 6e3a 7573 6572 2d6d 656e  tension:user-men
-000005f0: 752d 6261 7227 2c0a 2020 2020 6465 7363  u-bar',.    desc
-00000600: 7269 7074 696f 6e3a 2027 4164 6420 7573  ription: 'Add us
-00000610: 6572 206d 656e 7520 746f 2074 6865 2069  er menu to the i
-00000620: 6e74 6572 6661 6365 2e27 2c0a 2020 2020  nterface.',.    
-00000630: 6175 746f 5374 6172 743a 2074 7275 652c  autoStart: true,
-00000640: 0a20 2020 2072 6571 7569 7265 733a 205b  .    requires: [
-00000650: 4955 7365 724d 656e 752c 2049 546f 6f6c  IUserMenu, ITool
-00000660: 6261 7257 6964 6765 7452 6567 6973 7472  barWidgetRegistr
-00000670: 795d 2c0a 2020 2020 6163 7469 7661 7465  y],.    activate
-00000680: 3a20 6173 796e 6320 2861 7070 2c20 6d65  : async (app, me
-00000690: 6e75 2c20 746f 6f6c 6261 7252 6567 6973  nu, toolbarRegis
-000006a0: 7472 7929 203d 3e20 7b0a 2020 2020 2020  try) => {.      
-000006b0: 2020 636f 6e73 7420 7b20 7573 6572 207d    const { user }
-000006c0: 203d 2061 7070 2e73 6572 7669 6365 4d61   = app.serviceMa
-000006d0: 6e61 6765 723b 0a20 2020 2020 2020 2063  nager;.        c
-000006e0: 6f6e 7374 206d 656e 7542 6172 203d 206e  onst menuBar = n
-000006f0: 6577 204d 656e 7542 6172 287b 0a20 2020  ew MenuBar({.   
-00000700: 2020 2020 2020 2020 2066 6f72 6365 4974           forceIt
-00000710: 656d 7350 6f73 6974 696f 6e3a 207b 0a20  emsPosition: {. 
-00000720: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00000730: 6f72 6365 583a 2066 616c 7365 2c0a 2020  orceX: false,.  
-00000740: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-00000750: 7263 6559 3a20 6661 6c73 650a 2020 2020  rceY: false.    
-00000760: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
-00000770: 2020 2020 2020 2072 656e 6465 7265 723a         renderer:
-00000780: 206e 6577 2052 656e 6465 7265 7255 7365   new RendererUse
-00000790: 724d 656e 7528 7573 6572 290a 2020 2020  rMenu(user).    
-000007a0: 2020 2020 7d29 3b0a 2020 2020 2020 2020      });.        
-000007b0: 6d65 6e75 4261 722e 6964 203d 2027 6a70  menuBar.id = 'jp
-000007c0: 2d55 7365 724d 656e 7527 3b0a 2020 2020  -UserMenu';.    
-000007d0: 2020 2020 7573 6572 2e75 7365 7243 6861      user.userCha
-000007e0: 6e67 6564 2e63 6f6e 6e65 6374 2828 2920  nged.connect(() 
-000007f0: 3d3e 206d 656e 7542 6172 2e75 7064 6174  => menuBar.updat
-00000800: 6528 2929 3b0a 2020 2020 2020 2020 6d65  e());.        me
-00000810: 6e75 4261 722e 6164 644d 656e 7528 6d65  nuBar.addMenu(me
-00000820: 6e75 293b 0a20 2020 2020 2020 2074 6f6f  nu);.        too
-00000830: 6c62 6172 5265 6769 7374 7279 2e61 6464  lbarRegistry.add
-00000840: 4661 6374 6f72 7928 2754 6f70 4261 7227  Factory('TopBar'
-00000850: 2c20 2775 7365 722d 6d65 6e75 272c 2028  , 'user-menu', (
-00000860: 2920 3d3e 206d 656e 7542 6172 293b 0a20  ) => menuBar);. 
-00000870: 2020 207d 0a7d 3b0a 2f2a 2a0a 202a 204a     }.};./**. * J
-00000880: 7570 7974 6572 2070 6c75 6769 6e20 6372  upyter plugin cr
-00000890: 6561 7469 6e67 2061 2067 6c6f 6261 6c20  eating a global 
-000008a0: 6177 6172 656e 6573 7320 666f 7220 5254  awareness for RT
-000008b0: 432e 0a20 2a2f 0a65 7870 6f72 7420 636f  C.. */.export co
-000008c0: 6e73 7420 7274 6347 6c6f 6261 6c41 7761  nst rtcGlobalAwa
-000008d0: 7265 6e65 7373 506c 7567 696e 203d 207b  renessPlugin = {
-000008e0: 0a20 2020 2069 643a 2027 406a 7570 7974  .    id: '@jupyt
-000008f0: 6572 2f63 6f6c 6c61 626f 7261 7469 6f6e  er/collaboration
-00000900: 2d65 7874 656e 7369 6f6e 3a72 7463 476c  -extension:rtcGl
-00000910: 6f62 616c 4177 6172 656e 6573 7327 2c0a  obalAwareness',.
-00000920: 2020 2020 6465 7363 7269 7074 696f 6e3a      description:
-00000930: 2027 4164 6420 676c 6f62 616c 2061 7761   'Add global awa
-00000940: 7265 6e65 7373 2074 6f20 7368 6172 6520  reness to share 
-00000950: 776f 726b 696e 6720 646f 6375 6d65 6e74  working document
-00000960: 206f 6620 7573 6572 732e 272c 0a20 2020   of users.',.   
-00000970: 2072 6571 7569 7265 733a 205b 4953 7461   requires: [ISta
-00000980: 7465 4442 5d2c 0a20 2020 2070 726f 7669  teDB],.    provi
-00000990: 6465 733a 2049 476c 6f62 616c 4177 6172  des: IGlobalAwar
-000009a0: 656e 6573 732c 0a20 2020 2061 6374 6976  eness,.    activ
-000009b0: 6174 653a 2028 6170 702c 2073 7461 7465  ate: (app, state
-000009c0: 2920 3d3e 207b 0a20 2020 2020 2020 2063  ) => {.        c
-000009d0: 6f6e 7374 207b 2075 7365 7220 7d20 3d20  onst { user } = 
-000009e0: 6170 702e 7365 7276 6963 654d 616e 6167  app.serviceManag
-000009f0: 6572 3b0a 2020 2020 2020 2020 636f 6e73  er;.        cons
-00000a00: 7420 7964 6f63 203d 206e 6577 2059 2e44  t ydoc = new Y.D
-00000a10: 6f63 2829 3b0a 2020 2020 2020 2020 636f  oc();.        co
-00000a20: 6e73 7420 6177 6172 656e 6573 7320 3d20  nst awareness = 
-00000a30: 6e65 7720 4177 6172 656e 6573 7328 7964  new Awareness(yd
-00000a40: 6f63 293b 0a20 2020 2020 2020 2063 6f6e  oc);.        con
-00000a50: 7374 2073 6572 7665 7220 3d20 5365 7276  st server = Serv
-00000a60: 6572 436f 6e6e 6563 7469 6f6e 2e6d 616b  erConnection.mak
-00000a70: 6553 6574 7469 6e67 7328 293b 0a20 2020  eSettings();.   
-00000a80: 2020 2020 2063 6f6e 7374 2075 726c 203d       const url =
-00000a90: 2055 524c 4578 742e 6a6f 696e 2873 6572   URLExt.join(ser
-00000aa0: 7665 722e 7773 5572 6c2c 2027 6170 692f  ver.wsUrl, 'api/
-00000ab0: 636f 6c6c 6162 6f72 6174 696f 6e2f 726f  collaboration/ro
-00000ac0: 6f6d 2729 3b0a 2020 2020 2020 2020 6e65  om');.        ne
-00000ad0: 7720 5765 6253 6f63 6b65 7441 7761 7265  w WebSocketAware
-00000ae0: 6e65 7373 5072 6f76 6964 6572 287b 0a20  nessProvider({. 
-00000af0: 2020 2020 2020 2020 2020 2075 726c 3a20             url: 
-00000b00: 7572 6c2c 0a20 2020 2020 2020 2020 2020  url,.           
-00000b10: 2072 6f6f 6d49 443a 2027 4a75 7079 7465   roomID: 'Jupyte
-00000b20: 724c 6162 3a67 6c6f 6261 6c41 7761 7265  rLab:globalAware
-00000b30: 6e65 7373 272c 0a20 2020 2020 2020 2020  ness',.         
-00000b40: 2020 2061 7761 7265 6e65 7373 3a20 6177     awareness: aw
-00000b50: 6172 656e 6573 732c 0a20 2020 2020 2020  areness,.       
-00000b60: 2020 2020 2075 7365 723a 2075 7365 720a       user: user.
-00000b70: 2020 2020 2020 2020 7d29 3b0a 2020 2020          });.    
-00000b80: 2020 2020 7374 6174 652e 6368 616e 6765      state.change
-00000b90: 642e 636f 6e6e 6563 7428 6173 796e 6320  d.connect(async 
-00000ba0: 2829 203d 3e20 7b0a 2020 2020 2020 2020  () => {.        
-00000bb0: 2020 2020 7661 7220 5f61 2c20 5f62 3b0a      var _a, _b;.
-00000bc0: 2020 2020 2020 2020 2020 2020 636f 6e73              cons
-00000bd0: 7420 6461 7461 203d 2061 7761 6974 2073  t data = await s
-00000be0: 7461 7465 2e74 6f4a 534f 4e28 293b 0a20  tate.toJSON();. 
-00000bf0: 2020 2020 2020 2020 2020 2063 6f6e 7374             const
-00000c00: 2063 7572 7265 6e74 203d 2028 285f 6220   current = ((_b 
-00000c10: 3d20 285f 6120 3d20 6461 7461 5b27 6c61  = (_a = data['la
-00000c20: 796f 7574 2d72 6573 746f 7265 723a 6461  yout-restorer:da
-00000c30: 7461 275d 2920 3d3d 3d20 6e75 6c6c 207c  ta']) === null |
-00000c40: 7c20 5f61 203d 3d3d 2076 6f69 6420 3020  | _a === void 0 
-00000c50: 3f20 766f 6964 2030 203a 205f 612e 6d61  ? void 0 : _a.ma
-00000c60: 696e 2920 3d3d 3d20 6e75 6c6c 207c 7c20  in) === null || 
-00000c70: 5f62 203d 3d3d 2076 6f69 6420 3020 3f20  _b === void 0 ? 
-00000c80: 766f 6964 2030 203a 205f 622e 6375 7272  void 0 : _b.curr
-00000c90: 656e 7429 207c 7c20 2727 3b0a 2020 2020  ent) || '';.    
-00000ca0: 2020 2020 2020 2020 6966 2028 6375 7272          if (curr
-00000cb0: 656e 742e 7374 6172 7473 5769 7468 2827  ent.startsWith('
-00000cc0: 6564 6974 6f72 2729 207c 7c20 6375 7272  editor') || curr
-00000cd0: 656e 742e 7374 6172 7473 5769 7468 2827  ent.startsWith('
-00000ce0: 6e6f 7465 626f 6f6b 2729 2920 7b0a 2020  notebook')) {.  
-00000cf0: 2020 2020 2020 2020 2020 2020 2020 6177                aw
-00000d00: 6172 656e 6573 732e 7365 744c 6f63 616c  areness.setLocal
-00000d10: 5374 6174 6546 6965 6c64 2827 6375 7272  StateField('curr
-00000d20: 656e 7427 2c20 6375 7272 656e 7429 3b0a  ent', current);.
-00000d30: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
-00000d40: 2020 2020 2020 2020 2020 656c 7365 207b            else {
-00000d50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000d60: 2061 7761 7265 6e65 7373 2e73 6574 4c6f   awareness.setLo
-00000d70: 6361 6c53 7461 7465 4669 656c 6428 2763  calStateField('c
-00000d80: 7572 7265 6e74 272c 206e 756c 6c29 3b0a  urrent', null);.
-00000d90: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
-00000da0: 2020 2020 2020 7d29 3b0a 2020 2020 2020        });.      
-00000db0: 2020 7265 7475 726e 2061 7761 7265 6e65    return awarene
-00000dc0: 7373 3b0a 2020 2020 7d0a 7d3b 0a2f 2a2a  ss;.    }.};./**
-00000dd0: 0a20 2a20 4a75 7079 7465 7220 706c 7567  . * Jupyter plug
-00000de0: 696e 2061 6464 696e 6720 7468 6520 5254  in adding the RT
-00000df0: 4320 696e 666f 726d 6174 696f 6e20 746f  C information to
-00000e00: 2074 6865 2061 7070 6c69 6361 7469 6f6e   the application
-00000e10: 206c 6566 7420 7061 6e65 6c20 6966 2063   left panel if c
-00000e20: 6f6c 6c61 626f 7261 7469 7665 2066 6c61  ollaborative fla
-00000e30: 6720 656e 6162 6c65 642e 0a20 2a2f 0a65  g enabled.. */.e
-00000e40: 7870 6f72 7420 636f 6e73 7420 7274 6350  xport const rtcP
-00000e50: 616e 656c 506c 7567 696e 203d 207b 0a20  anelPlugin = {. 
-00000e60: 2020 2069 643a 2027 406a 7570 7974 6572     id: '@jupyter
-00000e70: 2f63 6f6c 6c61 626f 7261 7469 6f6e 2d65  /collaboration-e
-00000e80: 7874 656e 7369 6f6e 3a72 7463 5061 6e65  xtension:rtcPane
-00000e90: 6c27 2c0a 2020 2020 6465 7363 7269 7074  l',.    descript
-00000ea0: 696f 6e3a 2027 4164 6420 7369 6465 2070  ion: 'Add side p
-00000eb0: 616e 656c 2074 6f20 6469 7370 6c61 7920  anel to display 
-00000ec0: 616c 6c20 6375 7272 656e 746c 7920 636f  all currently co
-00000ed0: 6e6e 6563 7465 6420 7573 6572 732e 272c  nnected users.',
-00000ee0: 0a20 2020 2061 7574 6f53 7461 7274 3a20  .    autoStart: 
-00000ef0: 7472 7565 2c0a 2020 2020 7265 7175 6972  true,.    requir
-00000f00: 6573 3a20 5b49 476c 6f62 616c 4177 6172  es: [IGlobalAwar
-00000f10: 656e 6573 735d 2c0a 2020 2020 6f70 7469  eness],.    opti
-00000f20: 6f6e 616c 3a20 5b49 5472 616e 736c 6174  onal: [ITranslat
-00000f30: 6f72 5d2c 0a20 2020 2061 6374 6976 6174  or],.    activat
-00000f40: 653a 2028 6170 702c 2061 7761 7265 6e65  e: (app, awarene
-00000f50: 7373 2c20 7472 616e 736c 6174 6f72 2920  ss, translator) 
-00000f60: 3d3e 207b 0a20 2020 2020 2020 2063 6f6e  => {.        con
-00000f70: 7374 207b 2075 7365 7220 7d20 3d20 6170  st { user } = ap
-00000f80: 702e 7365 7276 6963 654d 616e 6167 6572  p.serviceManager
-00000f90: 3b0a 2020 2020 2020 2020 636f 6e73 7420  ;.        const 
-00000fa0: 7472 616e 7320 3d20 2874 7261 6e73 6c61  trans = (transla
-00000fb0: 746f 7220 213d 3d20 6e75 6c6c 2026 2620  tor !== null && 
-00000fc0: 7472 616e 736c 6174 6f72 2021 3d3d 2076  translator !== v
-00000fd0: 6f69 6420 3020 3f20 7472 616e 736c 6174  oid 0 ? translat
-00000fe0: 6f72 203a 206e 756c 6c54 7261 6e73 6c61  or : nullTransla
-00000ff0: 746f 7229 2e6c 6f61 6428 276a 7570 7974  tor).load('jupyt
-00001000: 6572 5f63 6f6c 6c61 626f 7261 7469 6f6e  er_collaboration
-00001010: 2729 3b0a 2020 2020 2020 2020 636f 6e73  ');.        cons
-00001020: 7420 7573 6572 5061 6e65 6c20 3d20 6e65  t userPanel = ne
-00001030: 7720 5369 6465 5061 6e65 6c28 7b0a 2020  w SidePanel({.  
-00001040: 2020 2020 2020 2020 2020 616c 6967 6e6d            alignm
-00001050: 656e 743a 2027 6a75 7374 6966 7927 0a20  ent: 'justify'. 
-00001060: 2020 2020 2020 207d 293b 0a20 2020 2020         });.     
-00001070: 2020 2075 7365 7250 616e 656c 2e69 6420     userPanel.id 
-00001080: 3d20 276a 702d 636f 6c6c 6162 6f72 6174  = 'jp-collaborat
-00001090: 696f 6e2d 7061 6e65 6c27 3b0a 2020 2020  ion-panel';.    
-000010a0: 2020 2020 7573 6572 5061 6e65 6c2e 7469      userPanel.ti
-000010b0: 746c 652e 6963 6f6e 203d 2075 7365 7273  tle.icon = users
-000010c0: 4963 6f6e 3b0a 2020 2020 2020 2020 7573  Icon;.        us
-000010d0: 6572 5061 6e65 6c2e 7469 746c 652e 6361  erPanel.title.ca
-000010e0: 7074 696f 6e20 3d20 7472 616e 732e 5f5f  ption = trans.__
-000010f0: 2827 436f 6c6c 6162 6f72 6174 696f 6e27  ('Collaboration'
-00001100: 293b 0a20 2020 2020 2020 2075 7365 7250  );.        userP
-00001110: 616e 656c 2e61 6464 436c 6173 7328 276a  anel.addClass('j
-00001120: 702d 5254 4350 616e 656c 2729 3b0a 2020  p-RTCPanel');.  
-00001130: 2020 2020 2020 6170 702e 7368 656c 6c2e        app.shell.
-00001140: 6164 6428 7573 6572 5061 6e65 6c2c 2027  add(userPanel, '
-00001150: 6c65 6674 272c 207b 2072 616e 6b3a 2033  left', { rank: 3
-00001160: 3030 207d 293b 0a20 2020 2020 2020 2063  00 });.        c
-00001170: 6f6e 7374 2063 7572 7265 6e74 5573 6572  onst currentUser
-00001180: 5061 6e65 6c20 3d20 6e65 7720 5573 6572  Panel = new User
-00001190: 496e 666f 5061 6e65 6c28 7573 6572 293b  InfoPanel(user);
-000011a0: 0a20 2020 2020 2020 2063 7572 7265 6e74  .        current
-000011b0: 5573 6572 5061 6e65 6c2e 7469 746c 652e  UserPanel.title.
-000011c0: 6c61 6265 6c20 3d20 7472 616e 732e 5f5f  label = trans.__
-000011d0: 2827 5573 6572 2069 6e66 6f27 293b 0a20  ('User info');. 
-000011e0: 2020 2020 2020 2063 7572 7265 6e74 5573         currentUs
-000011f0: 6572 5061 6e65 6c2e 7469 746c 652e 6361  erPanel.title.ca
-00001200: 7074 696f 6e20 3d20 7472 616e 732e 5f5f  ption = trans.__
-00001210: 2827 5573 6572 2069 6e66 6f72 6d61 7469  ('User informati
-00001220: 6f6e 2729 3b0a 2020 2020 2020 2020 7573  on');.        us
-00001230: 6572 5061 6e65 6c2e 6164 6457 6964 6765  erPanel.addWidge
-00001240: 7428 6375 7272 656e 7455 7365 7250 616e  t(currentUserPan
-00001250: 656c 293b 0a20 2020 2020 2020 2063 6f6e  el);.        con
-00001260: 7374 2066 696c 656f 7065 6e65 7220 3d20  st fileopener = 
-00001270: 2870 6174 6829 203d 3e20 7b0a 2020 2020  (path) => {.    
-00001280: 2020 2020 2020 2020 766f 6964 2061 7070          void app
-00001290: 2e63 6f6d 6d61 6e64 732e 6578 6563 7574  .commands.execut
-000012a0: 6528 2764 6f63 6d61 6e61 6765 723a 6f70  e('docmanager:op
-000012b0: 656e 272c 207b 2070 6174 6820 7d29 3b0a  en', { path });.
-000012c0: 2020 2020 2020 2020 7d3b 0a20 2020 2020          };.     
-000012d0: 2020 2063 6f6e 7374 2063 6f6c 6c61 626f     const collabo
-000012e0: 7261 746f 7273 5061 6e65 6c20 3d20 6e65  ratorsPanel = ne
-000012f0: 7720 436f 6c6c 6162 6f72 6174 6f72 7350  w CollaboratorsP
-00001300: 616e 656c 2875 7365 722c 2061 7761 7265  anel(user, aware
-00001310: 6e65 7373 2c20 6669 6c65 6f70 656e 6572  ness, fileopener
-00001320: 293b 0a20 2020 2020 2020 2063 6f6c 6c61  );.        colla
-00001330: 626f 7261 746f 7273 5061 6e65 6c2e 7469  boratorsPanel.ti
-00001340: 746c 652e 6c61 6265 6c20 3d20 7472 616e  tle.label = tran
-00001350: 732e 5f5f 2827 4f6e 6c69 6e65 2043 6f6c  s.__('Online Col
-00001360: 6c61 626f 7261 746f 7273 2729 3b0a 2020  laborators');.  
-00001370: 2020 2020 2020 7573 6572 5061 6e65 6c2e        userPanel.
-00001380: 6164 6457 6964 6765 7428 636f 6c6c 6162  addWidget(collab
-00001390: 6f72 6174 6f72 7350 616e 656c 293b 0a20  oratorsPanel);. 
-000013a0: 2020 207d 0a7d 3b0a 6578 706f 7274 2063     }.};.export c
-000013b0: 6f6e 7374 2075 7365 7245 6469 746f 7243  onst userEditorC
-000013c0: 7572 736f 7273 203d 207b 0a20 2020 2069  ursors = {.    i
-000013d0: 643a 2027 406a 7570 7974 6572 2f63 6f6c  d: '@jupyter/col
-000013e0: 6c61 626f 7261 7469 6f6e 2d65 7874 656e  laboration-exten
-000013f0: 7369 6f6e 3a75 7365 7245 6469 746f 7243  sion:userEditorC
-00001400: 7572 736f 7273 272c 0a20 2020 2064 6573  ursors',.    des
-00001410: 6372 6970 7469 6f6e 3a20 2741 6464 2043  cription: 'Add C
-00001420: 6f64 654d 6972 726f 7220 6578 7465 6e73  odeMirror extens
-00001430: 696f 6e20 746f 2064 6973 706c 6179 2072  ion to display r
-00001440: 656d 6f74 6520 7573 6572 2063 7572 736f  emote user curso
-00001450: 7273 2061 6e64 2073 656c 6563 7469 6f6e  rs and selection
-00001460: 732e 272c 0a20 2020 2061 7574 6f53 7461  s.',.    autoSta
-00001470: 7274 3a20 7472 7565 2c0a 2020 2020 7265  rt: true,.    re
-00001480: 7175 6972 6573 3a20 5b49 4564 6974 6f72  quires: [IEditor
-00001490: 4578 7465 6e73 696f 6e52 6567 6973 7472  ExtensionRegistr
-000014a0: 795d 2c0a 2020 2020 6163 7469 7661 7465  y],.    activate
-000014b0: 3a20 2861 7070 2c20 6578 7465 6e73 696f  : (app, extensio
-000014c0: 6e73 2920 3d3e 207b 0a20 2020 2020 2020  ns) => {.       
-000014d0: 2065 7874 656e 7369 6f6e 732e 6164 6445   extensions.addE
-000014e0: 7874 656e 7369 6f6e 287b 0a20 2020 2020  xtension({.     
-000014f0: 2020 2020 2020 206e 616d 653a 2027 7265         name: 're
-00001500: 6d6f 7465 2d75 7365 722d 6375 7273 6f72  mote-user-cursor
-00001510: 7327 2c0a 2020 2020 2020 2020 2020 2020  s',.            
-00001520: 6661 6374 6f72 7928 6f70 7469 6f6e 7329  factory(options)
-00001530: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-00001540: 2020 2063 6f6e 7374 207b 2061 7761 7265     const { aware
-00001550: 6e65 7373 2c20 7973 6f75 7263 653a 2079  ness, ysource: y
-00001560: 7465 7874 207d 203d 206f 7074 696f 6e73  text } = options
-00001570: 2e6d 6f64 656c 2e73 6861 7265 644d 6f64  .model.sharedMod
-00001580: 656c 3b0a 2020 2020 2020 2020 2020 2020  el;.            
-00001590: 2020 2020 7265 7475 726e 2045 6469 746f      return Edito
-000015a0: 7245 7874 656e 7369 6f6e 5265 6769 7374  rExtensionRegist
-000015b0: 7279 2e63 7265 6174 6549 6d6d 7574 6162  ry.createImmutab
-000015c0: 6c65 4578 7465 6e73 696f 6e28 7265 6d6f  leExtension(remo
-000015d0: 7465 5573 6572 4375 7273 6f72 7328 7b20  teUserCursors({ 
-000015e0: 6177 6172 656e 6573 732c 2079 7465 7874  awareness, ytext
-000015f0: 207d 2929 3b0a 2020 2020 2020 2020 2020   }));.          
-00001600: 2020 7d0a 2020 2020 2020 2020 7d29 3b0a    }.        });.
-00001610: 2020 2020 7d0a 7d3b 0a                       }.};.
+000000a0: 656e 7369 6f6e 0a20 2a2f 0a0a 696d 706f  ension. */..impo
+000000b0: 7274 207b 0a20 204a 7570 7974 6572 4672  rt {.  JupyterFr
+000000c0: 6f6e 7445 6e64 2c0a 2020 4a75 7079 7465  ontEnd,.  Jupyte
+000000d0: 7246 726f 6e74 456e 6450 6c75 6769 6e0a  rFrontEndPlugin.
+000000e0: 7d20 6672 6f6d 2027 406a 7570 7974 6572  } from '@jupyter
+000000f0: 6c61 622f 6170 706c 6963 6174 696f 6e27  lab/application'
+00000100: 3b0a 696d 706f 7274 207b 2049 546f 6f6c  ;.import { ITool
+00000110: 6261 7257 6964 6765 7452 6567 6973 7472  barWidgetRegistr
+00000120: 7920 7d20 6672 6f6d 2027 406a 7570 7974  y } from '@jupyt
+00000130: 6572 6c61 622f 6170 7075 7469 6c73 273b  erlab/apputils';
+00000140: 0a69 6d70 6f72 7420 7b0a 2020 4564 6974  .import {.  Edit
+00000150: 6f72 4578 7465 6e73 696f 6e52 6567 6973  orExtensionRegis
+00000160: 7472 792c 0a20 2049 4564 6974 6f72 4578  try,.  IEditorEx
+00000170: 7465 6e73 696f 6e52 6567 6973 7472 790a  tensionRegistry.
+00000180: 7d20 6672 6f6d 2027 406a 7570 7974 6572  } from '@jupyter
+00000190: 6c61 622f 636f 6465 6d69 7272 6f72 273b  lab/codemirror';
+000001a0: 0a69 6d70 6f72 7420 7b20 5765 6253 6f63  .import { WebSoc
+000001b0: 6b65 7441 7761 7265 6e65 7373 5072 6f76  ketAwarenessProv
+000001c0: 6964 6572 207d 2066 726f 6d20 2740 6a75  ider } from '@ju
+000001d0: 7079 7465 722f 646f 6370 726f 7669 6465  pyter/docprovide
+000001e0: 7227 3b0a 696d 706f 7274 207b 2053 6964  r';.import { Sid
+000001f0: 6550 616e 656c 2c20 7573 6572 7349 636f  ePanel, usersIco
+00000200: 6e20 7d20 6672 6f6d 2027 406a 7570 7974  n } from '@jupyt
+00000210: 6572 6c61 622f 7569 2d63 6f6d 706f 6e65  erlab/ui-compone
+00000220: 6e74 7327 3b0a 696d 706f 7274 207b 2055  nts';.import { U
+00000230: 524c 4578 7420 7d20 6672 6f6d 2027 406a  RLExt } from '@j
+00000240: 7570 7974 6572 6c61 622f 636f 7265 7574  upyterlab/coreut
+00000250: 696c 7327 3b0a 696d 706f 7274 207b 2053  ils';.import { S
+00000260: 6572 7665 7243 6f6e 6e65 6374 696f 6e20  erverConnection 
+00000270: 7d20 6672 6f6d 2027 406a 7570 7974 6572  } from '@jupyter
+00000280: 6c61 622f 7365 7276 6963 6573 273b 0a69  lab/services';.i
+00000290: 6d70 6f72 7420 7b20 4953 7461 7465 4442  mport { IStateDB
+000002a0: 2c20 5374 6174 6544 4220 7d20 6672 6f6d  , StateDB } from
+000002b0: 2027 406a 7570 7974 6572 6c61 622f 7374   '@jupyterlab/st
+000002c0: 6174 6564 6227 3b0a 696d 706f 7274 207b  atedb';.import {
+000002d0: 2049 5472 616e 736c 6174 6f72 2c20 6e75   ITranslator, nu
+000002e0: 6c6c 5472 616e 736c 6174 6f72 207d 2066  llTranslator } f
+000002f0: 726f 6d20 2740 6a75 7079 7465 726c 6162  rom '@jupyterlab
+00000300: 2f74 7261 6e73 6c61 7469 6f6e 273b 0a0a  /translation';..
+00000310: 696d 706f 7274 207b 204d 656e 752c 204d  import { Menu, M
+00000320: 656e 7542 6172 207d 2066 726f 6d20 2740  enuBar } from '@
+00000330: 6c75 6d69 6e6f 2f77 6964 6765 7473 273b  lumino/widgets';
+00000340: 0a0a 696d 706f 7274 207b 2049 4177 6172  ..import { IAwar
+00000350: 656e 6573 7320 7d20 6672 6f6d 2027 406a  eness } from '@j
+00000360: 7570 7974 6572 2f79 646f 6327 3b0a 0a69  upyter/ydoc';..i
+00000370: 6d70 6f72 7420 7b0a 2020 436f 6c6c 6162  mport {.  Collab
+00000380: 6f72 6174 6f72 7350 616e 656c 2c0a 2020  oratorsPanel,.  
+00000390: 4947 6c6f 6261 6c41 7761 7265 6e65 7373  IGlobalAwareness
+000003a0: 2c0a 2020 4955 7365 724d 656e 752c 0a20  ,.  IUserMenu,. 
+000003b0: 2072 656d 6f74 6555 7365 7243 7572 736f   remoteUserCurso
+000003c0: 7273 2c0a 2020 5265 6e64 6572 6572 5573  rs,.  RendererUs
+000003d0: 6572 4d65 6e75 2c0a 2020 5573 6572 496e  erMenu,.  UserIn
+000003e0: 666f 5061 6e65 6c2c 0a20 2055 7365 724d  foPanel,.  UserM
+000003f0: 656e 750a 7d20 6672 6f6d 2027 406a 7570  enu.} from '@jup
+00000400: 7974 6572 2f63 6f6c 6c61 626f 7261 7469  yter/collaborati
+00000410: 6f6e 273b 0a0a 696d 706f 7274 202a 2061  on';..import * a
+00000420: 7320 5920 6672 6f6d 2027 796a 7327 3b0a  s Y from 'yjs';.
+00000430: 696d 706f 7274 207b 2041 7761 7265 6e65  import { Awarene
+00000440: 7373 207d 2066 726f 6d20 2779 2d70 726f  ss } from 'y-pro
+00000450: 746f 636f 6c73 2f61 7761 7265 6e65 7373  tocols/awareness
+00000460: 273b 0a0a 2f2a 2a0a 202a 204a 7570 7974  ';../**. * Jupyt
+00000470: 6572 2070 6c75 6769 6e20 7072 6f76 6964  er plugin provid
+00000480: 696e 6720 7468 6520 4955 7365 724d 656e  ing the IUserMen
+00000490: 752e 0a20 2a2f 0a65 7870 6f72 7420 636f  u.. */.export co
+000004a0: 6e73 7420 7573 6572 4d65 6e75 506c 7567  nst userMenuPlug
+000004b0: 696e 3a20 4a75 7079 7465 7246 726f 6e74  in: JupyterFront
+000004c0: 456e 6450 6c75 6769 6e3c 4955 7365 724d  EndPlugin<IUserM
+000004d0: 656e 753e 203d 207b 0a20 2069 643a 2027  enu> = {.  id: '
+000004e0: 406a 7570 7974 6572 2f63 6f6c 6c61 626f  @jupyter/collabo
+000004f0: 7261 7469 6f6e 2d65 7874 656e 7369 6f6e  ration-extension
+00000500: 3a75 7365 724d 656e 7527 2c0a 2020 6465  :userMenu',.  de
+00000510: 7363 7269 7074 696f 6e3a 2027 5072 6f76  scription: 'Prov
+00000520: 6964 6520 636f 6e6e 6563 7465 6420 7573  ide connected us
+00000530: 6572 206d 656e 752e 272c 0a20 2072 6571  er menu.',.  req
+00000540: 7569 7265 733a 205b 5d2c 0a20 2070 726f  uires: [],.  pro
+00000550: 7669 6465 733a 2049 5573 6572 4d65 6e75  vides: IUserMenu
+00000560: 2c0a 2020 6163 7469 7661 7465 3a20 2861  ,.  activate: (a
+00000570: 7070 3a20 4a75 7079 7465 7246 726f 6e74  pp: JupyterFront
+00000580: 456e 6429 3a20 4955 7365 724d 656e 7520  End): IUserMenu 
+00000590: 3d3e 207b 0a20 2020 2063 6f6e 7374 207b  => {.    const {
+000005a0: 2063 6f6d 6d61 6e64 7320 7d20 3d20 6170   commands } = ap
+000005b0: 703b 0a20 2020 2063 6f6e 7374 207b 2075  p;.    const { u
+000005c0: 7365 7220 7d20 3d20 6170 702e 7365 7276  ser } = app.serv
+000005d0: 6963 654d 616e 6167 6572 3b0a 2020 2020  iceManager;.    
+000005e0: 7265 7475 726e 206e 6577 2055 7365 724d  return new UserM
+000005f0: 656e 7528 7b20 636f 6d6d 616e 6473 2c20  enu({ commands, 
+00000600: 7573 6572 207d 293b 0a20 207d 0a7d 3b0a  user });.  }.};.
+00000610: 0a2f 2a2a 0a20 2a20 4a75 7079 7465 7220  ./**. * Jupyter 
+00000620: 706c 7567 696e 2061 6464 696e 6720 7468  plugin adding th
+00000630: 6520 4955 7365 724d 656e 7520 746f 2074  e IUserMenu to t
+00000640: 6865 206d 656e 7520 6261 7220 6966 2063  he menu bar if c
+00000650: 6f6c 6c61 626f 7261 7469 7665 2066 6c61  ollaborative fla
+00000660: 6720 656e 6162 6c65 642e 0a20 2a2f 0a65  g enabled.. */.e
+00000670: 7870 6f72 7420 636f 6e73 7420 6d65 6e75  xport const menu
+00000680: 4261 7250 6c75 6769 6e3a 204a 7570 7974  BarPlugin: Jupyt
+00000690: 6572 4672 6f6e 7445 6e64 506c 7567 696e  erFrontEndPlugin
+000006a0: 3c76 6f69 643e 203d 207b 0a20 2069 643a  <void> = {.  id:
+000006b0: 2027 406a 7570 7974 6572 2f63 6f6c 6c61   '@jupyter/colla
+000006c0: 626f 7261 7469 6f6e 2d65 7874 656e 7369  boration-extensi
+000006d0: 6f6e 3a75 7365 722d 6d65 6e75 2d62 6172  on:user-menu-bar
+000006e0: 272c 0a20 2064 6573 6372 6970 7469 6f6e  ',.  description
+000006f0: 3a20 2741 6464 2075 7365 7220 6d65 6e75  : 'Add user menu
+00000700: 2074 6f20 7468 6520 696e 7465 7266 6163   to the interfac
+00000710: 652e 272c 0a20 2061 7574 6f53 7461 7274  e.',.  autoStart
+00000720: 3a20 7472 7565 2c0a 2020 7265 7175 6972  : true,.  requir
+00000730: 6573 3a20 5b49 5573 6572 4d65 6e75 2c20  es: [IUserMenu, 
+00000740: 4954 6f6f 6c62 6172 5769 6467 6574 5265  IToolbarWidgetRe
+00000750: 6769 7374 7279 5d2c 0a20 2061 6374 6976  gistry],.  activ
+00000760: 6174 653a 2061 7379 6e63 2028 0a20 2020  ate: async (.   
+00000770: 2061 7070 3a20 4a75 7079 7465 7246 726f   app: JupyterFro
+00000780: 6e74 456e 642c 0a20 2020 206d 656e 753a  ntEnd,.    menu:
+00000790: 2049 5573 6572 4d65 6e75 2c0a 2020 2020   IUserMenu,.    
+000007a0: 746f 6f6c 6261 7252 6567 6973 7472 793a  toolbarRegistry:
+000007b0: 2049 546f 6f6c 6261 7257 6964 6765 7452   IToolbarWidgetR
+000007c0: 6567 6973 7472 790a 2020 293a 2050 726f  egistry.  ): Pro
+000007d0: 6d69 7365 3c76 6f69 643e 203d 3e20 7b0a  mise<void> => {.
+000007e0: 2020 2020 636f 6e73 7420 7b20 7573 6572      const { user
+000007f0: 207d 203d 2061 7070 2e73 6572 7669 6365   } = app.service
+00000800: 4d61 6e61 6765 723b 0a0a 2020 2020 636f  Manager;..    co
+00000810: 6e73 7420 6d65 6e75 4261 7220 3d20 6e65  nst menuBar = ne
+00000820: 7720 4d65 6e75 4261 7228 7b0a 2020 2020  w MenuBar({.    
+00000830: 2020 666f 7263 6549 7465 6d73 506f 7369    forceItemsPosi
+00000840: 7469 6f6e 3a20 7b0a 2020 2020 2020 2020  tion: {.        
+00000850: 666f 7263 6558 3a20 6661 6c73 652c 0a20  forceX: false,. 
+00000860: 2020 2020 2020 2066 6f72 6365 593a 2066         forceY: f
+00000870: 616c 7365 0a20 2020 2020 207d 2c0a 2020  alse.      },.  
+00000880: 2020 2020 7265 6e64 6572 6572 3a20 6e65      renderer: ne
+00000890: 7720 5265 6e64 6572 6572 5573 6572 4d65  w RendererUserMe
+000008a0: 6e75 2875 7365 7229 0a20 2020 207d 293b  nu(user).    });
+000008b0: 0a20 2020 206d 656e 7542 6172 2e69 6420  .    menuBar.id 
+000008c0: 3d20 276a 702d 5573 6572 4d65 6e75 273b  = 'jp-UserMenu';
+000008d0: 0a20 2020 2075 7365 722e 7573 6572 4368  .    user.userCh
+000008e0: 616e 6765 642e 636f 6e6e 6563 7428 2829  anged.connect(()
+000008f0: 203d 3e20 6d65 6e75 4261 722e 7570 6461   => menuBar.upda
+00000900: 7465 2829 293b 0a20 2020 206d 656e 7542  te());.    menuB
+00000910: 6172 2e61 6464 4d65 6e75 286d 656e 7520  ar.addMenu(menu 
+00000920: 6173 204d 656e 7529 3b0a 0a20 2020 2074  as Menu);..    t
+00000930: 6f6f 6c62 6172 5265 6769 7374 7279 2e61  oolbarRegistry.a
+00000940: 6464 4661 6374 6f72 7928 2754 6f70 4261  ddFactory('TopBa
+00000950: 7227 2c20 2775 7365 722d 6d65 6e75 272c  r', 'user-menu',
+00000960: 2028 2920 3d3e 206d 656e 7542 6172 293b   () => menuBar);
+00000970: 0a20 207d 0a7d 3b0a 0a2f 2a2a 0a20 2a20  .  }.};../**. * 
+00000980: 4a75 7079 7465 7220 706c 7567 696e 2063  Jupyter plugin c
+00000990: 7265 6174 696e 6720 6120 676c 6f62 616c  reating a global
+000009a0: 2061 7761 7265 6e65 7373 2066 6f72 2052   awareness for R
+000009b0: 5443 2e0a 202a 2f0a 6578 706f 7274 2063  TC.. */.export c
+000009c0: 6f6e 7374 2072 7463 476c 6f62 616c 4177  onst rtcGlobalAw
+000009d0: 6172 656e 6573 7350 6c75 6769 6e3a 204a  arenessPlugin: J
+000009e0: 7570 7974 6572 4672 6f6e 7445 6e64 506c  upyterFrontEndPl
+000009f0: 7567 696e 3c49 4177 6172 656e 6573 733e  ugin<IAwareness>
+00000a00: 203d 207b 0a20 2069 643a 2027 406a 7570   = {.  id: '@jup
+00000a10: 7974 6572 2f63 6f6c 6c61 626f 7261 7469  yter/collaborati
+00000a20: 6f6e 2d65 7874 656e 7369 6f6e 3a72 7463  on-extension:rtc
+00000a30: 476c 6f62 616c 4177 6172 656e 6573 7327  GlobalAwareness'
+00000a40: 2c0a 2020 6465 7363 7269 7074 696f 6e3a  ,.  description:
+00000a50: 2027 4164 6420 676c 6f62 616c 2061 7761   'Add global awa
+00000a60: 7265 6e65 7373 2074 6f20 7368 6172 6520  reness to share 
+00000a70: 776f 726b 696e 6720 646f 6375 6d65 6e74  working document
+00000a80: 206f 6620 7573 6572 732e 272c 0a20 2072   of users.',.  r
+00000a90: 6571 7569 7265 733a 205b 4953 7461 7465  equires: [IState
+00000aa0: 4442 5d2c 0a20 2070 726f 7669 6465 733a  DB],.  provides:
+00000ab0: 2049 476c 6f62 616c 4177 6172 656e 6573   IGlobalAwarenes
+00000ac0: 732c 0a20 2061 6374 6976 6174 653a 2028  s,.  activate: (
+00000ad0: 6170 703a 204a 7570 7974 6572 4672 6f6e  app: JupyterFron
+00000ae0: 7445 6e64 2c20 7374 6174 653a 2053 7461  tEnd, state: Sta
+00000af0: 7465 4442 293a 2049 4177 6172 656e 6573  teDB): IAwarenes
+00000b00: 7320 3d3e 207b 0a20 2020 2063 6f6e 7374  s => {.    const
+00000b10: 207b 2075 7365 7220 7d20 3d20 6170 702e   { user } = app.
+00000b20: 7365 7276 6963 654d 616e 6167 6572 3b0a  serviceManager;.
+00000b30: 0a20 2020 2063 6f6e 7374 2079 646f 6320  .    const ydoc 
+00000b40: 3d20 6e65 7720 592e 446f 6328 293b 0a20  = new Y.Doc();. 
+00000b50: 2020 2063 6f6e 7374 2061 7761 7265 6e65     const awarene
+00000b60: 7373 203d 206e 6577 2041 7761 7265 6e65  ss = new Awarene
+00000b70: 7373 2879 646f 6329 3b0a 0a20 2020 2063  ss(ydoc);..    c
+00000b80: 6f6e 7374 2073 6572 7665 7220 3d20 5365  onst server = Se
+00000b90: 7276 6572 436f 6e6e 6563 7469 6f6e 2e6d  rverConnection.m
+00000ba0: 616b 6553 6574 7469 6e67 7328 293b 0a20  akeSettings();. 
+00000bb0: 2020 2063 6f6e 7374 2075 726c 203d 2055     const url = U
+00000bc0: 524c 4578 742e 6a6f 696e 2873 6572 7665  RLExt.join(serve
+00000bd0: 722e 7773 5572 6c2c 2027 6170 692f 636f  r.wsUrl, 'api/co
+00000be0: 6c6c 6162 6f72 6174 696f 6e2f 726f 6f6d  llaboration/room
+00000bf0: 2729 3b0a 0a20 2020 206e 6577 2057 6562  ');..    new Web
+00000c00: 536f 636b 6574 4177 6172 656e 6573 7350  SocketAwarenessP
+00000c10: 726f 7669 6465 7228 7b0a 2020 2020 2020  rovider({.      
+00000c20: 7572 6c3a 2075 726c 2c0a 2020 2020 2020  url: url,.      
+00000c30: 726f 6f6d 4944 3a20 274a 7570 7974 6572  roomID: 'Jupyter
+00000c40: 4c61 623a 676c 6f62 616c 4177 6172 656e  Lab:globalAwaren
+00000c50: 6573 7327 2c0a 2020 2020 2020 6177 6172  ess',.      awar
+00000c60: 656e 6573 733a 2061 7761 7265 6e65 7373  eness: awareness
+00000c70: 2c0a 2020 2020 2020 7573 6572 3a20 7573  ,.      user: us
+00000c80: 6572 0a20 2020 207d 293b 0a0a 2020 2020  er.    });..    
+00000c90: 7374 6174 652e 6368 616e 6765 642e 636f  state.changed.co
+00000ca0: 6e6e 6563 7428 6173 796e 6320 2829 203d  nnect(async () =
+00000cb0: 3e20 7b0a 2020 2020 2020 636f 6e73 7420  > {.      const 
+00000cc0: 6461 7461 3a20 616e 7920 3d20 6177 6169  data: any = awai
+00000cd0: 7420 7374 6174 652e 746f 4a53 4f4e 2829  t state.toJSON()
+00000ce0: 3b0a 2020 2020 2020 636f 6e73 7420 6375  ;.      const cu
+00000cf0: 7272 656e 7420 3d20 6461 7461 5b27 6c61  rrent = data['la
+00000d00: 796f 7574 2d72 6573 746f 7265 723a 6461  yout-restorer:da
+00000d10: 7461 275d 3f2e 6d61 696e 3f2e 6375 7272  ta']?.main?.curr
+00000d20: 656e 7420 7c7c 2027 273b 0a0a 2020 2020  ent || '';..    
+00000d30: 2020 6966 2028 6375 7272 656e 742e 7374    if (current.st
+00000d40: 6172 7473 5769 7468 2827 6564 6974 6f72  artsWith('editor
+00000d50: 2729 207c 7c20 6375 7272 656e 742e 7374  ') || current.st
+00000d60: 6172 7473 5769 7468 2827 6e6f 7465 626f  artsWith('notebo
+00000d70: 6f6b 2729 2920 7b0a 2020 2020 2020 2020  ok')) {.        
+00000d80: 6177 6172 656e 6573 732e 7365 744c 6f63  awareness.setLoc
+00000d90: 616c 5374 6174 6546 6965 6c64 2827 6375  alStateField('cu
+00000da0: 7272 656e 7427 2c20 6375 7272 656e 7429  rrent', current)
+00000db0: 3b0a 2020 2020 2020 7d20 656c 7365 207b  ;.      } else {
+00000dc0: 0a20 2020 2020 2020 2061 7761 7265 6e65  .        awarene
+00000dd0: 7373 2e73 6574 4c6f 6361 6c53 7461 7465  ss.setLocalState
+00000de0: 4669 656c 6428 2763 7572 7265 6e74 272c  Field('current',
+00000df0: 206e 756c 6c29 3b0a 2020 2020 2020 7d0a   null);.      }.
+00000e00: 2020 2020 7d29 3b0a 0a20 2020 2072 6574      });..    ret
+00000e10: 7572 6e20 6177 6172 656e 6573 733b 0a20  urn awareness;. 
+00000e20: 207d 0a7d 3b0a 0a2f 2a2a 0a20 2a20 4a75   }.};../**. * Ju
+00000e30: 7079 7465 7220 706c 7567 696e 2061 6464  pyter plugin add
+00000e40: 696e 6720 7468 6520 5254 4320 696e 666f  ing the RTC info
+00000e50: 726d 6174 696f 6e20 746f 2074 6865 2061  rmation to the a
+00000e60: 7070 6c69 6361 7469 6f6e 206c 6566 7420  pplication left 
+00000e70: 7061 6e65 6c20 6966 2063 6f6c 6c61 626f  panel if collabo
+00000e80: 7261 7469 7665 2066 6c61 6720 656e 6162  rative flag enab
+00000e90: 6c65 642e 0a20 2a2f 0a65 7870 6f72 7420  led.. */.export 
+00000ea0: 636f 6e73 7420 7274 6350 616e 656c 506c  const rtcPanelPl
+00000eb0: 7567 696e 3a20 4a75 7079 7465 7246 726f  ugin: JupyterFro
+00000ec0: 6e74 456e 6450 6c75 6769 6e3c 766f 6964  ntEndPlugin<void
+00000ed0: 3e20 3d20 7b0a 2020 6964 3a20 2740 6a75  > = {.  id: '@ju
+00000ee0: 7079 7465 722f 636f 6c6c 6162 6f72 6174  pyter/collaborat
+00000ef0: 696f 6e2d 6578 7465 6e73 696f 6e3a 7274  ion-extension:rt
+00000f00: 6350 616e 656c 272c 0a20 2064 6573 6372  cPanel',.  descr
+00000f10: 6970 7469 6f6e 3a20 2741 6464 2073 6964  iption: 'Add sid
+00000f20: 6520 7061 6e65 6c20 746f 2064 6973 706c  e panel to displ
+00000f30: 6179 2061 6c6c 2063 7572 7265 6e74 6c79  ay all currently
+00000f40: 2063 6f6e 6e65 6374 6564 2075 7365 7273   connected users
+00000f50: 2e27 2c0a 2020 6175 746f 5374 6172 743a  .',.  autoStart:
+00000f60: 2074 7275 652c 0a20 2072 6571 7569 7265   true,.  require
+00000f70: 733a 205b 4947 6c6f 6261 6c41 7761 7265  s: [IGlobalAware
+00000f80: 6e65 7373 5d2c 0a20 206f 7074 696f 6e61  ness],.  optiona
+00000f90: 6c3a 205b 4954 7261 6e73 6c61 746f 725d  l: [ITranslator]
+00000fa0: 2c0a 2020 6163 7469 7661 7465 3a20 280a  ,.  activate: (.
+00000fb0: 2020 2020 6170 703a 204a 7570 7974 6572      app: Jupyter
+00000fc0: 4672 6f6e 7445 6e64 2c0a 2020 2020 6177  FrontEnd,.    aw
+00000fd0: 6172 656e 6573 733a 2041 7761 7265 6e65  areness: Awarene
+00000fe0: 7373 2c0a 2020 2020 7472 616e 736c 6174  ss,.    translat
+00000ff0: 6f72 3a20 4954 7261 6e73 6c61 746f 7220  or: ITranslator 
+00001000: 7c20 6e75 6c6c 0a20 2029 3a20 766f 6964  | null.  ): void
+00001010: 203d 3e20 7b0a 2020 2020 636f 6e73 7420   => {.    const 
+00001020: 7b20 7573 6572 207d 203d 2061 7070 2e73  { user } = app.s
+00001030: 6572 7669 6365 4d61 6e61 6765 723b 0a0a  erviceManager;..
+00001040: 2020 2020 636f 6e73 7420 7472 616e 7320      const trans 
+00001050: 3d20 2874 7261 6e73 6c61 746f 7220 3f3f  = (translator ??
+00001060: 206e 756c 6c54 7261 6e73 6c61 746f 7229   nullTranslator)
+00001070: 2e6c 6f61 6428 276a 7570 7974 6572 5f63  .load('jupyter_c
+00001080: 6f6c 6c61 626f 7261 7469 6f6e 2729 3b0a  ollaboration');.
+00001090: 0a20 2020 2063 6f6e 7374 2075 7365 7250  .    const userP
+000010a0: 616e 656c 203d 206e 6577 2053 6964 6550  anel = new SideP
+000010b0: 616e 656c 287b 0a20 2020 2020 2061 6c69  anel({.      ali
+000010c0: 676e 6d65 6e74 3a20 276a 7573 7469 6679  gnment: 'justify
+000010d0: 270a 2020 2020 7d29 3b0a 2020 2020 7573  '.    });.    us
+000010e0: 6572 5061 6e65 6c2e 6964 203d 2027 6a70  erPanel.id = 'jp
+000010f0: 2d63 6f6c 6c61 626f 7261 7469 6f6e 2d70  -collaboration-p
+00001100: 616e 656c 273b 0a20 2020 2075 7365 7250  anel';.    userP
+00001110: 616e 656c 2e74 6974 6c65 2e69 636f 6e20  anel.title.icon 
+00001120: 3d20 7573 6572 7349 636f 6e3b 0a20 2020  = usersIcon;.   
+00001130: 2075 7365 7250 616e 656c 2e74 6974 6c65   userPanel.title
+00001140: 2e63 6170 7469 6f6e 203d 2074 7261 6e73  .caption = trans
+00001150: 2e5f 5f28 2743 6f6c 6c61 626f 7261 7469  .__('Collaborati
+00001160: 6f6e 2729 3b0a 2020 2020 7573 6572 5061  on');.    userPa
+00001170: 6e65 6c2e 6164 6443 6c61 7373 2827 6a70  nel.addClass('jp
+00001180: 2d52 5443 5061 6e65 6c27 293b 0a20 2020  -RTCPanel');.   
+00001190: 2061 7070 2e73 6865 6c6c 2e61 6464 2875   app.shell.add(u
+000011a0: 7365 7250 616e 656c 2c20 276c 6566 7427  serPanel, 'left'
+000011b0: 2c20 7b20 7261 6e6b 3a20 3330 3020 7d29  , { rank: 300 })
+000011c0: 3b0a 0a20 2020 2063 6f6e 7374 2063 7572  ;..    const cur
+000011d0: 7265 6e74 5573 6572 5061 6e65 6c20 3d20  rentUserPanel = 
+000011e0: 6e65 7720 5573 6572 496e 666f 5061 6e65  new UserInfoPane
+000011f0: 6c28 7573 6572 293b 0a20 2020 2063 7572  l(user);.    cur
+00001200: 7265 6e74 5573 6572 5061 6e65 6c2e 7469  rentUserPanel.ti
+00001210: 746c 652e 6c61 6265 6c20 3d20 7472 616e  tle.label = tran
+00001220: 732e 5f5f 2827 5573 6572 2069 6e66 6f27  s.__('User info'
+00001230: 293b 0a20 2020 2063 7572 7265 6e74 5573  );.    currentUs
+00001240: 6572 5061 6e65 6c2e 7469 746c 652e 6361  erPanel.title.ca
+00001250: 7074 696f 6e20 3d20 7472 616e 732e 5f5f  ption = trans.__
+00001260: 2827 5573 6572 2069 6e66 6f72 6d61 7469  ('User informati
+00001270: 6f6e 2729 3b0a 2020 2020 7573 6572 5061  on');.    userPa
+00001280: 6e65 6c2e 6164 6457 6964 6765 7428 6375  nel.addWidget(cu
+00001290: 7272 656e 7455 7365 7250 616e 656c 293b  rrentUserPanel);
+000012a0: 0a0a 2020 2020 636f 6e73 7420 6669 6c65  ..    const file
+000012b0: 6f70 656e 6572 203d 2028 7061 7468 3a20  opener = (path: 
+000012c0: 7374 7269 6e67 2920 3d3e 207b 0a20 2020  string) => {.   
+000012d0: 2020 2076 6f69 6420 6170 702e 636f 6d6d     void app.comm
+000012e0: 616e 6473 2e65 7865 6375 7465 2827 646f  ands.execute('do
+000012f0: 636d 616e 6167 6572 3a6f 7065 6e27 2c20  cmanager:open', 
+00001300: 7b20 7061 7468 207d 293b 0a20 2020 207d  { path });.    }
+00001310: 3b0a 0a20 2020 2063 6f6e 7374 2063 6f6c  ;..    const col
+00001320: 6c61 626f 7261 746f 7273 5061 6e65 6c20  laboratorsPanel 
+00001330: 3d20 6e65 7720 436f 6c6c 6162 6f72 6174  = new Collaborat
+00001340: 6f72 7350 616e 656c 280a 2020 2020 2020  orsPanel(.      
+00001350: 7573 6572 2c0a 2020 2020 2020 6177 6172  user,.      awar
+00001360: 656e 6573 732c 0a20 2020 2020 2066 696c  eness,.      fil
+00001370: 656f 7065 6e65 720a 2020 2020 293b 0a20  eopener.    );. 
+00001380: 2020 2063 6f6c 6c61 626f 7261 746f 7273     collaborators
+00001390: 5061 6e65 6c2e 7469 746c 652e 6c61 6265  Panel.title.labe
+000013a0: 6c20 3d20 7472 616e 732e 5f5f 2827 4f6e  l = trans.__('On
+000013b0: 6c69 6e65 2043 6f6c 6c61 626f 7261 746f  line Collaborato
+000013c0: 7273 2729 3b0a 2020 2020 7573 6572 5061  rs');.    userPa
+000013d0: 6e65 6c2e 6164 6457 6964 6765 7428 636f  nel.addWidget(co
+000013e0: 6c6c 6162 6f72 6174 6f72 7350 616e 656c  llaboratorsPanel
+000013f0: 293b 0a20 207d 0a7d 3b0a 0a65 7870 6f72  );.  }.};..expor
+00001400: 7420 636f 6e73 7420 7573 6572 4564 6974  t const userEdit
+00001410: 6f72 4375 7273 6f72 733a 204a 7570 7974  orCursors: Jupyt
+00001420: 6572 4672 6f6e 7445 6e64 506c 7567 696e  erFrontEndPlugin
+00001430: 3c76 6f69 643e 203d 207b 0a20 2069 643a  <void> = {.  id:
+00001440: 2027 406a 7570 7974 6572 2f63 6f6c 6c61   '@jupyter/colla
+00001450: 626f 7261 7469 6f6e 2d65 7874 656e 7369  boration-extensi
+00001460: 6f6e 3a75 7365 7245 6469 746f 7243 7572  on:userEditorCur
+00001470: 736f 7273 272c 0a20 2064 6573 6372 6970  sors',.  descrip
+00001480: 7469 6f6e 3a0a 2020 2020 2741 6464 2043  tion:.    'Add C
+00001490: 6f64 654d 6972 726f 7220 6578 7465 6e73  odeMirror extens
+000014a0: 696f 6e20 746f 2064 6973 706c 6179 2072  ion to display r
+000014b0: 656d 6f74 6520 7573 6572 2063 7572 736f  emote user curso
+000014c0: 7273 2061 6e64 2073 656c 6563 7469 6f6e  rs and selection
+000014d0: 732e 272c 0a20 2061 7574 6f53 7461 7274  s.',.  autoStart
+000014e0: 3a20 7472 7565 2c0a 2020 7265 7175 6972  : true,.  requir
+000014f0: 6573 3a20 5b49 4564 6974 6f72 4578 7465  es: [IEditorExte
+00001500: 6e73 696f 6e52 6567 6973 7472 795d 2c0a  nsionRegistry],.
+00001510: 2020 6163 7469 7661 7465 3a20 280a 2020    activate: (.  
+00001520: 2020 6170 703a 204a 7570 7974 6572 4672    app: JupyterFr
+00001530: 6f6e 7445 6e64 2c0a 2020 2020 6578 7465  ontEnd,.    exte
+00001540: 6e73 696f 6e73 3a20 4945 6469 746f 7245  nsions: IEditorE
+00001550: 7874 656e 7369 6f6e 5265 6769 7374 7279  xtensionRegistry
+00001560: 0a20 2029 3a20 766f 6964 203d 3e20 7b0a  .  ): void => {.
+00001570: 2020 2020 6578 7465 6e73 696f 6e73 2e61      extensions.a
+00001580: 6464 4578 7465 6e73 696f 6e28 7b0a 2020  ddExtension({.  
+00001590: 2020 2020 6e61 6d65 3a20 2772 656d 6f74      name: 'remot
+000015a0: 652d 7573 6572 2d63 7572 736f 7273 272c  e-user-cursors',
+000015b0: 0a20 2020 2020 2066 6163 746f 7279 286f  .      factory(o
+000015c0: 7074 696f 6e73 2920 7b0a 2020 2020 2020  ptions) {.      
+000015d0: 2020 636f 6e73 7420 7b20 6177 6172 656e    const { awaren
+000015e0: 6573 732c 2079 736f 7572 6365 3a20 7974  ess, ysource: yt
+000015f0: 6578 7420 7d20 3d20 6f70 7469 6f6e 732e  ext } = options.
+00001600: 6d6f 6465 6c2e 7368 6172 6564 4d6f 6465  model.sharedMode
+00001610: 6c20 6173 2061 6e79 3b0a 2020 2020 2020  l as any;.      
+00001620: 2020 7265 7475 726e 2045 6469 746f 7245    return EditorE
+00001630: 7874 656e 7369 6f6e 5265 6769 7374 7279  xtensionRegistry
+00001640: 2e63 7265 6174 6549 6d6d 7574 6162 6c65  .createImmutable
+00001650: 4578 7465 6e73 696f 6e28 0a20 2020 2020  Extension(.     
+00001660: 2020 2020 2072 656d 6f74 6555 7365 7243       remoteUserC
+00001670: 7572 736f 7273 287b 2061 7761 7265 6e65  ursors({ awarene
+00001680: 7373 2c20 7974 6578 7420 7d29 0a20 2020  ss, ytext }).   
+00001690: 2020 2020 2029 3b0a 2020 2020 2020 7d0a       );.      }.
+000016a0: 2020 2020 7d29 3b0a 2020 7d0a 7d3b 0a        });.  }.};.
```

### Comparing `jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/lib/sharedlink.js` & `jupyter_collaboration_ui-1.0.0a1/packages/collaboration-extension/src/sharedlink.ts`

 * *Files 14% similar despite different names*

```diff
@@ -1,99 +1,97 @@
 00000000: 2f2f 2043 6f70 7972 6967 6874 2028 6329  // Copyright (c)
 00000010: 204a 7570 7974 6572 2044 6576 656c 6f70   Jupyter Develop
 00000020: 6d65 6e74 2054 6561 6d2e 0a2f 2f20 4469  ment Team..// Di
 00000030: 7374 7269 6275 7465 6420 756e 6465 7220  stributed under 
 00000040: 7468 6520 7465 726d 7320 6f66 2074 6865  the terms of the
 00000050: 204d 6f64 6966 6965 6420 4253 4420 4c69   Modified BSD Li
-00000060: 6365 6e73 652e 0a69 6d70 6f72 7420 7b20  cense..import { 
-00000070: 436c 6970 626f 6172 642c 2049 436f 6d6d  Clipboard, IComm
-00000080: 616e 6450 616c 6574 7465 207d 2066 726f  andPalette } fro
-00000090: 6d20 2740 6a75 7079 7465 726c 6162 2f61  m '@jupyterlab/a
-000000a0: 7070 7574 696c 7327 3b0a 696d 706f 7274  pputils';.import
-000000b0: 207b 2049 5472 616e 736c 6174 6f72 2c20   { ITranslator, 
-000000c0: 6e75 6c6c 5472 616e 736c 6174 6f72 207d  nullTranslator }
-000000d0: 2066 726f 6d20 2740 6a75 7079 7465 726c   from '@jupyterl
-000000e0: 6162 2f74 7261 6e73 6c61 7469 6f6e 273b  ab/translation';
-000000f0: 0a69 6d70 6f72 7420 7b20 7368 6172 6549  .import { shareI
-00000100: 636f 6e20 7d20 6672 6f6d 2027 406a 7570  con } from '@jup
-00000110: 7974 6572 6c61 622f 7569 2d63 6f6d 706f  yterlab/ui-compo
-00000120: 6e65 6e74 7327 3b0a 696d 706f 7274 207b  nents';.import {
-00000130: 2073 686f 7753 6861 7265 644c 696e 6b44   showSharedLinkD
-00000140: 6961 6c6f 6720 7d20 6672 6f6d 2027 406a  ialog } from '@j
-00000150: 7570 7974 6572 2f63 6f6c 6c61 626f 7261  upyter/collabora
-00000160: 7469 6f6e 273b 0a2f 2a2a 0a20 2a20 5468  tion';./**. * Th
-00000170: 6520 636f 6d6d 616e 6420 4944 7320 7573  e command IDs us
-00000180: 6564 2062 7920 7468 6520 706c 7567 696e  ed by the plugin
-00000190: 2e0a 202a 2f0a 7661 7220 436f 6d6d 616e  .. */.var Comman
-000001a0: 6449 4473 3b0a 2866 756e 6374 696f 6e20  dIDs;.(function 
-000001b0: 2843 6f6d 6d61 6e64 4944 7329 207b 0a20  (CommandIDs) {. 
-000001c0: 2020 2043 6f6d 6d61 6e64 4944 732e 7368     CommandIDs.sh
-000001d0: 6172 6520 3d20 2763 6f6c 6c61 626f 7261  are = 'collabora
-000001e0: 7469 6f6e 3a73 6861 7265 642d 6c69 6e6b  tion:shared-link
-000001f0: 273b 0a7d 2928 436f 6d6d 616e 6449 4473  ';.})(CommandIDs
-00000200: 207c 7c20 2843 6f6d 6d61 6e64 4944 7320   || (CommandIDs 
-00000210: 3d20 7b7d 2929 3b0a 2f2a 2a0a 202a 2050  = {}));./**. * P
-00000220: 6c75 6769 6e20 746f 2073 6861 7265 2074  lugin to share t
-00000230: 6865 2055 524c 206f 6620 7468 6520 7275  he URL of the ru
-00000240: 6e6e 696e 6720 4a75 7079 7465 7220 5365  nning Jupyter Se
-00000250: 7276 6572 0a20 2a2f 0a65 7870 6f72 7420  rver. */.export 
-00000260: 636f 6e73 7420 7368 6172 6564 4c69 6e6b  const sharedLink
-00000270: 203d 207b 0a20 2020 2069 643a 2027 406a   = {.    id: '@j
-00000280: 7570 7974 6572 2f63 6f6c 6c61 626f 7261  upyter/collabora
-00000290: 7469 6f6e 2d65 7874 656e 7369 6f6e 3a73  tion-extension:s
-000002a0: 6861 7265 642d 6c69 6e6b 272c 0a20 2020  hared-link',.   
-000002b0: 2061 7574 6f53 7461 7274 3a20 7472 7565   autoStart: true
-000002c0: 2c0a 2020 2020 6f70 7469 6f6e 616c 3a20  ,.    optional: 
-000002d0: 5b49 436f 6d6d 616e 6450 616c 6574 7465  [ICommandPalette
-000002e0: 2c20 4954 7261 6e73 6c61 746f 725d 2c0a  , ITranslator],.
-000002f0: 2020 2020 6163 7469 7661 7465 3a20 6173      activate: as
-00000300: 796e 6320 2861 7070 2c20 7061 6c65 7474  ync (app, palett
-00000310: 652c 2074 7261 6e73 6c61 746f 7229 203d  e, translator) =
-00000320: 3e20 7b0a 2020 2020 2020 2020 636f 6e73  > {.        cons
-00000330: 7420 7b20 636f 6d6d 616e 6473 207d 203d  t { commands } =
-00000340: 2061 7070 3b0a 2020 2020 2020 2020 636f   app;.        co
-00000350: 6e73 7420 7472 616e 7320 3d20 2874 7261  nst trans = (tra
-00000360: 6e73 6c61 746f 7220 213d 3d20 6e75 6c6c  nslator !== null
-00000370: 2026 2620 7472 616e 736c 6174 6f72 2021   && translator !
-00000380: 3d3d 2076 6f69 6420 3020 3f20 7472 616e  == void 0 ? tran
-00000390: 736c 6174 6f72 203a 206e 756c 6c54 7261  slator : nullTra
-000003a0: 6e73 6c61 746f 7229 2e6c 6f61 6428 2763  nslator).load('c
-000003b0: 6f6c 6c61 626f 7261 7469 6f6e 2729 3b0a  ollaboration');.
-000003c0: 2020 2020 2020 2020 636f 6d6d 616e 6473          commands
-000003d0: 2e61 6464 436f 6d6d 616e 6428 436f 6d6d  .addCommand(Comm
-000003e0: 616e 6449 4473 2e73 6861 7265 2c20 7b0a  andIDs.share, {.
-000003f0: 2020 2020 2020 2020 2020 2020 6c61 6265              labe
-00000400: 6c3a 2074 7261 6e73 2e5f 5f28 2747 656e  l: trans.__('Gen
-00000410: 6572 6174 6520 6120 5368 6172 6564 204c  erate a Shared L
-00000420: 696e 6b27 292c 0a20 2020 2020 2020 2020  ink'),.         
-00000430: 2020 2069 636f 6e3a 2073 6861 7265 4963     icon: shareIc
-00000440: 6f6e 2c0a 2020 2020 2020 2020 2020 2020  on,.            
-00000450: 6578 6563 7574 653a 2061 7379 6e63 2028  execute: async (
-00000460: 2920 3d3e 207b 0a20 2020 2020 2020 2020  ) => {.         
-00000470: 2020 2020 2020 2063 6f6e 7374 2072 6573         const res
-00000480: 756c 7420 3d20 6177 6169 7420 7368 6f77  ult = await show
-00000490: 5368 6172 6564 4c69 6e6b 4469 616c 6f67  SharedLinkDialog
-000004a0: 287b 0a20 2020 2020 2020 2020 2020 2020  ({.             
-000004b0: 2020 2020 2020 2074 7261 6e73 6c61 746f         translato
-000004c0: 720a 2020 2020 2020 2020 2020 2020 2020  r.              
-000004d0: 2020 7d29 3b0a 2020 2020 2020 2020 2020    });.          
-000004e0: 2020 2020 2020 6966 2028 7265 7375 6c74        if (result
-000004f0: 2e62 7574 746f 6e2e 6163 6365 7074 2026  .button.accept &
-00000500: 2620 7265 7375 6c74 2e76 616c 7565 2920  & result.value) 
-00000510: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-00000520: 2020 2020 2020 436c 6970 626f 6172 642e        Clipboard.
-00000530: 636f 7079 546f 5379 7374 656d 2872 6573  copyToSystem(res
-00000540: 756c 742e 7661 6c75 6529 3b0a 2020 2020  ult.value);.    
-00000550: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
-00000560: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
-00000570: 2020 2020 7d29 3b0a 2020 2020 2020 2020      });.        
-00000580: 6966 2028 7061 6c65 7474 6529 207b 0a20  if (palette) {. 
-00000590: 2020 2020 2020 2020 2020 2070 616c 6574             palet
-000005a0: 7465 2e61 6464 4974 656d 287b 0a20 2020  te.addItem({.   
-000005b0: 2020 2020 2020 2020 2020 2020 2063 6f6d               com
-000005c0: 6d61 6e64 3a20 436f 6d6d 616e 6449 4473  mand: CommandIDs
-000005d0: 2e73 6861 7265 2c0a 2020 2020 2020 2020  .share,.        
-000005e0: 2020 2020 2020 2020 6361 7465 676f 7279          category
-000005f0: 3a20 7472 616e 732e 5f5f 2827 5365 7276  : trans.__('Serv
-00000600: 6572 2729 0a20 2020 2020 2020 2020 2020  er').           
-00000610: 207d 293b 0a20 2020 2020 2020 207d 0a20   });.        }. 
-00000620: 2020 207d 0a7d 3b0a                         }.};.
+00000060: 6365 6e73 652e 0a0a 696d 706f 7274 207b  cense...import {
+00000070: 0a20 204a 7570 7974 6572 4672 6f6e 7445  .  JupyterFrontE
+00000080: 6e64 2c0a 2020 4a75 7079 7465 7246 726f  nd,.  JupyterFro
+00000090: 6e74 456e 6450 6c75 6769 6e0a 7d20 6672  ntEndPlugin.} fr
+000000a0: 6f6d 2027 406a 7570 7974 6572 6c61 622f  om '@jupyterlab/
+000000b0: 6170 706c 6963 6174 696f 6e27 3b0a 696d  application';.im
+000000c0: 706f 7274 207b 2043 6c69 7062 6f61 7264  port { Clipboard
+000000d0: 2c20 4943 6f6d 6d61 6e64 5061 6c65 7474  , ICommandPalett
+000000e0: 6520 7d20 6672 6f6d 2027 406a 7570 7974  e } from '@jupyt
+000000f0: 6572 6c61 622f 6170 7075 7469 6c73 273b  erlab/apputils';
+00000100: 0a69 6d70 6f72 7420 7b20 4954 7261 6e73  .import { ITrans
+00000110: 6c61 746f 722c 206e 756c 6c54 7261 6e73  lator, nullTrans
+00000120: 6c61 746f 7220 7d20 6672 6f6d 2027 406a  lator } from '@j
+00000130: 7570 7974 6572 6c61 622f 7472 616e 736c  upyterlab/transl
+00000140: 6174 696f 6e27 3b0a 696d 706f 7274 207b  ation';.import {
+00000150: 2073 6861 7265 4963 6f6e 207d 2066 726f   shareIcon } fro
+00000160: 6d20 2740 6a75 7079 7465 726c 6162 2f75  m '@jupyterlab/u
+00000170: 692d 636f 6d70 6f6e 656e 7473 273b 0a0a  i-components';..
+00000180: 696d 706f 7274 207b 2073 686f 7753 6861  import { showSha
+00000190: 7265 644c 696e 6b44 6961 6c6f 6720 7d20  redLinkDialog } 
+000001a0: 6672 6f6d 2027 406a 7570 7974 6572 2f63  from '@jupyter/c
+000001b0: 6f6c 6c61 626f 7261 7469 6f6e 273b 0a0a  ollaboration';..
+000001c0: 2f2a 2a0a 202a 2054 6865 2063 6f6d 6d61  /**. * The comma
+000001d0: 6e64 2049 4473 2075 7365 6420 6279 2074  nd IDs used by t
+000001e0: 6865 2070 6c75 6769 6e2e 0a20 2a2f 0a6e  he plugin.. */.n
+000001f0: 616d 6573 7061 6365 2043 6f6d 6d61 6e64  amespace Command
+00000200: 4944 7320 7b0a 2020 6578 706f 7274 2063  IDs {.  export c
+00000210: 6f6e 7374 2073 6861 7265 203d 2027 636f  onst share = 'co
+00000220: 6c6c 6162 6f72 6174 696f 6e3a 7368 6172  llaboration:shar
+00000230: 6564 2d6c 696e 6b27 3b0a 7d0a 0a2f 2a2a  ed-link';.}../**
+00000240: 0a20 2a20 506c 7567 696e 2074 6f20 7368  . * Plugin to sh
+00000250: 6172 6520 7468 6520 5552 4c20 6f66 2074  are the URL of t
+00000260: 6865 2072 756e 6e69 6e67 204a 7570 7974  he running Jupyt
+00000270: 6572 2053 6572 7665 720a 202a 2f0a 6578  er Server. */.ex
+00000280: 706f 7274 2063 6f6e 7374 2073 6861 7265  port const share
+00000290: 644c 696e 6b3a 204a 7570 7974 6572 4672  dLink: JupyterFr
+000002a0: 6f6e 7445 6e64 506c 7567 696e 3c76 6f69  ontEndPlugin<voi
+000002b0: 643e 203d 207b 0a20 2069 643a 2027 406a  d> = {.  id: '@j
+000002c0: 7570 7974 6572 2f63 6f6c 6c61 626f 7261  upyter/collabora
+000002d0: 7469 6f6e 2d65 7874 656e 7369 6f6e 3a73  tion-extension:s
+000002e0: 6861 7265 642d 6c69 6e6b 272c 0a20 2061  hared-link',.  a
+000002f0: 7574 6f53 7461 7274 3a20 7472 7565 2c0a  utoStart: true,.
+00000300: 2020 6f70 7469 6f6e 616c 3a20 5b49 436f    optional: [ICo
+00000310: 6d6d 616e 6450 616c 6574 7465 2c20 4954  mmandPalette, IT
+00000320: 7261 6e73 6c61 746f 725d 2c0a 2020 6163  ranslator],.  ac
+00000330: 7469 7661 7465 3a20 6173 796e 6320 280a  tivate: async (.
+00000340: 2020 2020 6170 703a 204a 7570 7974 6572      app: Jupyter
+00000350: 4672 6f6e 7445 6e64 2c0a 2020 2020 7061  FrontEnd,.    pa
+00000360: 6c65 7474 653a 2049 436f 6d6d 616e 6450  lette: ICommandP
+00000370: 616c 6574 7465 207c 206e 756c 6c2c 0a20  alette | null,. 
+00000380: 2020 2074 7261 6e73 6c61 746f 723a 2049     translator: I
+00000390: 5472 616e 736c 6174 6f72 207c 206e 756c  Translator | nul
+000003a0: 6c0a 2020 2920 3d3e 207b 0a20 2020 2063  l.  ) => {.    c
+000003b0: 6f6e 7374 207b 2063 6f6d 6d61 6e64 7320  onst { commands 
+000003c0: 7d20 3d20 6170 703b 0a20 2020 2063 6f6e  } = app;.    con
+000003d0: 7374 2074 7261 6e73 203d 2028 7472 616e  st trans = (tran
+000003e0: 736c 6174 6f72 203f 3f20 6e75 6c6c 5472  slator ?? nullTr
+000003f0: 616e 736c 6174 6f72 292e 6c6f 6164 2827  anslator).load('
+00000400: 636f 6c6c 6162 6f72 6174 696f 6e27 293b  collaboration');
+00000410: 0a0a 2020 2020 636f 6d6d 616e 6473 2e61  ..    commands.a
+00000420: 6464 436f 6d6d 616e 6428 436f 6d6d 616e  ddCommand(Comman
+00000430: 6449 4473 2e73 6861 7265 2c20 7b0a 2020  dIDs.share, {.  
+00000440: 2020 2020 6c61 6265 6c3a 2074 7261 6e73      label: trans
+00000450: 2e5f 5f28 2747 656e 6572 6174 6520 6120  .__('Generate a 
+00000460: 5368 6172 6564 204c 696e 6b27 292c 0a20  Shared Link'),. 
+00000470: 2020 2020 2069 636f 6e3a 2073 6861 7265       icon: share
+00000480: 4963 6f6e 2c0a 2020 2020 2020 6578 6563  Icon,.      exec
+00000490: 7574 653a 2061 7379 6e63 2028 2920 3d3e  ute: async () =>
+000004a0: 207b 0a20 2020 2020 2020 2063 6f6e 7374   {.        const
+000004b0: 2072 6573 756c 7420 3d20 6177 6169 7420   result = await 
+000004c0: 7368 6f77 5368 6172 6564 4c69 6e6b 4469  showSharedLinkDi
+000004d0: 616c 6f67 287b 0a20 2020 2020 2020 2020  alog({.         
+000004e0: 2074 7261 6e73 6c61 746f 720a 2020 2020   translator.    
+000004f0: 2020 2020 7d29 3b0a 2020 2020 2020 2020      });.        
+00000500: 6966 2028 7265 7375 6c74 2e62 7574 746f  if (result.butto
+00000510: 6e2e 6163 6365 7074 2026 2620 7265 7375  n.accept && resu
+00000520: 6c74 2e76 616c 7565 2920 7b0a 2020 2020  lt.value) {.    
+00000530: 2020 2020 2020 436c 6970 626f 6172 642e        Clipboard.
+00000540: 636f 7079 546f 5379 7374 656d 2872 6573  copyToSystem(res
+00000550: 756c 742e 7661 6c75 6529 3b0a 2020 2020  ult.value);.    
+00000560: 2020 2020 7d0a 2020 2020 2020 7d0a 2020      }.      }.  
+00000570: 2020 7d29 3b0a 0a20 2020 2069 6620 2870    });..    if (p
+00000580: 616c 6574 7465 2920 7b0a 2020 2020 2020  alette) {.      
+00000590: 7061 6c65 7474 652e 6164 6449 7465 6d28  palette.addItem(
+000005a0: 7b0a 2020 2020 2020 2020 636f 6d6d 616e  {.        comman
+000005b0: 643a 2043 6f6d 6d61 6e64 4944 732e 7368  d: CommandIDs.sh
+000005c0: 6172 652c 0a20 2020 2020 2020 2063 6174  are,.        cat
+000005d0: 6567 6f72 793a 2074 7261 6e73 2e5f 5f28  egory: trans.__(
+000005e0: 2753 6572 7665 7227 290a 2020 2020 2020  'Server').      
+000005f0: 7d29 3b0a 2020 2020 7d0a 2020 7d0a 7d3b  });.    }.  }.};
+00000600: 0a                                       .
```

### Comparing `jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/package.json` & `jupyter_collaboration_ui-1.0.0a1/packages/docprovider-extension/package.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6219283629130176%*

 * *Differences: {"'bugs'": "{'url': 'https://github.com/jupyterlab/jupyter-collaboration/issues'}",*

 * * "'dependencies'": "{'@jupyterlab/translation': '^4.2.0-beta.0', '@lumino/commands': '^2.1.0', "*

 * *                   "'@jupyter/docprovider': '^3.0.0-alpha.1', '@jupyter/ydoc': '^1.1.0-a0', "*

 * *                   "'@jupyterlab/application': '^4.2.0-beta.0', '@jupyterlab/apputils': "*

 * *                   "'^4.2.0-beta.0', '@jupyterlab/docregistry': '^4.2.0-beta.0', "*

 * *                   "'@jupyterlab/filebrowser': '^4.2.0-beta.0',  […]*

```diff
@@ -1,83 +1,122 @@
 {
     "author": "Project Jupyter",
     "bugs": {
-        "url": "https://github.com/jupyterlab/jupyterlab/issues"
+        "url": "https://github.com/jupyterlab/jupyter-collaboration/issues"
     },
     "dependencies": {
-        "@jupyter/react-components": "^0.15.2",
-        "@jupyter/web-components": "^0.15.2",
-        "@jupyterlab/coreutils": "^6.2.0-beta.1",
-        "@jupyterlab/observables": "^5.2.0-beta.1",
-        "@jupyterlab/rendermime-interfaces": "^3.10.0-beta.1",
-        "@jupyterlab/translation": "^4.2.0-beta.1",
-        "@lumino/algorithm": "^2.0.1",
-        "@lumino/commands": "^2.3.0",
-        "@lumino/coreutils": "^2.1.2",
-        "@lumino/disposable": "^2.1.2",
-        "@lumino/messaging": "^2.0.1",
-        "@lumino/polling": "^2.1.2",
-        "@lumino/properties": "^2.0.1",
-        "@lumino/signaling": "^2.1.2",
-        "@lumino/virtualdom": "^2.0.1",
-        "@lumino/widgets": "^2.3.2",
-        "@rjsf/core": "^5.13.4",
-        "@rjsf/utils": "^5.13.4",
-        "react": "^18.2.0",
-        "react-dom": "^18.2.0",
-        "typestyle": "^2.0.4"
+        "@jupyter/docprovider": "^3.0.0-alpha.1",
+        "@jupyter/ydoc": "^1.1.0-a0",
+        "@jupyterlab/application": "^4.2.0-beta.0",
+        "@jupyterlab/apputils": "^4.2.0-beta.0",
+        "@jupyterlab/docregistry": "^4.2.0-beta.0",
+        "@jupyterlab/filebrowser": "^4.2.0-beta.0",
+        "@jupyterlab/fileeditor": "^4.2.0-beta.0",
+        "@jupyterlab/logconsole": "^4.2.0-beta.0",
+        "@jupyterlab/notebook": "^4.2.0-beta.0",
+        "@jupyterlab/settingregistry": "^4.2.0-beta.0",
+        "@jupyterlab/translation": "^4.2.0-beta.0",
+        "@lumino/commands": "^2.1.0",
+        "y-protocols": "^1.0.5",
+        "y-websocket": "^1.3.15",
+        "yjs": "^13.5.40"
     },
-    "description": "JupyterLab - UI components written in React",
+    "description": "JupyterLab - Collaborative Shared Models",
     "devDependencies": {
-        "@jupyterlab/testing": "^4.2.0-beta.1",
-        "@types/jest": "^29.2.0",
-        "@types/react": "^18.0.26",
-        "jest": "^29.2.0",
-        "rimraf": "~5.0.5",
-        "svgo": "^3.0.1",
-        "typedoc": "~0.24.7",
-        "typescript": "~5.1.6"
+        "@jupyterlab/builder": "^4.0.5",
+        "@types/react": "~18.0.26",
+        "npm-run-all": "^4.1.5",
+        "rimraf": "^4.1.2",
+        "typescript": "~5.0.4"
     },
     "directories": {
         "lib": "lib/"
     },
     "files": [
-        "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
-        "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
-        "style/index.js",
-        "src/**/*.{ts,tsx}"
+        "lib/*.d.ts",
+        "lib/*.js.map",
+        "lib/*.js",
+        "schema/*.json",
+        "style/*.css",
+        "style/index.js"
+    ],
+    "homepage": "https://github.com/jupyterlab/jupyter-collaboration",
+    "jupyterlab": {
+        "disabledExtensions": [
+            "@jupyterlab/filebrowser-extension:defaultFileBrowser",
+            "@jupyterlab/notebook-extension:cell-executor"
+        ],
+        "extension": true,
+        "outputDir": "../../projects/jupyter-docprovider/jupyter_docprovider/labextension",
+        "sharedPackages": {
+            "@codemirror/state": {
+                "bundled": false,
+                "singleton": true
+            },
+            "@codemirror/view": {
+                "bundled": false,
+                "singleton": true
+            },
+            "@jupyter/docprovider": {
+                "bundled": true,
+                "singleton": true
+            },
+            "@jupyter/ydoc": {
+                "bundled": false,
+                "singleton": true
+            },
+            "y-protocols": {
+                "bundled": false,
+                "singleton": true
+            },
+            "yjs": {
+                "bundled": false,
+                "singleton": true
+            }
+        }
+    },
+    "keywords": [
+        "jupyter",
+        "jupyterlab",
+        "jupyterlab-extension"
     ],
-    "homepage": "https://github.com/jupyterlab/jupyterlab",
     "license": "BSD-3-Clause",
     "main": "lib/index.js",
-    "name": "@jupyterlab/ui-components",
-    "peerDependencies": {
-        "react": "^18.2.0"
-    },
+    "name": "@jupyter/docprovider-extension",
     "publishConfig": {
         "access": "public"
     },
     "repository": {
         "type": "git",
-        "url": "https://github.com/jupyterlab/jupyterlab.git"
+        "url": "https://github.com/jupyterlab/jupyter-collaboration.git"
     },
     "scripts": {
-        "build": "tsc -b",
-        "build:test": "tsc --build tsconfig.test.json",
-        "clean": "rimraf lib && rimraf tsconfig.tsbuildinfo",
-        "cleansvg": "svgo --config svgo.yaml",
-        "docs": "typedoc src",
-        "docs:init": "bash docs/build.sh",
-        "test": "jest",
-        "test:cov": "jest --collect-coverage",
-        "test:debug": "node --inspect-brk ../../node_modules/.bin/jest --runInBand",
-        "test:debug:watch": "node --inspect-brk ../../node_modules/.bin/jest --runInBand --watch",
-        "watch": "tsc -b --watch"
+        "build": "jlpm run build:lib && jlpm run build:labextension:dev",
+        "build:labextension": "jupyter labextension build .",
+        "build:labextension:dev": "jupyter labextension build --development True .",
+        "build:lib": "tsc --sourceMap",
+        "build:lib:prod": "tsc",
+        "build:prod": "jlpm run clean && jlpm run build:lib:prod && jlpm run build:labextension",
+        "clean": "jlpm run clean:lib",
+        "clean:all": "jlpm run clean:lib && jlpm run clean:labextension",
+        "clean:labextension": "rimraf ../../projects/jupyter-docprovider/jupyter_docprovider/labextension",
+        "clean:lib": "rimraf lib tsconfig.tsbuildinfo node_modules",
+        "install:extension": "jlpm run build",
+        "watch": "run-p watch:src watch:labextension",
+        "watch:labextension": "jupyter labextension watch .",
+        "watch:src": "tsc -w"
     },
     "sideEffects": [
-        "style/**/*"
+        "style/*.css",
+        "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
+    "typedoc": {
+        "displayName": "@jupyter/docprovider-extension",
+        "entryPoint": "./src/index.ts",
+        "readmeFile": "./README.md",
+        "tsconfig": "./tsconfig.json"
+    },
     "types": "lib/index.d.ts",
-    "version": "4.2.0-beta.1"
+    "version": "3.0.0-alpha.1"
 }
```

### Comparing `jupyter_collaboration_ui-1.0.0a0/packages/collaboration-extension/src/index.ts` & `jupyter_collaboration_ui-1.0.0a1/packages/collaboration-extension/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration_ui-1.0.0a0/packages/docprovider/jest.config.js` & `jupyter_collaboration_ui-1.0.0a1/packages/docprovider/jest.config.js`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration_ui-1.0.0a0/packages/docprovider/lib/requests.js` & `jupyter_collaboration_ui-1.0.0a1/packages/docprovider/src/requests.ts`

 * *Files 19% similar despite different names*

```diff
@@ -10,79 +10,102 @@
 00000090: 6865 2074 6572 6d73 206f 6620 7468 6520  he terms of the 
 000000a0: 4d6f 6469 6669 6564 2042 5344 204c 6963  Modified BSD Lic
 000000b0: 656e 7365 2e0a 7c2d 2d2d 2d2d 2d2d 2d2d  ense..|---------
 000000c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000000d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000000e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000000f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000100: 2d2d 2d2a 2f0a 696d 706f 7274 207b 2055  ---*/.import { U
-00000110: 524c 4578 7420 7d20 6672 6f6d 2027 406a  RLExt } from '@j
-00000120: 7570 7974 6572 6c61 622f 636f 7265 7574  upyterlab/coreut
-00000130: 696c 7327 3b0a 696d 706f 7274 207b 2053  ils';.import { S
-00000140: 6572 7665 7243 6f6e 6e65 6374 696f 6e20  erverConnection 
-00000150: 7d20 6672 6f6d 2027 406a 7570 7974 6572  } from '@jupyter
-00000160: 6c61 622f 7365 7276 6963 6573 273b 0a2f  lab/services';./
-00000170: 2a2a 0a20 2a20 446f 6375 6d65 6e74 2073  **. * Document s
-00000180: 6573 7369 6f6e 2065 6e64 706f 696e 7420  ession endpoint 
-00000190: 7072 6f76 6964 6564 2062 7920 606a 7570  provided by `jup
-000001a0: 7974 6572 5f63 6f6c 6c61 626f 7261 7469  yter_collaborati
-000001b0: 6f6e 600a 202a 2053 6565 2068 7474 7073  on`. * See https
-000001c0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a75  ://github.com/ju
-000001d0: 7079 7465 726c 6162 2f6a 7570 7974 6572  pyterlab/jupyter
-000001e0: 5f63 6f6c 6c61 626f 7261 7469 6f6e 0a20  _collaboration. 
-000001f0: 2a2f 0a63 6f6e 7374 2044 4f43 5f53 4553  */.const DOC_SES
-00000200: 5349 4f4e 5f55 524c 203d 2027 6170 692f  SION_URL = 'api/
-00000210: 636f 6c6c 6162 6f72 6174 696f 6e2f 7365  collaboration/se
-00000220: 7373 696f 6e27 3b0a 6578 706f 7274 2061  ssion';.export a
-00000230: 7379 6e63 2066 756e 6374 696f 6e20 7265  sync function re
-00000240: 7175 6573 7444 6f63 5365 7373 696f 6e28  questDocSession(
-00000250: 666f 726d 6174 2c20 7479 7065 2c20 7061  format, type, pa
-00000260: 7468 2920 7b0a 2020 2020 636f 6e73 7420  th) {.    const 
-00000270: 7365 7474 696e 6773 203d 2053 6572 7665  settings = Serve
-00000280: 7243 6f6e 6e65 6374 696f 6e2e 6d61 6b65  rConnection.make
-00000290: 5365 7474 696e 6773 2829 3b0a 2020 2020  Settings();.    
-000002a0: 636f 6e73 7420 7572 6c20 3d20 5552 4c45  const url = URLE
-000002b0: 7874 2e6a 6f69 6e28 7365 7474 696e 6773  xt.join(settings
-000002c0: 2e62 6173 6555 726c 2c20 444f 435f 5345  .baseUrl, DOC_SE
-000002d0: 5353 494f 4e5f 5552 4c2c 2065 6e63 6f64  SSION_URL, encod
-000002e0: 6555 5249 436f 6d70 6f6e 656e 7428 7061  eURIComponent(pa
-000002f0: 7468 2929 3b0a 2020 2020 636f 6e73 7420  th));.    const 
-00000300: 626f 6479 203d 207b 0a20 2020 2020 2020  body = {.       
-00000310: 206d 6574 686f 643a 2027 5055 5427 2c0a   method: 'PUT',.
-00000320: 2020 2020 2020 2020 626f 6479 3a20 4a53          body: JS
-00000330: 4f4e 2e73 7472 696e 6769 6679 287b 2066  ON.stringify({ f
-00000340: 6f72 6d61 742c 2074 7970 6520 7d29 0a20  ormat, type }). 
-00000350: 2020 207d 3b0a 2020 2020 6c65 7420 7265     };.    let re
-00000360: 7370 6f6e 7365 3b0a 2020 2020 7472 7920  sponse;.    try 
-00000370: 7b0a 2020 2020 2020 2020 7265 7370 6f6e  {.        respon
-00000380: 7365 203d 2061 7761 6974 2053 6572 7665  se = await Serve
-00000390: 7243 6f6e 6e65 6374 696f 6e2e 6d61 6b65  rConnection.make
-000003a0: 5265 7175 6573 7428 7572 6c2c 2062 6f64  Request(url, bod
-000003b0: 792c 2073 6574 7469 6e67 7329 3b0a 2020  y, settings);.  
-000003c0: 2020 7d0a 2020 2020 6361 7463 6820 2865    }.    catch (e
-000003d0: 7272 6f72 2920 7b0a 2020 2020 2020 2020  rror) {.        
-000003e0: 7468 726f 7720 6e65 7720 5365 7276 6572  throw new Server
-000003f0: 436f 6e6e 6563 7469 6f6e 2e4e 6574 776f  Connection.Netwo
-00000400: 726b 4572 726f 7228 6572 726f 7229 3b0a  rkError(error);.
-00000410: 2020 2020 7d0a 2020 2020 6c65 7420 6461      }.    let da
-00000420: 7461 203d 2061 7761 6974 2072 6573 706f  ta = await respo
-00000430: 6e73 652e 7465 7874 2829 3b0a 2020 2020  nse.text();.    
-00000440: 6966 2028 6461 7461 2e6c 656e 6774 6820  if (data.length 
-00000450: 3e20 3029 207b 0a20 2020 2020 2020 2074  > 0) {.        t
-00000460: 7279 207b 0a20 2020 2020 2020 2020 2020  ry {.           
-00000470: 2064 6174 6120 3d20 4a53 4f4e 2e70 6172   data = JSON.par
-00000480: 7365 2864 6174 6129 3b0a 2020 2020 2020  se(data);.      
-00000490: 2020 7d0a 2020 2020 2020 2020 6361 7463    }.        catc
-000004a0: 6820 2865 7272 6f72 2920 7b0a 2020 2020  h (error) {.    
-000004b0: 2020 2020 2020 2020 636f 6e73 6f6c 652e          console.
-000004c0: 6c6f 6728 274e 6f74 2061 204a 534f 4e20  log('Not a JSON 
-000004d0: 7265 7370 6f6e 7365 2062 6f64 792e 272c  response body.',
-000004e0: 2072 6573 706f 6e73 6529 3b0a 2020 2020   response);.    
-000004f0: 2020 2020 7d0a 2020 2020 7d0a 2020 2020      }.    }.    
-00000500: 6966 2028 2172 6573 706f 6e73 652e 6f6b  if (!response.ok
-00000510: 2920 7b0a 2020 2020 2020 2020 7468 726f  ) {.        thro
-00000520: 7720 6e65 7720 5365 7276 6572 436f 6e6e  w new ServerConn
-00000530: 6563 7469 6f6e 2e52 6573 706f 6e73 6545  ection.ResponseE
-00000540: 7272 6f72 2872 6573 706f 6e73 652c 2064  rror(response, d
-00000550: 6174 612e 6d65 7373 6167 6520 7c7c 2064  ata.message || d
-00000560: 6174 6129 3b0a 2020 2020 7d0a 2020 2020  ata);.    }.    
-00000570: 7265 7475 726e 2064 6174 613b 0a7d 0a    return data;.}.
+00000100: 2d2d 2d2a 2f0a 0a69 6d70 6f72 7420 7b20  ---*/..import { 
+00000110: 5552 4c45 7874 207d 2066 726f 6d20 2740  URLExt } from '@
+00000120: 6a75 7079 7465 726c 6162 2f63 6f72 6575  jupyterlab/coreu
+00000130: 7469 6c73 273b 0a69 6d70 6f72 7420 7b20  tils';.import { 
+00000140: 5365 7276 6572 436f 6e6e 6563 7469 6f6e  ServerConnection
+00000150: 2c20 436f 6e74 656e 7473 207d 2066 726f  , Contents } fro
+00000160: 6d20 2740 6a75 7079 7465 726c 6162 2f73  m '@jupyterlab/s
+00000170: 6572 7669 6365 7327 3b0a 0a2f 2a2a 0a20  ervices';../**. 
+00000180: 2a20 446f 6375 6d65 6e74 2073 6573 7369  * Document sessi
+00000190: 6f6e 2065 6e64 706f 696e 7420 7072 6f76  on endpoint prov
+000001a0: 6964 6564 2062 7920 606a 7570 7974 6572  ided by `jupyter
+000001b0: 5f63 6f6c 6c61 626f 7261 7469 6f6e 600a  _collaboration`.
+000001c0: 202a 2053 6565 2068 7474 7073 3a2f 2f67   * See https://g
+000001d0: 6974 6875 622e 636f 6d2f 6a75 7079 7465  ithub.com/jupyte
+000001e0: 726c 6162 2f6a 7570 7974 6572 5f63 6f6c  rlab/jupyter_col
+000001f0: 6c61 626f 7261 7469 6f6e 0a20 2a2f 0a63  laboration. */.c
+00000200: 6f6e 7374 2044 4f43 5f53 4553 5349 4f4e  onst DOC_SESSION
+00000210: 5f55 524c 203d 2027 6170 692f 636f 6c6c  _URL = 'api/coll
+00000220: 6162 6f72 6174 696f 6e2f 7365 7373 696f  aboration/sessio
+00000230: 6e27 3b0a 0a2f 2a2a 0a20 2a20 446f 6375  n';../**. * Docu
+00000240: 6d65 6e74 2073 6573 7369 6f6e 206d 6f64  ment session mod
+00000250: 656c 0a20 2a2f 0a65 7870 6f72 7420 696e  el. */.export in
+00000260: 7465 7266 6163 6520 4953 6573 7369 6f6e  terface ISession
+00000270: 4d6f 6465 6c20 7b0a 2020 2f2a 2a0a 2020  Model {.  /**.  
+00000280: 202a 2044 6f63 756d 656e 7420 666f 726d   * Document form
+00000290: 6174 3b20 2774 6578 7427 2c20 2762 6173  at; 'text', 'bas
+000002a0: 6536 3427 2c2e 2e2e 0a20 2020 2a2f 0a20  e64',....   */. 
+000002b0: 2066 6f72 6d61 743a 2043 6f6e 7465 6e74   format: Content
+000002c0: 732e 4669 6c65 466f 726d 6174 3b0a 2020  s.FileFormat;.  
+000002d0: 2f2a 2a0a 2020 202a 2044 6f63 756d 656e  /**.   * Documen
+000002e0: 7420 7479 7065 0a20 2020 2a2f 0a20 2074  t type.   */.  t
+000002f0: 7970 653a 2043 6f6e 7465 6e74 732e 436f  ype: Contents.Co
+00000300: 6e74 656e 7454 7970 653b 0a20 202f 2a2a  ntentType;.  /**
+00000310: 0a20 2020 2a20 4669 6c65 2075 6e69 7175  .   * File uniqu
+00000320: 6520 6964 656e 7469 6669 6572 0a20 2020  e identifier.   
+00000330: 2a2f 0a20 2066 696c 6549 643a 2073 7472  */.  fileId: str
+00000340: 696e 673b 0a20 202f 2a2a 0a20 2020 2a20  ing;.  /**.   * 
+00000350: 5365 7276 6572 2073 6573 7369 6f6e 2069  Server session i
+00000360: 6465 6e74 6966 6965 720a 2020 202a 2f0a  dentifier.   */.
+00000370: 2020 7365 7373 696f 6e49 643a 2073 7472    sessionId: str
+00000380: 696e 673b 0a7d 0a0a 6578 706f 7274 2061  ing;.}..export a
+00000390: 7379 6e63 2066 756e 6374 696f 6e20 7265  sync function re
+000003a0: 7175 6573 7444 6f63 5365 7373 696f 6e28  questDocSession(
+000003b0: 0a20 2066 6f72 6d61 743a 2073 7472 696e  .  format: strin
+000003c0: 672c 0a20 2074 7970 653a 2073 7472 696e  g,.  type: strin
+000003d0: 672c 0a20 2070 6174 683a 2073 7472 696e  g,.  path: strin
+000003e0: 670a 293a 2050 726f 6d69 7365 3c49 5365  g.): Promise<ISe
+000003f0: 7373 696f 6e4d 6f64 656c 3e20 7b0a 2020  ssionModel> {.  
+00000400: 636f 6e73 7420 7365 7474 696e 6773 203d  const settings =
+00000410: 2053 6572 7665 7243 6f6e 6e65 6374 696f   ServerConnectio
+00000420: 6e2e 6d61 6b65 5365 7474 696e 6773 2829  n.makeSettings()
+00000430: 3b0a 2020 636f 6e73 7420 7572 6c20 3d20  ;.  const url = 
+00000440: 5552 4c45 7874 2e6a 6f69 6e28 0a20 2020  URLExt.join(.   
+00000450: 2073 6574 7469 6e67 732e 6261 7365 5572   settings.baseUr
+00000460: 6c2c 0a20 2020 2044 4f43 5f53 4553 5349  l,.    DOC_SESSI
+00000470: 4f4e 5f55 524c 2c0a 2020 2020 656e 636f  ON_URL,.    enco
+00000480: 6465 5552 4943 6f6d 706f 6e65 6e74 2870  deURIComponent(p
+00000490: 6174 6829 0a20 2029 3b0a 2020 636f 6e73  ath).  );.  cons
+000004a0: 7420 626f 6479 203d 207b 0a20 2020 206d  t body = {.    m
+000004b0: 6574 686f 643a 2027 5055 5427 2c0a 2020  ethod: 'PUT',.  
+000004c0: 2020 626f 6479 3a20 4a53 4f4e 2e73 7472    body: JSON.str
+000004d0: 696e 6769 6679 287b 2066 6f72 6d61 742c  ingify({ format,
+000004e0: 2074 7970 6520 7d29 0a20 207d 3b0a 0a20   type }).  };.. 
+000004f0: 206c 6574 2072 6573 706f 6e73 653a 2052   let response: R
+00000500: 6573 706f 6e73 653b 0a20 2074 7279 207b  esponse;.  try {
+00000510: 0a20 2020 2072 6573 706f 6e73 6520 3d20  .    response = 
+00000520: 6177 6169 7420 5365 7276 6572 436f 6e6e  await ServerConn
+00000530: 6563 7469 6f6e 2e6d 616b 6552 6571 7565  ection.makeReque
+00000540: 7374 2875 726c 2c20 626f 6479 2c20 7365  st(url, body, se
+00000550: 7474 696e 6773 293b 0a20 207d 2063 6174  ttings);.  } cat
+00000560: 6368 2028 6572 726f 7229 207b 0a20 2020  ch (error) {.   
+00000570: 2074 6872 6f77 206e 6577 2053 6572 7665   throw new Serve
+00000580: 7243 6f6e 6e65 6374 696f 6e2e 4e65 7477  rConnection.Netw
+00000590: 6f72 6b45 7272 6f72 2865 7272 6f72 2061  orkError(error a
+000005a0: 7320 4572 726f 7229 3b0a 2020 7d0a 0a20  s Error);.  }.. 
+000005b0: 206c 6574 2064 6174 613a 2061 6e79 203d   let data: any =
+000005c0: 2061 7761 6974 2072 6573 706f 6e73 652e   await response.
+000005d0: 7465 7874 2829 3b0a 0a20 2069 6620 2864  text();..  if (d
+000005e0: 6174 612e 6c65 6e67 7468 203e 2030 2920  ata.length > 0) 
+000005f0: 7b0a 2020 2020 7472 7920 7b0a 2020 2020  {.    try {.    
+00000600: 2020 6461 7461 203d 204a 534f 4e2e 7061    data = JSON.pa
+00000610: 7273 6528 6461 7461 293b 0a20 2020 207d  rse(data);.    }
+00000620: 2063 6174 6368 2028 6572 726f 7229 207b   catch (error) {
+00000630: 0a20 2020 2020 2063 6f6e 736f 6c65 2e6c  .      console.l
+00000640: 6f67 2827 4e6f 7420 6120 4a53 4f4e 2072  og('Not a JSON r
+00000650: 6573 706f 6e73 6520 626f 6479 2e27 2c20  esponse body.', 
+00000660: 7265 7370 6f6e 7365 293b 0a20 2020 207d  response);.    }
+00000670: 0a20 207d 0a0a 2020 6966 2028 2172 6573  .  }..  if (!res
+00000680: 706f 6e73 652e 6f6b 2920 7b0a 2020 2020  ponse.ok) {.    
+00000690: 7468 726f 7720 6e65 7720 5365 7276 6572  throw new Server
+000006a0: 436f 6e6e 6563 7469 6f6e 2e52 6573 706f  Connection.Respo
+000006b0: 6e73 6545 7272 6f72 2872 6573 706f 6e73  nseError(respons
+000006c0: 652c 2064 6174 612e 6d65 7373 6167 6520  e, data.message 
+000006d0: 7c7c 2064 6174 6129 3b0a 2020 7d0a 0a20  || data);.  }.. 
+000006e0: 2072 6574 7572 6e20 6461 7461 3b0a 7d0a   return data;.}.
```

### Comparing `jupyter_collaboration_ui-1.0.0a0/packages/docprovider/lib/tokens.d.ts` & `jupyter_collaboration_ui-1.0.0a1/packages/docprovider/src/tokens.ts`

 * *Files 18% similar despite different names*

```diff
@@ -1,50 +1,68 @@
+// Copyright (c) Jupyter Development Team.
+// Distributed under the terms of the Modified BSD License.
+
 import { DocumentChange, YDocument } from '@jupyter/ydoc';
 import { Contents } from '@jupyterlab/services';
+
 import { Token } from '@lumino/coreutils';
 import { IStream } from '@lumino/signaling';
+
 import { IChatMessage } from './awareness';
+
 /**
  * The collaborative drive.
  */
-export declare const ICollaborativeDrive: Token<ICollaborativeDrive>;
+export const ICollaborativeDrive = new Token<ICollaborativeDrive>(
+  '@jupyter/collaboration-extension:ICollaborativeDrive'
+);
+
 /**
  * A document factory for registering shared models
  */
-export type SharedDocumentFactory = (options: Contents.ISharedFactoryOptions) => YDocument<DocumentChange>;
+export type SharedDocumentFactory = (
+  options: Contents.ISharedFactoryOptions
+) => YDocument<DocumentChange>;
+
 /**
  * A Collaborative implementation for an `IDrive`, talking to the
  * server using the Jupyter REST API and a WebSocket connection.
  */
 export interface ICollaborativeDrive extends Contents.IDrive {
-    /**
-     * SharedModel factory for the YDrive.
-     */
-    readonly sharedModelFactory: ISharedModelFactory;
+  /**
+   * SharedModel factory for the YDrive.
+   */
+  readonly sharedModelFactory: ISharedModelFactory;
 }
+
 /**
  * Yjs sharedModel factory for real-time collaboration.
  */
 export interface ISharedModelFactory extends Contents.ISharedFactory {
-    /**
-     * Register a SharedDocumentFactory.
-     *
-     * @param type Document type
-     * @param factory Document factory
-     */
-    registerDocumentFactory(type: Contents.ContentType, factory: SharedDocumentFactory): void;
+  /**
+   * Register a SharedDocumentFactory.
+   *
+   * @param type Document type
+   * @param factory Document factory
+   */
+  registerDocumentFactory(
+    type: Contents.ContentType,
+    factory: SharedDocumentFactory
+  ): void;
 }
+
 /**
  * A provider interface for global awareness features.
  */
 export interface IAwarenessProvider {
-    /**
-     * A signal to subscribe for incoming messages.
-     */
-    readonly messageStream: IStream<this, IChatMessage>;
-    /**
-     * Send a message to every collaborator.
-     *
-     * @param msg message
-     */
-    sendMessage(msg: string): void;
+  /**
+   * A signal to subscribe for incoming messages.
+   */
+  readonly messageStream: IStream<this, IChatMessage>;
+
+  /**
+   * Send a message to every collaborator.
+   *
+   * @param msg message
+   */
+  sendMessage(msg: string): void;
 }
```

### Comparing `jupyter_collaboration_ui-1.0.0a0/packages/docprovider/src/awareness.ts` & `jupyter_collaboration_ui-1.0.0a1/packages/docprovider/src/awareness.ts`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration_ui-1.0.0a0/packages/docprovider/src/ydrive.ts` & `jupyter_collaboration_ui-1.0.0a1/packages/docprovider/src/ydrive.ts`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration_ui-1.0.0a0/packages/docprovider/src/yprovider.ts` & `jupyter_collaboration_ui-1.0.0a1/packages/docprovider/src/yprovider.ts`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/lib/executor.js` & `jupyter_collaboration_ui-1.0.0a1/packages/docprovider-extension/src/executor.ts`

 * *Files 18% similar despite different names*

```diff
@@ -4,139 +4,141 @@
 00000030: 7374 7269 6275 7465 6420 756e 6465 7220  stributed under 
 00000040: 7468 6520 7465 726d 7320 6f66 2074 6865  the terms of the
 00000050: 204d 6f64 6966 6965 6420 4253 4420 4c69   Modified BSD Li
 00000060: 6365 6e73 652e 0a2f 2a2a 0a20 2a20 4070  cense../**. * @p
 00000070: 6163 6b61 6765 446f 6375 6d65 6e74 6174  ackageDocumentat
 00000080: 696f 6e0a 202a 2040 6d6f 6475 6c65 2064  ion. * @module d
 00000090: 6f63 7072 6f76 6964 6572 2d65 7874 656e  ocprovider-exten
-000000a0: 7369 6f6e 0a20 2a2f 0a69 6d70 6f72 7420  sion. */.import 
-000000b0: 7b20 5061 6765 436f 6e66 6967 2c20 5552  { PageConfig, UR
-000000c0: 4c45 7874 207d 2066 726f 6d20 2740 6a75  LExt } from '@ju
-000000d0: 7079 7465 726c 6162 2f63 6f72 6575 7469  pyterlab/coreuti
-000000e0: 6c73 273b 0a69 6d70 6f72 7420 7b20 5365  ls';.import { Se
-000000f0: 7276 6572 436f 6e6e 6563 7469 6f6e 207d  rverConnection }
-00000100: 2066 726f 6d20 2740 6a75 7079 7465 726c   from '@jupyterl
-00000110: 6162 2f73 6572 7669 6365 7327 3b0a 696d  ab/services';.im
-00000120: 706f 7274 207b 2049 4e6f 7465 626f 6f6b  port { INotebook
-00000130: 4365 6c6c 4578 6563 7574 6f72 2c20 7275  CellExecutor, ru
-00000140: 6e43 656c 6c20 7d20 6672 6f6d 2027 406a  nCell } from '@j
-00000150: 7570 7974 6572 6c61 622f 6e6f 7465 626f  upyterlab/notebo
-00000160: 6f6b 273b 0a65 7870 6f72 7420 636f 6e73  ok';.export cons
-00000170: 7420 6e6f 7465 626f 6f6b 4365 6c6c 4578  t notebookCellEx
-00000180: 6563 7574 6f72 203d 207b 0a20 2020 2069  ecutor = {.    i
-00000190: 643a 2027 406a 7570 7974 6572 2f64 6f63  d: '@jupyter/doc
-000001a0: 7072 6f76 6964 6572 2d65 7874 656e 7369  provider-extensi
-000001b0: 6f6e 3a6e 6f74 6562 6f6f 6b2d 6365 6c6c  on:notebook-cell
-000001c0: 2d65 7865 6375 746f 7227 2c0a 2020 2020  -executor',.    
-000001d0: 6465 7363 7269 7074 696f 6e3a 2027 4164  description: 'Ad
-000001e0: 6420 6e6f 7465 626f 6f6b 2063 656c 6c20  d notebook cell 
-000001f0: 6578 6563 7574 6f72 2074 6861 7420 7573  executor that us
-00000200: 6573 2052 4553 5420 4150 4920 696e 7374  es REST API inst
-00000210: 6561 6420 6f66 206b 6572 6e65 6c20 7072  ead of kernel pr
-00000220: 6f74 6f63 6f6c 206f 7665 7220 5765 6253  otocol over WebS
-00000230: 6f63 6b65 742e 272c 0a20 2020 2061 7574  ocket.',.    aut
-00000240: 6f53 7461 7274 3a20 7472 7565 2c0a 2020  oStart: true,.  
-00000250: 2020 7072 6f76 6964 6573 3a20 494e 6f74    provides: INot
-00000260: 6562 6f6f 6b43 656c 6c45 7865 6375 746f  ebookCellExecuto
-00000270: 722c 0a20 2020 2061 6374 6976 6174 653a  r,.    activate:
-00000280: 2028 6170 7029 203d 3e20 7b0a 2020 2020   (app) => {.    
-00000290: 2020 2020 6966 2028 5061 6765 436f 6e66      if (PageConf
-000002a0: 6967 2e67 6574 4f70 7469 6f6e 2827 7365  ig.getOption('se
-000002b0: 7276 6572 5369 6465 4578 6563 7574 696f  rverSideExecutio
-000002c0: 6e27 2920 3d3d 3d20 2774 7275 6527 2920  n') === 'true') 
-000002d0: 7b0a 2020 2020 2020 2020 2020 2020 7265  {.            re
-000002e0: 7475 726e 204f 626a 6563 742e 6672 6565  turn Object.free
-000002f0: 7a65 287b 2072 756e 4365 6c6c 3a20 7275  ze({ runCell: ru
-00000300: 6e43 656c 6c53 6572 7665 7253 6964 6520  nCellServerSide 
-00000310: 7d29 3b0a 2020 2020 2020 2020 7d0a 2020  });.        }.  
-00000320: 2020 2020 2020 7265 7475 726e 204f 626a        return Obj
-00000330: 6563 742e 6672 6565 7a65 287b 2072 756e  ect.freeze({ run
-00000340: 4365 6c6c 207d 293b 0a20 2020 207d 0a7d  Cell });.    }.}
-00000350: 3b0a 6173 796e 6320 6675 6e63 7469 6f6e  ;.async function
-00000360: 2072 756e 4365 6c6c 5365 7276 6572 5369   runCellServerSi
-00000370: 6465 287b 2063 656c 6c2c 206e 6f74 6562  de({ cell, noteb
-00000380: 6f6f 6b2c 206e 6f74 6562 6f6f 6b43 6f6e  ook, notebookCon
-00000390: 6669 672c 206f 6e43 656c 6c45 7865 6375  fig, onCellExecu
-000003a0: 7465 642c 206f 6e43 656c 6c45 7865 6375  ted, onCellExecu
-000003b0: 7469 6f6e 5363 6865 6475 6c65 642c 2073  tionScheduled, s
-000003c0: 6573 7369 6f6e 436f 6e74 6578 742c 2073  essionContext, s
-000003d0: 6573 7369 6f6e 4469 616c 6f67 732c 2074  essionDialogs, t
-000003e0: 7261 6e73 6c61 746f 7220 7d29 207b 0a20  ranslator }) {. 
-000003f0: 2020 2076 6172 205f 612c 205f 623b 0a20     var _a, _b;. 
-00000400: 2020 2073 7769 7463 6820 2863 656c 6c2e     switch (cell.
-00000410: 6d6f 6465 6c2e 7479 7065 2920 7b0a 2020  model.type) {.  
-00000420: 2020 2020 2020 6361 7365 2027 6d61 726b        case 'mark
-00000430: 646f 776e 273a 0a20 2020 2020 2020 2020  down':.         
-00000440: 2020 2063 656c 6c2e 7265 6e64 6572 6564     cell.rendered
-00000450: 203d 2074 7275 653b 0a20 2020 2020 2020   = true;.       
-00000460: 2020 2020 2063 656c 6c2e 696e 7075 7448       cell.inputH
-00000470: 6964 6465 6e20 3d20 6661 6c73 653b 0a20  idden = false;. 
-00000480: 2020 2020 2020 2020 2020 206f 6e43 656c             onCel
-00000490: 6c45 7865 6375 7465 6428 7b20 6365 6c6c  lExecuted({ cell
-000004a0: 2c20 7375 6363 6573 733a 2074 7275 6520  , success: true 
-000004b0: 7d29 3b0a 2020 2020 2020 2020 2020 2020  });.            
-000004c0: 6272 6561 6b3b 0a20 2020 2020 2020 2063  break;.        c
-000004d0: 6173 6520 2763 6f64 6527 3a20 7b0a 2020  ase 'code': {.  
-000004e0: 2020 2020 2020 2020 2020 636f 6e73 7420            const 
-000004f0: 6b65 726e 656c 4964 203d 2028 5f62 203d  kernelId = (_b =
-00000500: 2028 5f61 203d 2073 6573 7369 6f6e 436f   (_a = sessionCo
-00000510: 6e74 6578 7420 3d3d 3d20 6e75 6c6c 207c  ntext === null |
-00000520: 7c20 7365 7373 696f 6e43 6f6e 7465 7874  | sessionContext
-00000530: 203d 3d3d 2076 6f69 6420 3020 3f20 766f   === void 0 ? vo
-00000540: 6964 2030 203a 2073 6573 7369 6f6e 436f  id 0 : sessionCo
-00000550: 6e74 6578 742e 7365 7373 696f 6e29 203d  ntext.session) =
-00000560: 3d3d 206e 756c 6c20 7c7c 205f 6120 3d3d  == null || _a ==
-00000570: 3d20 766f 6964 2030 203f 2076 6f69 6420  = void 0 ? void 
-00000580: 3020 3a20 5f61 2e6b 6572 6e65 6c29 203d  0 : _a.kernel) =
-00000590: 3d3d 206e 756c 6c20 7c7c 205f 6220 3d3d  == null || _b ==
-000005a0: 3d20 766f 6964 2030 203f 2076 6f69 6420  = void 0 ? void 
-000005b0: 3020 3a20 5f62 2e69 643b 0a20 2020 2020  0 : _b.id;.     
-000005c0: 2020 2020 2020 2063 6f6e 7374 2073 6574         const set
-000005d0: 7469 6e67 7320 3d20 5365 7276 6572 436f  tings = ServerCo
-000005e0: 6e6e 6563 7469 6f6e 2e6d 616b 6553 6574  nnection.makeSet
-000005f0: 7469 6e67 7328 293b 0a20 2020 2020 2020  tings();.       
-00000600: 2020 2020 2063 6f6e 7374 2061 7069 5552       const apiUR
-00000610: 4c20 3d20 5552 4c45 7874 2e6a 6f69 6e28  L = URLExt.join(
-00000620: 7365 7474 696e 6773 2e62 6173 6555 726c  settings.baseUrl
-00000630: 2c20 6061 7069 2f6b 6572 6e65 6c73 2f24  , `api/kernels/$
-00000640: 7b6b 6572 6e65 6c49 647d 2f65 7865 6375  {kernelId}/execu
-00000650: 7465 6029 3b0a 2020 2020 2020 2020 2020  te`);.          
-00000660: 2020 636f 6e73 7420 6365 6c6c 4964 203d    const cellId =
-00000670: 2063 656c 6c2e 6d6f 6465 6c2e 7368 6172   cell.model.shar
-00000680: 6564 4d6f 6465 6c2e 6765 7449 6428 293b  edModel.getId();
-00000690: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
-000006a0: 7374 2064 6f63 756d 656e 7449 6420 3d20  st documentId = 
-000006b0: 606a 736f 6e3a 6e6f 7465 626f 6f6b 3a24  `json:notebook:$
-000006c0: 7b6e 6f74 6562 6f6f 6b2e 7368 6172 6564  {notebook.shared
-000006d0: 4d6f 6465 6c2e 6765 7453 7461 7465 2827  Model.getState('
-000006e0: 6669 6c65 5f69 6427 297d 603b 0a20 2020  file_id')}`;.   
-000006f0: 2020 2020 2020 2020 2063 6f6e 7374 2062           const b
-00000700: 6f64 7920 3d20 607b 2263 656c 6c5f 6964  ody = `{"cell_id
-00000710: 223a 2224 7b63 656c 6c49 647d 222c 2264  ":"${cellId}","d
-00000720: 6f63 756d 656e 745f 6964 223a 2224 7b64  ocument_id":"${d
-00000730: 6f63 756d 656e 7449 647d 227d 603b 0a20  ocumentId}"}`;. 
-00000740: 2020 2020 2020 2020 2020 2063 6f6e 7374             const
-00000750: 2069 6e69 7420 3d20 7b0a 2020 2020 2020   init = {.      
-00000760: 2020 2020 2020 2020 2020 6d65 7468 6f64            method
-00000770: 3a20 2750 4f53 5427 2c0a 2020 2020 2020  : 'POST',.      
-00000780: 2020 2020 2020 2020 2020 626f 6479 0a20            body. 
-00000790: 2020 2020 2020 2020 2020 207d 3b0a 2020             };.  
-000007a0: 2020 2020 2020 2020 2020 7472 7920 7b0a            try {.
-000007b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000007c0: 6177 6169 7420 5365 7276 6572 436f 6e6e  await ServerConn
-000007d0: 6563 7469 6f6e 2e6d 616b 6552 6571 7565  ection.makeReque
-000007e0: 7374 2861 7069 5552 4c2c 2069 6e69 742c  st(apiURL, init,
-000007f0: 2073 6574 7469 6e67 7329 3b0a 2020 2020   settings);.    
-00000800: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-00000810: 2020 2020 2020 6361 7463 6820 2865 7272        catch (err
-00000820: 6f72 2920 7b0a 2020 2020 2020 2020 2020  or) {.          
-00000830: 2020 2020 2020 7468 726f 7720 6e65 7720        throw new 
-00000840: 5365 7276 6572 436f 6e6e 6563 7469 6f6e  ServerConnection
-00000850: 2e4e 6574 776f 726b 4572 726f 7228 6572  .NetworkError(er
-00000860: 726f 7229 3b0a 2020 2020 2020 2020 2020  ror);.          
-00000870: 2020 7d0a 2020 2020 2020 2020 2020 2020    }.            
-00000880: 6272 6561 6b3b 0a20 2020 2020 2020 207d  break;.        }
-00000890: 0a20 2020 2020 2020 2064 6566 6175 6c74  .        default
-000008a0: 3a0a 2020 2020 2020 2020 2020 2020 6272  :.            br
-000008b0: 6561 6b3b 0a20 2020 207d 0a20 2020 2072  eak;.    }.    r
-000008c0: 6574 7572 6e20 5072 6f6d 6973 652e 7265  eturn Promise.re
-000008d0: 736f 6c76 6528 7472 7565 293b 0a7d 0a    solve(true);.}.
+000000a0: 7369 6f6e 0a20 2a2f 0a0a 696d 706f 7274  sion. */..import
+000000b0: 207b 0a20 204a 7570 7974 6572 4672 6f6e   {.  JupyterFron
+000000c0: 7445 6e64 2c0a 2020 4a75 7079 7465 7246  tEnd,.  JupyterF
+000000d0: 726f 6e74 456e 6450 6c75 6769 6e0a 7d20  rontEndPlugin.} 
+000000e0: 6672 6f6d 2027 406a 7570 7974 6572 6c61  from '@jupyterla
+000000f0: 622f 6170 706c 6963 6174 696f 6e27 3b0a  b/application';.
+00000100: 696d 706f 7274 207b 2050 6167 6543 6f6e  import { PageCon
+00000110: 6669 672c 2055 524c 4578 7420 7d20 6672  fig, URLExt } fr
+00000120: 6f6d 2027 406a 7570 7974 6572 6c61 622f  om '@jupyterlab/
+00000130: 636f 7265 7574 696c 7327 3b0a 696d 706f  coreutils';.impo
+00000140: 7274 207b 2053 6572 7665 7243 6f6e 6e65  rt { ServerConne
+00000150: 6374 696f 6e20 7d20 6672 6f6d 2027 406a  ction } from '@j
+00000160: 7570 7974 6572 6c61 622f 7365 7276 6963  upyterlab/servic
+00000170: 6573 273b 0a0a 696d 706f 7274 207b 2074  es';..import { t
+00000180: 7970 6520 4d61 726b 646f 776e 4365 6c6c  ype MarkdownCell
+00000190: 207d 2066 726f 6d20 2740 6a75 7079 7465   } from '@jupyte
+000001a0: 726c 6162 2f63 656c 6c73 273b 0a69 6d70  rlab/cells';.imp
+000001b0: 6f72 7420 7b20 494e 6f74 6562 6f6f 6b43  ort { INotebookC
+000001c0: 656c 6c45 7865 6375 746f 722c 2072 756e  ellExecutor, run
+000001d0: 4365 6c6c 207d 2066 726f 6d20 2740 6a75  Cell } from '@ju
+000001e0: 7079 7465 726c 6162 2f6e 6f74 6562 6f6f  pyterlab/noteboo
+000001f0: 6b27 3b0a 0a65 7870 6f72 7420 636f 6e73  k';..export cons
+00000200: 7420 6e6f 7465 626f 6f6b 4365 6c6c 4578  t notebookCellEx
+00000210: 6563 7574 6f72 3a20 4a75 7079 7465 7246  ecutor: JupyterF
+00000220: 726f 6e74 456e 6450 6c75 6769 6e3c 494e  rontEndPlugin<IN
+00000230: 6f74 6562 6f6f 6b43 656c 6c45 7865 6375  otebookCellExecu
+00000240: 746f 723e 203d 0a20 207b 0a20 2020 2069  tor> =.  {.    i
+00000250: 643a 2027 406a 7570 7974 6572 2f64 6f63  d: '@jupyter/doc
+00000260: 7072 6f76 6964 6572 2d65 7874 656e 7369  provider-extensi
+00000270: 6f6e 3a6e 6f74 6562 6f6f 6b2d 6365 6c6c  on:notebook-cell
+00000280: 2d65 7865 6375 746f 7227 2c0a 2020 2020  -executor',.    
+00000290: 6465 7363 7269 7074 696f 6e3a 0a20 2020  description:.   
+000002a0: 2020 2027 4164 6420 6e6f 7465 626f 6f6b     'Add notebook
+000002b0: 2063 656c 6c20 6578 6563 7574 6f72 2074   cell executor t
+000002c0: 6861 7420 7573 6573 2052 4553 5420 4150  hat uses REST AP
+000002d0: 4920 696e 7374 6561 6420 6f66 206b 6572  I instead of ker
+000002e0: 6e65 6c20 7072 6f74 6f63 6f6c 206f 7665  nel protocol ove
+000002f0: 7220 5765 6253 6f63 6b65 742e 272c 0a20  r WebSocket.',. 
+00000300: 2020 2061 7574 6f53 7461 7274 3a20 7472     autoStart: tr
+00000310: 7565 2c0a 2020 2020 7072 6f76 6964 6573  ue,.    provides
+00000320: 3a20 494e 6f74 6562 6f6f 6b43 656c 6c45  : INotebookCellE
+00000330: 7865 6375 746f 722c 0a20 2020 2061 6374  xecutor,.    act
+00000340: 6976 6174 653a 2028 6170 703a 204a 7570  ivate: (app: Jup
+00000350: 7974 6572 4672 6f6e 7445 6e64 293a 2049  yterFrontEnd): I
+00000360: 4e6f 7465 626f 6f6b 4365 6c6c 4578 6563  NotebookCellExec
+00000370: 7574 6f72 203d 3e20 7b0a 2020 2020 2020  utor => {.      
+00000380: 6966 2028 5061 6765 436f 6e66 6967 2e67  if (PageConfig.g
+00000390: 6574 4f70 7469 6f6e 2827 7365 7276 6572  etOption('server
+000003a0: 5369 6465 4578 6563 7574 696f 6e27 2920  SideExecution') 
+000003b0: 3d3d 3d20 2774 7275 6527 2920 7b0a 2020  === 'true') {.  
+000003c0: 2020 2020 2020 7265 7475 726e 204f 626a        return Obj
+000003d0: 6563 742e 6672 6565 7a65 287b 2072 756e  ect.freeze({ run
+000003e0: 4365 6c6c 3a20 7275 6e43 656c 6c53 6572  Cell: runCellSer
+000003f0: 7665 7253 6964 6520 7d29 3b0a 2020 2020  verSide });.    
+00000400: 2020 7d0a 2020 2020 2020 7265 7475 726e    }.      return
+00000410: 204f 626a 6563 742e 6672 6565 7a65 287b   Object.freeze({
+00000420: 2072 756e 4365 6c6c 207d 293b 0a20 2020   runCell });.   
+00000430: 207d 0a20 207d 3b0a 0a61 7379 6e63 2066   }.  };..async f
+00000440: 756e 6374 696f 6e20 7275 6e43 656c 6c53  unction runCellS
+00000450: 6572 7665 7253 6964 6528 7b0a 2020 6365  erverSide({.  ce
+00000460: 6c6c 2c0a 2020 6e6f 7465 626f 6f6b 2c0a  ll,.  notebook,.
+00000470: 2020 6e6f 7465 626f 6f6b 436f 6e66 6967    notebookConfig
+00000480: 2c0a 2020 6f6e 4365 6c6c 4578 6563 7574  ,.  onCellExecut
+00000490: 6564 2c0a 2020 6f6e 4365 6c6c 4578 6563  ed,.  onCellExec
+000004a0: 7574 696f 6e53 6368 6564 756c 6564 2c0a  utionScheduled,.
+000004b0: 2020 7365 7373 696f 6e43 6f6e 7465 7874    sessionContext
+000004c0: 2c0a 2020 7365 7373 696f 6e44 6961 6c6f  ,.  sessionDialo
+000004d0: 6773 2c0a 2020 7472 616e 736c 6174 6f72  gs,.  translator
+000004e0: 0a7d 3a20 494e 6f74 6562 6f6f 6b43 656c  .}: INotebookCel
+000004f0: 6c45 7865 6375 746f 722e 4952 756e 4365  lExecutor.IRunCe
+00000500: 6c6c 4f70 7469 6f6e 7329 3a20 5072 6f6d  llOptions): Prom
+00000510: 6973 653c 626f 6f6c 6561 6e3e 207b 0a20  ise<boolean> {. 
+00000520: 2073 7769 7463 6820 2863 656c 6c2e 6d6f   switch (cell.mo
+00000530: 6465 6c2e 7479 7065 2920 7b0a 2020 2020  del.type) {.    
+00000540: 6361 7365 2027 6d61 726b 646f 776e 273a  case 'markdown':
+00000550: 0a20 2020 2020 2028 6365 6c6c 2061 7320  .      (cell as 
+00000560: 4d61 726b 646f 776e 4365 6c6c 292e 7265  MarkdownCell).re
+00000570: 6e64 6572 6564 203d 2074 7275 653b 0a20  ndered = true;. 
+00000580: 2020 2020 2063 656c 6c2e 696e 7075 7448       cell.inputH
+00000590: 6964 6465 6e20 3d20 6661 6c73 653b 0a20  idden = false;. 
+000005a0: 2020 2020 206f 6e43 656c 6c45 7865 6375       onCellExecu
+000005b0: 7465 6428 7b20 6365 6c6c 2c20 7375 6363  ted({ cell, succ
+000005c0: 6573 733a 2074 7275 6520 7d29 3b0a 2020  ess: true });.  
+000005d0: 2020 2020 6272 6561 6b3b 0a20 2020 2063      break;.    c
+000005e0: 6173 6520 2763 6f64 6527 3a20 7b0a 2020  ase 'code': {.  
+000005f0: 2020 2020 636f 6e73 7420 6b65 726e 656c      const kernel
+00000600: 4964 203d 2073 6573 7369 6f6e 436f 6e74  Id = sessionCont
+00000610: 6578 743f 2e73 6573 7369 6f6e 3f2e 6b65  ext?.session?.ke
+00000620: 726e 656c 3f2e 6964 3b0a 2020 2020 2020  rnel?.id;.      
+00000630: 636f 6e73 7420 7365 7474 696e 6773 203d  const settings =
+00000640: 2053 6572 7665 7243 6f6e 6e65 6374 696f   ServerConnectio
+00000650: 6e2e 6d61 6b65 5365 7474 696e 6773 2829  n.makeSettings()
+00000660: 3b0a 2020 2020 2020 636f 6e73 7420 6170  ;.      const ap
+00000670: 6955 524c 203d 2055 524c 4578 742e 6a6f  iURL = URLExt.jo
+00000680: 696e 280a 2020 2020 2020 2020 7365 7474  in(.        sett
+00000690: 696e 6773 2e62 6173 6555 726c 2c0a 2020  ings.baseUrl,.  
+000006a0: 2020 2020 2020 6061 7069 2f6b 6572 6e65        `api/kerne
+000006b0: 6c73 2f24 7b6b 6572 6e65 6c49 647d 2f65  ls/${kernelId}/e
+000006c0: 7865 6375 7465 600a 2020 2020 2020 293b  xecute`.      );
+000006d0: 0a20 2020 2020 2063 6f6e 7374 2063 656c  .      const cel
+000006e0: 6c49 6420 3d20 6365 6c6c 2e6d 6f64 656c  lId = cell.model
+000006f0: 2e73 6861 7265 644d 6f64 656c 2e67 6574  .sharedModel.get
+00000700: 4964 2829 3b0a 2020 2020 2020 636f 6e73  Id();.      cons
+00000710: 7420 646f 6375 6d65 6e74 4964 203d 2060  t documentId = `
+00000720: 6a73 6f6e 3a6e 6f74 6562 6f6f 6b3a 247b  json:notebook:${
+00000730: 6e6f 7465 626f 6f6b 2e73 6861 7265 644d  notebook.sharedM
+00000740: 6f64 656c 2e67 6574 5374 6174 6528 0a20  odel.getState(. 
+00000750: 2020 2020 2020 2027 6669 6c65 5f69 6427         'file_id'
+00000760: 0a20 2020 2020 2029 7d60 3b0a 2020 2020  .      )}`;.    
+00000770: 2020 636f 6e73 7420 626f 6479 203d 2060    const body = `
+00000780: 7b22 6365 6c6c 5f69 6422 3a22 247b 6365  {"cell_id":"${ce
+00000790: 6c6c 4964 7d22 2c22 646f 6375 6d65 6e74  llId}","document
+000007a0: 5f69 6422 3a22 247b 646f 6375 6d65 6e74  _id":"${document
+000007b0: 4964 7d22 7d60 3b0a 2020 2020 2020 636f  Id}"}`;.      co
+000007c0: 6e73 7420 696e 6974 203d 207b 0a20 2020  nst init = {.   
+000007d0: 2020 2020 206d 6574 686f 643a 2027 504f       method: 'PO
+000007e0: 5354 272c 0a20 2020 2020 2020 2062 6f64  ST',.        bod
+000007f0: 790a 2020 2020 2020 7d3b 0a20 2020 2020  y.      };.     
+00000800: 2074 7279 207b 0a20 2020 2020 2020 2061   try {.        a
+00000810: 7761 6974 2053 6572 7665 7243 6f6e 6e65  wait ServerConne
+00000820: 6374 696f 6e2e 6d61 6b65 5265 7175 6573  ction.makeReques
+00000830: 7428 6170 6955 524c 2c20 696e 6974 2c20  t(apiURL, init, 
+00000840: 7365 7474 696e 6773 293b 0a20 2020 2020  settings);.     
+00000850: 207d 2063 6174 6368 2028 6572 726f 723a   } catch (error:
+00000860: 2061 6e79 2920 7b0a 2020 2020 2020 2020   any) {.        
+00000870: 7468 726f 7720 6e65 7720 5365 7276 6572  throw new Server
+00000880: 436f 6e6e 6563 7469 6f6e 2e4e 6574 776f  Connection.Netwo
+00000890: 726b 4572 726f 7228 6572 726f 7229 3b0a  rkError(error);.
+000008a0: 2020 2020 2020 7d0a 2020 2020 2020 6272        }.      br
+000008b0: 6561 6b3b 0a20 2020 207d 0a20 2020 2064  eak;.    }.    d
+000008c0: 6566 6175 6c74 3a0a 2020 2020 2020 6272  efault:.      br
+000008d0: 6561 6b3b 0a20 207d 0a20 2072 6574 7572  eak;.  }.  retur
+000008e0: 6e20 5072 6f6d 6973 652e 7265 736f 6c76  n Promise.resolv
+000008f0: 6528 7472 7565 293b 0a7d 0a              e(true);.}.
```

### Comparing `jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/lib/filebrowser.js` & `jupyter_collaboration_ui-1.0.0a1/packages/docprovider-extension/src/filebrowser.ts`

 * *Files 16% similar despite different names*

```diff
@@ -1,606 +1,591 @@
 00000000: 2f2a 0a20 2a20 436f 7079 7269 6768 7420  /*. * Copyright 
 00000010: 2863 2920 4a75 7079 7465 7220 4465 7665  (c) Jupyter Deve
 00000020: 6c6f 706d 656e 7420 5465 616d 2e0a 202a  lopment Team.. *
 00000030: 2044 6973 7472 6962 7574 6564 2075 6e64   Distributed und
 00000040: 6572 2074 6865 2074 6572 6d73 206f 6620  er the terms of 
 00000050: 7468 6520 4d6f 6469 6669 6564 2042 5344  the Modified BSD
-00000060: 204c 6963 656e 7365 2e0a 202a 2f0a 696d   License.. */.im
-00000070: 706f 7274 207b 2049 4c61 6253 6865 6c6c  port { ILabShell
-00000080: 2c20 4952 6f75 7465 722c 204a 7570 7974  , IRouter, Jupyt
-00000090: 6572 4672 6f6e 7445 6e64 207d 2066 726f  erFrontEnd } fro
-000000a0: 6d20 2740 6a75 7079 7465 726c 6162 2f61  m '@jupyterlab/a
-000000b0: 7070 6c69 6361 7469 6f6e 273b 0a69 6d70  pplication';.imp
-000000c0: 6f72 7420 7b20 4469 616c 6f67 2c20 7368  ort { Dialog, sh
-000000d0: 6f77 4469 616c 6f67 207d 2066 726f 6d20  owDialog } from 
-000000e0: 2740 6a75 7079 7465 726c 6162 2f61 7070  '@jupyterlab/app
-000000f0: 7574 696c 7327 3b0a 696d 706f 7274 207b  utils';.import {
-00000100: 2049 4465 6661 756c 7446 696c 6542 726f   IDefaultFileBro
-00000110: 7773 6572 2c20 4946 696c 6542 726f 7773  wser, IFileBrows
-00000120: 6572 4661 6374 6f72 7920 7d20 6672 6f6d  erFactory } from
-00000130: 2027 406a 7570 7974 6572 6c61 622f 6669   '@jupyterlab/fi
-00000140: 6c65 6272 6f77 7365 7227 3b0a 696d 706f  lebrowser';.impo
-00000150: 7274 207b 2049 4564 6974 6f72 5472 6163  rt { IEditorTrac
-00000160: 6b65 7220 7d20 6672 6f6d 2027 406a 7570  ker } from '@jup
-00000170: 7974 6572 6c61 622f 6669 6c65 6564 6974  yterlab/fileedit
-00000180: 6f72 273b 0a69 6d70 6f72 7420 7b20 494c  or';.import { IL
-00000190: 6f67 6765 7252 6567 6973 7472 7920 7d20  oggerRegistry } 
-000001a0: 6672 6f6d 2027 406a 7570 7974 6572 6c61  from '@jupyterla
-000001b0: 622f 6c6f 6763 6f6e 736f 6c65 273b 0a69  b/logconsole';.i
-000001c0: 6d70 6f72 7420 7b20 494e 6f74 6562 6f6f  mport { INoteboo
-000001d0: 6b54 7261 636b 6572 207d 2066 726f 6d20  kTracker } from 
-000001e0: 2740 6a75 7079 7465 726c 6162 2f6e 6f74  '@jupyterlab/not
-000001f0: 6562 6f6f 6b27 3b0a 696d 706f 7274 207b  ebook';.import {
-00000200: 2049 5365 7474 696e 6752 6567 6973 7472   ISettingRegistr
-00000210: 7920 7d20 6672 6f6d 2027 406a 7570 7974  y } from '@jupyt
-00000220: 6572 6c61 622f 7365 7474 696e 6772 6567  erlab/settingreg
-00000230: 6973 7472 7927 3b0a 696d 706f 7274 207b  istry';.import {
-00000240: 2049 5472 616e 736c 6174 6f72 2c20 6e75   ITranslator, nu
-00000250: 6c6c 5472 616e 736c 6174 6f72 207d 2066  llTranslator } f
-00000260: 726f 6d20 2740 6a75 7079 7465 726c 6162  rom '@jupyterlab
-00000270: 2f74 7261 6e73 6c61 7469 6f6e 273b 0a69  /translation';.i
-00000280: 6d70 6f72 7420 7b20 5946 696c 652c 2059  mport { YFile, Y
-00000290: 4e6f 7465 626f 6f6b 207d 2066 726f 6d20  Notebook } from 
-000002a0: 2740 6a75 7079 7465 722f 7964 6f63 273b  '@jupyter/ydoc';
-000002b0: 0a69 6d70 6f72 7420 7b20 4943 6f6c 6c61  .import { IColla
-000002c0: 626f 7261 7469 7665 4472 6976 652c 2059  borativeDrive, Y
-000002d0: 4472 6976 6520 7d20 6672 6f6d 2027 406a  Drive } from '@j
-000002e0: 7570 7974 6572 2f64 6f63 7072 6f76 6964  upyter/docprovid
-000002f0: 6572 273b 0a2f 2a2a 0a20 2a20 5468 6520  er';./**. * The 
-00000300: 636f 6d6d 616e 6420 4944 7320 7573 6564  command IDs used
-00000310: 2062 7920 7468 6520 6669 6c65 2062 726f   by the file bro
-00000320: 7773 6572 2070 6c75 6769 6e2e 0a20 2a2f  wser plugin.. */
-00000330: 0a76 6172 2043 6f6d 6d61 6e64 4944 733b  .var CommandIDs;
-00000340: 0a28 6675 6e63 7469 6f6e 2028 436f 6d6d  .(function (Comm
-00000350: 616e 6449 4473 2920 7b0a 2020 2020 436f  andIDs) {.    Co
-00000360: 6d6d 616e 6449 4473 2e6f 7065 6e50 6174  mmandIDs.openPat
-00000370: 6820 3d20 2766 696c 6562 726f 7773 6572  h = 'filebrowser
-00000380: 3a6f 7065 6e2d 7061 7468 273b 0a7d 2928  :open-path';.})(
-00000390: 436f 6d6d 616e 6449 4473 207c 7c20 2843  CommandIDs || (C
-000003a0: 6f6d 6d61 6e64 4944 7320 3d20 7b7d 2929  ommandIDs = {}))
-000003b0: 3b0a 2f2a 2a0a 202a 2054 6865 2064 6566  ;./**. * The def
-000003c0: 6175 6c74 2063 6f6c 6c61 626f 7261 7469  ault collaborati
-000003d0: 7665 2064 7269 7665 2070 726f 7669 6465  ve drive provide
-000003e0: 722e 0a20 2a2f 0a65 7870 6f72 7420 636f  r.. */.export co
-000003f0: 6e73 7420 6472 6976 6520 3d20 7b0a 2020  nst drive = {.  
-00000400: 2020 6964 3a20 2740 6a75 7079 7465 722f    id: '@jupyter/
-00000410: 646f 6370 726f 7669 6465 722d 6578 7465  docprovider-exte
-00000420: 6e73 696f 6e3a 6472 6976 6527 2c0a 2020  nsion:drive',.  
-00000430: 2020 6465 7363 7269 7074 696f 6e3a 2027    description: '
-00000440: 5468 6520 6465 6661 756c 7420 636f 6c6c  The default coll
-00000450: 6162 6f72 6174 6976 6520 6472 6976 6520  aborative drive 
-00000460: 7072 6f76 6964 6572 272c 0a20 2020 2070  provider',.    p
-00000470: 726f 7669 6465 733a 2049 436f 6c6c 6162  rovides: ICollab
-00000480: 6f72 6174 6976 6544 7269 7665 2c0a 2020  orativeDrive,.  
-00000490: 2020 7265 7175 6972 6573 3a20 5b49 5472    requires: [ITr
-000004a0: 616e 736c 6174 6f72 5d2c 0a20 2020 206f  anslator],.    o
-000004b0: 7074 696f 6e61 6c3a 205b 5d2c 0a20 2020  ptional: [],.   
-000004c0: 2061 6374 6976 6174 653a 2028 6170 702c   activate: (app,
-000004d0: 2074 7261 6e73 6c61 746f 7229 203d 3e20   translator) => 
-000004e0: 7b0a 2020 2020 2020 2020 636f 6e73 7420  {.        const 
-000004f0: 7472 616e 7320 3d20 7472 616e 736c 6174  trans = translat
-00000500: 6f72 2e6c 6f61 6428 276a 7570 7974 6572  or.load('jupyter
-00000510: 5f63 6f6c 6c61 626f 7261 7469 6f6e 2729  _collaboration')
-00000520: 3b0a 2020 2020 2020 2020 636f 6e73 7420  ;.        const 
-00000530: 6472 6976 6520 3d20 6e65 7720 5944 7269  drive = new YDri
-00000540: 7665 2861 7070 2e73 6572 7669 6365 4d61  ve(app.serviceMa
-00000550: 6e61 6765 722e 7573 6572 2c20 7472 616e  nager.user, tran
-00000560: 7329 3b0a 2020 2020 2020 2020 6170 702e  s);.        app.
-00000570: 7365 7276 6963 654d 616e 6167 6572 2e63  serviceManager.c
-00000580: 6f6e 7465 6e74 732e 6164 6444 7269 7665  ontents.addDrive
-00000590: 2864 7269 7665 293b 0a20 2020 2020 2020  (drive);.       
-000005a0: 2072 6574 7572 6e20 6472 6976 653b 0a20   return drive;. 
-000005b0: 2020 207d 0a7d 3b0a 2f2a 2a0a 202a 2050     }.};./**. * P
-000005c0: 6c75 6769 6e20 746f 2072 6567 6973 7465  lugin to registe
-000005d0: 7220 7468 6520 7368 6172 6564 206d 6f64  r the shared mod
-000005e0: 656c 2066 6163 746f 7279 2066 6f72 2074  el factory for t
-000005f0: 6865 2063 6f6e 7465 6e74 2074 7970 6520  he content type 
-00000600: 2766 696c 6527 2e0a 202a 2f0a 6578 706f  'file'.. */.expo
-00000610: 7274 2063 6f6e 7374 2079 6669 6c65 203d  rt const yfile =
-00000620: 207b 0a20 2020 2069 643a 2027 406a 7570   {.    id: '@jup
-00000630: 7974 6572 2f64 6f63 7072 6f76 6964 6572  yter/docprovider
-00000640: 2d65 7874 656e 7369 6f6e 3a79 6669 6c65  -extension:yfile
-00000650: 272c 0a20 2020 2064 6573 6372 6970 7469  ',.    descripti
-00000660: 6f6e 3a20 2250 6c75 6769 6e20 746f 2072  on: "Plugin to r
-00000670: 6567 6973 7465 7220 7468 6520 7368 6172  egister the shar
-00000680: 6564 206d 6f64 656c 2066 6163 746f 7279  ed model factory
-00000690: 2066 6f72 2074 6865 2063 6f6e 7465 6e74   for the content
-000006a0: 2074 7970 6520 2766 696c 6527 222c 0a20   type 'file'",. 
-000006b0: 2020 2061 7574 6f53 7461 7274 3a20 7472     autoStart: tr
-000006c0: 7565 2c0a 2020 2020 7265 7175 6972 6573  ue,.    requires
-000006d0: 3a20 5b49 436f 6c6c 6162 6f72 6174 6976  : [ICollaborativ
-000006e0: 6544 7269 7665 5d2c 0a20 2020 206f 7074  eDrive],.    opt
-000006f0: 696f 6e61 6c3a 205b 5d2c 0a20 2020 2061  ional: [],.    a
-00000700: 6374 6976 6174 653a 2028 6170 702c 2064  ctivate: (app, d
-00000710: 7269 7665 2920 3d3e 207b 0a20 2020 2020  rive) => {.     
-00000720: 2020 2063 6f6e 7374 2079 4669 6c65 4661     const yFileFa
-00000730: 6374 6f72 7920 3d20 2829 203d 3e20 7b0a  ctory = () => {.
-00000740: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00000750: 726e 206e 6577 2059 4669 6c65 2829 3b0a  rn new YFile();.
-00000760: 2020 2020 2020 2020 7d3b 0a20 2020 2020          };.     
-00000770: 2020 2064 7269 7665 2e73 6861 7265 644d     drive.sharedM
-00000780: 6f64 656c 4661 6374 6f72 792e 7265 6769  odelFactory.regi
-00000790: 7374 6572 446f 6375 6d65 6e74 4661 6374  sterDocumentFact
-000007a0: 6f72 7928 2766 696c 6527 2c20 7946 696c  ory('file', yFil
-000007b0: 6546 6163 746f 7279 293b 0a20 2020 207d  eFactory);.    }
-000007c0: 0a7d 3b0a 2f2a 2a0a 202a 2050 6c75 6769  .};./**. * Plugi
-000007d0: 6e20 746f 2072 6567 6973 7465 7220 7468  n to register th
-000007e0: 6520 7368 6172 6564 206d 6f64 656c 2066  e shared model f
-000007f0: 6163 746f 7279 2066 6f72 2074 6865 2063  actory for the c
-00000800: 6f6e 7465 6e74 2074 7970 6520 276e 6f74  ontent type 'not
-00000810: 6562 6f6f 6b27 2e0a 202a 2f0a 6578 706f  ebook'.. */.expo
-00000820: 7274 2063 6f6e 7374 2079 6e6f 7465 626f  rt const ynotebo
-00000830: 6f6b 203d 207b 0a20 2020 2069 643a 2027  ok = {.    id: '
-00000840: 406a 7570 7974 6572 2f64 6f63 7072 6f76  @jupyter/docprov
-00000850: 6964 6572 2d65 7874 656e 7369 6f6e 3a79  ider-extension:y
-00000860: 6e6f 7465 626f 6f6b 272c 0a20 2020 2064  notebook',.    d
-00000870: 6573 6372 6970 7469 6f6e 3a20 2250 6c75  escription: "Plu
-00000880: 6769 6e20 746f 2072 6567 6973 7465 7220  gin to register 
-00000890: 7468 6520 7368 6172 6564 206d 6f64 656c  the shared model
-000008a0: 2066 6163 746f 7279 2066 6f72 2074 6865   factory for the
-000008b0: 2063 6f6e 7465 6e74 2074 7970 6520 276e   content type 'n
-000008c0: 6f74 6562 6f6f 6b27 222c 0a20 2020 2061  otebook'",.    a
-000008d0: 7574 6f53 7461 7274 3a20 7472 7565 2c0a  utoStart: true,.
-000008e0: 2020 2020 7265 7175 6972 6573 3a20 5b49      requires: [I
-000008f0: 436f 6c6c 6162 6f72 6174 6976 6544 7269  CollaborativeDri
-00000900: 7665 5d2c 0a20 2020 206f 7074 696f 6e61  ve],.    optiona
-00000910: 6c3a 205b 4953 6574 7469 6e67 5265 6769  l: [ISettingRegi
-00000920: 7374 7279 5d2c 0a20 2020 2061 6374 6976  stry],.    activ
-00000930: 6174 653a 2028 6170 702c 2064 7269 7665  ate: (app, drive
-00000940: 2c20 7365 7474 696e 6752 6567 6973 7472  , settingRegistr
-00000950: 7929 203d 3e20 7b0a 2020 2020 2020 2020  y) => {.        
-00000960: 6c65 7420 6469 7361 626c 6544 6f63 756d  let disableDocum
-00000970: 656e 7457 6964 6555 6e64 6f52 6564 6f20  entWideUndoRedo 
-00000980: 3d20 7472 7565 3b0a 2020 2020 2020 2020  = true;.        
-00000990: 2f2f 2046 6574 6368 2073 6574 7469 6e67  // Fetch setting
-000009a0: 7320 6966 2070 6f73 7369 626c 652e 0a20  s if possible.. 
-000009b0: 2020 2020 2020 2069 6620 2873 6574 7469         if (setti
-000009c0: 6e67 5265 6769 7374 7279 2920 7b0a 2020  ngRegistry) {.  
-000009d0: 2020 2020 2020 2020 2020 7365 7474 696e            settin
-000009e0: 6752 6567 6973 7472 790a 2020 2020 2020  gRegistry.      
-000009f0: 2020 2020 2020 2020 2020 2e6c 6f61 6428            .load(
-00000a00: 2740 6a75 7079 7465 726c 6162 2f6e 6f74  '@jupyterlab/not
-00000a10: 6562 6f6f 6b2d 6578 7465 6e73 696f 6e3a  ebook-extension:
-00000a20: 7472 6163 6b65 7227 290a 2020 2020 2020  tracker').      
-00000a30: 2020 2020 2020 2020 2020 2e74 6865 6e28            .then(
-00000a40: 7365 7474 696e 6773 203d 3e20 7b0a 2020  settings => {.  
-00000a50: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00000a60: 6e73 7420 7570 6461 7465 5365 7474 696e  nst updateSettin
-00000a70: 6773 203d 2028 7365 7474 696e 6773 2920  gs = (settings) 
-00000a80: 3d3e 207b 0a20 2020 2020 2020 2020 2020  => {.           
-00000a90: 2020 2020 2020 2020 2076 6172 205f 613b           var _a;
-00000aa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000ab0: 2020 2020 2063 6f6e 7374 2065 6e61 626c       const enabl
-00000ac0: 6544 6f63 5769 6465 556e 646f 203d 2073  eDocWideUndo = s
-00000ad0: 6574 7469 6e67 7320 3d3d 3d20 6e75 6c6c  ettings === null
-00000ae0: 207c 7c20 7365 7474 696e 6773 203d 3d3d   || settings ===
-00000af0: 2076 6f69 6420 3020 3f20 766f 6964 2030   void 0 ? void 0
-00000b00: 203a 2073 6574 7469 6e67 732e 6765 7428   : settings.get(
-00000b10: 2765 7870 6572 696d 656e 7461 6c45 6e61  'experimentalEna
-00000b20: 626c 6544 6f63 756d 656e 7457 6964 6555  bleDocumentWideU
-00000b30: 6e64 6f52 6564 6f27 292e 636f 6d70 6f73  ndoRedo').compos
-00000b40: 6974 653b 0a20 2020 2020 2020 2020 2020  ite;.           
-00000b50: 2020 2020 2020 2020 2064 6973 6162 6c65           disable
-00000b60: 446f 6375 6d65 6e74 5769 6465 556e 646f  DocumentWideUndo
-00000b70: 5265 646f 203d 2028 5f61 203d 2021 656e  Redo = (_a = !en
-00000b80: 6162 6c65 446f 6357 6964 6555 6e64 6f29  ableDocWideUndo)
-00000b90: 2021 3d3d 206e 756c 6c20 2626 205f 6120   !== null && _a 
-00000ba0: 213d 3d20 766f 6964 2030 203f 205f 6120  !== void 0 ? _a 
-00000bb0: 3a20 7472 7565 3b0a 2020 2020 2020 2020  : true;.        
-00000bc0: 2020 2020 2020 2020 7d3b 0a20 2020 2020          };.     
-00000bd0: 2020 2020 2020 2020 2020 2075 7064 6174             updat
-00000be0: 6553 6574 7469 6e67 7328 7365 7474 696e  eSettings(settin
-00000bf0: 6773 293b 0a20 2020 2020 2020 2020 2020  gs);.           
-00000c00: 2020 2020 2073 6574 7469 6e67 732e 6368       settings.ch
-00000c10: 616e 6765 642e 636f 6e6e 6563 7428 2873  anged.connect((s
-00000c20: 6574 7469 6e67 7329 203d 3e20 7570 6461  ettings) => upda
-00000c30: 7465 5365 7474 696e 6773 2873 6574 7469  teSettings(setti
-00000c40: 6e67 7329 293b 0a20 2020 2020 2020 2020  ngs));.         
-00000c50: 2020 207d 293b 0a20 2020 2020 2020 207d     });.        }
-00000c60: 0a20 2020 2020 2020 2063 6f6e 7374 2079  .        const y
-00000c70: 4e6f 7465 626f 6f6b 4661 6374 6f72 7920  NotebookFactory 
-00000c80: 3d20 2829 203d 3e20 7b0a 2020 2020 2020  = () => {.      
-00000c90: 2020 2020 2020 7265 7475 726e 206e 6577        return new
-00000ca0: 2059 4e6f 7465 626f 6f6b 287b 0a20 2020   YNotebook({.   
-00000cb0: 2020 2020 2020 2020 2020 2020 2064 6973               dis
-00000cc0: 6162 6c65 446f 6375 6d65 6e74 5769 6465  ableDocumentWide
-00000cd0: 556e 646f 5265 646f 0a20 2020 2020 2020  UndoRedo.       
-00000ce0: 2020 2020 207d 293b 0a20 2020 2020 2020       });.       
-00000cf0: 207d 3b0a 2020 2020 2020 2020 6472 6976   };.        driv
-00000d00: 652e 7368 6172 6564 4d6f 6465 6c46 6163  e.sharedModelFac
-00000d10: 746f 7279 2e72 6567 6973 7465 7244 6f63  tory.registerDoc
-00000d20: 756d 656e 7446 6163 746f 7279 2827 6e6f  umentFactory('no
-00000d30: 7465 626f 6f6b 272c 2079 4e6f 7465 626f  tebook', yNotebo
-00000d40: 6f6b 4661 6374 6f72 7929 3b0a 2020 2020  okFactory);.    
-00000d50: 7d0a 7d3b 0a2f 2a2a 0a20 2a20 5468 6520  }.};./**. * The 
-00000d60: 6465 6661 756c 7420 6669 6c65 2062 726f  default file bro
-00000d70: 7773 6572 2066 6163 746f 7279 2070 726f  wser factory pro
-00000d80: 7669 6465 722e 0a20 2a2f 0a65 7870 6f72  vider.. */.expor
-00000d90: 7420 636f 6e73 7420 6465 6661 756c 7446  t const defaultF
-00000da0: 696c 6542 726f 7773 6572 203d 207b 0a20  ileBrowser = {. 
-00000db0: 2020 2069 643a 2027 406a 7570 7974 6572     id: '@jupyter
-00000dc0: 2f64 6f63 7072 6f76 6964 6572 2d65 7874  /docprovider-ext
-00000dd0: 656e 7369 6f6e 3a64 6566 6175 6c74 4669  ension:defaultFi
-00000de0: 6c65 4272 6f77 7365 7227 2c0a 2020 2020  leBrowser',.    
-00000df0: 6465 7363 7269 7074 696f 6e3a 2027 5468  description: 'Th
-00000e00: 6520 6465 6661 756c 7420 6669 6c65 2062  e default file b
-00000e10: 726f 7773 6572 2066 6163 746f 7279 2070  rowser factory p
-00000e20: 726f 7669 6465 7227 2c0a 2020 2020 7072  rovider',.    pr
-00000e30: 6f76 6964 6573 3a20 4944 6566 6175 6c74  ovides: IDefault
-00000e40: 4669 6c65 4272 6f77 7365 722c 0a20 2020  FileBrowser,.   
-00000e50: 2072 6571 7569 7265 733a 205b 4943 6f6c   requires: [ICol
-00000e60: 6c61 626f 7261 7469 7665 4472 6976 652c  laborativeDrive,
-00000e70: 2049 4669 6c65 4272 6f77 7365 7246 6163   IFileBrowserFac
-00000e80: 746f 7279 5d2c 0a20 2020 206f 7074 696f  tory],.    optio
-00000e90: 6e61 6c3a 205b 0a20 2020 2020 2020 2049  nal: [.        I
-00000ea0: 526f 7574 6572 2c0a 2020 2020 2020 2020  Router,.        
-00000eb0: 4a75 7079 7465 7246 726f 6e74 456e 642e  JupyterFrontEnd.
-00000ec0: 4954 7265 6552 6573 6f6c 7665 722c 0a20  ITreeResolver,. 
-00000ed0: 2020 2020 2020 2049 4c61 6253 6865 6c6c         ILabShell
-00000ee0: 2c0a 2020 2020 2020 2020 4953 6574 7469  ,.        ISetti
-00000ef0: 6e67 5265 6769 7374 7279 0a20 2020 205d  ngRegistry.    ]
-00000f00: 2c0a 2020 2020 6163 7469 7661 7465 3a20  ,.    activate: 
-00000f10: 6173 796e 6320 2861 7070 2c20 6472 6976  async (app, driv
-00000f20: 652c 2066 696c 6542 726f 7773 6572 4661  e, fileBrowserFa
-00000f30: 6374 6f72 792c 2072 6f75 7465 722c 2074  ctory, router, t
-00000f40: 7265 652c 206c 6162 5368 656c 6c29 203d  ree, labShell) =
-00000f50: 3e20 7b0a 2020 2020 2020 2020 636f 6e73  > {.        cons
-00000f60: 7420 7b20 636f 6d6d 616e 6473 207d 203d  t { commands } =
-00000f70: 2061 7070 3b0a 2020 2020 2020 2020 6170   app;.        ap
-00000f80: 702e 7365 7276 6963 654d 616e 6167 6572  p.serviceManager
-00000f90: 2e63 6f6e 7465 6e74 732e 6164 6444 7269  .contents.addDri
-00000fa0: 7665 2864 7269 7665 293b 0a20 2020 2020  ve(drive);.     
-00000fb0: 2020 202f 2f20 4d61 6e75 616c 6c79 2072     // Manually r
-00000fc0: 6573 746f 7265 2061 6e64 206c 6f61 6420  estore and load 
-00000fd0: 7468 6520 6465 6661 756c 7420 6669 6c65  the default file
-00000fe0: 2062 726f 7773 6572 2e0a 2020 2020 2020   browser..      
-00000ff0: 2020 636f 6e73 7420 6465 6661 756c 7442    const defaultB
-00001000: 726f 7773 6572 203d 2066 696c 6542 726f  rowser = fileBro
-00001010: 7773 6572 4661 6374 6f72 792e 6372 6561  wserFactory.crea
-00001020: 7465 4669 6c65 4272 6f77 7365 7228 2766  teFileBrowser('f
-00001030: 696c 6562 726f 7773 6572 272c 207b 0a20  ilebrowser', {. 
-00001040: 2020 2020 2020 2020 2020 2061 7574 6f3a             auto:
-00001050: 2066 616c 7365 2c0a 2020 2020 2020 2020   false,.        
-00001060: 2020 2020 7265 7374 6f72 653a 2066 616c      restore: fal
-00001070: 7365 2c0a 2020 2020 2020 2020 2020 2020  se,.            
-00001080: 6472 6976 654e 616d 653a 2064 7269 7665  driveName: drive
-00001090: 2e6e 616d 650a 2020 2020 2020 2020 7d29  .name.        })
-000010a0: 3b0a 2020 2020 2020 2020 766f 6964 2050  ;.        void P
-000010b0: 7269 7661 7465 2e72 6573 746f 7265 4272  rivate.restoreBr
-000010c0: 6f77 7365 7228 6465 6661 756c 7442 726f  owser(defaultBro
-000010d0: 7773 6572 2c20 636f 6d6d 616e 6473 2c20  wser, commands, 
-000010e0: 726f 7574 6572 2c20 7472 6565 2c20 6c61  router, tree, la
-000010f0: 6253 6865 6c6c 293b 0a20 2020 2020 2020  bShell);.       
-00001100: 2072 6574 7572 6e20 6465 6661 756c 7442   return defaultB
-00001110: 726f 7773 6572 3b0a 2020 2020 7d0a 7d3b  rowser;.    }.};
-00001120: 0a2f 2a2a 0a20 2a20 5468 6520 6465 6661  ./**. * The defa
-00001130: 756c 7420 636f 6c6c 6162 6f72 6174 6976  ult collaborativ
-00001140: 6520 6472 6976 6520 7072 6f76 6964 6572  e drive provider
-00001150: 2e0a 202a 2f0a 6578 706f 7274 2063 6f6e  .. */.export con
-00001160: 7374 206c 6f67 6765 7220 3d20 7b0a 2020  st logger = {.  
-00001170: 2020 6964 3a20 2740 6a75 7079 7465 722f    id: '@jupyter/
-00001180: 646f 6370 726f 7669 6465 722d 6578 7465  docprovider-exte
-00001190: 6e73 696f 6e3a 6c6f 6767 6572 272c 0a20  nsion:logger',. 
-000011a0: 2020 2064 6573 6372 6970 7469 6f6e 3a20     description: 
-000011b0: 2741 206c 6f67 6769 6e67 2070 6c75 6769  'A logging plugi
-000011c0: 6e20 666f 7220 6465 6275 6767 696e 6720  n for debugging 
-000011d0: 7075 7270 6f73 6573 2e27 2c0a 2020 2020  purposes.',.    
-000011e0: 6175 746f 5374 6172 743a 2074 7275 652c  autoStart: true,
-000011f0: 0a20 2020 206f 7074 696f 6e61 6c3a 205b  .    optional: [
-00001200: 494c 6f67 6765 7252 6567 6973 7472 792c  ILoggerRegistry,
-00001210: 2049 4564 6974 6f72 5472 6163 6b65 722c   IEditorTracker,
-00001220: 2049 4e6f 7465 626f 6f6b 5472 6163 6b65   INotebookTracke
-00001230: 722c 2049 5472 616e 736c 6174 6f72 5d2c  r, ITranslator],
-00001240: 0a20 2020 2061 6374 6976 6174 653a 2028  .    activate: (
-00001250: 6170 702c 206c 6f67 6765 7252 6567 6973  app, loggerRegis
-00001260: 7472 792c 2066 696c 6554 7261 636b 6572  try, fileTracker
-00001270: 2c20 6e62 5472 6163 6b65 722c 2074 7261  , nbTracker, tra
-00001280: 6e73 6c61 746f 7229 203d 3e20 7b0a 2020  nslator) => {.  
-00001290: 2020 2020 2020 636f 6e73 7420 7472 616e        const tran
-000012a0: 7320 3d20 2874 7261 6e73 6c61 746f 7220  s = (translator 
-000012b0: 213d 3d20 6e75 6c6c 2026 2620 7472 616e  !== null && tran
-000012c0: 736c 6174 6f72 2021 3d3d 2076 6f69 6420  slator !== void 
-000012d0: 3020 3f20 7472 616e 736c 6174 6f72 203a  0 ? translator :
-000012e0: 206e 756c 6c54 7261 6e73 6c61 746f 7229   nullTranslator)
-000012f0: 2e6c 6f61 6428 276a 7570 7974 6572 5f63  .load('jupyter_c
-00001300: 6f6c 6c61 626f 7261 7469 6f6e 2729 3b0a  ollaboration');.
-00001310: 2020 2020 2020 2020 636f 6e73 7420 7363          const sc
-00001320: 6865 6d61 4944 203d 2027 6874 7470 733a  hemaID = 'https:
-00001330: 2f2f 7363 6865 6d61 2e6a 7570 7974 6572  //schema.jupyter
-00001340: 2e6f 7267 2f6a 7570 7974 6572 5f63 6f6c  .org/jupyter_col
-00001350: 6c61 626f 7261 7469 6f6e 2f73 6573 7369  laboration/sessi
-00001360: 6f6e 2f76 3127 3b0a 2020 2020 2020 2020  on/v1';.        
-00001370: 6966 2028 216c 6f67 6765 7252 6567 6973  if (!loggerRegis
-00001380: 7472 7929 207b 0a20 2020 2020 2020 2020  try) {.         
-00001390: 2020 2061 7070 2e73 6572 7669 6365 4d61     app.serviceMa
-000013a0: 6e61 6765 722e 6576 656e 7473 2e73 7472  nager.events.str
-000013b0: 6561 6d2e 636f 6e6e 6563 7428 285f 2c20  eam.connect((_, 
-000013c0: 656d 6973 7369 6f6e 2920 3d3e 207b 0a20  emission) => {. 
-000013d0: 2020 2020 2020 2020 2020 2020 2020 2076                 v
-000013e0: 6172 205f 612c 205f 623b 0a20 2020 2020  ar _a, _b;.     
-000013f0: 2020 2020 2020 2020 2020 2069 6620 2865             if (e
-00001400: 6d69 7373 696f 6e2e 7363 6865 6d61 5f69  mission.schema_i
-00001410: 6420 3d3d 3d20 7363 6865 6d61 4944 2920  d === schemaID) 
-00001420: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-00001430: 2020 2020 2020 636f 6e73 6f6c 652e 6465        console.de
-00001440: 6275 6728 605b 247b 656d 6973 7369 6f6e  bug(`[${emission
-00001450: 2e72 6f6f 6d7d 2824 7b65 6d69 7373 696f  .room}(${emissio
-00001460: 6e2e 7061 7468 7d29 5d20 247b 285f 6120  n.path})] ${(_a 
-00001470: 3d20 656d 6973 7369 6f6e 2e61 6374 696f  = emission.actio
-00001480: 6e29 2021 3d3d 206e 756c 6c20 2626 205f  n) !== null && _
-00001490: 6120 213d 3d20 766f 6964 2030 203f 205f  a !== void 0 ? _
-000014a0: 6120 3a20 2727 7d3a 2024 7b28 5f62 203d  a : ''}: ${(_b =
-000014b0: 2065 6d69 7373 696f 6e2e 6d73 6729 2021   emission.msg) !
-000014c0: 3d3d 206e 756c 6c20 2626 205f 6220 213d  == null && _b !=
-000014d0: 3d20 766f 6964 2030 203f 205f 6220 3a20  = void 0 ? _b : 
-000014e0: 2727 7d60 293b 0a20 2020 2020 2020 2020  ''}`);.         
-000014f0: 2020 2020 2020 2020 2020 2069 6620 2865             if (e
-00001500: 6d69 7373 696f 6e2e 6c65 7665 6c20 3d3d  mission.level ==
-00001510: 3d20 2757 4152 4e49 4e47 2729 207b 0a20  = 'WARNING') {. 
-00001520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001530: 2020 2020 2020 2073 686f 7744 6961 6c6f         showDialo
-00001540: 6728 7b0a 2020 2020 2020 2020 2020 2020  g({.            
-00001550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001560: 7469 746c 653a 2074 7261 6e73 2e5f 5f28  title: trans.__(
-00001570: 2757 6172 6e69 6e67 2729 2c0a 2020 2020  'Warning'),.    
-00001580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001590: 2020 2020 2020 2020 626f 6479 3a20 7472          body: tr
-000015a0: 616e 732e 5f5f 2860 5477 6f20 636f 6c6c  ans.__(`Two coll
-000015b0: 6162 6f72 6174 6976 6520 7365 7373 696f  aborative sessio
-000015c0: 6e73 2061 7265 2061 6363 6573 7369 6e67  ns are accessing
-000015d0: 2074 6865 2066 696c 6520 247b 656d 6973   the file ${emis
-000015e0: 7369 6f6e 2e70 6174 687d 2073 696d 756c  sion.path} simul
-000015f0: 7461 6e65 6f75 736c 792e 0a20 2020 2020  taneously..     
-00001600: 2020 2020 2020 2020 2020 205c 6e4f 7065             \nOpe
-00001610: 6e69 6e67 2074 6865 2073 616d 6520 6669  ning the same fi
-00001620: 6c65 2075 7369 6e67 2064 6966 6665 7265  le using differe
-00001630: 6e74 2076 6965 7773 2073 696d 756c 7461  nt views simulta
-00001640: 6e65 6f75 736c 7920 6973 206e 6f74 2073  neously is not s
-00001650: 7570 706f 7274 6564 2e20 506c 6561 7365  upported. Please
-00001660: 2c20 636c 6f73 6520 6f6e 6520 7669 6577  , close one view
-00001670: 3b20 6f74 6865 7277 6973 652c 2079 6f75  ; otherwise, you
-00001680: 206d 6967 6874 206c 6f73 6520 736f 6d65   might lose some
-00001690: 206f 6620 796f 7572 2070 726f 6772 6573   of your progres
-000016a0: 732e 6029 2c0a 2020 2020 2020 2020 2020  s.`),.          
-000016b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000016c0: 2020 6275 7474 6f6e 733a 205b 4469 616c    buttons: [Dial
-000016d0: 6f67 2e6f 6b42 7574 746f 6e28 295d 0a20  og.okButton()]. 
-000016e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000016f0: 2020 2020 2020 207d 293b 0a20 2020 2020         });.     
-00001700: 2020 2020 2020 2020 2020 2020 2020 207d                 }
-00001710: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001720: 207d 0a20 2020 2020 2020 2020 2020 207d   }.            }
-00001730: 293b 0a20 2020 2020 2020 2020 2020 2072  );.            r
-00001740: 6574 7572 6e3b 0a20 2020 2020 2020 207d  eturn;.        }
-00001750: 0a20 2020 2020 2020 2063 6f6e 7374 206c  .        const l
-00001760: 6f67 6765 7273 203d 206e 6577 204d 6170  oggers = new Map
-00001770: 2829 3b0a 2020 2020 2020 2020 636f 6e73  ();.        cons
-00001780: 7420 6164 644c 6f67 6765 7220 3d20 2873  t addLogger = (s
-00001790: 656e 6465 722c 2064 6f63 756d 656e 7429  ender, document)
-000017a0: 203d 3e20 7b0a 2020 2020 2020 2020 2020   => {.          
-000017b0: 2020 636f 6e73 7420 6c6f 6767 6572 203d    const logger =
-000017c0: 206c 6f67 6765 7252 6567 6973 7472 792e   loggerRegistry.
-000017d0: 6765 744c 6f67 6765 7228 646f 6375 6d65  getLogger(docume
-000017e0: 6e74 2e63 6f6e 7465 7874 2e70 6174 6829  nt.context.path)
-000017f0: 3b0a 2020 2020 2020 2020 2020 2020 6c6f  ;.            lo
-00001800: 6767 6572 732e 7365 7428 646f 6375 6d65  ggers.set(docume
-00001810: 6e74 2e63 6f6e 7465 7874 2e6c 6f63 616c  nt.context.local
-00001820: 5061 7468 2c20 6c6f 6767 6572 293b 0a20  Path, logger);. 
-00001830: 2020 2020 2020 2020 2020 2064 6f63 756d             docum
-00001840: 656e 742e 6469 7370 6f73 6564 2e63 6f6e  ent.disposed.con
-00001850: 6e65 6374 2864 6f63 756d 656e 7420 3d3e  nect(document =>
-00001860: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-00001870: 2020 206c 6f67 6765 7273 2e64 656c 6574     loggers.delet
-00001880: 6528 646f 6375 6d65 6e74 2e63 6f6e 7465  e(document.conte
-00001890: 7874 2e6c 6f63 616c 5061 7468 293b 0a20  xt.localPath);. 
-000018a0: 2020 2020 2020 2020 2020 207d 293b 0a20             });. 
-000018b0: 2020 2020 2020 207d 3b0a 2020 2020 2020         };.      
-000018c0: 2020 6966 2028 6669 6c65 5472 6163 6b65    if (fileTracke
-000018d0: 7229 207b 0a20 2020 2020 2020 2020 2020  r) {.           
-000018e0: 2066 696c 6554 7261 636b 6572 2e77 6964   fileTracker.wid
-000018f0: 6765 7441 6464 6564 2e63 6f6e 6e65 6374  getAdded.connect
-00001900: 2861 6464 4c6f 6767 6572 293b 0a20 2020  (addLogger);.   
-00001910: 2020 2020 207d 0a20 2020 2020 2020 2069       }.        i
-00001920: 6620 286e 6254 7261 636b 6572 2920 7b0a  f (nbTracker) {.
-00001930: 2020 2020 2020 2020 2020 2020 6e62 5472              nbTr
-00001940: 6163 6b65 722e 7769 6467 6574 4164 6465  acker.widgetAdde
-00001950: 642e 636f 6e6e 6563 7428 6164 644c 6f67  d.connect(addLog
-00001960: 6765 7229 3b0a 2020 2020 2020 2020 7d0a  ger);.        }.
-00001970: 2020 2020 2020 2020 766f 6964 2028 6173          void (as
-00001980: 796e 6320 2829 203d 3e20 7b0a 2020 2020  ync () => {.    
-00001990: 2020 2020 2020 2020 7661 7220 5f61 2c20          var _a, 
-000019a0: 5f62 3b0a 2020 2020 2020 2020 2020 2020  _b;.            
-000019b0: 636f 6e73 7420 7b20 6576 656e 7473 207d  const { events }
-000019c0: 203d 2061 7070 2e73 6572 7669 6365 4d61   = app.serviceMa
-000019d0: 6e61 6765 723b 0a20 2020 2020 2020 2020  nager;.         
-000019e0: 2020 2066 6f72 2061 7761 6974 2028 636f     for await (co
-000019f0: 6e73 7420 656d 6973 7369 6f6e 206f 6620  nst emission of 
-00001a00: 6576 656e 7473 2e73 7472 6561 6d29 207b  events.stream) {
-00001a10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001a20: 2069 6620 2865 6d69 7373 696f 6e2e 7363   if (emission.sc
-00001a30: 6865 6d61 5f69 6420 3d3d 3d20 7363 6865  hema_id === sche
-00001a40: 6d61 4944 2920 7b0a 2020 2020 2020 2020  maID) {.        
-00001a50: 2020 2020 2020 2020 2020 2020 636f 6e73              cons
-00001a60: 7420 6c6f 6767 6572 203d 206c 6f67 6765  t logger = logge
-00001a70: 7273 2e67 6574 2865 6d69 7373 696f 6e2e  rs.get(emission.
-00001a80: 7061 7468 293b 0a20 2020 2020 2020 2020  path);.         
-00001a90: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
-00001aa0: 7220 3d3d 3d20 6e75 6c6c 207c 7c20 6c6f  r === null || lo
-00001ab0: 6767 6572 203d 3d3d 2076 6f69 6420 3020  gger === void 0 
-00001ac0: 3f20 766f 6964 2030 203a 206c 6f67 6765  ? void 0 : logge
-00001ad0: 722e 6c6f 6728 7b0a 2020 2020 2020 2020  r.log({.        
-00001ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001af0: 7479 7065 3a20 2774 6578 7427 2c0a 2020  type: 'text',.  
-00001b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b10: 2020 2020 2020 6c65 7665 6c3a 2065 6d69        level: emi
-00001b20: 7373 696f 6e2e 6c65 7665 6c2e 746f 4c6f  ssion.level.toLo
-00001b30: 7765 7243 6173 6528 292c 0a20 2020 2020  werCase(),.     
-00001b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b50: 2020 2064 6174 613a 2060 5b24 7b65 6d69     data: `[${emi
-00001b60: 7373 696f 6e2e 726f 6f6d 7d5d 2024 7b28  ssion.room}] ${(
-00001b70: 5f61 203d 2065 6d69 7373 696f 6e2e 6163  _a = emission.ac
-00001b80: 7469 6f6e 2920 213d 3d20 6e75 6c6c 2026  tion) !== null &
-00001b90: 2620 5f61 2021 3d3d 2076 6f69 6420 3020  & _a !== void 0 
-00001ba0: 3f20 5f61 203a 2027 277d 3a20 247b 285f  ? _a : ''}: ${(_
-00001bb0: 6220 3d20 656d 6973 7369 6f6e 2e6d 7367  b = emission.msg
-00001bc0: 2920 213d 3d20 6e75 6c6c 2026 2620 5f62  ) !== null && _b
-00001bd0: 2021 3d3d 2076 6f69 6420 3020 3f20 5f62   !== void 0 ? _b
-00001be0: 203a 2027 277d 600a 2020 2020 2020 2020   : ''}`.        
-00001bf0: 2020 2020 2020 2020 2020 2020 7d29 3b0a              });.
-00001c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001c10: 2020 2020 6966 2028 656d 6973 7369 6f6e      if (emission
-00001c20: 2e6c 6576 656c 203d 3d3d 2027 5741 524e  .level === 'WARN
-00001c30: 494e 4727 2920 7b0a 2020 2020 2020 2020  ING') {.        
-00001c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001c50: 7368 6f77 4469 616c 6f67 287b 0a20 2020  showDialog({.   
-00001c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001c70: 2020 2020 2020 2020 2074 6974 6c65 3a20           title: 
-00001c80: 7472 616e 732e 5f5f 2827 5761 726e 696e  trans.__('Warnin
-00001c90: 6727 292c 0a20 2020 2020 2020 2020 2020  g'),.           
-00001ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001cb0: 2062 6f64 793a 2074 7261 6e73 2e5f 5f28   body: trans.__(
-00001cc0: 6054 776f 2063 6f6c 6c61 626f 7261 7469  `Two collaborati
-00001cd0: 7665 2073 6573 7369 6f6e 7320 6172 6520  ve sessions are 
-00001ce0: 6163 6365 7373 696e 6720 7468 6520 6669  accessing the fi
-00001cf0: 6c65 2025 3120 7369 6d75 6c74 616e 656f  le %1 simultaneo
-00001d00: 7573 6c79 2e0a 2020 2020 2020 2020 2020  usly..          
-00001d10: 2020 2020 2020 5c6e 4f70 656e 696e 6720        \nOpening 
-00001d20: 6120 646f 6375 6d65 6e74 2077 6974 6820  a document with 
-00001d30: 6d75 6c74 6970 6c65 2076 6965 7773 2073  multiple views s
-00001d40: 696d 756c 7461 6e65 6f75 736c 7920 6973  imultaneously is
-00001d50: 206e 6f74 2073 7570 706f 7274 6564 2e20   not supported. 
-00001d60: 506c 6561 7365 2063 6c6f 7365 206f 6e65  Please close one
-00001d70: 2076 6965 773b 206f 7468 6572 7769 7365   view; otherwise
-00001d80: 2c20 796f 7520 6d69 6768 7420 6c6f 7365  , you might lose
-00001d90: 2073 6f6d 6520 6f66 2079 6f75 7220 7072   some of your pr
-00001da0: 6f67 7265 7373 2e60 2c20 656d 6973 7369  ogress.`, emissi
-00001db0: 6f6e 2e70 6174 6829 2c0a 2020 2020 2020  on.path),.      
-00001dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001dd0: 2020 2020 2020 6275 7474 6f6e 733a 205b        buttons: [
-00001de0: 4469 616c 6f67 2e77 6172 6e42 7574 746f  Dialog.warnButto
-00001df0: 6e28 7b20 6c61 6265 6c3a 2074 7261 6e73  n({ label: trans
-00001e00: 2e5f 5f28 274f 6b27 2920 7d29 5d0a 2020  .__('Ok') })].  
-00001e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e20: 2020 2020 2020 7d29 3b0a 2020 2020 2020        });.      
-00001e30: 2020 2020 2020 2020 2020 2020 2020 7d0a                }.
-00001e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e50: 7d0a 2020 2020 2020 2020 2020 2020 7d0a  }.            }.
-00001e60: 2020 2020 2020 2020 7d29 2829 3b0a 2020          })();.  
-00001e70: 2020 7d0a 7d3b 0a76 6172 2050 7269 7661    }.};.var Priva
-00001e80: 7465 3b0a 2866 756e 6374 696f 6e20 2850  te;.(function (P
-00001e90: 7269 7661 7465 2920 7b0a 2020 2020 2f2a  rivate) {.    /*
-00001ea0: 2a0a 2020 2020 202a 2052 6573 746f 7265  *.     * Restore
-00001eb0: 7320 6669 6c65 2062 726f 7773 6572 2073  s file browser s
-00001ec0: 7461 7465 2061 6e64 206f 7665 7272 6964  tate and overrid
-00001ed0: 6573 2073 7461 7465 2069 6620 7472 6565  es state if tree
-00001ee0: 2072 6573 6f6c 7665 7220 7265 736f 6c76   resolver resolv
-00001ef0: 6573 2e0a 2020 2020 202a 2f0a 2020 2020  es..     */.    
-00001f00: 6173 796e 6320 6675 6e63 7469 6f6e 2072  async function r
-00001f10: 6573 746f 7265 4272 6f77 7365 7228 6272  estoreBrowser(br
-00001f20: 6f77 7365 722c 2063 6f6d 6d61 6e64 732c  owser, commands,
-00001f30: 2072 6f75 7465 722c 2074 7265 652c 206c   router, tree, l
-00001f40: 6162 5368 656c 6c29 207b 0a20 2020 2020  abShell) {.     
-00001f50: 2020 2063 6f6e 7374 2072 6573 746f 7269     const restori
-00001f60: 6e67 203d 2027 6a70 2d6d 6f64 2d72 6573  ng = 'jp-mod-res
-00001f70: 746f 7269 6e67 273b 0a20 2020 2020 2020  toring';.       
-00001f80: 2062 726f 7773 6572 2e61 6464 436c 6173   browser.addClas
-00001f90: 7328 7265 7374 6f72 696e 6729 3b0a 2020  s(restoring);.  
-00001fa0: 2020 2020 2020 6966 2028 2172 6f75 7465        if (!route
-00001fb0: 7229 207b 0a20 2020 2020 2020 2020 2020  r) {.           
-00001fc0: 2061 7761 6974 2062 726f 7773 6572 2e6d   await browser.m
-00001fd0: 6f64 656c 2e72 6573 746f 7265 2862 726f  odel.restore(bro
-00001fe0: 7773 6572 2e69 6429 3b0a 2020 2020 2020  wser.id);.      
-00001ff0: 2020 2020 2020 6177 6169 7420 6272 6f77        await brow
-00002000: 7365 722e 6d6f 6465 6c2e 7265 6672 6573  ser.model.refres
-00002010: 6828 293b 0a20 2020 2020 2020 2020 2020  h();.           
-00002020: 2062 726f 7773 6572 2e72 656d 6f76 6543   browser.removeC
-00002030: 6c61 7373 2872 6573 746f 7269 6e67 293b  lass(restoring);
-00002040: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00002050: 7572 6e3b 0a20 2020 2020 2020 207d 0a20  urn;.        }. 
-00002060: 2020 2020 2020 2063 6f6e 7374 206c 6973         const lis
-00002070: 7465 6e65 7220 3d20 6173 796e 6320 2829  tener = async ()
-00002080: 203d 3e20 7b0a 2020 2020 2020 2020 2020   => {.          
-00002090: 2020 726f 7574 6572 2e72 6f75 7465 642e    router.routed.
-000020a0: 6469 7363 6f6e 6e65 6374 286c 6973 7465  disconnect(liste
-000020b0: 6e65 7229 3b0a 2020 2020 2020 2020 2020  ner);.          
-000020c0: 2020 636f 6e73 7420 7061 7468 7320 3d20    const paths = 
-000020d0: 6177 6169 7420 2874 7265 6520 3d3d 3d20  await (tree === 
-000020e0: 6e75 6c6c 207c 7c20 7472 6565 203d 3d3d  null || tree ===
-000020f0: 2076 6f69 6420 3020 3f20 766f 6964 2030   void 0 ? void 0
-00002100: 203a 2074 7265 652e 7061 7468 7329 3b0a   : tree.paths);.
-00002110: 2020 2020 2020 2020 2020 2020 6966 2028              if (
-00002120: 2870 6174 6873 203d 3d3d 206e 756c 6c20  (paths === null 
-00002130: 7c7c 2070 6174 6873 203d 3d3d 2076 6f69  || paths === voi
-00002140: 6420 3020 3f20 766f 6964 2030 203a 2070  d 0 ? void 0 : p
-00002150: 6174 6873 2e66 696c 6529 207c 7c20 2870  aths.file) || (p
-00002160: 6174 6873 203d 3d3d 206e 756c 6c20 7c7c  aths === null ||
-00002170: 2070 6174 6873 203d 3d3d 2076 6f69 6420   paths === void 
-00002180: 3020 3f20 766f 6964 2030 203a 2070 6174  0 ? void 0 : pat
-00002190: 6873 2e62 726f 7773 6572 2929 207b 0a20  hs.browser)) {. 
-000021a0: 2020 2020 2020 2020 2020 2020 2020 202f                 /
-000021b0: 2f20 5265 7374 6f72 6520 7468 6520 6d6f  / Restore the mo
-000021c0: 6465 6c20 7769 7468 6f75 7420 706f 7075  del without popu
-000021d0: 6c61 7469 6e67 2069 742e 0a20 2020 2020  lating it..     
-000021e0: 2020 2020 2020 2020 2020 2061 7761 6974             await
-000021f0: 2062 726f 7773 6572 2e6d 6f64 656c 2e72   browser.model.r
-00002200: 6573 746f 7265 2862 726f 7773 6572 2e69  estore(browser.i
-00002210: 642c 2066 616c 7365 293b 0a20 2020 2020  d, false);.     
-00002220: 2020 2020 2020 2020 2020 2069 6620 2870             if (p
-00002230: 6174 6873 2e66 696c 6529 207b 0a20 2020  aths.file) {.   
-00002240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002250: 2061 7761 6974 2063 6f6d 6d61 6e64 732e   await commands.
-00002260: 6578 6563 7574 6528 436f 6d6d 616e 6449  execute(CommandI
-00002270: 4473 2e6f 7065 6e50 6174 682c 207b 0a20  Ds.openPath, {. 
-00002280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002290: 2020 2020 2020 2070 6174 683a 2070 6174         path: pat
-000022a0: 6873 2e66 696c 652c 0a20 2020 2020 2020  hs.file,.       
-000022b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000022c0: 2064 6f6e 7453 686f 7742 726f 7773 6572   dontShowBrowser
-000022d0: 3a20 7472 7565 0a20 2020 2020 2020 2020  : true.         
-000022e0: 2020 2020 2020 2020 2020 207d 293b 0a20             });. 
-000022f0: 2020 2020 2020 2020 2020 2020 2020 207d                 }
-00002300: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002310: 2069 6620 2870 6174 6873 2e62 726f 7773   if (paths.brows
-00002320: 6572 2920 7b0a 2020 2020 2020 2020 2020  er) {.          
-00002330: 2020 2020 2020 2020 2020 6177 6169 7420            await 
-00002340: 636f 6d6d 616e 6473 2e65 7865 6375 7465  commands.execute
-00002350: 2843 6f6d 6d61 6e64 4944 732e 6f70 656e  (CommandIDs.open
-00002360: 5061 7468 2c20 7b0a 2020 2020 2020 2020  Path, {.        
-00002370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002380: 7061 7468 3a20 7061 7468 732e 6272 6f77  path: paths.brow
-00002390: 7365 722c 0a20 2020 2020 2020 2020 2020  ser,.           
-000023a0: 2020 2020 2020 2020 2020 2020 2064 6f6e               don
-000023b0: 7453 686f 7742 726f 7773 6572 3a20 7472  tShowBrowser: tr
-000023c0: 7565 0a20 2020 2020 2020 2020 2020 2020  ue.             
-000023d0: 2020 2020 2020 207d 293b 0a20 2020 2020         });.     
-000023e0: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
-000023f0: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
-00002400: 2020 2020 2020 2065 6c73 6520 7b0a 2020         else {.  
-00002410: 2020 2020 2020 2020 2020 2020 2020 6177                aw
-00002420: 6169 7420 6272 6f77 7365 722e 6d6f 6465  ait browser.mode
-00002430: 6c2e 7265 7374 6f72 6528 6272 6f77 7365  l.restore(browse
-00002440: 722e 6964 293b 0a20 2020 2020 2020 2020  r.id);.         
-00002450: 2020 2020 2020 2061 7761 6974 2062 726f         await bro
-00002460: 7773 6572 2e6d 6f64 656c 2e72 6566 7265  wser.model.refre
-00002470: 7368 2829 3b0a 2020 2020 2020 2020 2020  sh();.          
-00002480: 2020 7d0a 2020 2020 2020 2020 2020 2020    }.            
-00002490: 6272 6f77 7365 722e 7265 6d6f 7665 436c  browser.removeCl
-000024a0: 6173 7328 7265 7374 6f72 696e 6729 3b0a  ass(restoring);.
-000024b0: 2020 2020 2020 2020 2020 2020 6966 2028              if (
-000024c0: 6c61 6253 6865 6c6c 203d 3d3d 206e 756c  labShell === nul
-000024d0: 6c20 7c7c 206c 6162 5368 656c 6c20 3d3d  l || labShell ==
-000024e0: 3d20 766f 6964 2030 203f 2076 6f69 6420  = void 0 ? void 
-000024f0: 3020 3a20 6c61 6253 6865 6c6c 2e69 7345  0 : labShell.isE
-00002500: 6d70 7479 2827 6d61 696e 2729 2920 7b0a  mpty('main')) {.
-00002510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002520: 766f 6964 2063 6f6d 6d61 6e64 732e 6578  void commands.ex
-00002530: 6563 7574 6528 276c 6175 6e63 6865 723a  ecute('launcher:
-00002540: 6372 6561 7465 2729 3b0a 2020 2020 2020  create');.      
-00002550: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-00002560: 7d3b 0a20 2020 2020 2020 2072 6f75 7465  };.        route
-00002570: 722e 726f 7574 6564 2e63 6f6e 6e65 6374  r.routed.connect
-00002580: 286c 6973 7465 6e65 7229 3b0a 2020 2020  (listener);.    
-00002590: 7d0a 2020 2020 5072 6976 6174 652e 7265  }.    Private.re
-000025a0: 7374 6f72 6542 726f 7773 6572 203d 2072  storeBrowser = r
-000025b0: 6573 746f 7265 4272 6f77 7365 723b 0a7d  estoreBrowser;.}
-000025c0: 2928 5072 6976 6174 6520 7c7c 2028 5072  )(Private || (Pr
-000025d0: 6976 6174 6520 3d20 7b7d 2929 3b0a       ivate = {}));.
+00000060: 204c 6963 656e 7365 2e0a 202a 2f0a 0a69   License.. */..i
+00000070: 6d70 6f72 7420 7b0a 2020 494c 6162 5368  mport {.  ILabSh
+00000080: 656c 6c2c 0a20 2049 526f 7574 6572 2c0a  ell,.  IRouter,.
+00000090: 2020 4a75 7079 7465 7246 726f 6e74 456e    JupyterFrontEn
+000000a0: 642c 0a20 204a 7570 7974 6572 4672 6f6e  d,.  JupyterFron
+000000b0: 7445 6e64 506c 7567 696e 0a7d 2066 726f  tEndPlugin.} fro
+000000c0: 6d20 2740 6a75 7079 7465 726c 6162 2f61  m '@jupyterlab/a
+000000d0: 7070 6c69 6361 7469 6f6e 273b 0a69 6d70  pplication';.imp
+000000e0: 6f72 7420 7b20 4469 616c 6f67 2c20 7368  ort { Dialog, sh
+000000f0: 6f77 4469 616c 6f67 207d 2066 726f 6d20  owDialog } from 
+00000100: 2740 6a75 7079 7465 726c 6162 2f61 7070  '@jupyterlab/app
+00000110: 7574 696c 7327 3b0a 696d 706f 7274 207b  utils';.import {
+00000120: 2049 446f 6375 6d65 6e74 5769 6467 6574   IDocumentWidget
+00000130: 207d 2066 726f 6d20 2740 6a75 7079 7465   } from '@jupyte
+00000140: 726c 6162 2f64 6f63 7265 6769 7374 7279  rlab/docregistry
+00000150: 273b 0a69 6d70 6f72 7420 7b0a 2020 4669  ';.import {.  Fi
+00000160: 6c65 4272 6f77 7365 722c 0a20 2049 4465  leBrowser,.  IDe
+00000170: 6661 756c 7446 696c 6542 726f 7773 6572  faultFileBrowser
+00000180: 2c0a 2020 4946 696c 6542 726f 7773 6572  ,.  IFileBrowser
+00000190: 4661 6374 6f72 790a 7d20 6672 6f6d 2027  Factory.} from '
+000001a0: 406a 7570 7974 6572 6c61 622f 6669 6c65  @jupyterlab/file
+000001b0: 6272 6f77 7365 7227 3b0a 696d 706f 7274  browser';.import
+000001c0: 207b 2049 4564 6974 6f72 5472 6163 6b65   { IEditorTracke
+000001d0: 7220 7d20 6672 6f6d 2027 406a 7570 7974  r } from '@jupyt
+000001e0: 6572 6c61 622f 6669 6c65 6564 6974 6f72  erlab/fileeditor
+000001f0: 273b 0a69 6d70 6f72 7420 7b20 494c 6f67  ';.import { ILog
+00000200: 6765 722c 2049 4c6f 6767 6572 5265 6769  ger, ILoggerRegi
+00000210: 7374 7279 207d 2066 726f 6d20 2740 6a75  stry } from '@ju
+00000220: 7079 7465 726c 6162 2f6c 6f67 636f 6e73  pyterlab/logcons
+00000230: 6f6c 6527 3b0a 696d 706f 7274 207b 2049  ole';.import { I
+00000240: 4e6f 7465 626f 6f6b 5472 6163 6b65 7220  NotebookTracker 
+00000250: 7d20 6672 6f6d 2027 406a 7570 7974 6572  } from '@jupyter
+00000260: 6c61 622f 6e6f 7465 626f 6f6b 273b 0a69  lab/notebook';.i
+00000270: 6d70 6f72 7420 7b20 4953 6574 7469 6e67  mport { ISetting
+00000280: 5265 6769 7374 7279 207d 2066 726f 6d20  Registry } from 
+00000290: 2740 6a75 7079 7465 726c 6162 2f73 6574  '@jupyterlab/set
+000002a0: 7469 6e67 7265 6769 7374 7279 273b 0a69  tingregistry';.i
+000002b0: 6d70 6f72 7420 7b20 4954 7261 6e73 6c61  mport { ITransla
+000002c0: 746f 722c 206e 756c 6c54 7261 6e73 6c61  tor, nullTransla
+000002d0: 746f 7220 7d20 6672 6f6d 2027 406a 7570  tor } from '@jup
+000002e0: 7974 6572 6c61 622f 7472 616e 736c 6174  yterlab/translat
+000002f0: 696f 6e27 3b0a 0a69 6d70 6f72 7420 7b20  ion';..import { 
+00000300: 436f 6d6d 616e 6452 6567 6973 7472 7920  CommandRegistry 
+00000310: 7d20 6672 6f6d 2027 406c 756d 696e 6f2f  } from '@lumino/
+00000320: 636f 6d6d 616e 6473 273b 0a0a 696d 706f  commands';..impo
+00000330: 7274 207b 2059 4669 6c65 2c20 594e 6f74  rt { YFile, YNot
+00000340: 6562 6f6f 6b20 7d20 6672 6f6d 2027 406a  ebook } from '@j
+00000350: 7570 7974 6572 2f79 646f 6327 3b0a 0a69  upyter/ydoc';..i
+00000360: 6d70 6f72 7420 7b20 4943 6f6c 6c61 626f  mport { ICollabo
+00000370: 7261 7469 7665 4472 6976 652c 2059 4472  rativeDrive, YDr
+00000380: 6976 6520 7d20 6672 6f6d 2027 406a 7570  ive } from '@jup
+00000390: 7974 6572 2f64 6f63 7072 6f76 6964 6572  yter/docprovider
+000003a0: 273b 0a0a 2f2a 2a0a 202a 2054 6865 2063  ';../**. * The c
+000003b0: 6f6d 6d61 6e64 2049 4473 2075 7365 6420  ommand IDs used 
+000003c0: 6279 2074 6865 2066 696c 6520 6272 6f77  by the file brow
+000003d0: 7365 7220 706c 7567 696e 2e0a 202a 2f0a  ser plugin.. */.
+000003e0: 6e61 6d65 7370 6163 6520 436f 6d6d 616e  namespace Comman
+000003f0: 6449 4473 207b 0a20 2065 7870 6f72 7420  dIDs {.  export 
+00000400: 636f 6e73 7420 6f70 656e 5061 7468 203d  const openPath =
+00000410: 2027 6669 6c65 6272 6f77 7365 723a 6f70   'filebrowser:op
+00000420: 656e 2d70 6174 6827 3b0a 7d0a 0a2f 2a2a  en-path';.}../**
+00000430: 0a20 2a20 5468 6520 6465 6661 756c 7420  . * The default 
+00000440: 636f 6c6c 6162 6f72 6174 6976 6520 6472  collaborative dr
+00000450: 6976 6520 7072 6f76 6964 6572 2e0a 202a  ive provider.. *
+00000460: 2f0a 6578 706f 7274 2063 6f6e 7374 2064  /.export const d
+00000470: 7269 7665 3a20 4a75 7079 7465 7246 726f  rive: JupyterFro
+00000480: 6e74 456e 6450 6c75 6769 6e3c 4943 6f6c  ntEndPlugin<ICol
+00000490: 6c61 626f 7261 7469 7665 4472 6976 653e  laborativeDrive>
+000004a0: 203d 207b 0a20 2069 643a 2027 406a 7570   = {.  id: '@jup
+000004b0: 7974 6572 2f64 6f63 7072 6f76 6964 6572  yter/docprovider
+000004c0: 2d65 7874 656e 7369 6f6e 3a64 7269 7665  -extension:drive
+000004d0: 272c 0a20 2064 6573 6372 6970 7469 6f6e  ',.  description
+000004e0: 3a20 2754 6865 2064 6566 6175 6c74 2063  : 'The default c
+000004f0: 6f6c 6c61 626f 7261 7469 7665 2064 7269  ollaborative dri
+00000500: 7665 2070 726f 7669 6465 7227 2c0a 2020  ve provider',.  
+00000510: 7072 6f76 6964 6573 3a20 4943 6f6c 6c61  provides: IColla
+00000520: 626f 7261 7469 7665 4472 6976 652c 0a20  borativeDrive,. 
+00000530: 2072 6571 7569 7265 733a 205b 4954 7261   requires: [ITra
+00000540: 6e73 6c61 746f 725d 2c0a 2020 6f70 7469  nslator],.  opti
+00000550: 6f6e 616c 3a20 5b5d 2c0a 2020 6163 7469  onal: [],.  acti
+00000560: 7661 7465 3a20 280a 2020 2020 6170 703a  vate: (.    app:
+00000570: 204a 7570 7974 6572 4672 6f6e 7445 6e64   JupyterFrontEnd
+00000580: 2c0a 2020 2020 7472 616e 736c 6174 6f72  ,.    translator
+00000590: 3a20 4954 7261 6e73 6c61 746f 720a 2020  : ITranslator.  
+000005a0: 293a 2049 436f 6c6c 6162 6f72 6174 6976  ): ICollaborativ
+000005b0: 6544 7269 7665 203d 3e20 7b0a 2020 2020  eDrive => {.    
+000005c0: 636f 6e73 7420 7472 616e 7320 3d20 7472  const trans = tr
+000005d0: 616e 736c 6174 6f72 2e6c 6f61 6428 276a  anslator.load('j
+000005e0: 7570 7974 6572 5f63 6f6c 6c61 626f 7261  upyter_collabora
+000005f0: 7469 6f6e 2729 3b0a 2020 2020 636f 6e73  tion');.    cons
+00000600: 7420 6472 6976 6520 3d20 6e65 7720 5944  t drive = new YD
+00000610: 7269 7665 2861 7070 2e73 6572 7669 6365  rive(app.service
+00000620: 4d61 6e61 6765 722e 7573 6572 2c20 7472  Manager.user, tr
+00000630: 616e 7329 3b0a 2020 2020 6170 702e 7365  ans);.    app.se
+00000640: 7276 6963 654d 616e 6167 6572 2e63 6f6e  rviceManager.con
+00000650: 7465 6e74 732e 6164 6444 7269 7665 2864  tents.addDrive(d
+00000660: 7269 7665 293b 0a20 2020 2072 6574 7572  rive);.    retur
+00000670: 6e20 6472 6976 653b 0a20 207d 0a7d 3b0a  n drive;.  }.};.
+00000680: 0a2f 2a2a 0a20 2a20 506c 7567 696e 2074  ./**. * Plugin t
+00000690: 6f20 7265 6769 7374 6572 2074 6865 2073  o register the s
+000006a0: 6861 7265 6420 6d6f 6465 6c20 6661 6374  hared model fact
+000006b0: 6f72 7920 666f 7220 7468 6520 636f 6e74  ory for the cont
+000006c0: 656e 7420 7479 7065 2027 6669 6c65 272e  ent type 'file'.
+000006d0: 0a20 2a2f 0a65 7870 6f72 7420 636f 6e73  . */.export cons
+000006e0: 7420 7966 696c 653a 204a 7570 7974 6572  t yfile: Jupyter
+000006f0: 4672 6f6e 7445 6e64 506c 7567 696e 3c76  FrontEndPlugin<v
+00000700: 6f69 643e 203d 207b 0a20 2069 643a 2027  oid> = {.  id: '
+00000710: 406a 7570 7974 6572 2f64 6f63 7072 6f76  @jupyter/docprov
+00000720: 6964 6572 2d65 7874 656e 7369 6f6e 3a79  ider-extension:y
+00000730: 6669 6c65 272c 0a20 2064 6573 6372 6970  file',.  descrip
+00000740: 7469 6f6e 3a0a 2020 2020 2250 6c75 6769  tion:.    "Plugi
+00000750: 6e20 746f 2072 6567 6973 7465 7220 7468  n to register th
+00000760: 6520 7368 6172 6564 206d 6f64 656c 2066  e shared model f
+00000770: 6163 746f 7279 2066 6f72 2074 6865 2063  actory for the c
+00000780: 6f6e 7465 6e74 2074 7970 6520 2766 696c  ontent type 'fil
+00000790: 6527 222c 0a20 2061 7574 6f53 7461 7274  e'",.  autoStart
+000007a0: 3a20 7472 7565 2c0a 2020 7265 7175 6972  : true,.  requir
+000007b0: 6573 3a20 5b49 436f 6c6c 6162 6f72 6174  es: [ICollaborat
+000007c0: 6976 6544 7269 7665 5d2c 0a20 206f 7074  iveDrive],.  opt
+000007d0: 696f 6e61 6c3a 205b 5d2c 0a20 2061 6374  ional: [],.  act
+000007e0: 6976 6174 653a 2028 6170 703a 204a 7570  ivate: (app: Jup
+000007f0: 7974 6572 4672 6f6e 7445 6e64 2c20 6472  yterFrontEnd, dr
+00000800: 6976 653a 2049 436f 6c6c 6162 6f72 6174  ive: ICollaborat
+00000810: 6976 6544 7269 7665 293a 2076 6f69 6420  iveDrive): void 
+00000820: 3d3e 207b 0a20 2020 2063 6f6e 7374 2079  => {.    const y
+00000830: 4669 6c65 4661 6374 6f72 7920 3d20 2829  FileFactory = ()
+00000840: 203d 3e20 7b0a 2020 2020 2020 7265 7475   => {.      retu
+00000850: 726e 206e 6577 2059 4669 6c65 2829 3b0a  rn new YFile();.
+00000860: 2020 2020 7d3b 0a20 2020 2064 7269 7665      };.    drive
+00000870: 2e73 6861 7265 644d 6f64 656c 4661 6374  .sharedModelFact
+00000880: 6f72 792e 7265 6769 7374 6572 446f 6375  ory.registerDocu
+00000890: 6d65 6e74 4661 6374 6f72 7928 2766 696c  mentFactory('fil
+000008a0: 6527 2c20 7946 696c 6546 6163 746f 7279  e', yFileFactory
+000008b0: 293b 0a20 207d 0a7d 3b0a 0a2f 2a2a 0a20  );.  }.};../**. 
+000008c0: 2a20 506c 7567 696e 2074 6f20 7265 6769  * Plugin to regi
+000008d0: 7374 6572 2074 6865 2073 6861 7265 6420  ster the shared 
+000008e0: 6d6f 6465 6c20 6661 6374 6f72 7920 666f  model factory fo
+000008f0: 7220 7468 6520 636f 6e74 656e 7420 7479  r the content ty
+00000900: 7065 2027 6e6f 7465 626f 6f6b 272e 0a20  pe 'notebook'.. 
+00000910: 2a2f 0a65 7870 6f72 7420 636f 6e73 7420  */.export const 
+00000920: 796e 6f74 6562 6f6f 6b3a 204a 7570 7974  ynotebook: Jupyt
+00000930: 6572 4672 6f6e 7445 6e64 506c 7567 696e  erFrontEndPlugin
+00000940: 3c76 6f69 643e 203d 207b 0a20 2069 643a  <void> = {.  id:
+00000950: 2027 406a 7570 7974 6572 2f64 6f63 7072   '@jupyter/docpr
+00000960: 6f76 6964 6572 2d65 7874 656e 7369 6f6e  ovider-extension
+00000970: 3a79 6e6f 7465 626f 6f6b 272c 0a20 2064  :ynotebook',.  d
+00000980: 6573 6372 6970 7469 6f6e 3a0a 2020 2020  escription:.    
+00000990: 2250 6c75 6769 6e20 746f 2072 6567 6973  "Plugin to regis
+000009a0: 7465 7220 7468 6520 7368 6172 6564 206d  ter the shared m
+000009b0: 6f64 656c 2066 6163 746f 7279 2066 6f72  odel factory for
+000009c0: 2074 6865 2063 6f6e 7465 6e74 2074 7970   the content typ
+000009d0: 6520 276e 6f74 6562 6f6f 6b27 222c 0a20  e 'notebook'",. 
+000009e0: 2061 7574 6f53 7461 7274 3a20 7472 7565   autoStart: true
+000009f0: 2c0a 2020 7265 7175 6972 6573 3a20 5b49  ,.  requires: [I
+00000a00: 436f 6c6c 6162 6f72 6174 6976 6544 7269  CollaborativeDri
+00000a10: 7665 5d2c 0a20 206f 7074 696f 6e61 6c3a  ve],.  optional:
+00000a20: 205b 4953 6574 7469 6e67 5265 6769 7374   [ISettingRegist
+00000a30: 7279 5d2c 0a20 2061 6374 6976 6174 653a  ry],.  activate:
+00000a40: 2028 0a20 2020 2061 7070 3a20 4a75 7079   (.    app: Jupy
+00000a50: 7465 7246 726f 6e74 456e 642c 0a20 2020  terFrontEnd,.   
+00000a60: 2064 7269 7665 3a20 4943 6f6c 6c61 626f   drive: ICollabo
+00000a70: 7261 7469 7665 4472 6976 652c 0a20 2020  rativeDrive,.   
+00000a80: 2073 6574 7469 6e67 5265 6769 7374 7279   settingRegistry
+00000a90: 3a20 4953 6574 7469 6e67 5265 6769 7374  : ISettingRegist
+00000aa0: 7279 207c 206e 756c 6c0a 2020 293a 2076  ry | null.  ): v
+00000ab0: 6f69 6420 3d3e 207b 0a20 2020 206c 6574  oid => {.    let
+00000ac0: 2064 6973 6162 6c65 446f 6375 6d65 6e74   disableDocument
+00000ad0: 5769 6465 556e 646f 5265 646f 203d 2074  WideUndoRedo = t
+00000ae0: 7275 653b 0a0a 2020 2020 2f2f 2046 6574  rue;..    // Fet
+00000af0: 6368 2073 6574 7469 6e67 7320 6966 2070  ch settings if p
+00000b00: 6f73 7369 626c 652e 0a20 2020 2069 6620  ossible..    if 
+00000b10: 2873 6574 7469 6e67 5265 6769 7374 7279  (settingRegistry
+00000b20: 2920 7b0a 2020 2020 2020 7365 7474 696e  ) {.      settin
+00000b30: 6752 6567 6973 7472 790a 2020 2020 2020  gRegistry.      
+00000b40: 2020 2e6c 6f61 6428 2740 6a75 7079 7465    .load('@jupyte
+00000b50: 726c 6162 2f6e 6f74 6562 6f6f 6b2d 6578  rlab/notebook-ex
+00000b60: 7465 6e73 696f 6e3a 7472 6163 6b65 7227  tension:tracker'
+00000b70: 290a 2020 2020 2020 2020 2e74 6865 6e28  ).        .then(
+00000b80: 7365 7474 696e 6773 203d 3e20 7b0a 2020  settings => {.  
+00000b90: 2020 2020 2020 2020 636f 6e73 7420 7570          const up
+00000ba0: 6461 7465 5365 7474 696e 6773 203d 2028  dateSettings = (
+00000bb0: 7365 7474 696e 6773 3a20 4953 6574 7469  settings: ISetti
+00000bc0: 6e67 5265 6769 7374 7279 2e49 5365 7474  ngRegistry.ISett
+00000bd0: 696e 6773 2920 3d3e 207b 0a20 2020 2020  ings) => {.     
+00000be0: 2020 2020 2020 2063 6f6e 7374 2065 6e61         const ena
+00000bf0: 626c 6544 6f63 5769 6465 556e 646f 203d  bleDocWideUndo =
+00000c00: 2073 6574 7469 6e67 733f 2e67 6574 280a   settings?.get(.
+00000c10: 2020 2020 2020 2020 2020 2020 2020 2765                'e
+00000c20: 7870 6572 696d 656e 7461 6c45 6e61 626c  xperimentalEnabl
+00000c30: 6544 6f63 756d 656e 7457 6964 6555 6e64  eDocumentWideUnd
+00000c40: 6f52 6564 6f27 0a20 2020 2020 2020 2020  oRedo'.         
+00000c50: 2020 2029 2e63 6f6d 706f 7369 7465 2061     ).composite a
+00000c60: 7320 626f 6f6c 6561 6e3b 0a0a 2020 2020  s boolean;..    
+00000c70: 2020 2020 2020 2020 6469 7361 626c 6544          disableD
+00000c80: 6f63 756d 656e 7457 6964 6555 6e64 6f52  ocumentWideUndoR
+00000c90: 6564 6f20 3d20 2165 6e61 626c 6544 6f63  edo = !enableDoc
+00000ca0: 5769 6465 556e 646f 203f 3f20 7472 7565  WideUndo ?? true
+00000cb0: 3b0a 2020 2020 2020 2020 2020 7d3b 0a0a  ;.          };..
+00000cc0: 2020 2020 2020 2020 2020 7570 6461 7465            update
+00000cd0: 5365 7474 696e 6773 2873 6574 7469 6e67  Settings(setting
+00000ce0: 7329 3b0a 2020 2020 2020 2020 2020 7365  s);.          se
+00000cf0: 7474 696e 6773 2e63 6861 6e67 6564 2e63  ttings.changed.c
+00000d00: 6f6e 6e65 6374 2828 7365 7474 696e 6773  onnect((settings
+00000d10: 3a20 4953 6574 7469 6e67 5265 6769 7374  : ISettingRegist
+00000d20: 7279 2e49 5365 7474 696e 6773 2920 3d3e  ry.ISettings) =>
+00000d30: 0a20 2020 2020 2020 2020 2020 2075 7064  .            upd
+00000d40: 6174 6553 6574 7469 6e67 7328 7365 7474  ateSettings(sett
+00000d50: 696e 6773 290a 2020 2020 2020 2020 2020  ings).          
+00000d60: 293b 0a20 2020 2020 2020 207d 293b 0a20  );.        });. 
+00000d70: 2020 207d 0a0a 2020 2020 636f 6e73 7420     }..    const 
+00000d80: 794e 6f74 6562 6f6f 6b46 6163 746f 7279  yNotebookFactory
+00000d90: 203d 2028 2920 3d3e 207b 0a20 2020 2020   = () => {.     
+00000da0: 2072 6574 7572 6e20 6e65 7720 594e 6f74   return new YNot
+00000db0: 6562 6f6f 6b28 7b0a 2020 2020 2020 2020  ebook({.        
+00000dc0: 6469 7361 626c 6544 6f63 756d 656e 7457  disableDocumentW
+00000dd0: 6964 6555 6e64 6f52 6564 6f0a 2020 2020  ideUndoRedo.    
+00000de0: 2020 7d29 3b0a 2020 2020 7d3b 0a20 2020    });.    };.   
+00000df0: 2064 7269 7665 2e73 6861 7265 644d 6f64   drive.sharedMod
+00000e00: 656c 4661 6374 6f72 792e 7265 6769 7374  elFactory.regist
+00000e10: 6572 446f 6375 6d65 6e74 4661 6374 6f72  erDocumentFactor
+00000e20: 7928 0a20 2020 2020 2027 6e6f 7465 626f  y(.      'notebo
+00000e30: 6f6b 272c 0a20 2020 2020 2079 4e6f 7465  ok',.      yNote
+00000e40: 626f 6f6b 4661 6374 6f72 790a 2020 2020  bookFactory.    
+00000e50: 293b 0a20 207d 0a7d 3b0a 0a2f 2a2a 0a20  );.  }.};../**. 
+00000e60: 2a20 5468 6520 6465 6661 756c 7420 6669  * The default fi
+00000e70: 6c65 2062 726f 7773 6572 2066 6163 746f  le browser facto
+00000e80: 7279 2070 726f 7669 6465 722e 0a20 2a2f  ry provider.. */
+00000e90: 0a65 7870 6f72 7420 636f 6e73 7420 6465  .export const de
+00000ea0: 6661 756c 7446 696c 6542 726f 7773 6572  faultFileBrowser
+00000eb0: 3a20 4a75 7079 7465 7246 726f 6e74 456e  : JupyterFrontEn
+00000ec0: 6450 6c75 6769 6e3c 4944 6566 6175 6c74  dPlugin<IDefault
+00000ed0: 4669 6c65 4272 6f77 7365 723e 203d 207b  FileBrowser> = {
+00000ee0: 0a20 2069 643a 2027 406a 7570 7974 6572  .  id: '@jupyter
+00000ef0: 2f64 6f63 7072 6f76 6964 6572 2d65 7874  /docprovider-ext
+00000f00: 656e 7369 6f6e 3a64 6566 6175 6c74 4669  ension:defaultFi
+00000f10: 6c65 4272 6f77 7365 7227 2c0a 2020 6465  leBrowser',.  de
+00000f20: 7363 7269 7074 696f 6e3a 2027 5468 6520  scription: 'The 
+00000f30: 6465 6661 756c 7420 6669 6c65 2062 726f  default file bro
+00000f40: 7773 6572 2066 6163 746f 7279 2070 726f  wser factory pro
+00000f50: 7669 6465 7227 2c0a 2020 7072 6f76 6964  vider',.  provid
+00000f60: 6573 3a20 4944 6566 6175 6c74 4669 6c65  es: IDefaultFile
+00000f70: 4272 6f77 7365 722c 0a20 2072 6571 7569  Browser,.  requi
+00000f80: 7265 733a 205b 4943 6f6c 6c61 626f 7261  res: [ICollabora
+00000f90: 7469 7665 4472 6976 652c 2049 4669 6c65  tiveDrive, IFile
+00000fa0: 4272 6f77 7365 7246 6163 746f 7279 5d2c  BrowserFactory],
+00000fb0: 0a20 206f 7074 696f 6e61 6c3a 205b 0a20  .  optional: [. 
+00000fc0: 2020 2049 526f 7574 6572 2c0a 2020 2020     IRouter,.    
+00000fd0: 4a75 7079 7465 7246 726f 6e74 456e 642e  JupyterFrontEnd.
+00000fe0: 4954 7265 6552 6573 6f6c 7665 722c 0a20  ITreeResolver,. 
+00000ff0: 2020 2049 4c61 6253 6865 6c6c 2c0a 2020     ILabShell,.  
+00001000: 2020 4953 6574 7469 6e67 5265 6769 7374    ISettingRegist
+00001010: 7279 0a20 205d 2c0a 2020 6163 7469 7661  ry.  ],.  activa
+00001020: 7465 3a20 6173 796e 6320 280a 2020 2020  te: async (.    
+00001030: 6170 703a 204a 7570 7974 6572 4672 6f6e  app: JupyterFron
+00001040: 7445 6e64 2c0a 2020 2020 6472 6976 653a  tEnd,.    drive:
+00001050: 2049 436f 6c6c 6162 6f72 6174 6976 6544   ICollaborativeD
+00001060: 7269 7665 2c0a 2020 2020 6669 6c65 4272  rive,.    fileBr
+00001070: 6f77 7365 7246 6163 746f 7279 3a20 4946  owserFactory: IF
+00001080: 696c 6542 726f 7773 6572 4661 6374 6f72  ileBrowserFactor
+00001090: 792c 0a20 2020 2072 6f75 7465 723a 2049  y,.    router: I
+000010a0: 526f 7574 6572 207c 206e 756c 6c2c 0a20  Router | null,. 
+000010b0: 2020 2074 7265 653a 204a 7570 7974 6572     tree: Jupyter
+000010c0: 4672 6f6e 7445 6e64 2e49 5472 6565 5265  FrontEnd.ITreeRe
+000010d0: 736f 6c76 6572 207c 206e 756c 6c2c 0a20  solver | null,. 
+000010e0: 2020 206c 6162 5368 656c 6c3a 2049 4c61     labShell: ILa
+000010f0: 6253 6865 6c6c 207c 206e 756c 6c0a 2020  bShell | null.  
+00001100: 293a 2050 726f 6d69 7365 3c49 4465 6661  ): Promise<IDefa
+00001110: 756c 7446 696c 6542 726f 7773 6572 3e20  ultFileBrowser> 
+00001120: 3d3e 207b 0a20 2020 2063 6f6e 7374 207b  => {.    const {
+00001130: 2063 6f6d 6d61 6e64 7320 7d20 3d20 6170   commands } = ap
+00001140: 703b 0a0a 2020 2020 6170 702e 7365 7276  p;..    app.serv
+00001150: 6963 654d 616e 6167 6572 2e63 6f6e 7465  iceManager.conte
+00001160: 6e74 732e 6164 6444 7269 7665 2864 7269  nts.addDrive(dri
+00001170: 7665 293b 0a0a 2020 2020 2f2f 204d 616e  ve);..    // Man
+00001180: 7561 6c6c 7920 7265 7374 6f72 6520 616e  ually restore an
+00001190: 6420 6c6f 6164 2074 6865 2064 6566 6175  d load the defau
+000011a0: 6c74 2066 696c 6520 6272 6f77 7365 722e  lt file browser.
+000011b0: 0a20 2020 2063 6f6e 7374 2064 6566 6175  .    const defau
+000011c0: 6c74 4272 6f77 7365 7220 3d20 6669 6c65  ltBrowser = file
+000011d0: 4272 6f77 7365 7246 6163 746f 7279 2e63  BrowserFactory.c
+000011e0: 7265 6174 6546 696c 6542 726f 7773 6572  reateFileBrowser
+000011f0: 2827 6669 6c65 6272 6f77 7365 7227 2c20  ('filebrowser', 
+00001200: 7b0a 2020 2020 2020 6175 746f 3a20 6661  {.      auto: fa
+00001210: 6c73 652c 0a20 2020 2020 2072 6573 746f  lse,.      resto
+00001220: 7265 3a20 6661 6c73 652c 0a20 2020 2020  re: false,.     
+00001230: 2064 7269 7665 4e61 6d65 3a20 6472 6976   driveName: driv
+00001240: 652e 6e61 6d65 0a20 2020 207d 293b 0a20  e.name.    });. 
+00001250: 2020 2076 6f69 6420 5072 6976 6174 652e     void Private.
+00001260: 7265 7374 6f72 6542 726f 7773 6572 280a  restoreBrowser(.
+00001270: 2020 2020 2020 6465 6661 756c 7442 726f        defaultBro
+00001280: 7773 6572 2c0a 2020 2020 2020 636f 6d6d  wser,.      comm
+00001290: 616e 6473 2c0a 2020 2020 2020 726f 7574  ands,.      rout
+000012a0: 6572 2c0a 2020 2020 2020 7472 6565 2c0a  er,.      tree,.
+000012b0: 2020 2020 2020 6c61 6253 6865 6c6c 0a20        labShell. 
+000012c0: 2020 2029 3b0a 0a20 2020 2072 6574 7572     );..    retur
+000012d0: 6e20 6465 6661 756c 7442 726f 7773 6572  n defaultBrowser
+000012e0: 3b0a 2020 7d0a 7d3b 0a0a 2f2a 2a0a 202a  ;.  }.};../**. *
+000012f0: 2054 6865 2064 6566 6175 6c74 2063 6f6c   The default col
+00001300: 6c61 626f 7261 7469 7665 2064 7269 7665  laborative drive
+00001310: 2070 726f 7669 6465 722e 0a20 2a2f 0a65   provider.. */.e
+00001320: 7870 6f72 7420 636f 6e73 7420 6c6f 6767  xport const logg
+00001330: 6572 3a20 4a75 7079 7465 7246 726f 6e74  er: JupyterFront
+00001340: 456e 6450 6c75 6769 6e3c 766f 6964 3e20  EndPlugin<void> 
+00001350: 3d20 7b0a 2020 6964 3a20 2740 6a75 7079  = {.  id: '@jupy
+00001360: 7465 722f 646f 6370 726f 7669 6465 722d  ter/docprovider-
+00001370: 6578 7465 6e73 696f 6e3a 6c6f 6767 6572  extension:logger
+00001380: 272c 0a20 2064 6573 6372 6970 7469 6f6e  ',.  description
+00001390: 3a20 2741 206c 6f67 6769 6e67 2070 6c75  : 'A logging plu
+000013a0: 6769 6e20 666f 7220 6465 6275 6767 696e  gin for debuggin
+000013b0: 6720 7075 7270 6f73 6573 2e27 2c0a 2020  g purposes.',.  
+000013c0: 6175 746f 5374 6172 743a 2074 7275 652c  autoStart: true,
+000013d0: 0a20 206f 7074 696f 6e61 6c3a 205b 494c  .  optional: [IL
+000013e0: 6f67 6765 7252 6567 6973 7472 792c 2049  oggerRegistry, I
+000013f0: 4564 6974 6f72 5472 6163 6b65 722c 2049  EditorTracker, I
+00001400: 4e6f 7465 626f 6f6b 5472 6163 6b65 722c  NotebookTracker,
+00001410: 2049 5472 616e 736c 6174 6f72 5d2c 0a20   ITranslator],. 
+00001420: 2061 6374 6976 6174 653a 2028 0a20 2020   activate: (.   
+00001430: 2061 7070 3a20 4a75 7079 7465 7246 726f   app: JupyterFro
+00001440: 6e74 456e 642c 0a20 2020 206c 6f67 6765  ntEnd,.    logge
+00001450: 7252 6567 6973 7472 793a 2049 4c6f 6767  rRegistry: ILogg
+00001460: 6572 5265 6769 7374 7279 207c 206e 756c  erRegistry | nul
+00001470: 6c2c 0a20 2020 2066 696c 6554 7261 636b  l,.    fileTrack
+00001480: 6572 3a20 4945 6469 746f 7254 7261 636b  er: IEditorTrack
+00001490: 6572 207c 206e 756c 6c2c 0a20 2020 206e  er | null,.    n
+000014a0: 6254 7261 636b 6572 3a20 494e 6f74 6562  bTracker: INoteb
+000014b0: 6f6f 6b54 7261 636b 6572 207c 206e 756c  ookTracker | nul
+000014c0: 6c2c 0a20 2020 2074 7261 6e73 6c61 746f  l,.    translato
+000014d0: 723a 2049 5472 616e 736c 6174 6f72 207c  r: ITranslator |
+000014e0: 206e 756c 6c0a 2020 293a 2076 6f69 6420   null.  ): void 
+000014f0: 3d3e 207b 0a20 2020 2063 6f6e 7374 2074  => {.    const t
+00001500: 7261 6e73 203d 2028 7472 616e 736c 6174  rans = (translat
+00001510: 6f72 203f 3f20 6e75 6c6c 5472 616e 736c  or ?? nullTransl
+00001520: 6174 6f72 292e 6c6f 6164 2827 6a75 7079  ator).load('jupy
+00001530: 7465 725f 636f 6c6c 6162 6f72 6174 696f  ter_collaboratio
+00001540: 6e27 293b 0a20 2020 2063 6f6e 7374 2073  n');.    const s
+00001550: 6368 656d 6149 4420 3d0a 2020 2020 2020  chemaID =.      
+00001560: 2768 7474 7073 3a2f 2f73 6368 656d 612e  'https://schema.
+00001570: 6a75 7079 7465 722e 6f72 672f 6a75 7079  jupyter.org/jupy
+00001580: 7465 725f 636f 6c6c 6162 6f72 6174 696f  ter_collaboratio
+00001590: 6e2f 7365 7373 696f 6e2f 7631 273b 0a0a  n/session/v1';..
+000015a0: 2020 2020 6966 2028 216c 6f67 6765 7252      if (!loggerR
+000015b0: 6567 6973 7472 7929 207b 0a20 2020 2020  egistry) {.     
+000015c0: 2061 7070 2e73 6572 7669 6365 4d61 6e61   app.serviceMana
+000015d0: 6765 722e 6576 656e 7473 2e73 7472 6561  ger.events.strea
+000015e0: 6d2e 636f 6e6e 6563 7428 285f 2c20 656d  m.connect((_, em
+000015f0: 6973 7369 6f6e 2920 3d3e 207b 0a20 2020  ission) => {.   
+00001600: 2020 2020 2069 6620 2865 6d69 7373 696f       if (emissio
+00001610: 6e2e 7363 6865 6d61 5f69 6420 3d3d 3d20  n.schema_id === 
+00001620: 7363 6865 6d61 4944 2920 7b0a 2020 2020  schemaID) {.    
+00001630: 2020 2020 2020 636f 6e73 6f6c 652e 6465        console.de
+00001640: 6275 6728 0a20 2020 2020 2020 2020 2020  bug(.           
+00001650: 2060 5b24 7b65 6d69 7373 696f 6e2e 726f   `[${emission.ro
+00001660: 6f6d 7d28 247b 656d 6973 7369 6f6e 2e70  om}(${emission.p
+00001670: 6174 687d 295d 2024 7b65 6d69 7373 696f  ath})] ${emissio
+00001680: 6e2e 6163 7469 6f6e 203f 3f20 2727 7d3a  n.action ?? ''}:
+00001690: 2024 7b0a 2020 2020 2020 2020 2020 2020   ${.            
+000016a0: 2020 656d 6973 7369 6f6e 2e6d 7367 203f    emission.msg ?
+000016b0: 3f20 2727 0a20 2020 2020 2020 2020 2020  ? ''.           
+000016c0: 207d 600a 2020 2020 2020 2020 2020 293b   }`.          );
+000016d0: 0a0a 2020 2020 2020 2020 2020 6966 2028  ..          if (
+000016e0: 656d 6973 7369 6f6e 2e6c 6576 656c 203d  emission.level =
+000016f0: 3d3d 2027 5741 524e 494e 4727 2920 7b0a  == 'WARNING') {.
+00001700: 2020 2020 2020 2020 2020 2020 7368 6f77              show
+00001710: 4469 616c 6f67 287b 0a20 2020 2020 2020  Dialog({.       
+00001720: 2020 2020 2020 2074 6974 6c65 3a20 7472         title: tr
+00001730: 616e 732e 5f5f 2827 5761 726e 696e 6727  ans.__('Warning'
+00001740: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+00001750: 2062 6f64 793a 2074 7261 6e73 2e5f 5f28   body: trans.__(
+00001760: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001770: 2060 5477 6f20 636f 6c6c 6162 6f72 6174   `Two collaborat
+00001780: 6976 6520 7365 7373 696f 6e73 2061 7265  ive sessions are
+00001790: 2061 6363 6573 7369 6e67 2074 6865 2066   accessing the f
+000017a0: 696c 6520 247b 656d 6973 7369 6f6e 2e70  ile ${emission.p
+000017b0: 6174 687d 2073 696d 756c 7461 6e65 6f75  ath} simultaneou
+000017c0: 736c 792e 0a20 2020 2020 2020 2020 2020  sly..           
+000017d0: 2020 2020 205c 6e4f 7065 6e69 6e67 2074       \nOpening t
+000017e0: 6865 2073 616d 6520 6669 6c65 2075 7369  he same file usi
+000017f0: 6e67 2064 6966 6665 7265 6e74 2076 6965  ng different vie
+00001800: 7773 2073 696d 756c 7461 6e65 6f75 736c  ws simultaneousl
+00001810: 7920 6973 206e 6f74 2073 7570 706f 7274  y is not support
+00001820: 6564 2e20 506c 6561 7365 2c20 636c 6f73  ed. Please, clos
+00001830: 6520 6f6e 6520 7669 6577 3b20 6f74 6865  e one view; othe
+00001840: 7277 6973 652c 2079 6f75 206d 6967 6874  rwise, you might
+00001850: 206c 6f73 6520 736f 6d65 206f 6620 796f   lose some of yo
+00001860: 7572 2070 726f 6772 6573 732e 600a 2020  ur progress.`.  
+00001870: 2020 2020 2020 2020 2020 2020 292c 0a20              ),. 
+00001880: 2020 2020 2020 2020 2020 2020 2062 7574               but
+00001890: 746f 6e73 3a20 5b44 6961 6c6f 672e 6f6b  tons: [Dialog.ok
+000018a0: 4275 7474 6f6e 2829 5d0a 2020 2020 2020  Button()].      
+000018b0: 2020 2020 2020 7d29 3b0a 2020 2020 2020        });.      
+000018c0: 2020 2020 7d0a 2020 2020 2020 2020 7d0a      }.        }.
+000018d0: 2020 2020 2020 7d29 3b0a 0a20 2020 2020        });..     
+000018e0: 2072 6574 7572 6e3b 0a20 2020 207d 0a0a   return;.    }..
+000018f0: 2020 2020 636f 6e73 7420 6c6f 6767 6572      const logger
+00001900: 733a 204d 6170 3c73 7472 696e 672c 2049  s: Map<string, I
+00001910: 4c6f 6767 6572 3e20 3d20 6e65 7720 4d61  Logger> = new Ma
+00001920: 7028 293b 0a0a 2020 2020 636f 6e73 7420  p();..    const 
+00001930: 6164 644c 6f67 6765 7220 3d20 2873 656e  addLogger = (sen
+00001940: 6465 723a 2075 6e6b 6e6f 776e 2c20 646f  der: unknown, do
+00001950: 6375 6d65 6e74 3a20 4944 6f63 756d 656e  cument: IDocumen
+00001960: 7457 6964 6765 7429 203d 3e20 7b0a 2020  tWidget) => {.  
+00001970: 2020 2020 636f 6e73 7420 6c6f 6767 6572      const logger
+00001980: 203d 206c 6f67 6765 7252 6567 6973 7472   = loggerRegistr
+00001990: 792e 6765 744c 6f67 6765 7228 646f 6375  y.getLogger(docu
+000019a0: 6d65 6e74 2e63 6f6e 7465 7874 2e70 6174  ment.context.pat
+000019b0: 6829 3b0a 2020 2020 2020 6c6f 6767 6572  h);.      logger
+000019c0: 732e 7365 7428 646f 6375 6d65 6e74 2e63  s.set(document.c
+000019d0: 6f6e 7465 7874 2e6c 6f63 616c 5061 7468  ontext.localPath
+000019e0: 2c20 6c6f 6767 6572 293b 0a0a 2020 2020  , logger);..    
+000019f0: 2020 646f 6375 6d65 6e74 2e64 6973 706f    document.dispo
+00001a00: 7365 642e 636f 6e6e 6563 7428 646f 6375  sed.connect(docu
+00001a10: 6d65 6e74 203d 3e20 7b0a 2020 2020 2020  ment => {.      
+00001a20: 2020 6c6f 6767 6572 732e 6465 6c65 7465    loggers.delete
+00001a30: 2864 6f63 756d 656e 742e 636f 6e74 6578  (document.contex
+00001a40: 742e 6c6f 6361 6c50 6174 6829 3b0a 2020  t.localPath);.  
+00001a50: 2020 2020 7d29 3b0a 2020 2020 7d3b 0a0a      });.    };..
+00001a60: 2020 2020 6966 2028 6669 6c65 5472 6163      if (fileTrac
+00001a70: 6b65 7229 207b 0a20 2020 2020 2066 696c  ker) {.      fil
+00001a80: 6554 7261 636b 6572 2e77 6964 6765 7441  eTracker.widgetA
+00001a90: 6464 6564 2e63 6f6e 6e65 6374 2861 6464  dded.connect(add
+00001aa0: 4c6f 6767 6572 293b 0a20 2020 207d 0a0a  Logger);.    }..
+00001ab0: 2020 2020 6966 2028 6e62 5472 6163 6b65      if (nbTracke
+00001ac0: 7229 207b 0a20 2020 2020 206e 6254 7261  r) {.      nbTra
+00001ad0: 636b 6572 2e77 6964 6765 7441 6464 6564  cker.widgetAdded
+00001ae0: 2e63 6f6e 6e65 6374 2861 6464 4c6f 6767  .connect(addLogg
+00001af0: 6572 293b 0a20 2020 207d 0a0a 2020 2020  er);.    }..    
+00001b00: 766f 6964 2028 6173 796e 6320 2829 203d  void (async () =
+00001b10: 3e20 7b0a 2020 2020 2020 636f 6e73 7420  > {.      const 
+00001b20: 7b20 6576 656e 7473 207d 203d 2061 7070  { events } = app
+00001b30: 2e73 6572 7669 6365 4d61 6e61 6765 723b  .serviceManager;
+00001b40: 0a20 2020 2020 2066 6f72 2061 7761 6974  .      for await
+00001b50: 2028 636f 6e73 7420 656d 6973 7369 6f6e   (const emission
+00001b60: 206f 6620 6576 656e 7473 2e73 7472 6561   of events.strea
+00001b70: 6d29 207b 0a20 2020 2020 2020 2069 6620  m) {.        if 
+00001b80: 2865 6d69 7373 696f 6e2e 7363 6865 6d61  (emission.schema
+00001b90: 5f69 6420 3d3d 3d20 7363 6865 6d61 4944  _id === schemaID
+00001ba0: 2920 7b0a 2020 2020 2020 2020 2020 636f  ) {.          co
+00001bb0: 6e73 7420 6c6f 6767 6572 203d 206c 6f67  nst logger = log
+00001bc0: 6765 7273 2e67 6574 2865 6d69 7373 696f  gers.get(emissio
+00001bd0: 6e2e 7061 7468 2061 7320 7374 7269 6e67  n.path as string
+00001be0: 293b 0a0a 2020 2020 2020 2020 2020 6c6f  );..          lo
+00001bf0: 6767 6572 3f2e 6c6f 6728 7b0a 2020 2020  gger?.log({.    
+00001c00: 2020 2020 2020 2020 7479 7065 3a20 2774          type: 't
+00001c10: 6578 7427 2c0a 2020 2020 2020 2020 2020  ext',.          
+00001c20: 2020 6c65 7665 6c3a 2028 656d 6973 7369    level: (emissi
+00001c30: 6f6e 2e6c 6576 656c 2061 7320 7374 7269  on.level as stri
+00001c40: 6e67 292e 746f 4c6f 7765 7243 6173 6528  ng).toLowerCase(
+00001c50: 2920 6173 2061 6e79 2c0a 2020 2020 2020  ) as any,.      
+00001c60: 2020 2020 2020 6461 7461 3a20 605b 247b        data: `[${
+00001c70: 656d 6973 7369 6f6e 2e72 6f6f 6d7d 5d20  emission.room}] 
+00001c80: 247b 656d 6973 7369 6f6e 2e61 6374 696f  ${emission.actio
+00001c90: 6e20 3f3f 2027 277d 3a20 247b 0a20 2020  n ?? ''}: ${.   
+00001ca0: 2020 2020 2020 2020 2020 2065 6d69 7373             emiss
+00001cb0: 696f 6e2e 6d73 6720 3f3f 2027 270a 2020  ion.msg ?? ''.  
+00001cc0: 2020 2020 2020 2020 2020 7d60 0a20 2020            }`.   
+00001cd0: 2020 2020 2020 207d 293b 0a0a 2020 2020         });..    
+00001ce0: 2020 2020 2020 6966 2028 656d 6973 7369        if (emissi
+00001cf0: 6f6e 2e6c 6576 656c 203d 3d3d 2027 5741  on.level === 'WA
+00001d00: 524e 494e 4727 2920 7b0a 2020 2020 2020  RNING') {.      
+00001d10: 2020 2020 2020 7368 6f77 4469 616c 6f67        showDialog
+00001d20: 287b 0a20 2020 2020 2020 2020 2020 2020  ({.             
+00001d30: 2074 6974 6c65 3a20 7472 616e 732e 5f5f   title: trans.__
+00001d40: 2827 5761 726e 696e 6727 292c 0a20 2020  ('Warning'),.   
+00001d50: 2020 2020 2020 2020 2020 2062 6f64 793a             body:
+00001d60: 2074 7261 6e73 2e5f 5f28 0a20 2020 2020   trans.__(.     
+00001d70: 2020 2020 2020 2020 2020 2060 5477 6f20             `Two 
+00001d80: 636f 6c6c 6162 6f72 6174 6976 6520 7365  collaborative se
+00001d90: 7373 696f 6e73 2061 7265 2061 6363 6573  ssions are acces
+00001da0: 7369 6e67 2074 6865 2066 696c 6520 2531  sing the file %1
+00001db0: 2073 696d 756c 7461 6e65 6f75 736c 792e   simultaneously.
+00001dc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001dd0: 205c 6e4f 7065 6e69 6e67 2061 2064 6f63   \nOpening a doc
+00001de0: 756d 656e 7420 7769 7468 206d 756c 7469  ument with multi
+00001df0: 706c 6520 7669 6577 7320 7369 6d75 6c74  ple views simult
+00001e00: 616e 656f 7573 6c79 2069 7320 6e6f 7420  aneously is not 
+00001e10: 7375 7070 6f72 7465 642e 2050 6c65 6173  supported. Pleas
+00001e20: 6520 636c 6f73 6520 6f6e 6520 7669 6577  e close one view
+00001e30: 3b20 6f74 6865 7277 6973 652c 2079 6f75  ; otherwise, you
+00001e40: 206d 6967 6874 206c 6f73 6520 736f 6d65   might lose some
+00001e50: 206f 6620 796f 7572 2070 726f 6772 6573   of your progres
+00001e60: 732e 602c 0a20 2020 2020 2020 2020 2020  s.`,.           
+00001e70: 2020 2020 2065 6d69 7373 696f 6e2e 7061       emission.pa
+00001e80: 7468 0a20 2020 2020 2020 2020 2020 2020  th.             
+00001e90: 2029 2c0a 2020 2020 2020 2020 2020 2020   ),.            
+00001ea0: 2020 6275 7474 6f6e 733a 205b 4469 616c    buttons: [Dial
+00001eb0: 6f67 2e77 6172 6e42 7574 746f 6e28 7b20  og.warnButton({ 
+00001ec0: 6c61 6265 6c3a 2074 7261 6e73 2e5f 5f28  label: trans.__(
+00001ed0: 274f 6b27 2920 7d29 5d0a 2020 2020 2020  'Ok') })].      
+00001ee0: 2020 2020 2020 7d29 3b0a 2020 2020 2020        });.      
+00001ef0: 2020 2020 7d0a 2020 2020 2020 2020 7d0a      }.        }.
+00001f00: 2020 2020 2020 7d0a 2020 2020 7d29 2829        }.    })()
+00001f10: 3b0a 2020 7d0a 7d3b 0a0a 6e61 6d65 7370  ;.  }.};..namesp
+00001f20: 6163 6520 5072 6976 6174 6520 7b0a 2020  ace Private {.  
+00001f30: 2f2a 2a0a 2020 202a 2052 6573 746f 7265  /**.   * Restore
+00001f40: 7320 6669 6c65 2062 726f 7773 6572 2073  s file browser s
+00001f50: 7461 7465 2061 6e64 206f 7665 7272 6964  tate and overrid
+00001f60: 6573 2073 7461 7465 2069 6620 7472 6565  es state if tree
+00001f70: 2072 6573 6f6c 7665 7220 7265 736f 6c76   resolver resolv
+00001f80: 6573 2e0a 2020 202a 2f0a 2020 6578 706f  es..   */.  expo
+00001f90: 7274 2061 7379 6e63 2066 756e 6374 696f  rt async functio
+00001fa0: 6e20 7265 7374 6f72 6542 726f 7773 6572  n restoreBrowser
+00001fb0: 280a 2020 2020 6272 6f77 7365 723a 2046  (.    browser: F
+00001fc0: 696c 6542 726f 7773 6572 2c0a 2020 2020  ileBrowser,.    
+00001fd0: 636f 6d6d 616e 6473 3a20 436f 6d6d 616e  commands: Comman
+00001fe0: 6452 6567 6973 7472 792c 0a20 2020 2072  dRegistry,.    r
+00001ff0: 6f75 7465 723a 2049 526f 7574 6572 207c  outer: IRouter |
+00002000: 206e 756c 6c2c 0a20 2020 2074 7265 653a   null,.    tree:
+00002010: 204a 7570 7974 6572 4672 6f6e 7445 6e64   JupyterFrontEnd
+00002020: 2e49 5472 6565 5265 736f 6c76 6572 207c  .ITreeResolver |
+00002030: 206e 756c 6c2c 0a20 2020 206c 6162 5368   null,.    labSh
+00002040: 656c 6c3a 2049 4c61 6253 6865 6c6c 207c  ell: ILabShell |
+00002050: 206e 756c 6c0a 2020 293a 2050 726f 6d69   null.  ): Promi
+00002060: 7365 3c76 6f69 643e 207b 0a20 2020 2063  se<void> {.    c
+00002070: 6f6e 7374 2072 6573 746f 7269 6e67 203d  onst restoring =
+00002080: 2027 6a70 2d6d 6f64 2d72 6573 746f 7269   'jp-mod-restori
+00002090: 6e67 273b 0a0a 2020 2020 6272 6f77 7365  ng';..    browse
+000020a0: 722e 6164 6443 6c61 7373 2872 6573 746f  r.addClass(resto
+000020b0: 7269 6e67 293b 0a0a 2020 2020 6966 2028  ring);..    if (
+000020c0: 2172 6f75 7465 7229 207b 0a20 2020 2020  !router) {.     
+000020d0: 2061 7761 6974 2062 726f 7773 6572 2e6d   await browser.m
+000020e0: 6f64 656c 2e72 6573 746f 7265 2862 726f  odel.restore(bro
+000020f0: 7773 6572 2e69 6429 3b0a 2020 2020 2020  wser.id);.      
+00002100: 6177 6169 7420 6272 6f77 7365 722e 6d6f  await browser.mo
+00002110: 6465 6c2e 7265 6672 6573 6828 293b 0a20  del.refresh();. 
+00002120: 2020 2020 2062 726f 7773 6572 2e72 656d       browser.rem
+00002130: 6f76 6543 6c61 7373 2872 6573 746f 7269  oveClass(restori
+00002140: 6e67 293b 0a20 2020 2020 2072 6574 7572  ng);.      retur
+00002150: 6e3b 0a20 2020 207d 0a0a 2020 2020 636f  n;.    }..    co
+00002160: 6e73 7420 6c69 7374 656e 6572 203d 2061  nst listener = a
+00002170: 7379 6e63 2028 2920 3d3e 207b 0a20 2020  sync () => {.   
+00002180: 2020 2072 6f75 7465 722e 726f 7574 6564     router.routed
+00002190: 2e64 6973 636f 6e6e 6563 7428 6c69 7374  .disconnect(list
+000021a0: 656e 6572 293b 0a0a 2020 2020 2020 636f  ener);..      co
+000021b0: 6e73 7420 7061 7468 7320 3d20 6177 6169  nst paths = awai
+000021c0: 7420 7472 6565 3f2e 7061 7468 733b 0a20  t tree?.paths;. 
+000021d0: 2020 2020 2069 6620 2870 6174 6873 3f2e       if (paths?.
+000021e0: 6669 6c65 207c 7c20 7061 7468 733f 2e62  file || paths?.b
+000021f0: 726f 7773 6572 2920 7b0a 2020 2020 2020  rowser) {.      
+00002200: 2020 2f2f 2052 6573 746f 7265 2074 6865    // Restore the
+00002210: 206d 6f64 656c 2077 6974 686f 7574 2070   model without p
+00002220: 6f70 756c 6174 696e 6720 6974 2e0a 2020  opulating it..  
+00002230: 2020 2020 2020 6177 6169 7420 6272 6f77        await brow
+00002240: 7365 722e 6d6f 6465 6c2e 7265 7374 6f72  ser.model.restor
+00002250: 6528 6272 6f77 7365 722e 6964 2c20 6661  e(browser.id, fa
+00002260: 6c73 6529 3b0a 2020 2020 2020 2020 6966  lse);.        if
+00002270: 2028 7061 7468 732e 6669 6c65 2920 7b0a   (paths.file) {.
+00002280: 2020 2020 2020 2020 2020 6177 6169 7420            await 
+00002290: 636f 6d6d 616e 6473 2e65 7865 6375 7465  commands.execute
+000022a0: 2843 6f6d 6d61 6e64 4944 732e 6f70 656e  (CommandIDs.open
+000022b0: 5061 7468 2c20 7b0a 2020 2020 2020 2020  Path, {.        
+000022c0: 2020 2020 7061 7468 3a20 7061 7468 732e      path: paths.
+000022d0: 6669 6c65 2c0a 2020 2020 2020 2020 2020  file,.          
+000022e0: 2020 646f 6e74 5368 6f77 4272 6f77 7365    dontShowBrowse
+000022f0: 723a 2074 7275 650a 2020 2020 2020 2020  r: true.        
+00002300: 2020 7d29 3b0a 2020 2020 2020 2020 7d0a    });.        }.
+00002310: 2020 2020 2020 2020 6966 2028 7061 7468          if (path
+00002320: 732e 6272 6f77 7365 7229 207b 0a20 2020  s.browser) {.   
+00002330: 2020 2020 2020 2061 7761 6974 2063 6f6d         await com
+00002340: 6d61 6e64 732e 6578 6563 7574 6528 436f  mands.execute(Co
+00002350: 6d6d 616e 6449 4473 2e6f 7065 6e50 6174  mmandIDs.openPat
+00002360: 682c 207b 0a20 2020 2020 2020 2020 2020  h, {.           
+00002370: 2070 6174 683a 2070 6174 6873 2e62 726f   path: paths.bro
+00002380: 7773 6572 2c0a 2020 2020 2020 2020 2020  wser,.          
+00002390: 2020 646f 6e74 5368 6f77 4272 6f77 7365    dontShowBrowse
+000023a0: 723a 2074 7275 650a 2020 2020 2020 2020  r: true.        
+000023b0: 2020 7d29 3b0a 2020 2020 2020 2020 7d0a    });.        }.
+000023c0: 2020 2020 2020 7d20 656c 7365 207b 0a20        } else {. 
+000023d0: 2020 2020 2020 2061 7761 6974 2062 726f         await bro
+000023e0: 7773 6572 2e6d 6f64 656c 2e72 6573 746f  wser.model.resto
+000023f0: 7265 2862 726f 7773 6572 2e69 6429 3b0a  re(browser.id);.
+00002400: 2020 2020 2020 2020 6177 6169 7420 6272          await br
+00002410: 6f77 7365 722e 6d6f 6465 6c2e 7265 6672  owser.model.refr
+00002420: 6573 6828 293b 0a20 2020 2020 207d 0a20  esh();.      }. 
+00002430: 2020 2020 2062 726f 7773 6572 2e72 656d       browser.rem
+00002440: 6f76 6543 6c61 7373 2872 6573 746f 7269  oveClass(restori
+00002450: 6e67 293b 0a0a 2020 2020 2020 6966 2028  ng);..      if (
+00002460: 6c61 6253 6865 6c6c 3f2e 6973 456d 7074  labShell?.isEmpt
+00002470: 7928 276d 6169 6e27 2929 207b 0a20 2020  y('main')) {.   
+00002480: 2020 2020 2076 6f69 6420 636f 6d6d 616e       void comman
+00002490: 6473 2e65 7865 6375 7465 2827 6c61 756e  ds.execute('laun
+000024a0: 6368 6572 3a63 7265 6174 6527 293b 0a20  cher:create');. 
+000024b0: 2020 2020 207d 0a20 2020 207d 3b0a 2020       }.    };.  
+000024c0: 2020 726f 7574 6572 2e72 6f75 7465 642e    router.routed.
+000024d0: 636f 6e6e 6563 7428 6c69 7374 656e 6572  connect(listener
+000024e0: 293b 0a20 207d 0a7d 0a                   );.  }.}.
```

### Comparing `jupyter_collaboration_ui-1.0.0a0/packages/docprovider-extension/src/index.ts` & `jupyter_collaboration_ui-1.0.0a1/packages/docprovider-extension/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration_ui-1.0.0a0/.gitignore` & `jupyter_collaboration_ui-1.0.0a1/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration_ui-1.0.0a0/LICENSE` & `jupyter_collaboration_ui-1.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration_ui-1.0.0a0/pyproject.toml` & `jupyter_collaboration_ui-1.0.0a1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration_ui-1.0.0a0/PKG-INFO` & `jupyter_collaboration_ui-1.0.0a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jupyter-collaboration-ui
-Version: 1.0.0a0
+Version: 1.0.0a1
 Summary: JupyterLab/Jupyter Notebook 7+ extension providing user interface integration for real time collaboration
 Project-URL: Documentation, https://jupyterlab-realtime-collaboration.readthedocs.io/
 Project-URL: Repository, https://github.com/jupyterlab/jupyter-collaboration
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: # Licensing terms
         
         This project is licensed under the terms of the Modified BSD License
```

