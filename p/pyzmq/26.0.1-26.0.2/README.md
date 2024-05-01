# Comparing `tmp/pyzmq-26.0.1.tar.gz` & `tmp/pyzmq-26.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyzmq-26.0.1.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "pyzmq-26.0.2.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `pyzmq-26.0.1.tar` & `pyzmq-26.0.2.tar`

### file list

```diff
@@ -1,286 +1,286 @@
--rw-r--r--   0        0        0     1853 2022-11-09 12:37:21.000000 pyzmq-26.0.1/.circleci/config.yml
--rw-r--r--   0        0        0      186 2022-11-09 12:37:21.000000 pyzmq-26.0.1/.coveragerc
--rw-r--r--   0        0        0      237 2022-11-09 12:37:21.000000 pyzmq-26.0.1/.flake8
--rw-r--r--   0        0        0     2697 2022-11-09 12:37:21.000000 pyzmq-26.0.1/.github/ISSUE_TEMPLATE/bug.yml
--rw-r--r--   0        0        0      515 2022-11-09 12:37:21.000000 pyzmq-26.0.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      323 2022-11-09 12:37:21.000000 pyzmq-26.0.1/.github/dependabot.yml
--rw-r--r--   0        0        0     1189 2022-11-09 12:37:21.000000 pyzmq-26.0.1/.github/workflows/test-docs.yml
--rw-r--r--   0        0        0     5095 2022-11-09 12:37:21.000000 pyzmq-26.0.1/.github/workflows/test.yml
--rw-r--r--   0        0        0     6029 2022-11-09 12:37:21.000000 pyzmq-26.0.1/.github/workflows/wheels.yml
--rw-r--r--   0        0        0      580 2022-11-09 12:37:21.000000 pyzmq-26.0.1/.gitignore
--rw-r--r--   0        0        0      733 2022-11-09 12:37:21.000000 pyzmq-26.0.1/.mailmap
--rw-r--r--   0        0        0      128 2022-11-09 12:37:21.000000 pyzmq-26.0.1/.obs/workflows.yml
--rw-r--r--   0        0        0     1637 2022-11-09 12:37:21.000000 pyzmq-26.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0       33 2022-11-09 12:37:21.000000 pyzmq-26.0.1/.prettierignore
--rw-r--r--   0        0        0      337 2022-11-09 12:37:21.000000 pyzmq-26.0.1/.readthedocs.yml
--rw-r--r--   0        0        0     4810 2022-11-09 12:37:21.000000 pyzmq-26.0.1/AUTHORS.md
--rw-r--r--   0        0        0    13745 2022-11-09 12:37:21.000000 pyzmq-26.0.1/CMakeLists.txt
--rw-r--r--   0        0        0     2251 2022-11-09 12:37:21.000000 pyzmq-26.0.1/CONTRIBUTING.md
--rw-r--r--   0        0        0     1545 2022-11-09 12:37:21.000000 pyzmq-26.0.1/LICENSE.md
--rw-r--r--   0        0        0      257 2022-11-09 12:37:21.000000 pyzmq-26.0.1/MANIFEST.in
--rw-r--r--   0        0        0     2964 2022-11-09 12:37:21.000000 pyzmq-26.0.1/README.md
--rw-r--r--   0        0        0     2116 2022-11-09 12:37:21.000000 pyzmq-26.0.1/RELICENSE/README.md
--rw-r--r--   0        0        0     2559 2022-11-09 12:37:21.000000 pyzmq-26.0.1/RELICENSE/authors.py
--rw-r--r--   0        0        0      721 2022-11-09 12:37:21.000000 pyzmq-26.0.1/RELICENSE/chrislaws.md
--rw-r--r--   0        0        0      734 2022-11-09 12:37:21.000000 pyzmq-26.0.1/RELICENSE/ellisonbg.md
--rw-r--r--   0        0        0      613 2022-11-09 12:37:21.000000 pyzmq-26.0.1/RELICENSE/frankwiles.md
--rw-r--r--   0        0        0      742 2022-11-09 12:37:21.000000 pyzmq-26.0.1/RELICENSE/juliantaylor.md
--rw-r--r--   0        0        0      600 2022-11-09 12:37:21.000000 pyzmq-26.0.1/RELICENSE/ledgerx.md
--rw-r--r--   0        0        0      731 2022-11-09 12:37:21.000000 pyzmq-26.0.1/RELICENSE/lothiraldan.md
--rw-r--r--   0        0        0      723 2022-11-09 12:37:21.000000 pyzmq-26.0.1/RELICENSE/minrk.md
--rw-r--r--   0        0        0      730 2022-11-09 12:37:21.000000 pyzmq-26.0.1/RELICENSE/takluyver.md
--rw-r--r--   0        0        0      616 2022-11-09 12:37:21.000000 pyzmq-26.0.1/RELICENSE/templates/relicense-template-bsd.txt
--rw-r--r--   0        0        0      809 2022-11-09 12:37:21.000000 pyzmq-26.0.1/RELICENSE/templates/relicense-template-mplv2-any-osi.txt
--rw-r--r--   0        0        0      624 2022-11-09 12:37:21.000000 pyzmq-26.0.1/RELICENSE/templates/relicense-template-mplv2.txt
--rw-r--r--   0        0        0     1541 2022-11-09 12:37:21.000000 pyzmq-26.0.1/SECURITY.md
--rw-r--r--   0        0        0     1070 2022-11-09 12:37:21.000000 pyzmq-26.0.1/Vagrantfile
--rw-r--r--   0        0        0      692 2022-11-09 12:37:21.000000 pyzmq-26.0.1/buildutils/build_cffi.py
--rw-r--r--   0        0        0     1657 2022-11-09 12:37:21.000000 pyzmq-26.0.1/buildutils/bundle.py
--rw-r--r--   0        0        0     3629 2022-11-09 12:37:21.000000 pyzmq-26.0.1/buildutils/constants.py
--rw-r--r--   0        0        0      180 2022-11-09 12:37:21.000000 pyzmq-26.0.1/buildutils/templates/constant_enums.pxi
--rw-r--r--   0        0        0       49 2022-11-09 12:37:21.000000 pyzmq-26.0.1/buildutils/templates/constants.py
--rw-r--r--   0        0        0    11525 2022-11-09 12:37:21.000000 pyzmq-26.0.1/cmake/FindVcvars.cmake
--rw-r--r--   0        0        0     1381 2022-11-09 12:37:21.000000 pyzmq-26.0.1/cmake/Findsodium.cmake
--rw-r--r--   0        0        0      187 2022-11-09 12:37:21.000000 pyzmq-26.0.1/codecov.yml
--rw-r--r--   0        0        0     3639 2022-11-09 12:37:21.000000 pyzmq-26.0.1/docs/Makefile
--rw-r--r--   0        0        0      121 2022-11-09 12:37:21.000000 pyzmq-26.0.1/docs/requirements.txt
--rw-r--r--   0        0        0     8686 2022-11-09 12:37:21.000000 pyzmq-26.0.1/docs/source/_static/logo.png
--rw-r--r--   0        0        0     1150 2022-11-09 12:37:21.000000 pyzmq-26.0.1/docs/source/_static/zeromq.ico
--rw-r--r--   0        0        0      377 2022-11-09 12:37:21.000000 pyzmq-26.0.1/docs/source/api/index.md
--rw-r--r--   0        0        0     1561 2022-11-09 12:37:21.000000 pyzmq-26.0.1/docs/source/api/zmq.asyncio.md
--rw-r--r--   0        0        0      298 2022-11-09 12:37:21.000000 pyzmq-26.0.1/docs/source/api/zmq.auth.asyncio.md
--rw-r--r--   0        0        0      167 2022-11-09 12:37:21.000000 pyzmq-26.0.1/docs/source/api/zmq.auth.ioloop.md
--rw-r--r--   0        0        0      420 2022-11-09 12:37:21.000000 pyzmq-26.0.1/docs/source/api/zmq.auth.md
--rw-r--r--   0        0        0      386 2022-11-09 12:37:21.000000 pyzmq-26.0.1/docs/source/api/zmq.auth.thread.md
--rw-r--r--   0        0        0      270 2022-11-09 12:37:21.000000 pyzmq-26.0.1/docs/source/api/zmq.decorators.md
--rw-r--r--   0        0        0     1674 2022-11-09 12:37:21.000000 pyzmq-26.0.1/docs/source/api/zmq.devices.md
--rw-r--r--   0        0        0     1807 2022-11-09 12:37:21.000000 pyzmq-26.0.1/docs/source/api/zmq.eventloop.future.md
--rw-r--r--   0        0        0      227 2022-11-09 12:37:21.000000 pyzmq-26.0.1/docs/source/api/zmq.eventloop.ioloop.md
--rw-r--r--   0        0        0      330 2022-11-09 12:37:21.000000 pyzmq-26.0.1/docs/source/api/zmq.eventloop.zmqstream.md
--rw-r--r--   0        0        0       82 2022-11-09 12:37:21.000000 pyzmq-26.0.1/docs/source/api/zmq.green.md
--rw-r--r--   0        0        0      442 2022-11-09 12:37:21.000000 pyzmq-26.0.1/docs/source/api/zmq.log.handlers.md
--rw-r--r--   0        0        0     4993 2022-11-09 12:37:21.000000 pyzmq-26.0.1/docs/source/api/zmq.md
--rw-r--r--   0        0        0      471 2022-11-09 12:37:21.000000 pyzmq-26.0.1/docs/source/api/zmq.ssh.tunnel.md
--rw-r--r--   0        0        0      324 2022-11-09 12:37:21.000000 pyzmq-26.0.1/docs/source/api/zmq.utils.jsonapi.md
--rw-r--r--   0        0        0      280 2022-11-09 12:37:21.000000 pyzmq-26.0.1/docs/source/api/zmq.utils.monitor.md
--rw-r--r--   0        0        0      219 2022-11-09 12:37:21.000000 pyzmq-26.0.1/docs/source/api/zmq.utils.win32.md
--rw-r--r--   0        0        0      302 2022-11-09 12:37:21.000000 pyzmq-26.0.1/docs/source/api/zmq.utils.z85.md
--rw-r--r--   0        0        0    42125 2022-11-09 12:37:21.000000 pyzmq-26.0.1/docs/source/changelog.md
--rw-r--r--   0        0        0     8279 2022-11-09 12:37:21.000000 pyzmq-26.0.1/docs/source/conf.py
--rw-r--r--   0        0        0    12342 2022-11-09 12:37:21.000000 pyzmq-26.0.1/docs/source/howto/build.md
--rw-r--r--   0        0        0     3450 2022-11-09 12:37:21.000000 pyzmq-26.0.1/docs/source/howto/cross-android.Dockerfile
--rw-r--r--   0        0        0     3250 2022-11-09 12:37:21.000000 pyzmq-26.0.1/docs/source/howto/cross.Dockerfile
--rw-r--r--   0        0        0     3980 2022-11-09 12:37:21.000000 pyzmq-26.0.1/docs/source/howto/devices.md
--rw-r--r--   0        0        0     1475 2022-11-09 12:37:21.000000 pyzmq-26.0.1/docs/source/howto/draft.md
--rw-r--r--   0        0        0     5732 2022-11-09 12:37:21.000000 pyzmq-26.0.1/docs/source/howto/eventloop.md
--rw-r--r--   0        0        0      125 2022-11-09 12:37:21.000000 pyzmq-26.0.1/docs/source/howto/index.md
--rw-r--r--   0        0        0     9610 2022-11-09 12:37:21.000000 pyzmq-26.0.1/docs/source/howto/logging.md
--rw-r--r--   0        0        0     6548 2022-11-09 12:37:21.000000 pyzmq-26.0.1/docs/source/howto/morethanbindings.md
--rw-r--r--   0        0        0     3569 2022-11-09 12:37:21.000000 pyzmq-26.0.1/docs/source/howto/serialization.md
--rw-r--r--   0        0        0     2877 2022-11-09 12:37:21.000000 pyzmq-26.0.1/docs/source/howto/ssh.md
--rw-r--r--   0        0        0     2025 2022-11-09 12:37:21.000000 pyzmq-26.0.1/docs/source/index.md
--rw-r--r--   0        0        0      162 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/LICENSE
--rw-r--r--   0        0        0      326 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/README.md
--rw-r--r--   0        0        0     1206 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/asyncio/coroutines.py
--rw-r--r--   0        0        0     6997 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/asyncio/helloworld_pubsub_dealerrouter.py
--rw-r--r--   0        0        0     2290 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/asyncio/router_router.py
--rw-r--r--   0        0        0      813 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/asyncio/tornado_asyncio.py
--rw-r--r--   0        0        0       11 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/cython/.gitignore
--rw-r--r--   0        0        0      892 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/cython/README.md
--rw-r--r--   0        0        0     1680 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/cython/cyzmq.pyx
--rw-r--r--   0        0        0     1765 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/cython/example.py
--rw-r--r--   0        0        0      352 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/cython/setup.py
--rw-r--r--   0        0        0     1597 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/device/device.py
--rw-r--r--   0        0        0      550 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/draft/client-server.py
--rw-r--r--   0        0        0     1066 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/draft/install.sh
--rw-r--r--   0        0        0      538 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/draft/radio-dish.py
--rw-r--r--   0        0        0     2038 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/eventloop/asyncweb.py
--rw-r--r--   0        0        0     1388 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/eventloop/coroutines.py
--rw-r--r--   0        0        0      791 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/eventloop/echo.py
--rw-r--r--   0        0        0      439 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/eventloop/echofuture.py
--rw-r--r--   0        0        0      475 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/eventloop/echostream.py
--rw-r--r--   0        0        0     1154 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/gevent/poll.py
--rw-r--r--   0        0        0     1109 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/gevent/reqrep.py
--rw-r--r--   0        0        0     1025 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/gevent/simple.py
--rw-r--r--   0        0        0      756 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/heartbeat/heart.py
--rw-r--r--   0        0        0     2775 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/heartbeat/heartbeater.py
--rw-r--r--   0        0        0      682 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/heartbeat/ping.py
--rw-r--r--   0        0        0      717 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/heartbeat/pong.py
--rw-r--r--   0        0        0     2309 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/logger/zmqlogger.py
--rw-r--r--   0        0        0     1555 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/mongodb/client.py
--rw-r--r--   0        0        0     3256 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/mongodb/controller.py
--rw-r--r--   0        0        0     2341 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/monitoring/simple_monitor.py
--rw-r--r--   0        0        0     5001 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/monitoring/zmq_monitor_class.py
--rw-r--r--   0        0        0     1414 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/poll/pair.py
--rw-r--r--   0        0        0     1401 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/poll/pubsub.py
--rw-r--r--   0        0        0     1767 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/poll/reqrep.py
--rw-r--r--   0        0        0     1506 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/pubsub/publisher.py
--rw-r--r--   0        0        0     1848 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/pubsub/subscriber.py
--rwxr-xr-x   0        0        0     2033 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/pubsub/topics_pub.py
--rwxr-xr-x   0        0        0     1773 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/pubsub/topics_sub.py
--rw-r--r--   0        0        0     3708 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/security/asyncio-ironhouse.py
--rw-r--r--   0        0        0     1969 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/security/generate_certificates.py
--rw-r--r--   0        0        0      566 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/security/grasslands.py
--rw-r--r--   0        0        0     4227 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/security/ioloop-ironhouse.py
--rw-r--r--   0        0        0     3134 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/security/ironhouse.py
--rw-r--r--   0        0        0     3143 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/security/stonehouse.py
--rw-r--r--   0        0        0     2177 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/security/strawhouse.py
--rw-r--r--   0        0        0     2315 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/security/woodhouse.py
--rw-r--r--   0        0        0     2575 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/serialization/serialsocket.py
--rw-r--r--   0        0        0     1352 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/win32-interrupt/display.py
--rw-r--r--   0        0        0      333 2022-11-09 12:37:21.000000 pyzmq-26.0.1/mypy.ini
--rw-r--r--   0        0        0      161 2022-11-09 12:37:21.000000 pyzmq-26.0.1/mypy_tests/test_context.py
--rw-r--r--   0        0        0      408 2022-11-09 12:37:21.000000 pyzmq-26.0.1/mypy_tests/test_socket.py
--rw-r--r--   0        0        0       68 2022-11-09 12:37:21.000000 pyzmq-26.0.1/mypy_tests/test_toplevel.py
--rw-r--r--   0        0        0      218 2022-11-09 12:37:21.000000 pyzmq-26.0.1/packaging/README.md
--rw-r--r--   0        0        0      150 2022-11-09 12:37:21.000000 pyzmq-26.0.1/packaging/debian/changelog
--rw-r--r--   0        0        0        2 2022-11-09 12:37:21.000000 pyzmq-26.0.1/packaging/debian/compat
--rw-r--r--   0        0        0     2298 2022-11-09 12:37:21.000000 pyzmq-26.0.1/packaging/debian/control
--rw-r--r--   0        0        0     6045 2022-11-09 12:37:21.000000 pyzmq-26.0.1/packaging/debian/copyright
--rw-r--r--   0        0        0      675 2022-11-09 12:37:21.000000 pyzmq-26.0.1/packaging/debian/pyzmq.dsc.obs
--rwxr-xr-x   0        0        0     1708 2022-11-09 12:37:21.000000 pyzmq-26.0.1/packaging/debian/rules
--rw-r--r--   0        0        0       13 2022-11-09 12:37:21.000000 pyzmq-26.0.1/packaging/debian/source/format
--rw-r--r--   0        0        0     2338 2022-11-09 12:37:21.000000 pyzmq-26.0.1/packaging/obs/_service
--rw-r--r--   0        0        0     7812 2022-11-09 12:37:21.000000 pyzmq-26.0.1/packaging/redhat/python-pyzmq.spec
--rw-r--r--   0        0        0      185 2022-11-09 12:37:21.000000 pyzmq-26.0.1/perf/Dockerfile
--rw-r--r--   0        0        0      710 2022-11-09 12:37:21.000000 pyzmq-26.0.1/perf/Makefile
--rw-r--r--   0        0        0     4538 2022-11-09 12:37:21.000000 pyzmq-26.0.1/perf/collect.py
--rw-r--r--   0        0        0    35487 2022-11-09 12:37:21.000000 pyzmq-26.0.1/perf/perf.ipynb
--rw-r--r--   0        0        0     6333 2022-11-09 12:37:21.000000 pyzmq-26.0.1/perf/perf.py
--rw-r--r--   0        0        0     5129 2022-11-09 12:37:21.000000 pyzmq-26.0.1/pyproject.toml
--rw-r--r--   0        0        0      304 2022-11-09 12:37:21.000000 pyzmq-26.0.1/pytest.ini
--rw-r--r--   0        0        0      980 2022-11-09 12:37:21.000000 pyzmq-26.0.1/test-requirements.txt
--rw-r--r--   0        0        0      192 2022-11-09 12:37:21.000000 pyzmq-26.0.1/tools/backend_imports.py
--rw-r--r--   0        0        0     1668 2022-11-09 12:37:21.000000 pyzmq-26.0.1/tools/collect_cmake.py
--rw-r--r--   0        0        0     1655 2022-11-09 12:37:21.000000 pyzmq-26.0.1/tools/find_vcredist.py
--rw-r--r--   0        0        0     2154 2022-11-09 12:37:21.000000 pyzmq-26.0.1/tools/install_libzmq.sh
--rw-r--r--   0        0        0     3786 2022-11-09 12:37:21.000000 pyzmq-26.0.1/tools/run_with_env.cmd
--rw-r--r--   0        0        0      247 2022-11-09 12:37:21.000000 pyzmq-26.0.1/tools/showvcvars.py
--rw-r--r--   0        0        0     1521 2022-11-09 12:37:21.000000 pyzmq-26.0.1/tools/test_sdist.py
--rw-r--r--   0        0        0     1999 2022-11-09 12:37:21.000000 pyzmq-26.0.1/tools/test_wheel.py
--rw-r--r--   0        0        0       64 2022-11-09 12:37:21.000000 pyzmq-26.0.1/tools/wheel-requirements.txt
--rw-r--r--   0        0        0       63 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/__init__.pxd
--rw-r--r--   0        0        0     2232 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/__init__.py
--rw-r--r--   0        0        0      960 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/__init__.pyi
--rw-r--r--   0        0        0    24919 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/_future.py
--rw-r--r--   0        0        0      720 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/_typing.py
--rw-r--r--   0        0        0     6266 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/asyncio.py
--rw-r--r--   0        0        0      346 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/auth/__init__.py
--rw-r--r--   0        0        0     1799 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/auth/asyncio.py
--rw-r--r--   0        0        0    16337 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/auth/base.py
--rw-r--r--   0        0        0     4331 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/auth/certs.py
--rw-r--r--   0        0        0     1298 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/auth/ioloop.py
--rw-r--r--   0        0        0     4103 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/auth/thread.py
--rw-r--r--   0        0        0      942 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/backend/__init__.py
--rw-r--r--   0        0        0     3379 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/backend/__init__.pyi
--rw-r--r--   0        0        0       95 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/backend/cffi/README.md
--rw-r--r--   0        0        0      833 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/backend/cffi/__init__.py
--rw-r--r--   0        0        0     2623 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/backend/cffi/_cdefs.h
--rw-r--r--   0        0        0     1314 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/backend/cffi/_cffi_src.c
--rw-r--r--   0        0        0     2886 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/backend/cffi/_poll.py
--rw-r--r--   0        0        0     1899 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/backend/cffi/context.py
--rw-r--r--   0        0        0     1572 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/backend/cffi/devices.py
--rw-r--r--   0        0        0      380 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/backend/cffi/error.py
--rw-r--r--   0        0        0     6488 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/backend/cffi/message.py
--rw-r--r--   0        0        0    11427 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/backend/cffi/socket.py
--rw-r--r--   0        0        0     2086 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/backend/cffi/utils.py
--rw-r--r--   0        0        0       60 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/backend/cython/__init__.pxd
--rw-r--r--   0        0        0      322 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/backend/cython/__init__.py
--rw-r--r--   0        0        0      339 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/backend/cython/_externs.pxd
--rw-r--r--   0        0        0     2186 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/backend/cython/_zmq.pxd
--rw-r--r--   0        0        0    57647 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/backend/cython/_zmq.py
--rw-r--r--   0        0        0     7562 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/backend/cython/constant_enums.pxi
--rw-r--r--   0        0        0     4564 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/backend/cython/libzmq.pxd
--rw-r--r--   0        0        0      902 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/backend/select.py
--rw-r--r--   0        0        0    28341 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/constants.py
--rw-r--r--   0        0        0     5099 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/decorators.py
--rw-r--r--   0        0        0      730 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/devices/__init__.py
--rw-r--r--   0        0        0     9580 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/devices/basedevice.py
--rw-r--r--   0        0        0     1294 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/devices/monitoredqueue.py
--rw-r--r--   0        0        0     1929 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/devices/monitoredqueuedevice.py
--rw-r--r--   0        0        0     2849 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/devices/proxydevice.py
--rw-r--r--   0        0        0     3212 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/devices/proxysteerabledevice.py
--rw-r--r--   0        0        0     5309 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/error.py
--rw-r--r--   0        0        0      103 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/eventloop/__init__.py
--rw-r--r--   0        0        0     6437 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/eventloop/_deprecated.py
--rw-r--r--   0        0        0     2612 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/eventloop/future.py
--rw-r--r--   0        0        0      766 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/eventloop/ioloop.py
--rw-r--r--   0        0        0    23439 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/eventloop/zmqstream.py
--rw-r--r--   0        0        0     1367 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/green/__init__.py
--rw-r--r--   0        0        0    10812 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/green/core.py
--rw-r--r--   0        0        0      978 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/green/device.py
--rw-r--r--   0        0        0       68 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/green/eventloop/__init__.py
--rw-r--r--   0        0        0       43 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/green/eventloop/ioloop.py
--rw-r--r--   0        0        0      291 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/green/eventloop/zmqstream.py
--rw-r--r--   0        0        0     2996 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/green/poll.py
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/log/__init__.py
--rw-r--r--   0        0        0     4005 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/log/__main__.py
--rw-r--r--   0        0        0     7228 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/log/handlers.py
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/py.typed
--rw-r--r--   0        0        0       29 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/ssh/__init__.py
--rw-r--r--   0        0        0     3280 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/ssh/forward.py
--rw-r--r--   0        0        0    13533 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/ssh/tunnel.py
--rw-r--r--   0        0        0      721 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/sugar/__init__.py
--rw-r--r--   0        0        0      219 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/sugar/__init__.pyi
--rw-r--r--   0        0        0     2638 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/sugar/attrsettr.py
--rw-r--r--   0        0        0    14644 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/sugar/context.py
--rw-r--r--   0        0        0     4259 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/sugar/frame.py
--rw-r--r--   0        0        0     5752 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/sugar/poll.py
--rw-r--r--   0        0        0    34703 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/sugar/socket.py
--rw-r--r--   0        0        0      935 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/sugar/stopwatch.py
--rw-r--r--   0        0        0     3605 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/sugar/tracker.py
--rw-r--r--   0        0        0     1613 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/sugar/version.py
--rw-r--r--   0        0        0     8134 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/__init__.py
--rw-r--r--   0        0        0     5564 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/conftest.py
--rw-r--r--   0        0        0      642 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/cython_ext.pyx
--rw-r--r--   0        0        0     9993 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/test_asyncio.py
--rw-r--r--   0        0        0    14750 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/test_auth.py
--rw-r--r--   0        0        0     8945 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/test_cffi_backend.py
--rw-r--r--   0        0        0      962 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/test_constants.py
--rw-r--r--   0        0        0    12600 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/test_context.py
--rw-r--r--   0        0        0     1383 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/test_cython.py
--rw-r--r--   0        0        0     9623 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/test_decorators.py
--rw-r--r--   0        0        0     6004 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/test_device.py
--rw-r--r--   0        0        0     1371 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/test_draft.py
--rw-r--r--   0        0        0     1125 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/test_error.py
--rw-r--r--   0        0        0      533 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/test_etc.py
--rw-r--r--   0        0        0      786 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/test_ext.py
--rw-r--r--   0        0        0    10608 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/test_future.py
--rw-r--r--   0        0        0     1973 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/test_imports.py
--rw-r--r--   0        0        0      883 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/test_includes.py
--rw-r--r--   0        0        0      641 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/test_ioloop.py
--rw-r--r--   0        0        0     6948 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/test_log.py
--rw-r--r--   0        0        0    11320 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/test_message.py
--rw-r--r--   0        0        0     3059 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/test_monitor.py
--rw-r--r--   0        0        0     8285 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/test_monqueue.py
--rw-r--r--   0        0        0      852 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/test_multipart.py
--rw-r--r--   0        0        0     1684 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/test_mypy.py
--rw-r--r--   0        0        0     1232 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/test_pair.py
--rw-r--r--   0        0        0     7106 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/test_poll.py
--rw-r--r--   0        0        0     4004 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/test_proxy_steerable.py
--rw-r--r--   0        0        0     1015 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/test_pubsub.py
--rw-r--r--   0        0        0     1764 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/test_reqrep.py
--rw-r--r--   0        0        0     2874 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/test_retry_eintr.py
--rw-r--r--   0        0        0     7792 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/test_security.py
--rw-r--r--   0        0        0    24126 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/test_socket.py
--rw-r--r--   0        0        0      235 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/test_ssh.py
--rw-r--r--   0        0        0     1208 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/test_version.py
--rw-r--r--   0        0        0     1661 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/test_win32_shim.py
--rw-r--r--   0        0        0     2108 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/test_z85.py
--rw-r--r--   0        0        0     4195 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/test_zmqstream.py
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/utils/__init__.py
--rw-r--r--   0        0        0     7031 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/utils/buffers.pxd
--rw-r--r--   0        0        0     6124 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/utils/garbage.py
--rw-r--r--   0        0        0      116 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/utils/getpid_compat.h
--rw-r--r--   0        0        0      685 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/utils/interop.py
--rw-r--r--   0        0        0      522 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/utils/ipcmaxlen.h
--rw-r--r--   0        0        0     1025 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/utils/jsonapi.py
--rw-r--r--   0        0        0     3312 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/utils/monitor.py
--rw-r--r--   0        0        0     1625 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/utils/mutex.h
--rw-r--r--   0        0        0      284 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/utils/pyversion_compat.h
--rw-r--r--   0        0        0     1376 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/utils/strtypes.py
--rw-r--r--   0        0        0     4940 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/utils/win32.py
--rw-r--r--   0        0        0     1841 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/utils/z85.py
--rw-r--r--   0        0        0     3184 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/utils/zmq_compat.h
--rw-r--r--   0        0        0     4042 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmqversion.py
--rw-r--r--   0        0        0     6124 2022-11-09 12:37:21.000000 pyzmq-26.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1853 2022-11-09 12:37:21.000000 pyzmq-26.0.2/.circleci/config.yml
+-rw-r--r--   0        0        0      186 2022-11-09 12:37:21.000000 pyzmq-26.0.2/.coveragerc
+-rw-r--r--   0        0        0      237 2022-11-09 12:37:21.000000 pyzmq-26.0.2/.flake8
+-rw-r--r--   0        0        0     2697 2022-11-09 12:37:21.000000 pyzmq-26.0.2/.github/ISSUE_TEMPLATE/bug.yml
+-rw-r--r--   0        0        0      515 2022-11-09 12:37:21.000000 pyzmq-26.0.2/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      323 2022-11-09 12:37:21.000000 pyzmq-26.0.2/.github/dependabot.yml
+-rw-r--r--   0        0        0     1189 2022-11-09 12:37:21.000000 pyzmq-26.0.2/.github/workflows/test-docs.yml
+-rw-r--r--   0        0        0     5095 2022-11-09 12:37:21.000000 pyzmq-26.0.2/.github/workflows/test.yml
+-rw-r--r--   0        0        0     6029 2022-11-09 12:37:21.000000 pyzmq-26.0.2/.github/workflows/wheels.yml
+-rw-r--r--   0        0        0      580 2022-11-09 12:37:21.000000 pyzmq-26.0.2/.gitignore
+-rw-r--r--   0        0        0      733 2022-11-09 12:37:21.000000 pyzmq-26.0.2/.mailmap
+-rw-r--r--   0        0        0      128 2022-11-09 12:37:21.000000 pyzmq-26.0.2/.obs/workflows.yml
+-rw-r--r--   0        0        0     1637 2022-11-09 12:37:21.000000 pyzmq-26.0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       33 2022-11-09 12:37:21.000000 pyzmq-26.0.2/.prettierignore
+-rw-r--r--   0        0        0      337 2022-11-09 12:37:21.000000 pyzmq-26.0.2/.readthedocs.yml
+-rw-r--r--   0        0        0     4810 2022-11-09 12:37:21.000000 pyzmq-26.0.2/AUTHORS.md
+-rw-r--r--   0        0        0    13786 2022-11-09 12:37:21.000000 pyzmq-26.0.2/CMakeLists.txt
+-rw-r--r--   0        0        0     2251 2022-11-09 12:37:21.000000 pyzmq-26.0.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1545 2022-11-09 12:37:21.000000 pyzmq-26.0.2/LICENSE.md
+-rw-r--r--   0        0        0      257 2022-11-09 12:37:21.000000 pyzmq-26.0.2/MANIFEST.in
+-rw-r--r--   0        0        0     2964 2022-11-09 12:37:21.000000 pyzmq-26.0.2/README.md
+-rw-r--r--   0        0        0     2116 2022-11-09 12:37:21.000000 pyzmq-26.0.2/RELICENSE/README.md
+-rw-r--r--   0        0        0     2559 2022-11-09 12:37:21.000000 pyzmq-26.0.2/RELICENSE/authors.py
+-rw-r--r--   0        0        0      721 2022-11-09 12:37:21.000000 pyzmq-26.0.2/RELICENSE/chrislaws.md
+-rw-r--r--   0        0        0      734 2022-11-09 12:37:21.000000 pyzmq-26.0.2/RELICENSE/ellisonbg.md
+-rw-r--r--   0        0        0      613 2022-11-09 12:37:21.000000 pyzmq-26.0.2/RELICENSE/frankwiles.md
+-rw-r--r--   0        0        0      742 2022-11-09 12:37:21.000000 pyzmq-26.0.2/RELICENSE/juliantaylor.md
+-rw-r--r--   0        0        0      600 2022-11-09 12:37:21.000000 pyzmq-26.0.2/RELICENSE/ledgerx.md
+-rw-r--r--   0        0        0      731 2022-11-09 12:37:21.000000 pyzmq-26.0.2/RELICENSE/lothiraldan.md
+-rw-r--r--   0        0        0      723 2022-11-09 12:37:21.000000 pyzmq-26.0.2/RELICENSE/minrk.md
+-rw-r--r--   0        0        0      730 2022-11-09 12:37:21.000000 pyzmq-26.0.2/RELICENSE/takluyver.md
+-rw-r--r--   0        0        0      616 2022-11-09 12:37:21.000000 pyzmq-26.0.2/RELICENSE/templates/relicense-template-bsd.txt
+-rw-r--r--   0        0        0      809 2022-11-09 12:37:21.000000 pyzmq-26.0.2/RELICENSE/templates/relicense-template-mplv2-any-osi.txt
+-rw-r--r--   0        0        0      624 2022-11-09 12:37:21.000000 pyzmq-26.0.2/RELICENSE/templates/relicense-template-mplv2.txt
+-rw-r--r--   0        0        0     1541 2022-11-09 12:37:21.000000 pyzmq-26.0.2/SECURITY.md
+-rw-r--r--   0        0        0     1070 2022-11-09 12:37:21.000000 pyzmq-26.0.2/Vagrantfile
+-rw-r--r--   0        0        0      692 2022-11-09 12:37:21.000000 pyzmq-26.0.2/buildutils/build_cffi.py
+-rw-r--r--   0        0        0     1657 2022-11-09 12:37:21.000000 pyzmq-26.0.2/buildutils/bundle.py
+-rw-r--r--   0        0        0     3629 2022-11-09 12:37:21.000000 pyzmq-26.0.2/buildutils/constants.py
+-rw-r--r--   0        0        0      180 2022-11-09 12:37:21.000000 pyzmq-26.0.2/buildutils/templates/constant_enums.pxi
+-rw-r--r--   0        0        0       49 2022-11-09 12:37:21.000000 pyzmq-26.0.2/buildutils/templates/constants.py
+-rw-r--r--   0        0        0    11525 2022-11-09 12:37:21.000000 pyzmq-26.0.2/cmake/FindVcvars.cmake
+-rw-r--r--   0        0        0     1381 2022-11-09 12:37:21.000000 pyzmq-26.0.2/cmake/Findsodium.cmake
+-rw-r--r--   0        0        0      187 2022-11-09 12:37:21.000000 pyzmq-26.0.2/codecov.yml
+-rw-r--r--   0        0        0     3639 2022-11-09 12:37:21.000000 pyzmq-26.0.2/docs/Makefile
+-rw-r--r--   0        0        0      121 2022-11-09 12:37:21.000000 pyzmq-26.0.2/docs/requirements.txt
+-rw-r--r--   0        0        0     8686 2022-11-09 12:37:21.000000 pyzmq-26.0.2/docs/source/_static/logo.png
+-rw-r--r--   0        0        0     1150 2022-11-09 12:37:21.000000 pyzmq-26.0.2/docs/source/_static/zeromq.ico
+-rw-r--r--   0        0        0      377 2022-11-09 12:37:21.000000 pyzmq-26.0.2/docs/source/api/index.md
+-rw-r--r--   0        0        0     1561 2022-11-09 12:37:21.000000 pyzmq-26.0.2/docs/source/api/zmq.asyncio.md
+-rw-r--r--   0        0        0      298 2022-11-09 12:37:21.000000 pyzmq-26.0.2/docs/source/api/zmq.auth.asyncio.md
+-rw-r--r--   0        0        0      167 2022-11-09 12:37:21.000000 pyzmq-26.0.2/docs/source/api/zmq.auth.ioloop.md
+-rw-r--r--   0        0        0      420 2022-11-09 12:37:21.000000 pyzmq-26.0.2/docs/source/api/zmq.auth.md
+-rw-r--r--   0        0        0      386 2022-11-09 12:37:21.000000 pyzmq-26.0.2/docs/source/api/zmq.auth.thread.md
+-rw-r--r--   0        0        0      270 2022-11-09 12:37:21.000000 pyzmq-26.0.2/docs/source/api/zmq.decorators.md
+-rw-r--r--   0        0        0     1674 2022-11-09 12:37:21.000000 pyzmq-26.0.2/docs/source/api/zmq.devices.md
+-rw-r--r--   0        0        0     1807 2022-11-09 12:37:21.000000 pyzmq-26.0.2/docs/source/api/zmq.eventloop.future.md
+-rw-r--r--   0        0        0      227 2022-11-09 12:37:21.000000 pyzmq-26.0.2/docs/source/api/zmq.eventloop.ioloop.md
+-rw-r--r--   0        0        0      330 2022-11-09 12:37:21.000000 pyzmq-26.0.2/docs/source/api/zmq.eventloop.zmqstream.md
+-rw-r--r--   0        0        0       82 2022-11-09 12:37:21.000000 pyzmq-26.0.2/docs/source/api/zmq.green.md
+-rw-r--r--   0        0        0      442 2022-11-09 12:37:21.000000 pyzmq-26.0.2/docs/source/api/zmq.log.handlers.md
+-rw-r--r--   0        0        0     4993 2022-11-09 12:37:21.000000 pyzmq-26.0.2/docs/source/api/zmq.md
+-rw-r--r--   0        0        0      471 2022-11-09 12:37:21.000000 pyzmq-26.0.2/docs/source/api/zmq.ssh.tunnel.md
+-rw-r--r--   0        0        0      324 2022-11-09 12:37:21.000000 pyzmq-26.0.2/docs/source/api/zmq.utils.jsonapi.md
+-rw-r--r--   0        0        0      280 2022-11-09 12:37:21.000000 pyzmq-26.0.2/docs/source/api/zmq.utils.monitor.md
+-rw-r--r--   0        0        0      219 2022-11-09 12:37:21.000000 pyzmq-26.0.2/docs/source/api/zmq.utils.win32.md
+-rw-r--r--   0        0        0      302 2022-11-09 12:37:21.000000 pyzmq-26.0.2/docs/source/api/zmq.utils.z85.md
+-rw-r--r--   0        0        0    42282 2022-11-09 12:37:21.000000 pyzmq-26.0.2/docs/source/changelog.md
+-rw-r--r--   0        0        0     8279 2022-11-09 12:37:21.000000 pyzmq-26.0.2/docs/source/conf.py
+-rw-r--r--   0        0        0    12342 2022-11-09 12:37:21.000000 pyzmq-26.0.2/docs/source/howto/build.md
+-rw-r--r--   0        0        0     3450 2022-11-09 12:37:21.000000 pyzmq-26.0.2/docs/source/howto/cross-android.Dockerfile
+-rw-r--r--   0        0        0     3250 2022-11-09 12:37:21.000000 pyzmq-26.0.2/docs/source/howto/cross.Dockerfile
+-rw-r--r--   0        0        0     3980 2022-11-09 12:37:21.000000 pyzmq-26.0.2/docs/source/howto/devices.md
+-rw-r--r--   0        0        0     1475 2022-11-09 12:37:21.000000 pyzmq-26.0.2/docs/source/howto/draft.md
+-rw-r--r--   0        0        0     5732 2022-11-09 12:37:21.000000 pyzmq-26.0.2/docs/source/howto/eventloop.md
+-rw-r--r--   0        0        0      125 2022-11-09 12:37:21.000000 pyzmq-26.0.2/docs/source/howto/index.md
+-rw-r--r--   0        0        0     9610 2022-11-09 12:37:21.000000 pyzmq-26.0.2/docs/source/howto/logging.md
+-rw-r--r--   0        0        0     6548 2022-11-09 12:37:21.000000 pyzmq-26.0.2/docs/source/howto/morethanbindings.md
+-rw-r--r--   0        0        0     3569 2022-11-09 12:37:21.000000 pyzmq-26.0.2/docs/source/howto/serialization.md
+-rw-r--r--   0        0        0     2877 2022-11-09 12:37:21.000000 pyzmq-26.0.2/docs/source/howto/ssh.md
+-rw-r--r--   0        0        0     2025 2022-11-09 12:37:21.000000 pyzmq-26.0.2/docs/source/index.md
+-rw-r--r--   0        0        0      162 2022-11-09 12:37:21.000000 pyzmq-26.0.2/examples/LICENSE
+-rw-r--r--   0        0        0      326 2022-11-09 12:37:21.000000 pyzmq-26.0.2/examples/README.md
+-rw-r--r--   0        0        0     1206 2022-11-09 12:37:21.000000 pyzmq-26.0.2/examples/asyncio/coroutines.py
+-rw-r--r--   0        0        0     6997 2022-11-09 12:37:21.000000 pyzmq-26.0.2/examples/asyncio/helloworld_pubsub_dealerrouter.py
+-rw-r--r--   0        0        0     2290 2022-11-09 12:37:21.000000 pyzmq-26.0.2/examples/asyncio/router_router.py
+-rw-r--r--   0        0        0      813 2022-11-09 12:37:21.000000 pyzmq-26.0.2/examples/asyncio/tornado_asyncio.py
+-rw-r--r--   0        0        0       11 2022-11-09 12:37:21.000000 pyzmq-26.0.2/examples/cython/.gitignore
+-rw-r--r--   0        0        0      892 2022-11-09 12:37:21.000000 pyzmq-26.0.2/examples/cython/README.md
+-rw-r--r--   0        0        0     1680 2022-11-09 12:37:21.000000 pyzmq-26.0.2/examples/cython/cyzmq.pyx
+-rw-r--r--   0        0        0     1765 2022-11-09 12:37:21.000000 pyzmq-26.0.2/examples/cython/example.py
+-rw-r--r--   0        0        0      352 2022-11-09 12:37:21.000000 pyzmq-26.0.2/examples/cython/setup.py
+-rw-r--r--   0        0        0     1597 2022-11-09 12:37:21.000000 pyzmq-26.0.2/examples/device/device.py
+-rw-r--r--   0        0        0      550 2022-11-09 12:37:21.000000 pyzmq-26.0.2/examples/draft/client-server.py
+-rw-r--r--   0        0        0     1066 2022-11-09 12:37:21.000000 pyzmq-26.0.2/examples/draft/install.sh
+-rw-r--r--   0        0        0      538 2022-11-09 12:37:21.000000 pyzmq-26.0.2/examples/draft/radio-dish.py
+-rw-r--r--   0        0        0     2038 2022-11-09 12:37:21.000000 pyzmq-26.0.2/examples/eventloop/asyncweb.py
+-rw-r--r--   0        0        0     1388 2022-11-09 12:37:21.000000 pyzmq-26.0.2/examples/eventloop/coroutines.py
+-rw-r--r--   0        0        0      791 2022-11-09 12:37:21.000000 pyzmq-26.0.2/examples/eventloop/echo.py
+-rw-r--r--   0        0        0      439 2022-11-09 12:37:21.000000 pyzmq-26.0.2/examples/eventloop/echofuture.py
+-rw-r--r--   0        0        0      475 2022-11-09 12:37:21.000000 pyzmq-26.0.2/examples/eventloop/echostream.py
+-rw-r--r--   0        0        0     1154 2022-11-09 12:37:21.000000 pyzmq-26.0.2/examples/gevent/poll.py
+-rw-r--r--   0        0        0     1109 2022-11-09 12:37:21.000000 pyzmq-26.0.2/examples/gevent/reqrep.py
+-rw-r--r--   0        0        0     1025 2022-11-09 12:37:21.000000 pyzmq-26.0.2/examples/gevent/simple.py
+-rw-r--r--   0        0        0      756 2022-11-09 12:37:21.000000 pyzmq-26.0.2/examples/heartbeat/heart.py
+-rw-r--r--   0        0        0     2775 2022-11-09 12:37:21.000000 pyzmq-26.0.2/examples/heartbeat/heartbeater.py
+-rw-r--r--   0        0        0      682 2022-11-09 12:37:21.000000 pyzmq-26.0.2/examples/heartbeat/ping.py
+-rw-r--r--   0        0        0      717 2022-11-09 12:37:21.000000 pyzmq-26.0.2/examples/heartbeat/pong.py
+-rw-r--r--   0        0        0     2309 2022-11-09 12:37:21.000000 pyzmq-26.0.2/examples/logger/zmqlogger.py
+-rw-r--r--   0        0        0     1555 2022-11-09 12:37:21.000000 pyzmq-26.0.2/examples/mongodb/client.py
+-rw-r--r--   0        0        0     3256 2022-11-09 12:37:21.000000 pyzmq-26.0.2/examples/mongodb/controller.py
+-rw-r--r--   0        0        0     2341 2022-11-09 12:37:21.000000 pyzmq-26.0.2/examples/monitoring/simple_monitor.py
+-rw-r--r--   0        0        0     5001 2022-11-09 12:37:21.000000 pyzmq-26.0.2/examples/monitoring/zmq_monitor_class.py
+-rw-r--r--   0        0        0     1414 2022-11-09 12:37:21.000000 pyzmq-26.0.2/examples/poll/pair.py
+-rw-r--r--   0        0        0     1401 2022-11-09 12:37:21.000000 pyzmq-26.0.2/examples/poll/pubsub.py
+-rw-r--r--   0        0        0     1767 2022-11-09 12:37:21.000000 pyzmq-26.0.2/examples/poll/reqrep.py
+-rw-r--r--   0        0        0     1506 2022-11-09 12:37:21.000000 pyzmq-26.0.2/examples/pubsub/publisher.py
+-rw-r--r--   0        0        0     1848 2022-11-09 12:37:21.000000 pyzmq-26.0.2/examples/pubsub/subscriber.py
+-rwxr-xr-x   0        0        0     2033 2022-11-09 12:37:21.000000 pyzmq-26.0.2/examples/pubsub/topics_pub.py
+-rwxr-xr-x   0        0        0     1773 2022-11-09 12:37:21.000000 pyzmq-26.0.2/examples/pubsub/topics_sub.py
+-rw-r--r--   0        0        0     3708 2022-11-09 12:37:21.000000 pyzmq-26.0.2/examples/security/asyncio-ironhouse.py
+-rw-r--r--   0        0        0     1969 2022-11-09 12:37:21.000000 pyzmq-26.0.2/examples/security/generate_certificates.py
+-rw-r--r--   0        0        0      566 2022-11-09 12:37:21.000000 pyzmq-26.0.2/examples/security/grasslands.py
+-rw-r--r--   0        0        0     4227 2022-11-09 12:37:21.000000 pyzmq-26.0.2/examples/security/ioloop-ironhouse.py
+-rw-r--r--   0        0        0     3134 2022-11-09 12:37:21.000000 pyzmq-26.0.2/examples/security/ironhouse.py
+-rw-r--r--   0        0        0     3143 2022-11-09 12:37:21.000000 pyzmq-26.0.2/examples/security/stonehouse.py
+-rw-r--r--   0        0        0     2177 2022-11-09 12:37:21.000000 pyzmq-26.0.2/examples/security/strawhouse.py
+-rw-r--r--   0        0        0     2315 2022-11-09 12:37:21.000000 pyzmq-26.0.2/examples/security/woodhouse.py
+-rw-r--r--   0        0        0     2575 2022-11-09 12:37:21.000000 pyzmq-26.0.2/examples/serialization/serialsocket.py
+-rw-r--r--   0        0        0     1352 2022-11-09 12:37:21.000000 pyzmq-26.0.2/examples/win32-interrupt/display.py
+-rw-r--r--   0        0        0      333 2022-11-09 12:37:21.000000 pyzmq-26.0.2/mypy.ini
+-rw-r--r--   0        0        0      161 2022-11-09 12:37:21.000000 pyzmq-26.0.2/mypy_tests/test_context.py
+-rw-r--r--   0        0        0      408 2022-11-09 12:37:21.000000 pyzmq-26.0.2/mypy_tests/test_socket.py
+-rw-r--r--   0        0        0       68 2022-11-09 12:37:21.000000 pyzmq-26.0.2/mypy_tests/test_toplevel.py
+-rw-r--r--   0        0        0      218 2022-11-09 12:37:21.000000 pyzmq-26.0.2/packaging/README.md
+-rw-r--r--   0        0        0      150 2022-11-09 12:37:21.000000 pyzmq-26.0.2/packaging/debian/changelog
+-rw-r--r--   0        0        0        2 2022-11-09 12:37:21.000000 pyzmq-26.0.2/packaging/debian/compat
+-rw-r--r--   0        0        0     2298 2022-11-09 12:37:21.000000 pyzmq-26.0.2/packaging/debian/control
+-rw-r--r--   0        0        0     6045 2022-11-09 12:37:21.000000 pyzmq-26.0.2/packaging/debian/copyright
+-rw-r--r--   0        0        0      675 2022-11-09 12:37:21.000000 pyzmq-26.0.2/packaging/debian/pyzmq.dsc.obs
+-rwxr-xr-x   0        0        0     1708 2022-11-09 12:37:21.000000 pyzmq-26.0.2/packaging/debian/rules
+-rw-r--r--   0        0        0       13 2022-11-09 12:37:21.000000 pyzmq-26.0.2/packaging/debian/source/format
+-rw-r--r--   0        0        0     2338 2022-11-09 12:37:21.000000 pyzmq-26.0.2/packaging/obs/_service
+-rw-r--r--   0        0        0     7812 2022-11-09 12:37:21.000000 pyzmq-26.0.2/packaging/redhat/python-pyzmq.spec
+-rw-r--r--   0        0        0      185 2022-11-09 12:37:21.000000 pyzmq-26.0.2/perf/Dockerfile
+-rw-r--r--   0        0        0      710 2022-11-09 12:37:21.000000 pyzmq-26.0.2/perf/Makefile
+-rw-r--r--   0        0        0     4538 2022-11-09 12:37:21.000000 pyzmq-26.0.2/perf/collect.py
+-rw-r--r--   0        0        0    35487 2022-11-09 12:37:21.000000 pyzmq-26.0.2/perf/perf.ipynb
+-rw-r--r--   0        0        0     6333 2022-11-09 12:37:21.000000 pyzmq-26.0.2/perf/perf.py
+-rw-r--r--   0        0        0     5129 2022-11-09 12:37:21.000000 pyzmq-26.0.2/pyproject.toml
+-rw-r--r--   0        0        0      304 2022-11-09 12:37:21.000000 pyzmq-26.0.2/pytest.ini
+-rw-r--r--   0        0        0      980 2022-11-09 12:37:21.000000 pyzmq-26.0.2/test-requirements.txt
+-rw-r--r--   0        0        0      192 2022-11-09 12:37:21.000000 pyzmq-26.0.2/tools/backend_imports.py
+-rw-r--r--   0        0        0     1668 2022-11-09 12:37:21.000000 pyzmq-26.0.2/tools/collect_cmake.py
+-rw-r--r--   0        0        0     1655 2022-11-09 12:37:21.000000 pyzmq-26.0.2/tools/find_vcredist.py
+-rw-r--r--   0        0        0     2189 2022-11-09 12:37:21.000000 pyzmq-26.0.2/tools/install_libzmq.sh
+-rw-r--r--   0        0        0     3786 2022-11-09 12:37:21.000000 pyzmq-26.0.2/tools/run_with_env.cmd
+-rw-r--r--   0        0        0      247 2022-11-09 12:37:21.000000 pyzmq-26.0.2/tools/showvcvars.py
+-rw-r--r--   0        0        0     1521 2022-11-09 12:37:21.000000 pyzmq-26.0.2/tools/test_sdist.py
+-rw-r--r--   0        0        0     1999 2022-11-09 12:37:21.000000 pyzmq-26.0.2/tools/test_wheel.py
+-rw-r--r--   0        0        0       64 2022-11-09 12:37:21.000000 pyzmq-26.0.2/tools/wheel-requirements.txt
+-rw-r--r--   0        0        0       63 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/__init__.pxd
+-rw-r--r--   0        0        0     2232 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/__init__.py
+-rw-r--r--   0        0        0      960 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/__init__.pyi
+-rw-r--r--   0        0        0    24919 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/_future.py
+-rw-r--r--   0        0        0      720 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/_typing.py
+-rw-r--r--   0        0        0     6266 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/asyncio.py
+-rw-r--r--   0        0        0      346 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/auth/__init__.py
+-rw-r--r--   0        0        0     1799 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/auth/asyncio.py
+-rw-r--r--   0        0        0    16337 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/auth/base.py
+-rw-r--r--   0        0        0     4331 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/auth/certs.py
+-rw-r--r--   0        0        0     1298 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/auth/ioloop.py
+-rw-r--r--   0        0        0     4103 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/auth/thread.py
+-rw-r--r--   0        0        0      942 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/backend/__init__.py
+-rw-r--r--   0        0        0     3379 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/backend/__init__.pyi
+-rw-r--r--   0        0        0       95 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/backend/cffi/README.md
+-rw-r--r--   0        0        0      833 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/backend/cffi/__init__.py
+-rw-r--r--   0        0        0     2623 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/backend/cffi/_cdefs.h
+-rw-r--r--   0        0        0     1314 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/backend/cffi/_cffi_src.c
+-rw-r--r--   0        0        0     2886 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/backend/cffi/_poll.py
+-rw-r--r--   0        0        0     1899 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/backend/cffi/context.py
+-rw-r--r--   0        0        0     1572 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/backend/cffi/devices.py
+-rw-r--r--   0        0        0      380 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/backend/cffi/error.py
+-rw-r--r--   0        0        0     6488 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/backend/cffi/message.py
+-rw-r--r--   0        0        0    11427 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/backend/cffi/socket.py
+-rw-r--r--   0        0        0     2086 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/backend/cffi/utils.py
+-rw-r--r--   0        0        0       60 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/backend/cython/__init__.pxd
+-rw-r--r--   0        0        0      322 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/backend/cython/__init__.py
+-rw-r--r--   0        0        0      339 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/backend/cython/_externs.pxd
+-rw-r--r--   0        0        0     2186 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/backend/cython/_zmq.pxd
+-rw-r--r--   0        0        0    57647 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/backend/cython/_zmq.py
+-rw-r--r--   0        0        0     7562 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/backend/cython/constant_enums.pxi
+-rw-r--r--   0        0        0     4564 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/backend/cython/libzmq.pxd
+-rw-r--r--   0        0        0      902 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/backend/select.py
+-rw-r--r--   0        0        0    28341 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/constants.py
+-rw-r--r--   0        0        0     5099 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/decorators.py
+-rw-r--r--   0        0        0      730 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/devices/__init__.py
+-rw-r--r--   0        0        0     9580 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/devices/basedevice.py
+-rw-r--r--   0        0        0     1294 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/devices/monitoredqueue.py
+-rw-r--r--   0        0        0     1929 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/devices/monitoredqueuedevice.py
+-rw-r--r--   0        0        0     2849 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/devices/proxydevice.py
+-rw-r--r--   0        0        0     3212 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/devices/proxysteerabledevice.py
+-rw-r--r--   0        0        0     5309 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/error.py
+-rw-r--r--   0        0        0      103 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/eventloop/__init__.py
+-rw-r--r--   0        0        0     6437 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/eventloop/_deprecated.py
+-rw-r--r--   0        0        0     2612 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/eventloop/future.py
+-rw-r--r--   0        0        0      766 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/eventloop/ioloop.py
+-rw-r--r--   0        0        0    23439 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/eventloop/zmqstream.py
+-rw-r--r--   0        0        0     1367 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/green/__init__.py
+-rw-r--r--   0        0        0    10812 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/green/core.py
+-rw-r--r--   0        0        0      978 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/green/device.py
+-rw-r--r--   0        0        0       68 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/green/eventloop/__init__.py
+-rw-r--r--   0        0        0       43 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/green/eventloop/ioloop.py
+-rw-r--r--   0        0        0      291 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/green/eventloop/zmqstream.py
+-rw-r--r--   0        0        0     2996 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/green/poll.py
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/log/__init__.py
+-rw-r--r--   0        0        0     4005 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/log/__main__.py
+-rw-r--r--   0        0        0     7228 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/log/handlers.py
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/py.typed
+-rw-r--r--   0        0        0       29 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/ssh/__init__.py
+-rw-r--r--   0        0        0     3280 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/ssh/forward.py
+-rw-r--r--   0        0        0    13533 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/ssh/tunnel.py
+-rw-r--r--   0        0        0      721 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/sugar/__init__.py
+-rw-r--r--   0        0        0      219 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/sugar/__init__.pyi
+-rw-r--r--   0        0        0     2638 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/sugar/attrsettr.py
+-rw-r--r--   0        0        0    14644 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/sugar/context.py
+-rw-r--r--   0        0        0     4259 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/sugar/frame.py
+-rw-r--r--   0        0        0     5752 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/sugar/poll.py
+-rw-r--r--   0        0        0    34703 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/sugar/socket.py
+-rw-r--r--   0        0        0      935 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/sugar/stopwatch.py
+-rw-r--r--   0        0        0     3605 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/sugar/tracker.py
+-rw-r--r--   0        0        0     1613 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/sugar/version.py
+-rw-r--r--   0        0        0     8134 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/tests/__init__.py
+-rw-r--r--   0        0        0     5564 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/tests/conftest.py
+-rw-r--r--   0        0        0      642 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/tests/cython_ext.pyx
+-rw-r--r--   0        0        0     9993 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/tests/test_asyncio.py
+-rw-r--r--   0        0        0    14750 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/tests/test_auth.py
+-rw-r--r--   0        0        0     8945 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/tests/test_cffi_backend.py
+-rw-r--r--   0        0        0      962 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/tests/test_constants.py
+-rw-r--r--   0        0        0    12600 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/tests/test_context.py
+-rw-r--r--   0        0        0     1383 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/tests/test_cython.py
+-rw-r--r--   0        0        0     9623 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/tests/test_decorators.py
+-rw-r--r--   0        0        0     6004 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/tests/test_device.py
+-rw-r--r--   0        0        0     1371 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/tests/test_draft.py
+-rw-r--r--   0        0        0     1125 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/tests/test_error.py
+-rw-r--r--   0        0        0      533 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/tests/test_etc.py
+-rw-r--r--   0        0        0      786 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/tests/test_ext.py
+-rw-r--r--   0        0        0    10608 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/tests/test_future.py
+-rw-r--r--   0        0        0     1973 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/tests/test_imports.py
+-rw-r--r--   0        0        0      883 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/tests/test_includes.py
+-rw-r--r--   0        0        0      641 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/tests/test_ioloop.py
+-rw-r--r--   0        0        0     6948 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/tests/test_log.py
+-rw-r--r--   0        0        0    11320 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/tests/test_message.py
+-rw-r--r--   0        0        0     3059 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/tests/test_monitor.py
+-rw-r--r--   0        0        0     8285 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/tests/test_monqueue.py
+-rw-r--r--   0        0        0      852 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/tests/test_multipart.py
+-rw-r--r--   0        0        0     1684 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/tests/test_mypy.py
+-rw-r--r--   0        0        0     1232 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/tests/test_pair.py
+-rw-r--r--   0        0        0     7106 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/tests/test_poll.py
+-rw-r--r--   0        0        0     4004 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/tests/test_proxy_steerable.py
+-rw-r--r--   0        0        0     1015 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/tests/test_pubsub.py
+-rw-r--r--   0        0        0     1764 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/tests/test_reqrep.py
+-rw-r--r--   0        0        0     2874 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/tests/test_retry_eintr.py
+-rw-r--r--   0        0        0     7792 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/tests/test_security.py
+-rw-r--r--   0        0        0    24126 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/tests/test_socket.py
+-rw-r--r--   0        0        0      235 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/tests/test_ssh.py
+-rw-r--r--   0        0        0     1208 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/tests/test_version.py
+-rw-r--r--   0        0        0     1661 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/tests/test_win32_shim.py
+-rw-r--r--   0        0        0     2108 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/tests/test_z85.py
+-rw-r--r--   0        0        0     4195 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/tests/test_zmqstream.py
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/utils/__init__.py
+-rw-r--r--   0        0        0     7031 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/utils/buffers.pxd
+-rw-r--r--   0        0        0     6124 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/utils/garbage.py
+-rw-r--r--   0        0        0      116 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/utils/getpid_compat.h
+-rw-r--r--   0        0        0      685 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/utils/interop.py
+-rw-r--r--   0        0        0      522 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/utils/ipcmaxlen.h
+-rw-r--r--   0        0        0     1025 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/utils/jsonapi.py
+-rw-r--r--   0        0        0     3312 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/utils/monitor.py
+-rw-r--r--   0        0        0     1625 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/utils/mutex.h
+-rw-r--r--   0        0        0      284 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/utils/pyversion_compat.h
+-rw-r--r--   0        0        0     1376 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/utils/strtypes.py
+-rw-r--r--   0        0        0     4940 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/utils/win32.py
+-rw-r--r--   0        0        0     1841 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/utils/z85.py
+-rw-r--r--   0        0        0     3184 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmq/utils/zmq_compat.h
+-rw-r--r--   0        0        0     4042 2022-11-09 12:37:21.000000 pyzmq-26.0.2/zmqversion.py
+-rw-r--r--   0        0        0     6124 2022-11-09 12:37:21.000000 pyzmq-26.0.2/PKG-INFO
```

### Comparing `pyzmq-26.0.1/.circleci/config.yml` & `pyzmq-26.0.2/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/.github/ISSUE_TEMPLATE/bug.yml` & `pyzmq-26.0.2/.github/ISSUE_TEMPLATE/bug.yml`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/.github/ISSUE_TEMPLATE/config.yml` & `pyzmq-26.0.2/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/.github/workflows/test-docs.yml` & `pyzmq-26.0.2/.github/workflows/test-docs.yml`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/.github/workflows/test.yml` & `pyzmq-26.0.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/.github/workflows/wheels.yml` & `pyzmq-26.0.2/.github/workflows/wheels.yml`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/.gitignore` & `pyzmq-26.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/.mailmap` & `pyzmq-26.0.2/.mailmap`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/.pre-commit-config.yaml` & `pyzmq-26.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/AUTHORS.md` & `pyzmq-26.0.2/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/CMakeLists.txt` & `pyzmq-26.0.2/CMakeLists.txt`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
 if(ZMQ_DRAFT_API)
   message(STATUS "enabling ZMQ_DRAFT_API")
   add_compile_definitions(ZMQ_BUILD_DRAFT_API=1)
 endif()
 
 if (PYZMQ_LIBSODIUM_VERSION AND NOT PYZMQ_LIBSODIUM_URL)
-  set(PYZMQ_LIBSODIUM_URL "https://download.libsodium.org/libsodium/releases/libsodium-${PYZMQ_LIBSODIUM_VERSION}.tar.gz")
+  set(PYZMQ_LIBSODIUM_URL "https://github.com/jedisct1/libsodium/releases/download/${PYZMQ_LIBSODIUM_VERSION}-RELEASE/libsodium-${PYZMQ_LIBSODIUM_VERSION}.tar.gz")
 endif()
 
 if (PYZMQ_LIBZMQ_VERSION AND NOT PYZMQ_LIBZMQ_URL)
   set(PYZMQ_LIBZMQ_URL "https://github.com/zeromq/libzmq/releases/download/v${PYZMQ_LIBZMQ_VERSION}/zeromq-${PYZMQ_LIBZMQ_VERSION}.tar.gz")
 endif()
 
 #------- bundle libzmq ------
```

### Comparing `pyzmq-26.0.1/CONTRIBUTING.md` & `pyzmq-26.0.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/LICENSE.md` & `pyzmq-26.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/README.md` & `pyzmq-26.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/RELICENSE/README.md` & `pyzmq-26.0.2/RELICENSE/README.md`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/RELICENSE/authors.py` & `pyzmq-26.0.2/RELICENSE/authors.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/RELICENSE/chrislaws.md` & `pyzmq-26.0.2/RELICENSE/chrislaws.md`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/RELICENSE/ellisonbg.md` & `pyzmq-26.0.2/RELICENSE/ellisonbg.md`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/RELICENSE/frankwiles.md` & `pyzmq-26.0.2/RELICENSE/frankwiles.md`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/RELICENSE/juliantaylor.md` & `pyzmq-26.0.2/RELICENSE/juliantaylor.md`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/RELICENSE/ledgerx.md` & `pyzmq-26.0.2/RELICENSE/ledgerx.md`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/RELICENSE/lothiraldan.md` & `pyzmq-26.0.2/RELICENSE/lothiraldan.md`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/RELICENSE/minrk.md` & `pyzmq-26.0.2/RELICENSE/minrk.md`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/RELICENSE/takluyver.md` & `pyzmq-26.0.2/RELICENSE/takluyver.md`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/RELICENSE/templates/relicense-template-bsd.txt` & `pyzmq-26.0.2/RELICENSE/templates/relicense-template-bsd.txt`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/RELICENSE/templates/relicense-template-mplv2-any-osi.txt` & `pyzmq-26.0.2/RELICENSE/templates/relicense-template-mplv2-any-osi.txt`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/RELICENSE/templates/relicense-template-mplv2.txt` & `pyzmq-26.0.2/RELICENSE/templates/relicense-template-mplv2.txt`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/SECURITY.md` & `pyzmq-26.0.2/SECURITY.md`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/Vagrantfile` & `pyzmq-26.0.2/Vagrantfile`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/buildutils/build_cffi.py` & `pyzmq-26.0.2/buildutils/build_cffi.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/buildutils/bundle.py` & `pyzmq-26.0.2/buildutils/bundle.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/buildutils/constants.py` & `pyzmq-26.0.2/buildutils/constants.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/cmake/FindVcvars.cmake` & `pyzmq-26.0.2/cmake/FindVcvars.cmake`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/cmake/Findsodium.cmake` & `pyzmq-26.0.2/cmake/Findsodium.cmake`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/docs/Makefile` & `pyzmq-26.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/docs/source/_static/logo.png` & `pyzmq-26.0.2/docs/source/_static/logo.png`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/docs/source/_static/zeromq.ico` & `pyzmq-26.0.2/docs/source/_static/zeromq.ico`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/docs/source/api/zmq.asyncio.md` & `pyzmq-26.0.2/docs/source/api/zmq.asyncio.md`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/docs/source/api/zmq.devices.md` & `pyzmq-26.0.2/docs/source/api/zmq.devices.md`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/docs/source/api/zmq.eventloop.future.md` & `pyzmq-26.0.2/docs/source/api/zmq.eventloop.future.md`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/docs/source/api/zmq.md` & `pyzmq-26.0.2/docs/source/api/zmq.md`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/docs/source/changelog.md` & `pyzmq-26.0.2/docs/source/changelog.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,19 @@
 # Changes in PyZMQ
 
 This is a coarse summary of changes in pyzmq versions.
 For a full changelog, consult the [git log](https://github.com/zeromq/pyzmq/commits).
 
 ## 26
 
+### 26.0.2
+
+- When bundling libsodium, download from libsodium's releases on GitHub instead of download.libsodium.org,
+  which appears to error frequently.
+
 ### 26.0.1
 
 - Fix install from source with cmake \< 3.21
 
 ### 26.0.0
 
 pyzmq 26 is a small release, but with some big changes _hopefully_ nobody will notice,
```

### Comparing `pyzmq-26.0.1/docs/source/conf.py` & `pyzmq-26.0.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/docs/source/howto/build.md` & `pyzmq-26.0.2/docs/source/howto/build.md`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/docs/source/howto/cross-android.Dockerfile` & `pyzmq-26.0.2/docs/source/howto/cross-android.Dockerfile`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/docs/source/howto/cross.Dockerfile` & `pyzmq-26.0.2/docs/source/howto/cross.Dockerfile`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/docs/source/howto/devices.md` & `pyzmq-26.0.2/docs/source/howto/devices.md`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/docs/source/howto/draft.md` & `pyzmq-26.0.2/docs/source/howto/draft.md`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/docs/source/howto/eventloop.md` & `pyzmq-26.0.2/docs/source/howto/eventloop.md`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/docs/source/howto/logging.md` & `pyzmq-26.0.2/docs/source/howto/logging.md`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/docs/source/howto/morethanbindings.md` & `pyzmq-26.0.2/docs/source/howto/morethanbindings.md`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/docs/source/howto/serialization.md` & `pyzmq-26.0.2/docs/source/howto/serialization.md`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/docs/source/howto/ssh.md` & `pyzmq-26.0.2/docs/source/howto/ssh.md`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/docs/source/index.md` & `pyzmq-26.0.2/docs/source/index.md`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/examples/asyncio/coroutines.py` & `pyzmq-26.0.2/examples/asyncio/coroutines.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/examples/asyncio/helloworld_pubsub_dealerrouter.py` & `pyzmq-26.0.2/examples/asyncio/helloworld_pubsub_dealerrouter.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/examples/asyncio/router_router.py` & `pyzmq-26.0.2/examples/asyncio/router_router.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/examples/asyncio/tornado_asyncio.py` & `pyzmq-26.0.2/examples/asyncio/tornado_asyncio.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/examples/cython/README.md` & `pyzmq-26.0.2/examples/cython/README.md`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/examples/cython/cyzmq.pyx` & `pyzmq-26.0.2/examples/cython/cyzmq.pyx`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/examples/cython/example.py` & `pyzmq-26.0.2/examples/cython/example.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/examples/device/device.py` & `pyzmq-26.0.2/examples/device/device.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/examples/draft/client-server.py` & `pyzmq-26.0.2/examples/draft/client-server.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/examples/draft/install.sh` & `pyzmq-26.0.2/examples/draft/install.sh`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/examples/draft/radio-dish.py` & `pyzmq-26.0.2/examples/draft/radio-dish.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/examples/eventloop/asyncweb.py` & `pyzmq-26.0.2/examples/eventloop/asyncweb.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/examples/eventloop/coroutines.py` & `pyzmq-26.0.2/examples/eventloop/coroutines.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/examples/eventloop/echo.py` & `pyzmq-26.0.2/examples/eventloop/echo.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/examples/gevent/poll.py` & `pyzmq-26.0.2/examples/gevent/poll.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/examples/gevent/reqrep.py` & `pyzmq-26.0.2/examples/gevent/reqrep.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/examples/gevent/simple.py` & `pyzmq-26.0.2/examples/gevent/simple.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/examples/heartbeat/heart.py` & `pyzmq-26.0.2/examples/heartbeat/heart.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/examples/heartbeat/heartbeater.py` & `pyzmq-26.0.2/examples/heartbeat/heartbeater.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/examples/heartbeat/ping.py` & `pyzmq-26.0.2/examples/heartbeat/ping.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/examples/heartbeat/pong.py` & `pyzmq-26.0.2/examples/heartbeat/pong.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/examples/logger/zmqlogger.py` & `pyzmq-26.0.2/examples/logger/zmqlogger.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/examples/mongodb/client.py` & `pyzmq-26.0.2/examples/mongodb/client.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/examples/mongodb/controller.py` & `pyzmq-26.0.2/examples/mongodb/controller.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/examples/monitoring/simple_monitor.py` & `pyzmq-26.0.2/examples/monitoring/simple_monitor.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/examples/monitoring/zmq_monitor_class.py` & `pyzmq-26.0.2/examples/monitoring/zmq_monitor_class.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/examples/poll/pair.py` & `pyzmq-26.0.2/examples/poll/pair.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/examples/poll/pubsub.py` & `pyzmq-26.0.2/examples/poll/pubsub.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/examples/poll/reqrep.py` & `pyzmq-26.0.2/examples/poll/reqrep.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/examples/pubsub/publisher.py` & `pyzmq-26.0.2/examples/pubsub/publisher.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/examples/pubsub/subscriber.py` & `pyzmq-26.0.2/examples/pubsub/subscriber.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/examples/pubsub/topics_pub.py` & `pyzmq-26.0.2/examples/pubsub/topics_pub.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/examples/pubsub/topics_sub.py` & `pyzmq-26.0.2/examples/pubsub/topics_sub.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/examples/security/asyncio-ironhouse.py` & `pyzmq-26.0.2/examples/security/asyncio-ironhouse.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/examples/security/generate_certificates.py` & `pyzmq-26.0.2/examples/security/generate_certificates.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/examples/security/grasslands.py` & `pyzmq-26.0.2/examples/security/grasslands.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/examples/security/ioloop-ironhouse.py` & `pyzmq-26.0.2/examples/security/ioloop-ironhouse.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/examples/security/ironhouse.py` & `pyzmq-26.0.2/examples/security/ironhouse.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/examples/security/stonehouse.py` & `pyzmq-26.0.2/examples/security/stonehouse.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/examples/security/strawhouse.py` & `pyzmq-26.0.2/examples/security/strawhouse.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/examples/security/woodhouse.py` & `pyzmq-26.0.2/examples/security/woodhouse.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/examples/serialization/serialsocket.py` & `pyzmq-26.0.2/examples/serialization/serialsocket.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/examples/win32-interrupt/display.py` & `pyzmq-26.0.2/examples/win32-interrupt/display.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/packaging/debian/control` & `pyzmq-26.0.2/packaging/debian/control`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/packaging/debian/copyright` & `pyzmq-26.0.2/packaging/debian/copyright`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/packaging/debian/pyzmq.dsc.obs` & `pyzmq-26.0.2/packaging/debian/pyzmq.dsc.obs`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/packaging/debian/rules` & `pyzmq-26.0.2/packaging/debian/rules`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/packaging/obs/_service` & `pyzmq-26.0.2/packaging/obs/_service`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/packaging/redhat/python-pyzmq.spec` & `pyzmq-26.0.2/packaging/redhat/python-pyzmq.spec`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/perf/Makefile` & `pyzmq-26.0.2/perf/Makefile`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/perf/collect.py` & `pyzmq-26.0.2/perf/collect.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/perf/perf.ipynb` & `pyzmq-26.0.2/perf/perf.ipynb`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/perf/perf.py` & `pyzmq-26.0.2/perf/perf.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/pyproject.toml` & `pyzmq-26.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 # build-backend = "setuptools.build_meta"
 
 # Project metadata
 # ref: https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html
 [project]
 name = "pyzmq"
-version = "26.0.1"
+version = "26.0.2"
 authors = [
   { name = "PyZMQ Contributors", email = "zeromq-dev@lists.zeromq.org" },
   { name = "Brian E. Granger" },
   { name = "Min Ragan-Kelley" },
 ]
 license = { file = "LICENSE.md" }
 requires-python = ">=3.7"
@@ -113,15 +113,15 @@
 skip = ["zmq/__init__.py"]
 
 [tool.tbump]
 # Uncomment this if your project is hosted on GitHub:
 github_url = "https://github.com/zeromq/pyzmq"
 
 [tool.tbump.version]
-current = "26.0.1"
+current = "26.0.2"
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
   (?P<pre>((a|b|rc|)\d+)|.dev\d*|)
```

### Comparing `pyzmq-26.0.1/test-requirements.txt` & `pyzmq-26.0.2/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/tools/collect_cmake.py` & `pyzmq-26.0.2/tools/collect_cmake.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/tools/find_vcredist.py` & `pyzmq-26.0.2/tools/find_vcredist.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/tools/install_libzmq.sh` & `pyzmq-26.0.2/tools/install_libzmq.sh`

 * *Files 6% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         export CXXFLAGS="-arch ${arch} ${CXXFLAGS:-}"
         export LDFLAGS="-arch ${arch} ${LDFLAGS:-}"
     done
 fi
 
 PREFIX="${ZMQ_PREFIX:-/usr/local}"
 
-curl -L -O "https://download.libsodium.org/libsodium/releases/libsodium-${LIBSODIUM_VERSION}.tar.gz"
+curl -L -O "https://github.com/jedisct1/libsodium/releases/download/${LIBSODIUM_VERSION}-RELEASE/libsodium-${LIBSODIUM_VERSION}.tar.gz"
 
 curl -L -O "https://github.com/zeromq/libzmq/releases/download/v${LIBZMQ_VERSION}/zeromq-${LIBZMQ_VERSION}.tar.gz"
 
 tar -xzf libsodium-${LIBSODIUM_VERSION}.tar.gz
 cd libsodium-*/
 cp LICENSE "${LICENSE_DIR}/LICENSE.libsodium.txt"
 ./configure --prefix="$PREFIX"
```

### Comparing `pyzmq-26.0.1/tools/run_with_env.cmd` & `pyzmq-26.0.2/tools/run_with_env.cmd`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/tools/test_sdist.py` & `pyzmq-26.0.2/tools/test_sdist.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/tools/test_wheel.py` & `pyzmq-26.0.2/tools/test_wheel.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/__init__.py` & `pyzmq-26.0.2/zmq/__init__.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/__init__.pyi` & `pyzmq-26.0.2/zmq/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/_future.py` & `pyzmq-26.0.2/zmq/_future.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/_typing.py` & `pyzmq-26.0.2/zmq/_typing.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/asyncio.py` & `pyzmq-26.0.2/zmq/asyncio.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/auth/asyncio.py` & `pyzmq-26.0.2/zmq/auth/asyncio.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/auth/base.py` & `pyzmq-26.0.2/zmq/auth/base.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/auth/certs.py` & `pyzmq-26.0.2/zmq/auth/certs.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/auth/ioloop.py` & `pyzmq-26.0.2/zmq/auth/ioloop.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/auth/thread.py` & `pyzmq-26.0.2/zmq/auth/thread.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/backend/__init__.py` & `pyzmq-26.0.2/zmq/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/backend/__init__.pyi` & `pyzmq-26.0.2/zmq/backend/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/backend/cffi/__init__.py` & `pyzmq-26.0.2/zmq/backend/cffi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/backend/cffi/_cdefs.h` & `pyzmq-26.0.2/zmq/backend/cffi/_cdefs.h`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/backend/cffi/_cffi_src.c` & `pyzmq-26.0.2/zmq/backend/cffi/_cffi_src.c`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/backend/cffi/_poll.py` & `pyzmq-26.0.2/zmq/backend/cffi/_poll.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/backend/cffi/context.py` & `pyzmq-26.0.2/zmq/backend/cffi/context.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/backend/cffi/devices.py` & `pyzmq-26.0.2/zmq/backend/cffi/devices.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/backend/cffi/message.py` & `pyzmq-26.0.2/zmq/backend/cffi/message.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/backend/cffi/socket.py` & `pyzmq-26.0.2/zmq/backend/cffi/socket.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/backend/cffi/utils.py` & `pyzmq-26.0.2/zmq/backend/cffi/utils.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/backend/cython/_zmq.pxd` & `pyzmq-26.0.2/zmq/backend/cython/_zmq.pxd`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/backend/cython/_zmq.py` & `pyzmq-26.0.2/zmq/backend/cython/_zmq.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/backend/cython/constant_enums.pxi` & `pyzmq-26.0.2/zmq/backend/cython/constant_enums.pxi`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/backend/cython/libzmq.pxd` & `pyzmq-26.0.2/zmq/backend/cython/libzmq.pxd`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/backend/select.py` & `pyzmq-26.0.2/zmq/backend/select.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/constants.py` & `pyzmq-26.0.2/zmq/constants.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/decorators.py` & `pyzmq-26.0.2/zmq/decorators.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/devices/__init__.py` & `pyzmq-26.0.2/zmq/devices/__init__.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/devices/basedevice.py` & `pyzmq-26.0.2/zmq/devices/basedevice.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/devices/monitoredqueue.py` & `pyzmq-26.0.2/zmq/devices/monitoredqueue.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/devices/monitoredqueuedevice.py` & `pyzmq-26.0.2/zmq/devices/monitoredqueuedevice.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/devices/proxydevice.py` & `pyzmq-26.0.2/zmq/devices/proxydevice.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/devices/proxysteerabledevice.py` & `pyzmq-26.0.2/zmq/devices/proxysteerabledevice.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/error.py` & `pyzmq-26.0.2/zmq/error.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/eventloop/_deprecated.py` & `pyzmq-26.0.2/zmq/eventloop/_deprecated.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/eventloop/future.py` & `pyzmq-26.0.2/zmq/eventloop/future.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/eventloop/ioloop.py` & `pyzmq-26.0.2/zmq/eventloop/ioloop.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/eventloop/zmqstream.py` & `pyzmq-26.0.2/zmq/eventloop/zmqstream.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/green/__init__.py` & `pyzmq-26.0.2/zmq/green/__init__.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/green/core.py` & `pyzmq-26.0.2/zmq/green/core.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/green/device.py` & `pyzmq-26.0.2/zmq/green/device.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/green/poll.py` & `pyzmq-26.0.2/zmq/green/poll.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/log/__main__.py` & `pyzmq-26.0.2/zmq/log/__main__.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/log/handlers.py` & `pyzmq-26.0.2/zmq/log/handlers.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/ssh/forward.py` & `pyzmq-26.0.2/zmq/ssh/forward.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/ssh/tunnel.py` & `pyzmq-26.0.2/zmq/ssh/tunnel.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/sugar/__init__.py` & `pyzmq-26.0.2/zmq/sugar/__init__.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/sugar/attrsettr.py` & `pyzmq-26.0.2/zmq/sugar/attrsettr.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/sugar/context.py` & `pyzmq-26.0.2/zmq/sugar/context.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/sugar/frame.py` & `pyzmq-26.0.2/zmq/sugar/frame.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/sugar/poll.py` & `pyzmq-26.0.2/zmq/sugar/poll.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/sugar/socket.py` & `pyzmq-26.0.2/zmq/sugar/socket.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/sugar/stopwatch.py` & `pyzmq-26.0.2/zmq/sugar/stopwatch.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/sugar/tracker.py` & `pyzmq-26.0.2/zmq/sugar/tracker.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/sugar/version.py` & `pyzmq-26.0.2/zmq/sugar/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from __future__ import annotations
 
 import re
 from typing import Match, cast
 
 from zmq.backend import zmq_version_info
 
-__version__: str = "26.0.1"
+__version__: str = "26.0.2"
 _version_pat = re.compile(r"(\d+)\.(\d+)\.(\d+)(.*)")
 _match = cast(Match, _version_pat.match(__version__))
 _version_groups = _match.groups()
 
 VERSION_MAJOR = int(_version_groups[0])
 VERSION_MINOR = int(_version_groups[1])
 VERSION_PATCH = int(_version_groups[2])
```

### Comparing `pyzmq-26.0.1/zmq/tests/__init__.py` & `pyzmq-26.0.2/zmq/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/tests/conftest.py` & `pyzmq-26.0.2/zmq/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/tests/cython_ext.pyx` & `pyzmq-26.0.2/zmq/tests/cython_ext.pyx`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/tests/test_asyncio.py` & `pyzmq-26.0.2/zmq/tests/test_asyncio.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/tests/test_auth.py` & `pyzmq-26.0.2/zmq/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/tests/test_cffi_backend.py` & `pyzmq-26.0.2/zmq/tests/test_cffi_backend.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/tests/test_constants.py` & `pyzmq-26.0.2/zmq/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/tests/test_context.py` & `pyzmq-26.0.2/zmq/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/tests/test_cython.py` & `pyzmq-26.0.2/zmq/tests/test_cython.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/tests/test_decorators.py` & `pyzmq-26.0.2/zmq/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/tests/test_device.py` & `pyzmq-26.0.2/zmq/tests/test_device.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/tests/test_draft.py` & `pyzmq-26.0.2/zmq/tests/test_draft.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/tests/test_error.py` & `pyzmq-26.0.2/zmq/tests/test_error.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/tests/test_etc.py` & `pyzmq-26.0.2/zmq/tests/test_etc.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/tests/test_ext.py` & `pyzmq-26.0.2/zmq/tests/test_ext.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/tests/test_future.py` & `pyzmq-26.0.2/zmq/tests/test_future.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/tests/test_imports.py` & `pyzmq-26.0.2/zmq/tests/test_imports.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/tests/test_includes.py` & `pyzmq-26.0.2/zmq/tests/test_includes.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/tests/test_ioloop.py` & `pyzmq-26.0.2/zmq/tests/test_ioloop.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/tests/test_log.py` & `pyzmq-26.0.2/zmq/tests/test_log.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/tests/test_message.py` & `pyzmq-26.0.2/zmq/tests/test_message.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/tests/test_monitor.py` & `pyzmq-26.0.2/zmq/tests/test_monitor.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/tests/test_monqueue.py` & `pyzmq-26.0.2/zmq/tests/test_monqueue.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/tests/test_multipart.py` & `pyzmq-26.0.2/zmq/tests/test_multipart.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/tests/test_mypy.py` & `pyzmq-26.0.2/zmq/tests/test_mypy.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/tests/test_pair.py` & `pyzmq-26.0.2/zmq/tests/test_pair.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/tests/test_poll.py` & `pyzmq-26.0.2/zmq/tests/test_poll.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/tests/test_proxy_steerable.py` & `pyzmq-26.0.2/zmq/tests/test_proxy_steerable.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/tests/test_pubsub.py` & `pyzmq-26.0.2/zmq/tests/test_pubsub.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/tests/test_reqrep.py` & `pyzmq-26.0.2/zmq/tests/test_reqrep.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/tests/test_retry_eintr.py` & `pyzmq-26.0.2/zmq/tests/test_retry_eintr.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/tests/test_security.py` & `pyzmq-26.0.2/zmq/tests/test_security.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/tests/test_socket.py` & `pyzmq-26.0.2/zmq/tests/test_socket.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/tests/test_version.py` & `pyzmq-26.0.2/zmq/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/tests/test_win32_shim.py` & `pyzmq-26.0.2/zmq/tests/test_win32_shim.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/tests/test_z85.py` & `pyzmq-26.0.2/zmq/tests/test_z85.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/tests/test_zmqstream.py` & `pyzmq-26.0.2/zmq/tests/test_zmqstream.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/utils/buffers.pxd` & `pyzmq-26.0.2/zmq/utils/buffers.pxd`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/utils/garbage.py` & `pyzmq-26.0.2/zmq/utils/garbage.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/utils/interop.py` & `pyzmq-26.0.2/zmq/utils/interop.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/utils/ipcmaxlen.h` & `pyzmq-26.0.2/zmq/utils/ipcmaxlen.h`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/utils/jsonapi.py` & `pyzmq-26.0.2/zmq/utils/jsonapi.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/utils/monitor.py` & `pyzmq-26.0.2/zmq/utils/monitor.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/utils/mutex.h` & `pyzmq-26.0.2/zmq/utils/mutex.h`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/utils/strtypes.py` & `pyzmq-26.0.2/zmq/utils/strtypes.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/utils/win32.py` & `pyzmq-26.0.2/zmq/utils/win32.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/utils/z85.py` & `pyzmq-26.0.2/zmq/utils/z85.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmq/utils/zmq_compat.h` & `pyzmq-26.0.2/zmq/utils/zmq_compat.h`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/zmqversion.py` & `pyzmq-26.0.2/zmqversion.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.1/PKG-INFO` & `pyzmq-26.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyzmq
-Version: 26.0.1
+Version: 26.0.2
 Summary: Python bindings for 0MQ
 Author: Brian E. Granger, Min Ragan-Kelley
 Author-Email: PyZMQ Contributors <zeromq-dev@lists.zeromq.org>
 License: BSD 3-Clause License
         
         Copyright (c) 2009-2012, Brian Granger, Min Ragan-Kelley
```

