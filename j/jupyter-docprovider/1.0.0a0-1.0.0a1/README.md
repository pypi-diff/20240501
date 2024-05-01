# Comparing `tmp/jupyter_docprovider-1.0.0a0.tar.gz` & `tmp/jupyter_docprovider-1.0.0a1.tar.gz`

## Comparing `jupyter_docprovider-1.0.0a0.tar` & `jupyter_docprovider-1.0.0a1.tar`

### file list

```diff
@@ -1,1720 +1,40 @@
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/install.json
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/setup.py
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/jupyter_docprovider/__init__.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/jupyter_docprovider/_version.py
--rw-r--r--   0        0        0     3769 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/jupyter_docprovider/labextension/package.json
--rw-r--r--   0        0        0     5274 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/jupyter_docprovider/labextension/static/341.3263d2726bd17de1c784.js
--rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/jupyter_docprovider/labextension/static/422.3ab44960b241aac9f303.js
--rw-r--r--   0        0        0     5558 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/jupyter_docprovider/labextension/static/544.31cdd3fa47e3d8404c4e.js
--rw-r--r--   0        0        0     5274 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/jupyter_docprovider/labextension/static/722.2c1eed8483724a302f59.js
--rw-r--r--   0        0        0     8193 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/jupyter_docprovider/labextension/static/944.80e0d65b220a1dfdc0ff.js
--rw-r--r--   0        0        0    13097 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/jupyter_docprovider/labextension/static/994.c290665e94ae9503337f.js
--rw-r--r--   0        0        0     8491 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/jupyter_docprovider/labextension/static/remoteEntry.2108b01380418facade4.js
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/jupyter_docprovider/labextension/static/style.js
--rw-r--r--   0        0        0     7762 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/jupyter_docprovider/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/README.md
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/package.json
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/tsconfig.json
--rw-r--r--   0        0        0    59498 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/tsconfig.tsbuildinfo
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/lib/collaboratorspanel.d.ts
--rw-r--r--   0        0        0     3630 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/lib/collaboratorspanel.js
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/lib/components.d.ts
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/lib/components.js
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/lib/cursors.d.ts
--rw-r--r--   0        0        0    11806 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/lib/cursors.js
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/lib/index.d.ts
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/lib/index.js
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/lib/menu.d.ts
--rw-r--r--   0        0        0     2531 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/lib/menu.js
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/lib/sharedlink.d.ts
--rw-r--r--   0        0        0     5465 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/lib/sharedlink.js
--rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/lib/tokens.d.ts
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/lib/tokens.js
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/lib/userinfopanel.d.ts
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/lib/userinfopanel.js
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/observables/README.md
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/observables/package.json
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/observables/lib/index.d.ts
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/observables/lib/index.js
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/observables/lib/index.js.map
--rw-r--r--   0        0        0    11923 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/observables/lib/modeldb.d.ts
--rw-r--r--   0        0        0     7771 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/observables/lib/modeldb.js
--rw-r--r--   0        0        0     4552 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/observables/lib/modeldb.js.map
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/observables/lib/observablejson.d.ts
--rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/observables/lib/observablejson.js
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/observables/lib/observablejson.js.map
--rw-r--r--   0        0        0    13574 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/observables/lib/observablelist.d.ts
--rw-r--r--   0        0        0    10600 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/observables/lib/observablelist.js
--rw-r--r--   0        0        0     5415 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/observables/lib/observablelist.js.map
--rw-r--r--   0        0        0     5533 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/observables/lib/observablemap.d.ts
--rw-r--r--   0        0        0     4474 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/observables/lib/observablemap.js
--rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/observables/lib/observablemap.js.map
--rw-r--r--   0        0        0     3598 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/observables/lib/observablestring.d.ts
--rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/observables/lib/observablestring.js
--rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/observables/lib/observablestring.js.map
--rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/observables/lib/undoablelist.d.ts
--rw-r--r--   0        0        0     6313 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/observables/lib/undoablelist.js
--rw-r--r--   0        0        0     5042 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/observables/lib/undoablelist.js.map
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/observables/src/index.ts
--rw-r--r--   0        0        0    13906 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/observables/src/modeldb.ts
--rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/observables/src/observablejson.ts
--rw-r--r--   0        0        0    16451 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/observables/src/observablelist.ts
--rw-r--r--   0        0        0     7293 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/observables/src/observablemap.ts
--rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/observables/src/observablestring.ts
--rw-r--r--   0        0        0     6938 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/observables/src/undoablelist.ts
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/rendermime-interfaces/README.md
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/rendermime-interfaces/package.json
--rw-r--r--   0        0        0    20160 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/rendermime-interfaces/lib/index.d.ts
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/rendermime-interfaces/lib/index.js
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/rendermime-interfaces/lib/index.js.map
--rw-r--r--   0        0        0    18715 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/rendermime-interfaces/src/index.ts
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/statedb/package.json
--rw-r--r--   0        0        0     2803 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/statedb/lib/dataconnector.d.ts
--rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/statedb/lib/dataconnector.js
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/statedb/lib/dataconnector.js.map
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/statedb/lib/index.d.ts
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/statedb/lib/index.js
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/statedb/lib/index.js.map
--rw-r--r--   0        0        0     8115 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/statedb/lib/interfaces.d.ts
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/statedb/lib/interfaces.js
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/statedb/lib/interfaces.js.map
--rw-r--r--   0        0        0     4814 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/statedb/lib/restorablepool.d.ts
--rw-r--r--   0        0        0     9787 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/statedb/lib/restorablepool.js
--rw-r--r--   0        0        0     6469 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/statedb/lib/restorablepool.js.map
--rw-r--r--   0        0        0     6621 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/statedb/lib/statedb.d.ts
--rw-r--r--   0        0        0     7682 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/statedb/lib/statedb.js
--rw-r--r--   0        0        0     4490 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/statedb/lib/statedb.js.map
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/statedb/lib/tokens.d.ts
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/statedb/lib/tokens.js
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/statedb/lib/tokens.js.map
--rw-r--r--   0        0        0     3053 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/statedb/src/dataconnector.ts
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/statedb/src/index.ts
--rw-r--r--   0        0        0     7839 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/statedb/src/interfaces.ts
--rw-r--r--   0        0        0     9580 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/statedb/src/restorablepool.ts
--rw-r--r--   0        0        0     9489 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/statedb/src/statedb.ts
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/statedb/src/tokens.ts
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/translation/README.md
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/translation/package.json
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/translation/lib/base.d.ts
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/translation/lib/base.js
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/translation/lib/base.js.map
--rw-r--r--   0        0        0    10433 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/translation/lib/gettext.d.ts
--rw-r--r--   0        0        0    16610 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/translation/lib/gettext.js
--rw-r--r--   0        0        0     8576 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/translation/lib/gettext.js.map
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/translation/lib/index.d.ts
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/translation/lib/index.js
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/translation/lib/index.js.map
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/translation/lib/manager.d.ts
--rw-r--r--   0        0        0     3582 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/translation/lib/manager.js
--rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/translation/lib/manager.js.map
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/translation/lib/server.d.ts
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/translation/lib/server.js
--rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/translation/lib/server.js.map
--rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/translation/lib/tokens.d.ts
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/translation/lib/tokens.js
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/translation/lib/tokens.js.map
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/translation/lib/utils.d.ts
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/translation/lib/utils.js
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/translation/lib/utils.js.map
--rw-r--r--   0        0        0     2247 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/translation/src/base.ts
--rw-r--r--   0        0        0    18944 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/translation/src/gettext.ts
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/translation/src/index.ts
--rw-r--r--   0        0        0     3303 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/translation/src/manager.ts
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/translation/src/server.ts
--rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/translation/src/tokens.ts
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/translation/src/utils.ts
--rw-r--r--   0        0        0    11754 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/README.md
--rw-r--r--   0        0        0     2477 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/package.json
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/FormRendererRegistry.d.ts
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/FormRendererRegistry.js
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/FormRendererRegistry.js.map
--rw-r--r--   0        0        0     3835 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/hoverbox.d.ts
--rw-r--r--   0        0        0    10279 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/hoverbox.js
--rw-r--r--   0        0        0     7792 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/hoverbox.js.map
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/index.d.ts
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/index.js
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/index.js.map
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/tokens.d.ts
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/tokens.js
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/tokens.js.map
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/utils.d.ts
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/utils.js
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/utils.js.map
--rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/accordiontoolbar.d.ts
--rw-r--r--   0        0        0     7922 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/accordiontoolbar.js
--rw-r--r--   0        0        0     3750 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/accordiontoolbar.js.map
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/button.d.ts
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/button.js
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/button.js.map
--rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/collapser.d.ts
--rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/collapser.js
--rw-r--r--   0        0        0     3882 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/collapser.js.map
--rw-r--r--   0        0        0     3450 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/form.d.ts
--rw-r--r--   0        0        0    15525 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/form.js
--rw-r--r--   0        0        0    11514 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/form.js.map
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/htmlselect.d.ts
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/htmlselect.js
--rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/htmlselect.js.map
--rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/iframe.d.ts
--rw-r--r--   0        0        0     2749 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/iframe.js
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/iframe.js.map
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/index.d.ts
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/index.js
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/index.js.map
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/inputgroup.d.ts
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/inputgroup.js
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/inputgroup.js.map
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/interface.d.ts
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/interface.js
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/interface.js.map
--rw-r--r--   0        0        0     4385 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/menu.d.ts
--rw-r--r--   0        0        0     8343 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/menu.js
--rw-r--r--   0        0        0     5842 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/menu.js.map
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/panelwithtoolbar.d.ts
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/panelwithtoolbar.js
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/panelwithtoolbar.js.map
--rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/search.d.ts
--rw-r--r--   0        0        0     3780 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/search.js
--rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/search.js.map
--rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/sidepanel.d.ts
--rw-r--r--   0        0        0     3189 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/sidepanel.js
--rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/sidepanel.js.map
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/spinner.d.ts
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/spinner.js
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/spinner.js.map
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/styling.d.ts
--rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/styling.js
--rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/styling.js.map
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/switch.d.ts
--rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/switch.js
--rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/switch.js.map
--rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/table.d.ts
--rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/table.js
--rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/table.js.map
--rw-r--r--   0        0        0    14473 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/toolbar.d.ts
--rw-r--r--   0        0        0    37396 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/toolbar.js
--rw-r--r--   0        0        0    23630 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/toolbar.js.map
--rw-r--r--   0        0        0     5635 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/vdom.d.ts
--rw-r--r--   0        0        0     6383 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/vdom.js
--rw-r--r--   0        0        0     3921 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/vdom.js.map
--rw-r--r--   0        0        0    28187 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/windowedlist.d.ts
--rw-r--r--   0        0        0    53471 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/windowedlist.js
--rw-r--r--   0        0        0    32391 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/components/windowedlist.js.map
--rw-r--r--   0        0        0     4514 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/icon/iconimports.d.ts
--rw-r--r--   0        0        0    17726 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/icon/iconimports.js
--rw-r--r--   0        0        0    14441 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/icon/iconimports.js.map
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/icon/index.d.ts
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/icon/index.js
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/icon/index.js.map
--rw-r--r--   0        0        0    11503 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/icon/labicon.d.ts
--rw-r--r--   0        0        0    25278 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/icon/labicon.js
--rw-r--r--   0        0        0    14573 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/icon/labicon.js.map
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/icon/widgets/commandpalettesvg.d.ts
--rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/icon/widgets/commandpalettesvg.js
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/icon/widgets/commandpalettesvg.js.map
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/icon/widgets/index.d.ts
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/icon/widgets/index.js
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/icon/widgets/index.js.map
--rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/icon/widgets/menusvg.d.ts
--rw-r--r--   0        0        0     6138 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/icon/widgets/menusvg.js
--rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/icon/widgets/menusvg.js.map
--rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/icon/widgets/tabbarsvg.d.ts
--rw-r--r--   0        0        0     3788 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/icon/widgets/tabbarsvg.js
--rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/icon/widgets/tabbarsvg.js.map
--rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/style/icon.d.ts
--rw-r--r--   0        0        0    11068 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/style/icon.js
--rw-r--r--   0        0        0     7175 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/style/icon.js.map
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/style/index.d.ts
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/style/index.js
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/lib/style/index.js.map
--rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/src/FormRendererRegistry.tsx
--rw-r--r--   0        0        0    11545 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/src/hoverbox.ts
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/src/index.ts
--rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/src/svg.d.ts
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/src/tokens.ts
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/src/utils.ts
--rw-r--r--   0        0        0     7363 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/src/components/accordiontoolbar.ts
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/src/components/button.tsx
--rw-r--r--   0        0        0     4821 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/src/components/collapser.ts
--rw-r--r--   0        0        0    18987 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/src/components/form.tsx
--rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/src/components/htmlselect.tsx
--rw-r--r--   0        0        0     4216 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/src/components/iframe.ts
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/src/components/index.ts
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/src/components/inputgroup.tsx
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/src/components/interface.ts
--rw-r--r--   0        0        0    10224 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/src/components/menu.ts
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/src/components/panelwithtoolbar.ts
--rw-r--r--   0        0        0     4914 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/src/components/search.tsx
--rw-r--r--   0        0        0     4161 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/src/components/sidepanel.ts
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/src/components/spinner.ts
--rw-r--r--   0        0        0     2995 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/src/components/styling.ts
--rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/src/components/switch.ts
--rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/src/components/table.tsx
--rw-r--r--   0        0        0    37219 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/src/components/toolbar.tsx
--rw-r--r--   0        0        0     8376 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/src/components/vdom.ts
--rw-r--r--   0        0        0    59996 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/src/components/windowedlist.ts
--rw-r--r--   0        0        0    17691 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/src/icon/iconimports.ts
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/src/icon/index.ts
--rw-r--r--   0        0        0    28069 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/src/icon/labicon.tsx
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/src/icon/widgets/commandpalettesvg.ts
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/src/icon/widgets/index.ts
--rw-r--r--   0        0        0     5952 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/src/icon/widgets/menusvg.ts
--rw-r--r--   0        0        0     3543 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/src/icon/widgets/tabbarsvg.ts
--rw-r--r--   0        0        0    13354 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/src/style/icon.ts
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/src/style/index.ts
--rw-r--r--   0        0        0     4209 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/base.css
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/collapse.css
--rw-r--r--   0        0        0    13082 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/deprecated.css
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/deprecatedExtra.css
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/hoverbox.css
--rw-r--r--   0        0        0     6108 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons.css
--rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/iconsalt.css
--rw-r--r--   0        0        0     4762 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/iconshover.css
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/iframe.css
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/index.css
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/index.js
--rw-r--r--   0        0        0     5704 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/rjsfTemplates.css
--rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/sidepanel.css
--rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/spinner.css
--rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/styling.css
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/switch.css
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/tabbar.css
--rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/table.css
--rw-r--r--   0        0        0     3401 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/toolbar.css
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/windowedlist.css
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/debug/bad.svg
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/debug/blank.svg
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/deprecated/check-disabled.svg
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/error.svg
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/history.svg
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/info.svg
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/lock.svg
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/arrow/caret-down-empty-thin.svg
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/arrow/caret-down-empty.svg
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/arrow/caret-down.svg
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/arrow/caret-left.svg
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/arrow/caret-right.svg
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/arrow/caret-up-empty-thin.svg
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/arrow/caret-up.svg
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/filetype/console.svg
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/filetype/file.svg
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/filetype/folder-favorite.svg
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/filetype/folder.svg
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/filetype/home.svg
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/filetype/html5.svg
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/filetype/image.svg
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/filetype/inspector.svg
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/filetype/json.svg
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/filetype/julia.svg
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/filetype/keyboard.svg
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/filetype/launcher.svg
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/filetype/markdown.svg
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/filetype/mermaid.svg
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/filetype/notebook.svg
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/filetype/pdf.svg
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/filetype/python.svg
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/filetype/r-kernel.svg
--rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/filetype/react.svg
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/filetype/settings.svg
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/filetype/spreadsheet.svg
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/filetype/text-editor.svg
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/filetype/vega.svg
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/filetype/yaml.svg
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/jupyter/jupyter-favicon.svg
--rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/jupyter/jupyter.svg
--rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/jupyter/jupyterlab-wordmark.svg
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/licenses/copyright.svg
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/lsp/code-check.svg
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/output/collapse.svg
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/output/expand.svg
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/search/case-sensitive.svg
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/search/filter-dot.svg
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/search/filter.svg
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/search/regex.svg
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/search/word.svg
--rw-r--r--   0        0        0     2430 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/sidebar/build.svg
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/sidebar/extension.svg
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/sidebar/palette.svg
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/sidebar/running.svg
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/sidebar/share.svg
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/sidebar/tab.svg
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/sidebar/toc.svg
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/sidebar/user.svg
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/sidebar/users.svg
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/statusbar/bell.svg
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/statusbar/kernel.svg
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/statusbar/line-form.svg
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/statusbar/list.svg
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/statusbar/not-trusted.svg
--rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/statusbar/terminal.svg
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/statusbar/trusted.svg
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/add-above.svg
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/add-below.svg
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/add.svg
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/bug-dot.svg
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/bug.svg
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/check.svg
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/circle-empty.svg
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/circle.svg
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/clear.svg
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/close.svg
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/code.svg
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/collapse-all.svg
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/copy.svg
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/cut.svg
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/delete.svg
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/download.svg
--rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/duplicate.svg
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/edit.svg
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/ellipses.svg
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/expand-all.svg
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/fast-forward.svg
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/file-upload.svg
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/filter-list.svg
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/launch.svg
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/link.svg
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/move-down.svg
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/move-up.svg
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/new-folder.svg
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/numbering.svg
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/offline-bolt.svg
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/paste.svg
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/redo.svg
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/refresh.svg
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/run.svg
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/save.svg
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/search.svg
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/stop.svg
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/table-rows.svg
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/tag.svg
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/tree-view.svg
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/icons/toolbar/undo.svg
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/unused/home.svg
--rw-r--r--   0        0        0    16859 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/unused/jupyterlab.svg
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/ui-components/style/unused/text-editor-alt.svg
--rw-r--r--   0        0        0     3917 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/src/collaboratorspanel.tsx
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/src/components.tsx
--rw-r--r--   0        0        0    11810 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/src/cursors.ts
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/src/index.ts
--rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/src/menu.ts
--rw-r--r--   0        0        0     5638 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/src/sharedlink.ts
--rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/src/tokens.ts
--rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/src/userinfopanel.tsx
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/style/base.css
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/style/index.css
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/style/index.js
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/style/menu.css
--rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration/style/sidepanel.css
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/README.md
--rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/package.json
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/tsconfig.json
--rw-r--r--   0        0        0    98773 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/tsconfig.tsbuildinfo
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/lib/collaboration.d.ts
--rw-r--r--   0        0        0     5657 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/lib/collaboration.js
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/lib/index.d.ts
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/lib/index.js
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/lib/sharedlink.d.ts
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/lib/sharedlink.js
--rw-r--r--   0        0        0    11754 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/README.md
--rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/package.json
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/FormRendererRegistry.d.ts
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/FormRendererRegistry.js
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/FormRendererRegistry.js.map
--rw-r--r--   0        0        0     3991 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/hoverbox.d.ts
--rw-r--r--   0        0        0    10279 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/hoverbox.js
--rw-r--r--   0        0        0     7792 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/hoverbox.js.map
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/index.d.ts
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/index.js
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/index.js.map
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/tokens.d.ts
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/tokens.js
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/tokens.js.map
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/utils.d.ts
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/utils.js
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/utils.js.map
--rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/accordiontoolbar.d.ts
--rw-r--r--   0        0        0     7922 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/accordiontoolbar.js
--rw-r--r--   0        0        0     3750 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/accordiontoolbar.js.map
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/button.d.ts
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/button.js
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/button.js.map
--rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/collapser.d.ts
--rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/collapser.js
--rw-r--r--   0        0        0     3882 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/collapser.js.map
--rw-r--r--   0        0        0     3450 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/form.d.ts
--rw-r--r--   0        0        0    15525 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/form.js
--rw-r--r--   0        0        0    11514 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/form.js.map
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/htmlselect.d.ts
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/htmlselect.js
--rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/htmlselect.js.map
--rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/iframe.d.ts
--rw-r--r--   0        0        0     2749 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/iframe.js
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/iframe.js.map
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/index.d.ts
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/index.js
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/index.js.map
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/inputgroup.d.ts
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/inputgroup.js
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/inputgroup.js.map
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/interface.d.ts
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/interface.js
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/interface.js.map
--rw-r--r--   0        0        0     4385 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/menu.d.ts
--rw-r--r--   0        0        0     8343 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/menu.js
--rw-r--r--   0        0        0     5842 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/menu.js.map
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/panelwithtoolbar.d.ts
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/panelwithtoolbar.js
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/panelwithtoolbar.js.map
--rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/search.d.ts
--rw-r--r--   0        0        0     3780 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/search.js
--rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/search.js.map
--rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/sidepanel.d.ts
--rw-r--r--   0        0        0     3189 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/sidepanel.js
--rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/sidepanel.js.map
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/spinner.d.ts
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/spinner.js
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/spinner.js.map
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/styling.d.ts
--rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/styling.js
--rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/styling.js.map
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/switch.d.ts
--rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/switch.js
--rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/switch.js.map
--rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/table.d.ts
--rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/table.js
--rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/table.js.map
--rw-r--r--   0        0        0    14396 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/toolbar.d.ts
--rw-r--r--   0        0        0    37369 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/toolbar.js
--rw-r--r--   0        0        0    23689 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/toolbar.js.map
--rw-r--r--   0        0        0     5635 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/vdom.d.ts
--rw-r--r--   0        0        0     6383 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/vdom.js
--rw-r--r--   0        0        0     3921 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/vdom.js.map
--rw-r--r--   0        0        0    28402 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/windowedlist.d.ts
--rw-r--r--   0        0        0    53928 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/windowedlist.js
--rw-r--r--   0        0        0    32680 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/components/windowedlist.js.map
--rw-r--r--   0        0        0     4514 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/icon/iconimports.d.ts
--rw-r--r--   0        0        0    17726 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/icon/iconimports.js
--rw-r--r--   0        0        0    14441 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/icon/iconimports.js.map
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/icon/index.d.ts
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/icon/index.js
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/icon/index.js.map
--rw-r--r--   0        0        0    11503 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/icon/labicon.d.ts
--rw-r--r--   0        0        0    25278 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/icon/labicon.js
--rw-r--r--   0        0        0    14573 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/icon/labicon.js.map
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/icon/widgets/commandpalettesvg.d.ts
--rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/icon/widgets/commandpalettesvg.js
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/icon/widgets/commandpalettesvg.js.map
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/icon/widgets/index.d.ts
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/icon/widgets/index.js
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/icon/widgets/index.js.map
--rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/icon/widgets/menusvg.d.ts
--rw-r--r--   0        0        0     6138 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/icon/widgets/menusvg.js
--rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/icon/widgets/menusvg.js.map
--rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/icon/widgets/tabbarsvg.d.ts
--rw-r--r--   0        0        0     3788 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/icon/widgets/tabbarsvg.js
--rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/icon/widgets/tabbarsvg.js.map
--rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/style/icon.d.ts
--rw-r--r--   0        0        0    11068 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/style/icon.js
--rw-r--r--   0        0        0     7175 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/style/icon.js.map
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/style/index.d.ts
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/style/index.js
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/lib/style/index.js.map
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/README.md
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/package.json
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/lib/activitymonitor.d.ts
--rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/lib/activitymonitor.js
--rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/lib/activitymonitor.js.map
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/lib/index.d.ts
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/lib/index.js
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/lib/index.js.map
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/lib/interfaces.d.ts
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/lib/interfaces.js
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/lib/interfaces.js.map
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/lib/lru.d.ts
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/lib/lru.js
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/lib/lru.js.map
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/lib/markdowncodeblocks.d.ts
--rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/lib/markdowncodeblocks.js
--rw-r--r--   0        0        0     2158 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/lib/markdowncodeblocks.js.map
--rw-r--r--   0        0        0     4590 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/lib/pageconfig.d.ts
--rw-r--r--   0        0        0    10629 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/lib/pageconfig.js
--rw-r--r--   0        0        0     6260 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/lib/pageconfig.js.map
--rw-r--r--   0        0        0     4071 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/lib/path.d.ts
--rw-r--r--   0        0        0     5518 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/lib/path.js
--rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/lib/path.js.map
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/lib/signal.d.ts
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/lib/signal.js
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/lib/signal.js.map
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/lib/testutils.d.ts
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/lib/testutils.js
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/lib/testutils.js.map
--rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/lib/text.d.ts
--rw-r--r--   0        0        0     3929 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/lib/text.js
--rw-r--r--   0        0        0     2208 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/lib/text.js.map
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/lib/time.d.ts
--rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/lib/time.js
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/lib/time.js.map
--rw-r--r--   0        0        0     3399 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/lib/url.d.ts
--rw-r--r--   0        0        0     4717 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/lib/url.js
--rw-r--r--   0        0        0     3272 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/lib/url.js.map
--rw-r--r--   0        0        0     2616 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/src/activitymonitor.ts
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/src/index.ts
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/src/interfaces.ts
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/src/lru.ts
--rw-r--r--   0        0        0     3057 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/src/markdowncodeblocks.ts
--rw-r--r--   0        0        0     9854 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/src/pageconfig.ts
--rw-r--r--   0        0        0     4862 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/src/path.ts
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/src/signal.ts
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/src/testutils.ts
--rw-r--r--   0        0        0     3332 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/src/text.ts
--rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/src/time.ts
--rw-r--r--   0        0        0     5347 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/node_modules/@jupyterlab/coreutils/src/url.ts
--rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/src/FormRendererRegistry.tsx
--rw-r--r--   0        0        0    11700 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/src/hoverbox.ts
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/src/index.ts
--rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/src/svg.d.ts
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/src/tokens.ts
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/src/utils.ts
--rw-r--r--   0        0        0     7363 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/src/components/accordiontoolbar.ts
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/src/components/button.tsx
--rw-r--r--   0        0        0     4821 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/src/components/collapser.ts
--rw-r--r--   0        0        0    18987 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/src/components/form.tsx
--rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/src/components/htmlselect.tsx
--rw-r--r--   0        0        0     4216 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/src/components/iframe.ts
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/src/components/index.ts
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/src/components/inputgroup.tsx
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/src/components/interface.ts
--rw-r--r--   0        0        0    10224 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/src/components/menu.ts
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/src/components/panelwithtoolbar.ts
--rw-r--r--   0        0        0     4914 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/src/components/search.tsx
--rw-r--r--   0        0        0     4161 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/src/components/sidepanel.ts
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/src/components/spinner.ts
--rw-r--r--   0        0        0     2995 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/src/components/styling.ts
--rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/src/components/switch.ts
--rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/src/components/table.tsx
--rw-r--r--   0        0        0    37192 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/src/components/toolbar.tsx
--rw-r--r--   0        0        0     8376 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/src/components/vdom.ts
--rw-r--r--   0        0        0    60687 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/src/components/windowedlist.ts
--rw-r--r--   0        0        0    17691 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/src/icon/iconimports.ts
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/src/icon/index.ts
--rw-r--r--   0        0        0    28069 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/src/icon/labicon.tsx
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/src/icon/widgets/commandpalettesvg.ts
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/src/icon/widgets/index.ts
--rw-r--r--   0        0        0     5952 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/src/icon/widgets/menusvg.ts
--rw-r--r--   0        0        0     3543 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/src/icon/widgets/tabbarsvg.ts
--rw-r--r--   0        0        0    13354 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/src/style/icon.ts
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/src/style/index.ts
--rw-r--r--   0        0        0     4209 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/base.css
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/collapse.css
--rw-r--r--   0        0        0    13082 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/deprecated.css
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/deprecatedExtra.css
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/hoverbox.css
--rw-r--r--   0        0        0     6117 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons.css
--rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/iconsalt.css
--rw-r--r--   0        0        0     4762 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/iconshover.css
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/iframe.css
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/index.css
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/index.js
--rw-r--r--   0        0        0     5722 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/rjsfTemplates.css
--rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/sidepanel.css
--rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/spinner.css
--rw-r--r--   0        0        0     2617 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/styling.css
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/switch.css
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/tabbar.css
--rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/table.css
--rw-r--r--   0        0        0     3401 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/toolbar.css
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/windowedlist.css
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/debug/bad.svg
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/debug/blank.svg
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/deprecated/check-disabled.svg
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/error.svg
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/history.svg
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/info.svg
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/lock.svg
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/arrow/caret-down-empty-thin.svg
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/arrow/caret-down-empty.svg
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/arrow/caret-down.svg
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/arrow/caret-left.svg
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/arrow/caret-right.svg
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/arrow/caret-up-empty-thin.svg
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/arrow/caret-up.svg
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/filetype/console.svg
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/filetype/file.svg
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/filetype/folder-favorite.svg
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/filetype/folder.svg
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/filetype/home.svg
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/filetype/html5.svg
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/filetype/image.svg
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/filetype/inspector.svg
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/filetype/json.svg
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/filetype/julia.svg
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/filetype/keyboard.svg
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/filetype/launcher.svg
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/filetype/markdown.svg
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/filetype/mermaid.svg
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/filetype/notebook.svg
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/filetype/pdf.svg
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/filetype/python.svg
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/filetype/r-kernel.svg
--rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/filetype/react.svg
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/filetype/settings.svg
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/filetype/spreadsheet.svg
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/filetype/text-editor.svg
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/filetype/vega.svg
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/filetype/yaml.svg
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/jupyter/jupyter-favicon.svg
--rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/jupyter/jupyter.svg
--rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/jupyter/jupyterlab-wordmark.svg
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/licenses/copyright.svg
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/lsp/code-check.svg
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/output/collapse.svg
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/output/expand.svg
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/search/case-sensitive.svg
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/search/filter-dot.svg
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/search/filter.svg
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/search/regex.svg
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/search/word.svg
--rw-r--r--   0        0        0     2430 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/sidebar/build.svg
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/sidebar/extension.svg
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/sidebar/palette.svg
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/sidebar/running.svg
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/sidebar/share.svg
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/sidebar/tab.svg
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/sidebar/toc.svg
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/sidebar/user.svg
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/sidebar/users.svg
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/statusbar/bell.svg
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/statusbar/kernel.svg
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/statusbar/line-form.svg
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/statusbar/list.svg
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/statusbar/not-trusted.svg
--rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/statusbar/terminal.svg
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/statusbar/trusted.svg
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/add-above.svg
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/add-below.svg
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/add.svg
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/bug-dot.svg
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/bug.svg
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/check.svg
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/circle-empty.svg
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/circle.svg
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/clear.svg
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/close.svg
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/code.svg
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/collapse-all.svg
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/copy.svg
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/cut.svg
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/delete.svg
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/download.svg
--rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/duplicate.svg
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/edit.svg
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/ellipses.svg
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/expand-all.svg
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/fast-forward.svg
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/file-upload.svg
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/filter-list.svg
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/launch.svg
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/link.svg
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/move-down.svg
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/move-up.svg
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/new-folder.svg
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/numbering.svg
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/offline-bolt.svg
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/paste.svg
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/redo.svg
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/refresh.svg
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/run.svg
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/save.svg
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/search.svg
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/stop.svg
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/table-rows.svg
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/tag.svg
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/tree-view.svg
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/icons/toolbar/undo.svg
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/unused/home.svg
--rw-r--r--   0        0        0    16859 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/unused/jupyterlab.svg
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@jupyterlab/ui-components/style/unused/text-editor-alt.svg
--rw-r--r--   0        0        0    10947 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/LICENSE.md
--rw-r--r--   0        0        0     3764 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/README.md
--rw-r--r--   0        0        0     3293 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/package.json
--rw-r--r--   0        0        0   131120 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/dist/core.umd.js
--rw-r--r--   0        0        0   131364 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/dist/index.esm.js
--rw-r--r--   0        0        0   261719 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/dist/index.esm.js.map
--rw-r--r--   0        0        0   138979 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/dist/index.js
--rw-r--r--   0        0        0   259198 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/dist/index.js.map
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/getDefaultRegistry.d.ts
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/getDefaultRegistry.js
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/getDefaultRegistry.js.map
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/index.d.ts
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/index.js
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/index.js.map
--rw-r--r--   0        0        0    72060 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/tsconfig.tsbuildinfo
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/withTheme.d.ts
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/withTheme.js
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/withTheme.js.map
--rw-r--r--   0        0        0    21834 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/Form.d.ts
--rw-r--r--   0        0        0    28563 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/Form.js
--rw-r--r--   0        0        0    16852 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/Form.js.map
--rw-r--r--   0        0        0     9098 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/fields/ArrayField.d.ts
--rw-r--r--   0        0        0    30510 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/fields/ArrayField.js
--rw-r--r--   0        0        0    20629 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/fields/ArrayField.js.map
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/fields/BooleanField.d.ts
--rw-r--r--   0        0        0     3345 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/fields/BooleanField.js
--rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/fields/BooleanField.js.map
--rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/fields/MultiSchemaField.d.ts
--rw-r--r--   0        0        0     9207 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/fields/MultiSchemaField.js
--rw-r--r--   0        0        0     6539 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/fields/MultiSchemaField.js.map
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/fields/NullField.d.ts
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/fields/NullField.js
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/fields/NullField.js.map
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/fields/NumberField.d.ts
--rw-r--r--   0        0        0     3484 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/fields/NumberField.js
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/fields/NumberField.js.map
--rw-r--r--   0        0        0     3898 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/fields/ObjectField.d.ts
--rw-r--r--   0        0        0    11814 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/fields/ObjectField.js
--rw-r--r--   0        0        0     7324 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/fields/ObjectField.js.map
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/fields/SchemaField.d.ts
--rw-r--r--   0        0        0    10578 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/fields/SchemaField.js
--rw-r--r--   0        0        0     8353 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/fields/SchemaField.js.map
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/fields/StringField.d.ts
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/fields/StringField.js
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/fields/StringField.js.map
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/fields/index.d.ts
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/fields/index.js
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/fields/index.js.map
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/ArrayFieldDescriptionTemplate.d.ts
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/ArrayFieldDescriptionTemplate.js
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/ArrayFieldDescriptionTemplate.js.map
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/ArrayFieldItemTemplate.d.ts
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/ArrayFieldItemTemplate.js
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/ArrayFieldItemTemplate.js.map
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/ArrayFieldTemplate.d.ts
--rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/ArrayFieldTemplate.js
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/ArrayFieldTemplate.js.map
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/ArrayFieldTitleTemplate.d.ts
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/ArrayFieldTitleTemplate.js
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/ArrayFieldTitleTemplate.js.map
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/BaseInputTemplate.d.ts
--rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/BaseInputTemplate.js
--rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/BaseInputTemplate.js.map
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/DescriptionField.d.ts
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/DescriptionField.js
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/DescriptionField.js.map
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/ErrorList.d.ts
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/ErrorList.js
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/ErrorList.js.map
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/FieldErrorTemplate.d.ts
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/FieldErrorTemplate.js
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/FieldErrorTemplate.js.map
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/FieldHelpTemplate.d.ts
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/FieldHelpTemplate.js
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/FieldHelpTemplate.js.map
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/ObjectFieldTemplate.d.ts
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/ObjectFieldTemplate.js
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/ObjectFieldTemplate.js.map
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/TitleField.d.ts
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/TitleField.js
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/TitleField.js.map
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/UnsupportedField.d.ts
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/UnsupportedField.js
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/UnsupportedField.js.map
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/WrapIfAdditionalTemplate.d.ts
--rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/WrapIfAdditionalTemplate.js
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/WrapIfAdditionalTemplate.js.map
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/index.d.ts
--rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/index.js
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/index.js.map
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/ButtonTemplates/AddButton.d.ts
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/ButtonTemplates/AddButton.js
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/ButtonTemplates/AddButton.js.map
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/ButtonTemplates/IconButton.d.ts
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/ButtonTemplates/IconButton.js
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/ButtonTemplates/IconButton.js.map
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/ButtonTemplates/SubmitButton.d.ts
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/ButtonTemplates/SubmitButton.js
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/ButtonTemplates/SubmitButton.js.map
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/ButtonTemplates/index.d.ts
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/ButtonTemplates/index.js
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/ButtonTemplates/index.js.map
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/FieldTemplate/FieldTemplate.d.ts
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/FieldTemplate/FieldTemplate.js
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/FieldTemplate/FieldTemplate.js.map
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/FieldTemplate/Label.d.ts
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/FieldTemplate/Label.js
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/FieldTemplate/Label.js.map
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/FieldTemplate/index.d.ts
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/FieldTemplate/index.js
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/templates/FieldTemplate/index.js.map
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/AltDateTimeWidget.d.ts
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/AltDateTimeWidget.js
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/AltDateTimeWidget.js.map
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/AltDateWidget.d.ts
--rw-r--r--   0        0        0     3927 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/AltDateWidget.js
--rw-r--r--   0        0        0     4140 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/AltDateWidget.js.map
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/CheckboxWidget.d.ts
--rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/CheckboxWidget.js
--rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/CheckboxWidget.js.map
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/CheckboxesWidget.d.ts
--rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/CheckboxesWidget.js
--rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/CheckboxesWidget.js.map
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/ColorWidget.d.ts
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/ColorWidget.js
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/ColorWidget.js.map
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/DateTimeWidget.d.ts
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/DateTimeWidget.js
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/DateTimeWidget.js.map
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/DateWidget.d.ts
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/DateWidget.js
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/DateWidget.js.map
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/EmailWidget.d.ts
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/EmailWidget.js
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/EmailWidget.js.map
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/FileWidget.d.ts
--rw-r--r--   0        0        0     5527 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/FileWidget.js
--rw-r--r--   0        0        0     4878 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/FileWidget.js.map
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/HiddenWidget.d.ts
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/HiddenWidget.js
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/HiddenWidget.js.map
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/PasswordWidget.d.ts
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/PasswordWidget.js
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/PasswordWidget.js.map
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/RadioWidget.d.ts
--rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/RadioWidget.js
--rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/RadioWidget.js.map
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/RangeWidget.d.ts
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/RangeWidget.js
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/RangeWidget.js.map
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/SelectWidget.d.ts
--rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/SelectWidget.js
--rw-r--r--   0        0        0     2565 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/SelectWidget.js.map
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/TextWidget.d.ts
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/TextWidget.js
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/TextWidget.js.map
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/TextareaWidget.d.ts
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/TextareaWidget.js
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/TextareaWidget.js.map
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/TimeWidget.d.ts
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/TimeWidget.js
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/TimeWidget.js.map
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/URLWidget.d.ts
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/URLWidget.js
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/URLWidget.js.map
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/UpDownWidget.d.ts
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/UpDownWidget.js
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/UpDownWidget.js.map
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/index.d.ts
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/index.js
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/lib/components/widgets/index.js.map
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/getDefaultRegistry.ts
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/index.ts
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/tsconfig.json
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/withTheme.tsx
--rw-r--r--   0        0        0    39338 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/Form.tsx
--rw-r--r--   0        0        0    30440 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/fields/ArrayField.tsx
--rw-r--r--   0        0        0     3349 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/fields/BooleanField.tsx
--rw-r--r--   0        0        0     9539 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/fields/MultiSchemaField.tsx
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/fields/NullField.tsx
--rw-r--r--   0        0        0     3560 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/fields/NumberField.tsx
--rw-r--r--   0        0        0    11443 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/fields/ObjectField.tsx
--rw-r--r--   0        0        0    12037 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/fields/SchemaField.tsx
--rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/fields/StringField.tsx
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/fields/index.ts
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/templates/ArrayFieldDescriptionTemplate.tsx
--rw-r--r--   0        0        0     2665 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/templates/ArrayFieldItemTemplate.tsx
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/templates/ArrayFieldTemplate.tsx
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/templates/ArrayFieldTitleTemplate.tsx
--rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/templates/BaseInputTemplate.tsx
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/templates/DescriptionField.tsx
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/templates/ErrorList.tsx
--rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/templates/FieldErrorTemplate.tsx
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/templates/FieldHelpTemplate.tsx
--rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/templates/ObjectFieldTemplate.tsx
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/templates/TitleField.tsx
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/templates/UnsupportedField.tsx
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/templates/WrapIfAdditionalTemplate.tsx
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/templates/index.ts
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/templates/ButtonTemplates/AddButton.tsx
--rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/templates/ButtonTemplates/IconButton.tsx
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/templates/ButtonTemplates/SubmitButton.tsx
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/templates/ButtonTemplates/index.ts
--rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/templates/FieldTemplate/FieldTemplate.tsx
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/templates/FieldTemplate/Label.tsx
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/templates/FieldTemplate/index.ts
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/widgets/AltDateTimeWidget.tsx
--rw-r--r--   0        0        0     5070 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/widgets/AltDateWidget.tsx
--rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/widgets/CheckboxWidget.tsx
--rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/widgets/CheckboxesWidget.tsx
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/widgets/ColorWidget.tsx
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/widgets/DateTimeWidget.tsx
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/widgets/DateWidget.tsx
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/widgets/EmailWidget.tsx
--rw-r--r--   0        0        0     6045 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/widgets/FileWidget.tsx
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/widgets/HiddenWidget.tsx
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/widgets/PasswordWidget.tsx
--rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/widgets/RadioWidget.tsx
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/widgets/RangeWidget.tsx
--rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/widgets/SelectWidget.tsx
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/widgets/TextWidget.tsx
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/widgets/TextareaWidget.tsx
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/widgets/TimeWidget.tsx
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/widgets/URLWidget.tsx
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/widgets/UpDownWidget.tsx
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/core/src/components/widgets/index.ts
--rw-r--r--   0        0        0    10947 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/LICENSE.md
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/README.md
--rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/package.json
--rw-r--r--   0        0        0   103957 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/dist/index.js
--rw-r--r--   0        0        0   265256 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/dist/index.js.map
--rw-r--r--   0        0        0    96830 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/dist/utils.esm.js
--rw-r--r--   0        0        0   259446 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/dist/utils.esm.js.map
--rw-r--r--   0        0        0   103426 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/dist/utils.umd.js
--rw-r--r--   0        0        0     3758 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/ErrorSchemaBuilder.d.ts
--rw-r--r--   0        0        0     5254 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/ErrorSchemaBuilder.js
--rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/ErrorSchemaBuilder.js.map
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/allowAdditionalItems.d.ts
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/allowAdditionalItems.js
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/allowAdditionalItems.js.map
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/asNumber.d.ts
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/asNumber.js
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/asNumber.js.map
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/canExpand.d.ts
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/canExpand.js
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/canExpand.js.map
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/constants.d.ts
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/constants.js
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/constants.js.map
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/createErrorHandler.d.ts
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/createErrorHandler.js
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/createErrorHandler.js.map
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/createSchemaUtils.d.ts
--rw-r--r--   0        0        0    13359 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/createSchemaUtils.js
--rw-r--r--   0        0        0     3216 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/createSchemaUtils.js.map
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/dataURItoBlob.d.ts
--rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/dataURItoBlob.js
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/dataURItoBlob.js.map
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/deepEquals.d.ts
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/deepEquals.js
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/deepEquals.js.map
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/englishStringTranslator.d.ts
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/englishStringTranslator.js
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/englishStringTranslator.js.map
--rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/enumOptionsDeselectValue.d.ts
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/enumOptionsDeselectValue.js
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/enumOptionsDeselectValue.js.map
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/enumOptionsIndexForValue.d.ts
--rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/enumOptionsIndexForValue.js
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/enumOptionsIndexForValue.js.map
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/enumOptionsIsSelected.d.ts
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/enumOptionsIsSelected.js
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/enumOptionsIsSelected.js.map
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/enumOptionsSelectValue.d.ts
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/enumOptionsSelectValue.js
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/enumOptionsSelectValue.js.map
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/enumOptionsValueForIndex.d.ts
--rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/enumOptionsValueForIndex.js
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/enumOptionsValueForIndex.js.map
--rw-r--r--   0        0        0     3931 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/enums.d.ts
--rw-r--r--   0        0        0     4801 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/enums.js
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/enums.js.map
--rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/findSchemaDefinition.d.ts
--rw-r--r--   0        0        0     3977 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/findSchemaDefinition.js
--rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/findSchemaDefinition.js.map
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/getDateElementProps.d.ts
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/getDateElementProps.js
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/getDateElementProps.js.map
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/getDiscriminatorFieldFromSchema.d.ts
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/getDiscriminatorFieldFromSchema.js
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/getDiscriminatorFieldFromSchema.js.map
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/getInputProps.d.ts
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/getInputProps.js
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/getInputProps.js.map
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/getOptionMatchingSimpleDiscriminator.d.ts
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/getOptionMatchingSimpleDiscriminator.js
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/getOptionMatchingSimpleDiscriminator.js.map
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/getSchemaType.d.ts
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/getSchemaType.js
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/getSchemaType.js.map
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/getSubmitButtonOptions.d.ts
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/getSubmitButtonOptions.js
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/getSubmitButtonOptions.js.map
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/getTemplate.d.ts
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/getTemplate.js
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/getTemplate.js.map
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/getUiOptions.d.ts
--rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/getUiOptions.js
--rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/getUiOptions.js.map
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/getWidget.d.ts
--rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/getWidget.js
--rw-r--r--   0        0        0     2739 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/getWidget.js.map
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/guessType.d.ts
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/guessType.js
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/guessType.js.map
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/hasWidget.d.ts
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/hasWidget.js
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/hasWidget.js.map
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/hashForSchema.d.ts
--rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/hashForSchema.js
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/hashForSchema.js.map
--rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/idGenerators.d.ts
--rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/idGenerators.js
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/idGenerators.js.map
--rw-r--r--   0        0        0     3881 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/index.d.ts
--rw-r--r--   0        0        0     3867 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/index.js
--rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/index.js.map
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/isConstant.d.ts
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/isConstant.js
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/isConstant.js.map
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/isCustomWidget.d.ts
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/isCustomWidget.js
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/isCustomWidget.js.map
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/isFixedItems.d.ts
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/isFixedItems.js
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/isFixedItems.js.map
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/isObject.d.ts
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/isObject.js
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/isObject.js.map
--rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/labelValue.d.ts
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/labelValue.js
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/labelValue.js.map
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/localToUTC.d.ts
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/localToUTC.js
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/localToUTC.js.map
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/mergeDefaultsWithFormData.d.ts
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/mergeDefaultsWithFormData.js
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/mergeDefaultsWithFormData.js.map
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/mergeObjects.d.ts
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/mergeObjects.js
--rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/mergeObjects.js.map
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/mergeSchemas.d.ts
--rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/mergeSchemas.js
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/mergeSchemas.js.map
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/optionsList.d.ts
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/optionsList.js
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/optionsList.js.map
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/orderProperties.d.ts
--rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/orderProperties.js
--rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/orderProperties.js.map
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/pad.d.ts
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/pad.js
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/pad.js.map
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/parseDateString.d.ts
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/parseDateString.js
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/parseDateString.js.map
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/rangeSpec.d.ts
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/rangeSpec.js
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/rangeSpec.js.map
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/replaceStringParameters.d.ts
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/replaceStringParameters.js
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/replaceStringParameters.js.map
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schemaRequiresTrueValue.d.ts
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schemaRequiresTrueValue.js
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schemaRequiresTrueValue.js.map
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/shouldRender.d.ts
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/shouldRender.js
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/shouldRender.js.map
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/toConstant.d.ts
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/toConstant.js
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/toConstant.js.map
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/toDateString.d.ts
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/toDateString.js
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/toDateString.js.map
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/toErrorList.d.ts
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/toErrorList.js
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/toErrorList.js.map
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/toErrorSchema.d.ts
--rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/toErrorSchema.js
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/toErrorSchema.js.map
--rw-r--r--   0        0        0    67837 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/tsconfig.tsbuildinfo
--rw-r--r--   0        0        0    57219 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/types.d.ts
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/types.js
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/types.js.map
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/unwrapErrorHandler.d.ts
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/unwrapErrorHandler.js
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/unwrapErrorHandler.js.map
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/utcToLocal.d.ts
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/utcToLocal.js
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/utcToLocal.js.map
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/validationDataMerge.d.ts
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/validationDataMerge.js
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/validationDataMerge.js.map
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/withIdRefPrefix.d.ts
--rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/withIdRefPrefix.js
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/withIdRefPrefix.js.map
--rw-r--r--   0        0        0     4257 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/parser/ParserValidator.d.ts
--rw-r--r--   0        0        0     5010 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/parser/ParserValidator.js
--rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/parser/ParserValidator.js.map
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/parser/index.d.ts
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/parser/index.js
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/parser/index.js.map
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/parser/schemaParser.d.ts
--rw-r--r--   0        0        0     2672 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/parser/schemaParser.js
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/parser/schemaParser.js.map
--rw-r--r--   0        0        0     4194 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/getClosestMatchingOption.d.ts
--rw-r--r--   0        0        0     8998 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/getClosestMatchingOption.js
--rw-r--r--   0        0        0     4361 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/getClosestMatchingOption.js.map
--rw-r--r--   0        0        0     5391 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/getDefaultFormState.d.ts
--rw-r--r--   0        0        0    22107 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/getDefaultFormState.js
--rw-r--r--   0        0        0    10811 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/getDefaultFormState.js.map
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/getDisplayLabel.d.ts
--rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/getDisplayLabel.js
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/getDisplayLabel.js.map
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/getFirstMatchingOption.d.ts
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/getFirstMatchingOption.js
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/getFirstMatchingOption.js.map
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/getMatchingOption.d.ts
--rw-r--r--   0        0        0     4231 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/getMatchingOption.js
--rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/getMatchingOption.js.map
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/index.d.ts
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/index.js
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/index.js.map
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/isFilesArray.d.ts
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/isFilesArray.js
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/isFilesArray.js.map
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/isMultiSelect.d.ts
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/isMultiSelect.js
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/isMultiSelect.js.map
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/isSelect.d.ts
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/isSelect.js
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/isSelect.js.map
--rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/mergeValidationData.d.ts
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/mergeValidationData.js
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/mergeValidationData.js.map
--rw-r--r--   0        0        0    15291 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/retrieveSchema.d.ts
--rw-r--r--   0        0        0    28066 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/retrieveSchema.js
--rw-r--r--   0        0        0    13290 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/retrieveSchema.js.map
--rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/sanitizeDataForNewSchema.d.ts
--rw-r--r--   0        0        0    11577 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/sanitizeDataForNewSchema.js
--rw-r--r--   0        0        0     4889 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/sanitizeDataForNewSchema.js.map
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/toIdSchema.d.ts
--rw-r--r--   0        0        0     3499 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/toIdSchema.js
--rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/toIdSchema.js.map
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/toPathSchema.d.ts
--rw-r--r--   0        0        0     4764 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/toPathSchema.js
--rw-r--r--   0        0        0     3182 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/lib/schema/toPathSchema.js.map
--rw-r--r--   0        0        0     5215 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/ErrorSchemaBuilder.ts
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/allowAdditionalItems.ts
--rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/asNumber.ts
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/canExpand.ts
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/constants.ts
--rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/createErrorHandler.ts
--rw-r--r--   0        0        0    14372 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/createSchemaUtils.ts
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/dataURItoBlob.ts
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/deepEquals.ts
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/englishStringTranslator.ts
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/enumOptionsDeselectValue.ts
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/enumOptionsIndexForValue.ts
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/enumOptionsIsSelected.ts
--rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/enumOptionsSelectValue.ts
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/enumOptionsValueForIndex.ts
--rw-r--r--   0        0        0     3914 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/enums.ts
--rw-r--r--   0        0        0     4067 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/findSchemaDefinition.ts
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/getDateElementProps.ts
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/getDiscriminatorFieldFromSchema.ts
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/getInputProps.ts
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/getOptionMatchingSimpleDiscriminator.ts
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/getSchemaType.ts
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/getSubmitButtonOptions.ts
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/getTemplate.ts
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/getUiOptions.ts
--rw-r--r--   0        0        0     4671 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/getWidget.tsx
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/guessType.ts
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/hasWidget.ts
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/hashForSchema.ts
--rw-r--r--   0        0        0     3310 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/idGenerators.ts
--rw-r--r--   0        0        0     4004 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/index.ts
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/isConstant.ts
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/isCustomWidget.ts
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/isFixedItems.ts
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/isObject.ts
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/labelValue.ts
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/localToUTC.ts
--rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/mergeDefaultsWithFormData.ts
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/mergeObjects.ts
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/mergeSchemas.ts
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/optionsList.ts
--rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/orderProperties.ts
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/pad.ts
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/parseDateString.ts
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/rangeSpec.ts
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/replaceStringParameters.ts
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/schemaRequiresTrueValue.ts
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/shouldRender.ts
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/toConstant.ts
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/toDateString.ts
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/toErrorList.ts
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/toErrorSchema.ts
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/tsconfig.json
--rw-r--r--   0        0        0    56287 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/types.ts
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/unwrapErrorHandler.ts
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/utcToLocal.ts
--rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/validationDataMerge.ts
--rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/withIdRefPrefix.ts
--rw-r--r--   0        0        0     5622 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/parser/ParserValidator.ts
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/parser/index.ts
--rw-r--r--   0        0        0     2902 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/parser/schemaParser.ts
--rw-r--r--   0        0        0     9294 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/schema/getClosestMatchingOption.ts
--rw-r--r--   0        0        0    21319 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/schema/getDefaultFormState.ts
--rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/schema/getDisplayLabel.ts
--rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/schema/getFirstMatchingOption.ts
--rw-r--r--   0        0        0     4060 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/schema/getMatchingOption.ts
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/schema/index.ts
--rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/schema/isFilesArray.ts
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/schema/isMultiSelect.ts
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/schema/isSelect.ts
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/schema/mergeValidationData.ts
--rw-r--r--   0        0        0    30469 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/schema/retrieveSchema.ts
--rw-r--r--   0        0        0    11171 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/schema/sanitizeDataForNewSchema.ts
--rw-r--r--   0        0        0     4110 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/schema/toIdSchema.ts
--rw-r--r--   0        0        0     5403 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@rjsf/utils/src/schema/toPathSchema.ts
--rwxr-xr-x   0        0        0     1141 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@types/react/LICENSE
--rwxr-xr-x   0        0        0     1916 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@types/react/README.md
--rwxr-xr-x   0        0        0     4743 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@types/react/experimental.d.ts
--rwxr-xr-x   0        0        0     7431 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@types/react/global.d.ts
--rwxr-xr-x   0        0        0   156037 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@types/react/index.d.ts
--rwxr-xr-x   0        0        0       61 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@types/react/jsx-dev-runtime.d.ts
--rwxr-xr-x   0        0        0       61 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@types/react/jsx-runtime.d.ts
--rwxr-xr-x   0        0        0     2929 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@types/react/next.d.ts
--rwxr-xr-x   0        0        0     6002 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@types/react/package.json
--rwxr-xr-x   0        0        0     4613 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@types/react/ts5.0/experimental.d.ts
--rwxr-xr-x   0        0        0     7409 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@types/react/ts5.0/global.d.ts
--rwxr-xr-x   0        0        0   152997 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@types/react/ts5.0/index.d.ts
--rwxr-xr-x   0        0        0       61 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@types/react/ts5.0/jsx-dev-runtime.d.ts
--rwxr-xr-x   0        0        0       61 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@types/react/ts5.0/jsx-runtime.d.ts
--rwxr-xr-x   0        0        0     2929 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/@types/react/ts5.0/next.d.ts
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/markdown-to-jsx/LICENSE
--rw-r--r--   0        0        0    19014 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/markdown-to-jsx/README.md
--rw-r--r--   0        0        0     4073 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/markdown-to-jsx/package.json
--rw-r--r--   0        0        0    16150 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/markdown-to-jsx/dist/index.cjs
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/markdown-to-jsx/dist/index.cjs.d.ts
--rw-r--r--   0        0        0    90164 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/markdown-to-jsx/dist/index.cjs.map
--rw-r--r--   0        0        0    13626 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/markdown-to-jsx/dist/index.d.ts
--rw-r--r--   0        0        0    14946 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/markdown-to-jsx/dist/index.modern.js
--rw-r--r--   0        0        0    89358 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/markdown-to-jsx/dist/index.modern.js.map
--rw-r--r--   0        0        0    15880 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/markdown-to-jsx/dist/index.module.js
--rw-r--r--   0        0        0    89921 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/markdown-to-jsx/dist/index.module.js.map
--rw-r--r--   0        0        0    16345 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/markdown-to-jsx/dist/index.umd.js
--rw-r--r--   0        0        0    90167 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/markdown-to-jsx/dist/index.umd.js.map
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/markdown-to-jsx/dist/site.d.ts
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/react-dom/LICENSE
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/react-dom/README.md
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/react-dom/client.js
--rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/react-dom/index.js
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/react-dom/package.json
--rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/react-dom/profiling.js
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/react-dom/server.browser.js
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/react-dom/server.js
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/react-dom/server.node.js
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/react-dom/test-utils.js
--rw-r--r--   0        0        0   243900 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/react-dom/cjs/react-dom-server-legacy.browser.development.js
--rw-r--r--   0        0        0    35019 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/react-dom/cjs/react-dom-server-legacy.browser.production.min.js
--rw-r--r--   0        0        0   245608 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/react-dom/cjs/react-dom-server-legacy.node.development.js
--rw-r--r--   0        0        0    38796 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/react-dom/cjs/react-dom-server-legacy.node.production.min.js
--rw-r--r--   0        0        0   242789 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/react-dom/cjs/react-dom-server.browser.development.js
--rw-r--r--   0        0        0    35597 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/react-dom/cjs/react-dom-server.browser.production.min.js
--rw-r--r--   0        0        0   244170 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/react-dom/cjs/react-dom-server.node.development.js
--rw-r--r--   0        0        0    39058 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/react-dom/cjs/react-dom-server.node.production.min.js
--rw-r--r--   0        0        0    55073 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/react-dom/cjs/react-dom-test-utils.development.js
--rw-r--r--   0        0        0    12616 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/react-dom/cjs/react-dom-test-utils.production.min.js
--rw-r--r--   0        0        0  1026501 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/react-dom/cjs/react-dom.development.js
--rw-r--r--   0        0        0   131737 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/react-dom/cjs/react-dom.production.min.js
--rw-r--r--   0        0        0   141164 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/react-dom/cjs/react-dom.profiling.min.js
--rw-r--r--   0        0        0   255793 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/react-dom/umd/react-dom-server-legacy.browser.development.js
--rw-r--r--   0        0        0    35128 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/react-dom/umd/react-dom-server-legacy.browser.production.min.js
--rw-r--r--   0        0        0   254652 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/react-dom/umd/react-dom-server.browser.development.js
--rw-r--r--   0        0        0    35699 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/react-dom/umd/react-dom-server.browser.production.min.js
--rw-r--r--   0        0        0    58151 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/react-dom/umd/react-dom-test-utils.development.js
--rw-r--r--   0        0        0    12689 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/react-dom/umd/react-dom-test-utils.production.min.js
--rw-r--r--   0        0        0  1077022 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/react-dom/umd/react-dom.development.js
--rw-r--r--   0        0        0   131882 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/react-dom/umd/react-dom.production.min.js
--rw-r--r--   0        0        0   140615 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/node_modules/react-dom/umd/react-dom.profiling.min.js
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/schema/shared-link.json
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/schema/user-menu-bar.json
--rw-r--r--   0        0        0     5807 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/src/collaboration.ts
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/src/index.ts
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/src/sharedlink.ts
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/style/index.css
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/collaboration-extension/style/index.js
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider/babel.config.js
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider/jest.config.js
--rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider/package.json
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider/tsconfig.json
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider/tsconfig.test.json
--rw-r--r--   0        0        0    71721 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider/tsconfig.tsbuildinfo
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider/lib/awareness.d.ts
--rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider/lib/awareness.js
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider/lib/index.d.ts
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider/lib/index.js
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider/lib/requests.d.ts
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider/lib/requests.js
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider/lib/tokens.d.ts
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider/lib/tokens.js
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider/lib/utils.d.ts
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider/lib/utils.js
--rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider/lib/ydrive.d.ts
--rw-r--r--   0        0        0     6599 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider/lib/ydrive.js
--rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider/lib/yprovider.d.ts
--rw-r--r--   0        0        0     3906 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider/lib/yprovider.js
--rw-r--r--   0        0        0     3594 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider/src/awareness.ts
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider/src/index.ts
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider/src/requests.ts
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider/src/tokens.ts
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider/src/utils.ts
--rw-r--r--   0        0        0     6975 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider/src/ydrive.ts
--rw-r--r--   0        0        0     5061 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider/src/yprovider.ts
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider/src/__tests__/yprovider.spec.ts
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/README.md
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/package.json
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/tsconfig.json
--rw-r--r--   0        0        0   130558 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/tsconfig.tsbuildinfo
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/lib/executor.d.ts
--rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/lib/executor.js
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/lib/filebrowser.d.ts
--rw-r--r--   0        0        0     9694 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/lib/filebrowser.js
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/lib/index.d.ts
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/lib/index.js
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@jupyterlab/settingregistry/package.json
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@jupyterlab/settingregistry/lib/index.d.ts
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@jupyterlab/settingregistry/lib/index.js
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@jupyterlab/settingregistry/lib/index.js.map
--rw-r--r--   0        0        0    13651 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@jupyterlab/settingregistry/lib/plugin-schema.json
--rw-r--r--   0        0        0    15495 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@jupyterlab/settingregistry/lib/settingregistry.d.ts
--rw-r--r--   0        0        0    43561 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@jupyterlab/settingregistry/lib/settingregistry.js
--rw-r--r--   0        0        0    28805 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@jupyterlab/settingregistry/lib/settingregistry.js.map
--rw-r--r--   0        0        0    20288 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@jupyterlab/settingregistry/lib/tokens.d.ts
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@jupyterlab/settingregistry/lib/tokens.js
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@jupyterlab/settingregistry/lib/tokens.js.map
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@jupyterlab/settingregistry/src/index.ts
--rw-r--r--   0        0        0    10239 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@jupyterlab/settingregistry/src/plugin-schema.json
--rw-r--r--   0        0        0    45173 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@jupyterlab/settingregistry/src/settingregistry.ts
--rw-r--r--   0        0        0    18913 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@jupyterlab/settingregistry/src/tokens.ts
--rw-r--r--   0        0        0    10947 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/LICENSE.md
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/README.md
--rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/package.json
--rw-r--r--   0        0        0   103957 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/dist/index.js
--rw-r--r--   0        0        0   265256 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/dist/index.js.map
--rw-r--r--   0        0        0    96830 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/dist/utils.esm.js
--rw-r--r--   0        0        0   259446 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/dist/utils.esm.js.map
--rw-r--r--   0        0        0   103426 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/dist/utils.umd.js
--rw-r--r--   0        0        0     3758 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/ErrorSchemaBuilder.d.ts
--rw-r--r--   0        0        0     5254 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/ErrorSchemaBuilder.js
--rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/ErrorSchemaBuilder.js.map
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/allowAdditionalItems.d.ts
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/allowAdditionalItems.js
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/allowAdditionalItems.js.map
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/asNumber.d.ts
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/asNumber.js
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/asNumber.js.map
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/canExpand.d.ts
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/canExpand.js
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/canExpand.js.map
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/constants.d.ts
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/constants.js
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/constants.js.map
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/createErrorHandler.d.ts
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/createErrorHandler.js
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/createErrorHandler.js.map
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/createSchemaUtils.d.ts
--rw-r--r--   0        0        0    13359 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/createSchemaUtils.js
--rw-r--r--   0        0        0     3216 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/createSchemaUtils.js.map
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/dataURItoBlob.d.ts
--rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/dataURItoBlob.js
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/dataURItoBlob.js.map
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/deepEquals.d.ts
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/deepEquals.js
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/deepEquals.js.map
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/englishStringTranslator.d.ts
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/englishStringTranslator.js
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/englishStringTranslator.js.map
--rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/enumOptionsDeselectValue.d.ts
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/enumOptionsDeselectValue.js
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/enumOptionsDeselectValue.js.map
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/enumOptionsIndexForValue.d.ts
--rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/enumOptionsIndexForValue.js
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/enumOptionsIndexForValue.js.map
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/enumOptionsIsSelected.d.ts
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/enumOptionsIsSelected.js
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/enumOptionsIsSelected.js.map
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/enumOptionsSelectValue.d.ts
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/enumOptionsSelectValue.js
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/enumOptionsSelectValue.js.map
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/enumOptionsValueForIndex.d.ts
--rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/enumOptionsValueForIndex.js
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/enumOptionsValueForIndex.js.map
--rw-r--r--   0        0        0     3931 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/enums.d.ts
--rw-r--r--   0        0        0     4801 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/enums.js
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/enums.js.map
--rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/findSchemaDefinition.d.ts
--rw-r--r--   0        0        0     3977 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/findSchemaDefinition.js
--rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/findSchemaDefinition.js.map
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/getDateElementProps.d.ts
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/getDateElementProps.js
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/getDateElementProps.js.map
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/getDiscriminatorFieldFromSchema.d.ts
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/getDiscriminatorFieldFromSchema.js
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/getDiscriminatorFieldFromSchema.js.map
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/getInputProps.d.ts
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/getInputProps.js
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/getInputProps.js.map
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/getOptionMatchingSimpleDiscriminator.d.ts
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/getOptionMatchingSimpleDiscriminator.js
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/getOptionMatchingSimpleDiscriminator.js.map
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/getSchemaType.d.ts
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/getSchemaType.js
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/getSchemaType.js.map
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/getSubmitButtonOptions.d.ts
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/getSubmitButtonOptions.js
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/getSubmitButtonOptions.js.map
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/getTemplate.d.ts
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/getTemplate.js
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/getTemplate.js.map
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/getUiOptions.d.ts
--rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/getUiOptions.js
--rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/getUiOptions.js.map
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/getWidget.d.ts
--rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/getWidget.js
--rw-r--r--   0        0        0     2739 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/getWidget.js.map
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/guessType.d.ts
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/guessType.js
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/guessType.js.map
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/hasWidget.d.ts
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/hasWidget.js
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/hasWidget.js.map
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/hashForSchema.d.ts
--rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/hashForSchema.js
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/hashForSchema.js.map
--rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/idGenerators.d.ts
--rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/idGenerators.js
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/idGenerators.js.map
--rw-r--r--   0        0        0     3881 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/index.d.ts
--rw-r--r--   0        0        0     3867 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/index.js
--rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/index.js.map
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/isConstant.d.ts
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/isConstant.js
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/isConstant.js.map
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/isCustomWidget.d.ts
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/isCustomWidget.js
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/isCustomWidget.js.map
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/isFixedItems.d.ts
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/isFixedItems.js
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/isFixedItems.js.map
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/isObject.d.ts
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/isObject.js
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/isObject.js.map
--rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/labelValue.d.ts
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/labelValue.js
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/labelValue.js.map
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/localToUTC.d.ts
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/localToUTC.js
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/localToUTC.js.map
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/mergeDefaultsWithFormData.d.ts
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/mergeDefaultsWithFormData.js
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/mergeDefaultsWithFormData.js.map
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/mergeObjects.d.ts
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/mergeObjects.js
--rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/mergeObjects.js.map
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/mergeSchemas.d.ts
--rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/mergeSchemas.js
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/mergeSchemas.js.map
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/optionsList.d.ts
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/optionsList.js
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/optionsList.js.map
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/orderProperties.d.ts
--rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/orderProperties.js
--rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/orderProperties.js.map
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/pad.d.ts
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/pad.js
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/pad.js.map
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/parseDateString.d.ts
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/parseDateString.js
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/parseDateString.js.map
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/rangeSpec.d.ts
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/rangeSpec.js
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/rangeSpec.js.map
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/replaceStringParameters.d.ts
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/replaceStringParameters.js
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/replaceStringParameters.js.map
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schemaRequiresTrueValue.d.ts
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schemaRequiresTrueValue.js
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schemaRequiresTrueValue.js.map
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/shouldRender.d.ts
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/shouldRender.js
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/shouldRender.js.map
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/toConstant.d.ts
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/toConstant.js
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/toConstant.js.map
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/toDateString.d.ts
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/toDateString.js
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/toDateString.js.map
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/toErrorList.d.ts
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/toErrorList.js
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/toErrorList.js.map
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/toErrorSchema.d.ts
--rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/toErrorSchema.js
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/toErrorSchema.js.map
--rw-r--r--   0        0        0    67837 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/tsconfig.tsbuildinfo
--rw-r--r--   0        0        0    57219 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/types.d.ts
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/types.js
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/types.js.map
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/unwrapErrorHandler.d.ts
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/unwrapErrorHandler.js
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/unwrapErrorHandler.js.map
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/utcToLocal.d.ts
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/utcToLocal.js
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/utcToLocal.js.map
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/validationDataMerge.d.ts
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/validationDataMerge.js
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/validationDataMerge.js.map
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/withIdRefPrefix.d.ts
--rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/withIdRefPrefix.js
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/withIdRefPrefix.js.map
--rw-r--r--   0        0        0     4257 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/parser/ParserValidator.d.ts
--rw-r--r--   0        0        0     5010 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/parser/ParserValidator.js
--rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/parser/ParserValidator.js.map
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/parser/index.d.ts
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/parser/index.js
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/parser/index.js.map
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/parser/schemaParser.d.ts
--rw-r--r--   0        0        0     2672 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/parser/schemaParser.js
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/parser/schemaParser.js.map
--rw-r--r--   0        0        0     4194 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/getClosestMatchingOption.d.ts
--rw-r--r--   0        0        0     8998 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/getClosestMatchingOption.js
--rw-r--r--   0        0        0     4361 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/getClosestMatchingOption.js.map
--rw-r--r--   0        0        0     5391 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/getDefaultFormState.d.ts
--rw-r--r--   0        0        0    22107 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/getDefaultFormState.js
--rw-r--r--   0        0        0    10811 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/getDefaultFormState.js.map
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/getDisplayLabel.d.ts
--rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/getDisplayLabel.js
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/getDisplayLabel.js.map
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/getFirstMatchingOption.d.ts
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/getFirstMatchingOption.js
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/getFirstMatchingOption.js.map
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/getMatchingOption.d.ts
--rw-r--r--   0        0        0     4231 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/getMatchingOption.js
--rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/getMatchingOption.js.map
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/index.d.ts
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/index.js
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/index.js.map
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/isFilesArray.d.ts
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/isFilesArray.js
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/isFilesArray.js.map
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/isMultiSelect.d.ts
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/isMultiSelect.js
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/isMultiSelect.js.map
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/isSelect.d.ts
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/isSelect.js
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/isSelect.js.map
--rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/mergeValidationData.d.ts
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/mergeValidationData.js
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/mergeValidationData.js.map
--rw-r--r--   0        0        0    15291 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/retrieveSchema.d.ts
--rw-r--r--   0        0        0    28066 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/retrieveSchema.js
--rw-r--r--   0        0        0    13290 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/retrieveSchema.js.map
--rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/sanitizeDataForNewSchema.d.ts
--rw-r--r--   0        0        0    11577 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/sanitizeDataForNewSchema.js
--rw-r--r--   0        0        0     4889 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/sanitizeDataForNewSchema.js.map
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/toIdSchema.d.ts
--rw-r--r--   0        0        0     3499 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/toIdSchema.js
--rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/toIdSchema.js.map
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/toPathSchema.d.ts
--rw-r--r--   0        0        0     4764 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/toPathSchema.js
--rw-r--r--   0        0        0     3182 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/lib/schema/toPathSchema.js.map
--rw-r--r--   0        0        0     5215 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/ErrorSchemaBuilder.ts
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/allowAdditionalItems.ts
--rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/asNumber.ts
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/canExpand.ts
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/constants.ts
--rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/createErrorHandler.ts
--rw-r--r--   0        0        0    14372 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/createSchemaUtils.ts
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/dataURItoBlob.ts
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/deepEquals.ts
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/englishStringTranslator.ts
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/enumOptionsDeselectValue.ts
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/enumOptionsIndexForValue.ts
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/enumOptionsIsSelected.ts
--rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/enumOptionsSelectValue.ts
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/enumOptionsValueForIndex.ts
--rw-r--r--   0        0        0     3914 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/enums.ts
--rw-r--r--   0        0        0     4067 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/findSchemaDefinition.ts
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/getDateElementProps.ts
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/getDiscriminatorFieldFromSchema.ts
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/getInputProps.ts
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/getOptionMatchingSimpleDiscriminator.ts
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/getSchemaType.ts
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/getSubmitButtonOptions.ts
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/getTemplate.ts
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/getUiOptions.ts
--rw-r--r--   0        0        0     4671 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/getWidget.tsx
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/guessType.ts
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/hasWidget.ts
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/hashForSchema.ts
--rw-r--r--   0        0        0     3310 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/idGenerators.ts
--rw-r--r--   0        0        0     4004 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/index.ts
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/isConstant.ts
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/isCustomWidget.ts
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/isFixedItems.ts
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/isObject.ts
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/labelValue.ts
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/localToUTC.ts
--rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/mergeDefaultsWithFormData.ts
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/mergeObjects.ts
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/mergeSchemas.ts
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/optionsList.ts
--rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/orderProperties.ts
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/pad.ts
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/parseDateString.ts
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/rangeSpec.ts
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/replaceStringParameters.ts
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/schemaRequiresTrueValue.ts
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/shouldRender.ts
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/toConstant.ts
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/toDateString.ts
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/toErrorList.ts
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/toErrorSchema.ts
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/tsconfig.json
--rw-r--r--   0        0        0    56287 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/types.ts
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/unwrapErrorHandler.ts
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/utcToLocal.ts
--rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/validationDataMerge.ts
--rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/withIdRefPrefix.ts
--rw-r--r--   0        0        0     5622 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/parser/ParserValidator.ts
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/parser/index.ts
--rw-r--r--   0        0        0     2902 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/parser/schemaParser.ts
--rw-r--r--   0        0        0     9294 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/schema/getClosestMatchingOption.ts
--rw-r--r--   0        0        0    21319 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/schema/getDefaultFormState.ts
--rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/schema/getDisplayLabel.ts
--rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/schema/getFirstMatchingOption.ts
--rw-r--r--   0        0        0     4060 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/schema/getMatchingOption.ts
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/schema/index.ts
--rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/schema/isFilesArray.ts
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/schema/isMultiSelect.ts
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/schema/isSelect.ts
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/schema/mergeValidationData.ts
--rw-r--r--   0        0        0    30469 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/schema/retrieveSchema.ts
--rw-r--r--   0        0        0    11171 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/schema/sanitizeDataForNewSchema.ts
--rw-r--r--   0        0        0     4110 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/schema/toIdSchema.ts
--rw-r--r--   0        0        0     5403 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@rjsf/utils/src/schema/toPathSchema.ts
--rwxr-xr-x   0        0        0     1141 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@types/react/LICENSE
--rwxr-xr-x   0        0        0     1916 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@types/react/README.md
--rwxr-xr-x   0        0        0     4743 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@types/react/experimental.d.ts
--rwxr-xr-x   0        0        0     7431 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@types/react/global.d.ts
--rwxr-xr-x   0        0        0   156037 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@types/react/index.d.ts
--rwxr-xr-x   0        0        0       61 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@types/react/jsx-dev-runtime.d.ts
--rwxr-xr-x   0        0        0       61 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@types/react/jsx-runtime.d.ts
--rwxr-xr-x   0        0        0     2929 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@types/react/next.d.ts
--rwxr-xr-x   0        0        0     6002 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@types/react/package.json
--rwxr-xr-x   0        0        0     4613 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@types/react/ts5.0/experimental.d.ts
--rwxr-xr-x   0        0        0     7409 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@types/react/ts5.0/global.d.ts
--rwxr-xr-x   0        0        0   152997 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@types/react/ts5.0/index.d.ts
--rwxr-xr-x   0        0        0       61 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@types/react/ts5.0/jsx-dev-runtime.d.ts
--rwxr-xr-x   0        0        0       61 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@types/react/ts5.0/jsx-runtime.d.ts
--rwxr-xr-x   0        0        0     2929 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/node_modules/@types/react/ts5.0/next.d.ts
--rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/src/executor.ts
--rw-r--r--   0        0        0     9449 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/src/filebrowser.ts
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/src/index.ts
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/style/index.css
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/packages/docprovider-extension/style/index.js
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/.gitignore
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/LICENSE
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/README.md
--rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/pyproject.toml
--rw-r--r--   0        0        0     4764 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a0/PKG-INFO
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/install.json
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/setup.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/jupyter_docprovider/__init__.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/jupyter_docprovider/_version.py
+-rw-r--r--   0        0        0     3769 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/jupyter_docprovider/labextension/package.json
+-rw-r--r--   0        0        0     5274 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/jupyter_docprovider/labextension/static/341.998da4ec9a27d6dbdb1a.js
+-rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/jupyter_docprovider/labextension/static/422.3ab44960b241aac9f303.js
+-rw-r--r--   0        0        0     5559 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/jupyter_docprovider/labextension/static/544.1c4f1124ffffdb64812e.js
+-rw-r--r--   0        0        0     5274 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/jupyter_docprovider/labextension/static/722.06cb6508a379f7976e9e.js
+-rw-r--r--   0        0        0     8193 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/jupyter_docprovider/labextension/static/944.80e0d65b220a1dfdc0ff.js
+-rw-r--r--   0        0        0    13097 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/jupyter_docprovider/labextension/static/994.c290665e94ae9503337f.js
+-rw-r--r--   0        0        0     8493 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/jupyter_docprovider/labextension/static/remoteEntry.6347eb8bae6b74aa4edc.js
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/jupyter_docprovider/labextension/static/style.js
+-rw-r--r--   0        0        0     7762 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/jupyter_docprovider/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/packages/docprovider/babel.config.js
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/packages/docprovider/jest.config.js
+-rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/packages/docprovider/package.json
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/packages/docprovider/tsconfig.json
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/packages/docprovider/tsconfig.test.json
+-rw-r--r--   0        0        0     3594 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/packages/docprovider/src/awareness.ts
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/packages/docprovider/src/index.ts
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/packages/docprovider/src/requests.ts
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/packages/docprovider/src/tokens.ts
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/packages/docprovider/src/utils.ts
+-rw-r--r--   0        0        0     6975 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/packages/docprovider/src/ydrive.ts
+-rw-r--r--   0        0        0     5061 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/packages/docprovider/src/yprovider.ts
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/packages/docprovider/src/__tests__/yprovider.spec.ts
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/packages/docprovider-extension/README.md
+-rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/packages/docprovider-extension/package.json
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/packages/docprovider-extension/tsconfig.json
+-rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/packages/docprovider-extension/src/executor.ts
+-rw-r--r--   0        0        0     9449 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/packages/docprovider-extension/src/filebrowser.ts
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/packages/docprovider-extension/src/index.ts
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/packages/docprovider-extension/style/index.css
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/packages/docprovider-extension/style/index.js
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/.gitignore
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/LICENSE
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/README.md
+-rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/pyproject.toml
+-rw-r--r--   0        0        0     4764 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/PKG-INFO
```

### Comparing `jupyter_docprovider-1.0.0a0/jupyter_docprovider/labextension/package.json` & `jupyter_docprovider-1.0.0a1/jupyter_docprovider/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761363636363637%*

 * *Differences: {"'dependencies'": "{'@jupyter/docprovider': '^3.0.0-alpha.1'}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.6347eb8bae6b74aa4edc.js'}}",*

 * * "'version'": "'3.0.0-alpha.1'"}*

```diff
@@ -1,14 +1,14 @@
 {
     "author": "Project Jupyter",
     "bugs": {
         "url": "https://github.com/jupyterlab/jupyter-collaboration/issues"
     },
     "dependencies": {
-        "@jupyter/docprovider": "^3.0.0-alpha.0",
+        "@jupyter/docprovider": "^3.0.0-alpha.1",
         "@jupyter/ydoc": "^1.1.0-a0",
         "@jupyterlab/application": "^4.2.0-beta.0",
         "@jupyterlab/apputils": "^4.2.0-beta.0",
         "@jupyterlab/docregistry": "^4.2.0-beta.0",
         "@jupyterlab/filebrowser": "^4.2.0-beta.0",
         "@jupyterlab/fileeditor": "^4.2.0-beta.0",
         "@jupyterlab/logconsole": "^4.2.0-beta.0",
@@ -39,15 +39,15 @@
         "style/*.css",
         "style/index.js"
     ],
     "homepage": "https://github.com/jupyterlab/jupyter-collaboration",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.2108b01380418facade4.js",
+            "load": "static/remoteEntry.6347eb8bae6b74aa4edc.js",
             "style": "./style"
         },
         "disabledExtensions": [
             "@jupyterlab/filebrowser-extension:defaultFileBrowser",
             "@jupyterlab/notebook-extension:cell-executor"
         ],
         "extension": true,
@@ -119,9 +119,9 @@
     "typedoc": {
         "displayName": "@jupyter/docprovider-extension",
         "entryPoint": "./src/index.ts",
         "readmeFile": "./README.md",
         "tsconfig": "./tsconfig.json"
     },
     "types": "lib/index.d.ts",
-    "version": "3.0.0-alpha.0"
+    "version": "3.0.0-alpha.1"
 }
```

### Comparing `jupyter_docprovider-1.0.0a0/jupyter_docprovider/labextension/static/341.3263d2726bd17de1c784.js` & `jupyter_docprovider-1.0.0a1/jupyter_docprovider/labextension/static/341.998da4ec9a27d6dbdb1a.js`

 * *Files 1% similar despite different names*

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
-            var h = t(597),
-                d = t(486),
-                _ = t(638),
+            var h = t(655),
+                d = t(824),
+                _ = t(440),
                 l = t(262);
             class p {
                 constructor(e) {
                     this._onConnectionClosed = e => {
                         1003 === e.code && (console.error("Document provider closed:", e.reason), (0, _.showErrorMessage)(this._trans.__("Document session error"), e.reason, [_.Dialog.okButton()]), this._sharedModel.dispose())
                     }, this._onSync = e => {
                         var s;
```

### Comparing `jupyter_docprovider-1.0.0a0/jupyter_docprovider/labextension/static/422.3ab44960b241aac9f303.js` & `jupyter_docprovider-1.0.0a1/jupyter_docprovider/labextension/static/422.3ab44960b241aac9f303.js`

 * *Files identical despite different names*

### Comparing `jupyter_docprovider-1.0.0a0/jupyter_docprovider/labextension/static/544.31cdd3fa47e3d8404c4e.js` & `jupyter_docprovider-1.0.0a1/jupyter_docprovider/labextension/static/544.1c4f1124ffffdb64812e.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,24 +1,24 @@
 "use strict";
 (self.webpackChunk_jupyter_docprovider_extension = self.webpackChunk_jupyter_docprovider_extension || []).push([
     [544], {
         544: (e, o, t) => {
             t.r(o), t.d(o, {
                 default: () => _
             });
-            var r, n = t(465),
-                i = t(638),
-                a = t(221),
-                s = t(74),
-                l = t(478),
-                c = t(372),
-                d = t(618),
-                u = t(714),
+            var r, n = t(371),
+                i = t(440),
+                a = t(943),
+                s = t(716),
+                l = t(312),
+                c = t(506),
+                d = t(500),
+                u = t(844),
                 v = t(667),
-                p = t(424);
+                p = t(835);
             ! function(e) {
                 e.openPath = "filebrowser:open-path"
             }(r || (r = {}));
             const g = {
                     id: "@jupyter/docprovider-extension:drive",
                     description: "The default collaborative drive provider",
                     provides: p.ICollaborativeDrive,
@@ -139,16 +139,16 @@
                             path: l.browser,
                             dontShowBrowser: !0
                         })) : (await e.model.restore(e.id), await e.model.refresh()), e.removeClass(a), (null == i ? void 0 : i.isEmpty("main")) && o.execute("launcher:create")
                     };
                     t.routed.connect(s)
                 }
             }(b || (b = {}));
-            var f = t(597),
-                k = t(486);
+            var f = t(655),
+                k = t(824);
             async function x({
                 cell: e,
                 notebook: o,
                 notebookConfig: t,
                 onCellExecuted: r,
                 onCellExecutionScheduled: n,
                 sessionContext: i,
```

### Comparing `jupyter_docprovider-1.0.0a0/jupyter_docprovider/labextension/static/722.2c1eed8483724a302f59.js` & `jupyter_docprovider-1.0.0a1/jupyter_docprovider/labextension/static/722.06cb6508a379f7976e9e.js`

 * *Files 1% similar despite different names*

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
-            var h = t(597),
-                d = t(486),
-                _ = t(638),
+            var h = t(655),
+                d = t(824),
+                _ = t(440),
                 l = t(262);
             class p {
                 constructor(e) {
                     this._onConnectionClosed = e => {
                         1003 === e.code && (console.error("Document provider closed:", e.reason), (0, _.showErrorMessage)(this._trans.__("Document session error"), e.reason, [_.Dialog.okButton()]), this._sharedModel.dispose())
                     }, this._onSync = e => {
                         var s;
```

### Comparing `jupyter_docprovider-1.0.0a0/jupyter_docprovider/labextension/static/944.80e0d65b220a1dfdc0ff.js` & `jupyter_docprovider-1.0.0a1/jupyter_docprovider/labextension/static/944.80e0d65b220a1dfdc0ff.js`

 * *Files identical despite different names*

### Comparing `jupyter_docprovider-1.0.0a0/jupyter_docprovider/labextension/static/994.c290665e94ae9503337f.js` & `jupyter_docprovider-1.0.0a1/jupyter_docprovider/labextension/static/994.c290665e94ae9503337f.js`

 * *Files identical despite different names*

### Comparing `jupyter_docprovider-1.0.0a0/jupyter_docprovider/labextension/static/remoteEntry.2108b01380418facade4.js` & `jupyter_docprovider-1.0.0a1/jupyter_docprovider/labextension/static/remoteEntry.6347eb8bae6b74aa4edc.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -1,31 +1,31 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, o, n, a, i, l, u, f, d, s, p, c, h, v, b, y, g, m, j, w = {
-            141: (e, r, t) => {
+    var e, r, t, o, a, n, i, l, u, f, s, d, p, c, h, v, b, y, g, m, j, w = {
+            496: (e, r, t) => {
                 var o = {
-                        "./index": () => Promise.all([t.e(327), t.e(544)]).then((() => () => t(544))),
-                        "./extension": () => Promise.all([t.e(327), t.e(544)]).then((() => () => t(544))),
+                        "./index": () => Promise.all([t.e(393), t.e(544)]).then((() => () => t(544))),
+                        "./extension": () => Promise.all([t.e(393), t.e(544)]).then((() => () => t(544))),
                         "./style": () => t.e(944).then((() => () => t(944)))
                     },
-                    n = (e, r) => (t.R = r, r = t.o(o, e) ? o[e]() : Promise.resolve().then((() => {
+                    a = (e, r) => (t.R = r, r = t.o(o, e) ? o[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
-                    a = (e, r) => {
+                    n = (e, r) => {
                         if (t.S) {
                             var o = "default",
-                                n = t.S[o];
-                            if (n && n !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
+                                a = t.S[o];
+                            if (a && a !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
                             return t.S[o] = e, t.I(o, r)
                         }
                     };
                 t.d(r, {
-                    get: () => n,
-                    init: () => a
+                    get: () => a,
+                    init: () => n
                 })
             }
         },
         P = {};
 
     function S(e) {
         var r = P[e];
@@ -44,92 +44,92 @@
     }, S.d = (e, r) => {
         for (var t in r) S.o(r, t) && !S.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, S.f = {}, S.e = e => Promise.all(Object.keys(S.f).reduce(((r, t) => (S.f[t](e, r), r)), [])), S.u = e => e + "." + {
         206: "346950b0376f11c0b868",
-        327: "a7c710e443f77972800b",
-        341: "3263d2726bd17de1c784",
+        341: "998da4ec9a27d6dbdb1a",
+        393: "39aa8f8542ebf94ba223",
         422: "3ab44960b241aac9f303",
-        544: "31cdd3fa47e3d8404c4e",
+        544: "1c4f1124ffffdb64812e",
         652: "282f02247000ea4106c5",
-        722: "2c1eed8483724a302f59",
+        722: "06cb6508a379f7976e9e",
         944: "80e0d65b220a1dfdc0ff",
         994: "c290665e94ae9503337f"
     } [e] + ".js?v=" + {
         206: "346950b0376f11c0b868",
-        327: "a7c710e443f77972800b",
-        341: "3263d2726bd17de1c784",
+        341: "998da4ec9a27d6dbdb1a",
+        393: "39aa8f8542ebf94ba223",
         422: "3ab44960b241aac9f303",
-        544: "31cdd3fa47e3d8404c4e",
+        544: "1c4f1124ffffdb64812e",
         652: "282f02247000ea4106c5",
-        722: "2c1eed8483724a302f59",
+        722: "06cb6508a379f7976e9e",
         944: "80e0d65b220a1dfdc0ff",
         994: "c290665e94ae9503337f"
     } [e], S.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), S.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@jupyter/docprovider-extension:", S.l = (t, o, n, a) => {
+    }(), S.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@jupyter/docprovider-extension:", S.l = (t, o, a, n) => {
         if (e[t]) e[t].push(o);
         else {
             var i, l;
-            if (void 0 !== n)
+            if (void 0 !== a)
                 for (var u = document.getElementsByTagName("script"), f = 0; f < u.length; f++) {
-                    var d = u[f];
-                    if (d.getAttribute("src") == t || d.getAttribute("data-webpack") == r + n) {
-                        i = d;
+                    var s = u[f];
+                    if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + a) {
+                        i = s;
                         break
                     }
                 }
-            i || (l = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, S.nc && i.setAttribute("nonce", S.nc), i.setAttribute("data-webpack", r + n), i.src = t), e[t] = [o];
-            var s = (r, o) => {
+            i || (l = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, S.nc && i.setAttribute("nonce", S.nc), i.setAttribute("data-webpack", r + a), i.src = t), e[t] = [o];
+            var d = (r, o) => {
                     i.onerror = i.onload = null, clearTimeout(p);
-                    var n = e[t];
-                    if (delete e[t], i.parentNode && i.parentNode.removeChild(i), n && n.forEach((e => e(o))), r) return r(o)
+                    var a = e[t];
+                    if (delete e[t], i.parentNode && i.parentNode.removeChild(i), a && a.forEach((e => e(o))), r) return r(o)
                 },
-                p = setTimeout(s.bind(null, void 0, {
+                p = setTimeout(d.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = s.bind(null, i.onerror), i.onload = s.bind(null, i.onload), l && document.head.appendChild(i)
+            i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), l && document.head.appendChild(i)
         }
     }, S.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
     }, (() => {
         S.S = {};
         var e = {},
             r = {};
         S.I = (t, o) => {
             o || (o = []);
-            var n = r[t];
-            if (n || (n = r[t] = {}), !(o.indexOf(n) >= 0)) {
-                if (o.push(n), e[t]) return e[t];
+            var a = r[t];
+            if (a || (a = r[t] = {}), !(o.indexOf(a) >= 0)) {
+                if (o.push(a), e[t]) return e[t];
                 S.o(S.S, t) || (S.S[t] = {});
-                var a = S.S[t],
+                var n = S.S[t],
                     i = "@jupyter/docprovider-extension",
                     l = (e, r, t, o) => {
-                        var n = a[e] = a[e] || {},
-                            l = n[r];
-                        (!l || !l.loaded && (!o != !l.eager ? o : i > l.from)) && (n[r] = {
+                        var a = n[e] = n[e] || {},
+                            l = a[r];
+                        (!l || !l.loaded && (!o != !l.eager ? o : i > l.from)) && (a[r] = {
                             get: t,
                             from: i,
                             eager: !!o
                         })
                     },
                     u = [];
-                return "default" === t && (l("@jupyter/docprovider-extension", "3.0.0-alpha.0", (() => Promise.all([S.e(327), S.e(544)]).then((() => () => S(544))))), l("@jupyter/docprovider", "3.0.0-alpha.0", (() => Promise.all([S.e(422), S.e(652), S.e(327), S.e(341)]).then((() => () => S(341))))), l("y-websocket", "1.5.4", (() => Promise.all([S.e(422), S.e(994), S.e(206)]).then((() => () => S(994)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                return "default" === t && (l("@jupyter/docprovider-extension", "3.0.0-alpha.1", (() => Promise.all([S.e(393), S.e(544)]).then((() => () => S(544))))), l("@jupyter/docprovider", "3.0.0-alpha.1", (() => Promise.all([S.e(422), S.e(652), S.e(393), S.e(341)]).then((() => () => S(341))))), l("y-websocket", "1.5.4", (() => Promise.all([S.e(422), S.e(994), S.e(206)]).then((() => () => S(994)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         S.g.importScripts && (e = S.g.location + "");
         var r = S.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -144,119 +144,119 @@
             t = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
             o = t[1] ? r(t[1]) : [];
         return t[2] && (o.length++, o.push.apply(o, r(t[2]))), t[3] && (o.push([]), o.push.apply(o, r(t[3]))), o
     }, o = (e, r) => {
         e = t(e), r = t(r);
         for (var o = 0;;) {
             if (o >= e.length) return o < r.length && "u" != (typeof r[o])[0];
-            var n = e[o],
-                a = (typeof n)[0];
-            if (o >= r.length) return "u" == a;
+            var a = e[o],
+                n = (typeof a)[0];
+            if (o >= r.length) return "u" == n;
             var i = r[o],
                 l = (typeof i)[0];
-            if (a != l) return "o" == a && "n" == l || "s" == l || "u" == a;
-            if ("o" != a && "u" != a && n != i) return n < i;
+            if (n != l) return "o" == n && "n" == l || "s" == l || "u" == n;
+            if ("o" != n && "u" != n && a != i) return a < i;
             o++
         }
-    }, n = e => {
+    }, a = e => {
         var r = e[0],
             t = "";
         if (1 === e.length) return "*";
         if (r + .5) {
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
-            for (var o = 1, a = 1; a < e.length; a++) o--, t += "u" == (typeof(l = e[a]))[0] ? "-" : (o > 0 ? "." : "") + (o = 2, l);
+            for (var o = 1, n = 1; n < e.length; n++) o--, t += "u" == (typeof(l = e[n]))[0] ? "-" : (o > 0 ? "." : "") + (o = 2, l);
             return t
         }
         var i = [];
-        for (a = 1; a < e.length; a++) {
-            var l = e[a];
-            i.push(0 === l ? "not(" + u() + ")" : 1 === l ? "(" + u() + " || " + u() + ")" : 2 === l ? i.pop() + " " + i.pop() : n(l))
+        for (n = 1; n < e.length; n++) {
+            var l = e[n];
+            i.push(0 === l ? "not(" + u() + ")" : 1 === l ? "(" + u() + " || " + u() + ")" : 2 === l ? i.pop() + " " + i.pop() : a(l))
         }
         return u();
 
         function u() {
             return i.pop().replace(/^\((.+)\)$/, "$1")
         }
-    }, a = (e, r) => {
+    }, n = (e, r) => {
         if (0 in e) {
             r = t(r);
             var o = e[0],
-                n = o < 0;
-            n && (o = -o - 1);
+                a = o < 0;
+            a && (o = -o - 1);
             for (var i = 0, l = 1, u = !0;; l++, i++) {
-                var f, d, s = l < e.length ? (typeof e[l])[0] : "";
-                if (i >= r.length || "o" == (d = (typeof(f = r[i]))[0])) return !u || ("u" == s ? l > o && !n : "" == s != n);
-                if ("u" == d) {
-                    if (!u || "u" != s) return !1
+                var f, s, d = l < e.length ? (typeof e[l])[0] : "";
+                if (i >= r.length || "o" == (s = (typeof(f = r[i]))[0])) return !u || ("u" == d ? l > o && !a : "" == d != a);
+                if ("u" == s) {
+                    if (!u || "u" != d) return !1
                 } else if (u)
-                    if (s == d)
+                    if (d == s)
                         if (l <= o) {
                             if (f != e[l]) return !1
                         } else {
-                            if (n ? f > e[l] : f < e[l]) return !1;
+                            if (a ? f > e[l] : f < e[l]) return !1;
                             f != e[l] && (u = !1)
                         }
-                else if ("s" != s && "n" != s) {
-                    if (n || l <= o) return !1;
+                else if ("s" != d && "n" != d) {
+                    if (a || l <= o) return !1;
                     u = !1, l--
                 } else {
-                    if (l <= o || d < s != n) return !1;
+                    if (l <= o || s < d != a) return !1;
                     u = !1
-                } else "s" != s && "n" != s && (u = !1, l--)
+                } else "s" != d && "n" != d && (u = !1, l--)
             }
         }
         var p = [],
             c = p.pop.bind(p);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
-            p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? a(h, r) : !c())
+            p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? n(h, r) : !c())
         }
         return !!c()
     }, i = (e, r) => {
         var t = S.S[e];
         if (!t || !S.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, l = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && o(e, r) ? r : e), 0)
-    }, u = (e, r, t, o) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + n(o) + ")", f = (e, r, t, o) => {
-        var n = l(e, t);
-        return a(o, n) || s(u(e, t, n, o)), p(e[t][n])
-    }, d = (e, r, t) => {
-        var n = e[r];
-        return (r = Object.keys(n).reduce(((e, r) => !a(t, r) || e && !o(e, r) ? e : r), 0)) && n[r]
-    }, s = e => {
+    }, u = (e, r, t, o) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + a(o) + ")", f = (e, r, t, o) => {
+        var a = l(e, t);
+        return n(o, a) || d(u(e, t, a, o)), p(e[t][a])
+    }, s = (e, r, t) => {
+        var a = e[r];
+        return (r = Object.keys(a).reduce(((e, r) => !n(t, r) || e && !o(e, r) ? e : r), 0)) && a[r]
+    }, d = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
-    }, p = e => (e.loaded = 1, e.get()), h = (c = e => function(r, t, o, n) {
-        var a = S.I(r);
-        return a && a.then ? a.then(e.bind(e, r, S.S[r], t, o, n)) : e(r, S.S[r], t, o, n)
-    })(((e, r, t, o) => (i(e, t), f(r, 0, t, o)))), v = c(((e, r, t, o, n) => r && S.o(r, t) ? f(r, 0, t, o) : n())), b = c(((e, r, t, o, n) => {
-        var a = r && S.o(r, t) && d(r, t, o);
-        return a ? p(a) : n()
+    }, p = e => (e.loaded = 1, e.get()), h = (c = e => function(r, t, o, a) {
+        var n = S.I(r);
+        return n && n.then ? n.then(e.bind(e, r, S.S[r], t, o, a)) : e(r, S.S[r], t, o, a)
+    })(((e, r, t, o) => (i(e, t), f(r, 0, t, o)))), v = c(((e, r, t, o, a) => r && S.o(r, t) ? f(r, 0, t, o) : a())), b = c(((e, r, t, o, a) => {
+        var n = r && S.o(r, t) && s(r, t, o);
+        return n ? p(n) : a()
     })), y = {}, g = {
-        486: () => h("default", "@jupyterlab/services", [1, 7, 1, 6]),
-        597: () => h("default", "@jupyterlab/coreutils", [1, 6, 1, 6]),
-        638: () => h("default", "@jupyterlab/apputils", [1, 4, 2, 6]),
-        74: () => h("default", "@jupyterlab/fileeditor", [1, 4, 1, 6]),
-        221: () => h("default", "@jupyterlab/filebrowser", [1, 4, 1, 6]),
-        372: () => h("default", "@jupyterlab/notebook", [1, 4, 1, 6]),
-        424: () => v("default", "@jupyter/docprovider", [1, 3, 0, 0, , "alpha", 0], (() => Promise.all([S.e(422), S.e(652), S.e(722)]).then((() => () => S(341))))),
-        465: () => h("default", "@jupyterlab/application", [1, 4, 1, 6]),
-        478: () => h("default", "@jupyterlab/logconsole", [1, 4, 1, 6]),
-        618: () => h("default", "@jupyterlab/settingregistry", [1, 4, 1, 6]),
+        440: () => h("default", "@jupyterlab/apputils", [1, 4, 2, 8]),
+        655: () => h("default", "@jupyterlab/coreutils", [1, 6, 1, 8]),
+        824: () => h("default", "@jupyterlab/services", [1, 7, 1, 8]),
+        312: () => h("default", "@jupyterlab/logconsole", [1, 4, 1, 8]),
+        371: () => h("default", "@jupyterlab/application", [1, 4, 1, 8]),
+        500: () => h("default", "@jupyterlab/settingregistry", [1, 4, 1, 8]),
+        506: () => h("default", "@jupyterlab/notebook", [1, 4, 1, 8]),
         667: () => h("default", "@jupyter/ydoc", [1, 1, 1, 1]),
-        714: () => h("default", "@jupyterlab/translation", [1, 4, 1, 6]),
+        716: () => h("default", "@jupyterlab/fileeditor", [1, 4, 1, 8]),
+        835: () => v("default", "@jupyter/docprovider", [1, 3, 0, 0, , "alpha", 1], (() => Promise.all([S.e(422), S.e(652), S.e(722)]).then((() => () => S(341))))),
+        844: () => h("default", "@jupyterlab/translation", [1, 4, 1, 8]),
+        943: () => h("default", "@jupyterlab/filebrowser", [1, 4, 1, 8]),
         262: () => h("default", "@lumino/coreutils", [1, 2, 0, 0]),
         560: () => b("default", "y-websocket", [1, 1, 3, 15], (() => Promise.all([S.e(994), S.e(206)]).then((() => () => S(994))))),
         602: () => h("default", "@lumino/signaling", [1, 2, 0, 0]),
         206: () => h("default", "yjs", [1, 13, 5, 40])
     }, m = {
         206: [206],
-        327: [486, 597, 638],
-        544: [74, 221, 372, 424, 465, 478, 618, 667, 714],
+        393: [440, 655, 824],
+        544: [312, 371, 500, 506, 667, 716, 835, 844, 943],
         652: [262, 560, 602]
     }, j = {}, S.f.consumes = (e, r) => {
         S.o(m, e) && m[e].forEach((e => {
             if (S.o(y, e)) return r.push(y[e]);
             if (!j[e]) {
                 var t = r => {
                     y[e] = 0, S.m[e] = t => {
@@ -266,52 +266,52 @@
                 j[e] = !0;
                 var o = r => {
                     delete y[e], S.m[e] = t => {
                         throw delete S.c[e], r
                     }
                 };
                 try {
-                    var n = g[e]();
-                    n.then ? r.push(y[e] = n.then(t).catch(o)) : t(n)
+                    var a = g[e]();
+                    a.then ? r.push(y[e] = a.then(t).catch(o)) : t(a)
                 } catch (e) {
                     o(e)
                 }
             }
         }))
     }, (() => {
         var e = {
             552: 0
         };
         S.f.j = (r, t) => {
             var o = S.o(e, r) ? e[r] : void 0;
             if (0 !== o)
                 if (o) t.push(o[2]);
-                else if (/^(206|327|652)$/.test(r)) e[r] = 0;
+                else if (/^(206|393|652)$/.test(r)) e[r] = 0;
             else {
-                var n = new Promise(((t, n) => o = e[r] = [t, n]));
-                t.push(o[2] = n);
-                var a = S.p + S.u(r),
+                var a = new Promise(((t, a) => o = e[r] = [t, a]));
+                t.push(o[2] = a);
+                var n = S.p + S.u(r),
                     i = new Error;
-                S.l(a, (t => {
+                S.l(n, (t => {
                     if (S.o(e, r) && (0 !== (o = e[r]) && (e[r] = void 0), o)) {
-                        var n = t && ("load" === t.type ? "missing" : t.type),
-                            a = t && t.target && t.target.src;
-                        i.message = "Loading chunk " + r + " failed.\n(" + n + ": " + a + ")", i.name = "ChunkLoadError", i.type = n, i.request = a, o[1](i)
+                        var a = t && ("load" === t.type ? "missing" : t.type),
+                            n = t && t.target && t.target.src;
+                        i.message = "Loading chunk " + r + " failed.\n(" + a + ": " + n + ")", i.name = "ChunkLoadError", i.type = a, i.request = n, o[1](i)
                     }
                 }), "chunk-" + r, r)
             }
         };
         var r = (r, t) => {
-                var o, n, [a, i, l] = t,
+                var o, a, [n, i, l] = t,
                     u = 0;
-                if (a.some((r => 0 !== e[r]))) {
+                if (n.some((r => 0 !== e[r]))) {
                     for (o in i) S.o(i, o) && (S.m[o] = i[o]);
                     l && l(S)
                 }
-                for (r && r(t); u < a.length; u++) n = a[u], S.o(e, n) && e[n] && e[n][0](), e[n] = 0
+                for (r && r(t); u < n.length; u++) a = n[u], S.o(e, a) && e[a] && e[a][0](), e[a] = 0
             },
             t = self.webpackChunk_jupyter_docprovider_extension = self.webpackChunk_jupyter_docprovider_extension || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), S.nc = void 0;
-    var x = S(141);
+    var x = S(496);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@jupyter/docprovider-extension"] = x
 })();
```

### Comparing `jupyter_docprovider-1.0.0a0/jupyter_docprovider/labextension/static/third-party-licenses.json` & `jupyter_docprovider-1.0.0a1/jupyter_docprovider/labextension/static/third-party-licenses.json`

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

### Comparing `jupyter_docprovider-1.0.0a0/packages/collaboration/node_modules/@jupyterlab/observables/package.json` & `jupyter_docprovider-1.0.0a1/packages/docprovider/package.json`

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

### Comparing `jupyter_docprovider-1.0.0a0/packages/collaboration-extension/package.json` & `jupyter_docprovider-1.0.0a1/packages/docprovider-extension/package.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9014979338842977%*

 * *Differences: {"'dependencies'": "{'@jupyter/docprovider': '^3.0.0-alpha.1', '@jupyterlab/docregistry': "*

 * *                   "'^4.2.0-beta.0', '@jupyterlab/filebrowser': '^4.2.0-beta.0', "*

 * *                   "'@jupyterlab/fileeditor': '^4.2.0-beta.0', '@jupyterlab/logconsole': "*

 * *                   "'^4.2.0-beta.0', '@jupyterlab/notebook': '^4.2.0-beta.0', "*

 * *                   "'@jupyterlab/settingregistry': '^4.2.0-beta.0', '@lumino/commands': '^2.1.0', "*

 * *                   "delete: ['@jupyter/collaboration', '@jupyterla […]*

```diff
@@ -1,30 +1,30 @@
 {
     "author": "Project Jupyter",
     "bugs": {
         "url": "https://github.com/jupyterlab/jupyter-collaboration/issues"
     },
     "dependencies": {
-        "@jupyter/collaboration": "^3.0.0-alpha.0",
-        "@jupyter/docprovider": "^3.0.0-alpha.0",
+        "@jupyter/docprovider": "^3.0.0-alpha.1",
         "@jupyter/ydoc": "^1.1.0-a0",
         "@jupyterlab/application": "^4.2.0-beta.0",
         "@jupyterlab/apputils": "^4.2.0-beta.0",
-        "@jupyterlab/codemirror": "^4.2.0-beta.0",
-        "@jupyterlab/coreutils": "^6.0.5",
-        "@jupyterlab/services": "^7.0.5",
-        "@jupyterlab/statedb": "^4.2.0-beta.0",
+        "@jupyterlab/docregistry": "^4.2.0-beta.0",
+        "@jupyterlab/filebrowser": "^4.2.0-beta.0",
+        "@jupyterlab/fileeditor": "^4.2.0-beta.0",
+        "@jupyterlab/logconsole": "^4.2.0-beta.0",
+        "@jupyterlab/notebook": "^4.2.0-beta.0",
+        "@jupyterlab/settingregistry": "^4.2.0-beta.0",
         "@jupyterlab/translation": "^4.2.0-beta.0",
-        "@jupyterlab/ui-components": "^4.2.0-beta.0",
-        "@lumino/widgets": "^2.1.0",
+        "@lumino/commands": "^2.1.0",
         "y-protocols": "^1.0.5",
         "y-websocket": "^1.3.15",
         "yjs": "^13.5.40"
     },
-    "description": "JupyterLab - Real-Time Collaboration Extension",
+    "description": "JupyterLab - Collaborative Shared Models",
     "devDependencies": {
         "@jupyterlab/builder": "^4.0.5",
         "@types/react": "~18.0.26",
         "npm-run-all": "^4.1.5",
         "rimraf": "^4.1.2",
         "typescript": "~5.0.4"
     },
@@ -37,30 +37,29 @@
         "lib/*.js",
         "schema/*.json",
         "style/*.css",
         "style/index.js"
     ],
     "homepage": "https://github.com/jupyterlab/jupyter-collaboration",
     "jupyterlab": {
+        "disabledExtensions": [
+            "@jupyterlab/filebrowser-extension:defaultFileBrowser",
+            "@jupyterlab/notebook-extension:cell-executor"
+        ],
         "extension": true,
-        "outputDir": "../../projects/jupyter-collaboration-ui/jupyter_collaboration_ui/labextension",
-        "schemaDir": "./schema",
+        "outputDir": "../../projects/jupyter-docprovider/jupyter_docprovider/labextension",
         "sharedPackages": {
             "@codemirror/state": {
                 "bundled": false,
                 "singleton": true
             },
             "@codemirror/view": {
                 "bundled": false,
                 "singleton": true
             },
-            "@jupyter/collaboration": {
-                "bundled": true,
-                "singleton": true
-            },
             "@jupyter/docprovider": {
                 "bundled": true,
                 "singleton": true
             },
             "@jupyter/ydoc": {
                 "bundled": false,
                 "singleton": true
@@ -78,15 +77,15 @@
     "keywords": [
         "jupyter",
         "jupyterlab",
         "jupyterlab-extension"
     ],
     "license": "BSD-3-Clause",
     "main": "lib/index.js",
-    "name": "@jupyter/collaboration-extension",
+    "name": "@jupyter/docprovider-extension",
     "publishConfig": {
         "access": "public"
     },
     "repository": {
         "type": "git",
         "url": "https://github.com/jupyterlab/jupyter-collaboration.git"
     },
@@ -95,29 +94,29 @@
         "build:labextension": "jupyter labextension build .",
         "build:labextension:dev": "jupyter labextension build --development True .",
         "build:lib": "tsc --sourceMap",
         "build:lib:prod": "tsc",
         "build:prod": "jlpm run clean && jlpm run build:lib:prod && jlpm run build:labextension",
         "clean": "jlpm run clean:lib",
         "clean:all": "jlpm run clean:lib && jlpm run clean:labextension",
-        "clean:labextension": "rimraf ../../projects/jupyter-collaboration-ui/jupyter_collaboration_ui/labextension",
+        "clean:labextension": "rimraf ../../projects/jupyter-docprovider/jupyter_docprovider/labextension",
         "clean:lib": "rimraf lib tsconfig.tsbuildinfo node_modules",
         "install:extension": "jlpm run build",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "typedoc": {
-        "displayName": "@jupyter/collaboration-extension",
+        "displayName": "@jupyter/docprovider-extension",
         "entryPoint": "./src/index.ts",
         "readmeFile": "./README.md",
         "tsconfig": "./tsconfig.json"
     },
     "types": "lib/index.d.ts",
-    "version": "3.0.0-alpha.0"
+    "version": "3.0.0-alpha.1"
 }
```

### Comparing `jupyter_docprovider-1.0.0a0/packages/docprovider/jest.config.js` & `jupyter_docprovider-1.0.0a1/packages/docprovider/jest.config.js`

 * *Files identical despite different names*

### Comparing `jupyter_docprovider-1.0.0a0/packages/docprovider/lib/requests.js` & `jupyter_docprovider-1.0.0a1/packages/docprovider/src/requests.ts`

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

### Comparing `jupyter_docprovider-1.0.0a0/packages/docprovider/lib/tokens.d.ts` & `jupyter_docprovider-1.0.0a1/packages/docprovider/src/tokens.ts`

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

### Comparing `jupyter_docprovider-1.0.0a0/packages/docprovider/src/awareness.ts` & `jupyter_docprovider-1.0.0a1/packages/docprovider/src/awareness.ts`

 * *Files identical despite different names*

### Comparing `jupyter_docprovider-1.0.0a0/packages/docprovider/src/ydrive.ts` & `jupyter_docprovider-1.0.0a1/packages/docprovider/src/ydrive.ts`

 * *Files identical despite different names*

### Comparing `jupyter_docprovider-1.0.0a0/packages/docprovider/src/yprovider.ts` & `jupyter_docprovider-1.0.0a1/packages/docprovider/src/yprovider.ts`

 * *Files identical despite different names*

### Comparing `jupyter_docprovider-1.0.0a0/packages/docprovider-extension/lib/executor.js` & `jupyter_docprovider-1.0.0a1/packages/docprovider-extension/src/executor.ts`

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

### Comparing `jupyter_docprovider-1.0.0a0/packages/docprovider-extension/lib/filebrowser.js` & `jupyter_docprovider-1.0.0a1/packages/docprovider-extension/src/filebrowser.ts`

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

### Comparing `jupyter_docprovider-1.0.0a0/packages/docprovider-extension/src/index.ts` & `jupyter_docprovider-1.0.0a1/packages/docprovider-extension/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyter_docprovider-1.0.0a0/.gitignore` & `jupyter_docprovider-1.0.0a1/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyter_docprovider-1.0.0a0/LICENSE` & `jupyter_docprovider-1.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_docprovider-1.0.0a0/pyproject.toml` & `jupyter_docprovider-1.0.0a1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -41,15 +41,16 @@
 path = "jupyter_docprovider/_version.py"
 
 [tool.hatch.build.targets.sdist]
 artifacts = ["jupyter_docprovider/labextension"]
 exclude = ["/.github", "/binder", "node_modules"]
 
 [tool.hatch.build.targets.sdist.force-include]
-"../../packages" = "packages"
+"../../packages/docprovider" = "packages/docprovider"
+"../../packages/docprovider-extension" = "packages/docprovider-extension"
 
 [tool.hatch.build.targets.wheel.shared-data]
 "jupyter_docprovider/labextension" = "share/jupyter/labextensions/@jupyter/docprovider-extension"
 "install.json" = "share/jupyter/labextensions/@jupyter/docprovider-extension/install.json"
 
 [tool.hatch.build.hooks.jupyter-builder]
 dependencies = ["hatch-jupyter-builder>=0.5"]
```

### Comparing `jupyter_docprovider-1.0.0a0/PKG-INFO` & `jupyter_docprovider-1.0.0a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jupyter-docprovider
-Version: 1.0.0a0
+Version: 1.0.0a1
 Summary: JupyterLab/Jupyter Notebook 7+ extension integrating collaborative shared models.
 Project-URL: Documentation, https://jupyterlab-realtime-collaboration.readthedocs.io/
 Project-URL: Repository, https://github.com/jupyterlab/jupyter-collaboration
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: # Licensing terms
         
         This project is licensed under the terms of the Modified BSD License
```

