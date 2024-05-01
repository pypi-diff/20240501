# Comparing `tmp/ultralytics-8.2.4.tar.gz` & `tmp/ultralytics-8.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ultralytics-8.2.4.tar", last modified: Sat Apr 27 19:48:15 2024, max compression
+gzip compressed data, was "ultralytics-8.2.5.tar", last modified: Mon Apr 29 08:59:40 2024, max compression
```

## Comparing `ultralytics-8.2.4.tar` & `ultralytics-8.2.5.tar`

### file list

```diff
@@ -1,258 +1,259 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:48:15.793806 ultralytics-8.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-27 19:46:54.000000 ultralytics-8.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    40530 2024-04-27 19:48:15.793806 ultralytics-8.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    36782 2024-04-27 19:46:54.000000 ultralytics-8.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     7334 2024-04-27 19:46:54.000000 ultralytics-8.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 19:48:15.793806 ultralytics-8.2.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:48:15.753806 ultralytics-8.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-04-27 19:46:54.000000 ultralytics-8.2.4/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-04-27 19:46:54.000000 ultralytics-8.2.4/tests/test_cuda.py
--rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-04-27 19:46:54.000000 ultralytics-8.2.4/tests/test_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-04-27 19:46:54.000000 ultralytics-8.2.4/tests/test_explorer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6053 2024-04-27 19:46:54.000000 ultralytics-8.2.4/tests/test_integrations.py
--rw-r--r--   0 runner    (1001) docker     (127)    23016 2024-04-27 19:46:54.000000 ultralytics-8.2.4/tests/test_python.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:48:15.753806 ultralytics-8.2.4/ultralytics/
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:48:15.757806 ultralytics-8.2.4/ultralytics/assets/
--rw-r--r--   0 runner    (1001) docker     (127)   137419 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/assets/bus.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    50427 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/assets/zidane.jpg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:48:15.757806 ultralytics-8.2.4/ultralytics/cfg/
--rw-r--r--   0 runner    (1001) docker     (127)    21312 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/cfg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:48:15.761806 ultralytics-8.2.4/ultralytics/cfg/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/cfg/datasets/Argoverse.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/cfg/datasets/DOTAv1.5.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/cfg/datasets/DOTAv1.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/cfg/datasets/GlobalWheat2020.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    42507 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/cfg/datasets/ImageNet.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     9324 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/cfg/datasets/Objects365.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/cfg/datasets/SKU-110K.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/cfg/datasets/VOC.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/cfg/datasets/VisDrone.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/cfg/datasets/african-wildlife.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/cfg/datasets/brain-tumor.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/cfg/datasets/carparts-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/cfg/datasets/coco-pose.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/cfg/datasets/coco.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/cfg/datasets/coco128-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/cfg/datasets/coco128.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/cfg/datasets/coco8-pose.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/cfg/datasets/coco8-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/cfg/datasets/coco8.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/cfg/datasets/crack-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/cfg/datasets/dota8.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    29705 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/cfg/datasets/lvis.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    12493 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/cfg/datasets/open-images-v7.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/cfg/datasets/package-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/cfg/datasets/tiger-pose.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/cfg/datasets/xView.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8211 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/cfg/default.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:48:15.749806 ultralytics-8.2.4/ultralytics/cfg/models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:48:15.761806 ultralytics-8.2.4/ultralytics/cfg/models/rt-detr/
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/cfg/models/rt-detr/rtdetr-l.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/cfg/models/rt-detr/rtdetr-resnet101.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/cfg/models/rt-detr/rtdetr-resnet50.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/cfg/models/rt-detr/rtdetr-x.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:48:15.761806 ultralytics-8.2.4/ultralytics/cfg/models/v3/
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/cfg/models/v3/yolov3-spp.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/cfg/models/v3/yolov3-tiny.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/cfg/models/v3/yolov3.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:48:15.761806 ultralytics-8.2.4/ultralytics/cfg/models/v5/
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/cfg/models/v5/yolov5-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/cfg/models/v5/yolov5.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:48:15.761806 ultralytics-8.2.4/ultralytics/cfg/models/v6/
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/cfg/models/v6/yolov6.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:48:15.765806 ultralytics-8.2.4/ultralytics/cfg/models/v8/
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/cfg/models/v8/yolov8-cls-resnet101.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/cfg/models/v8/yolov8-cls-resnet50.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/cfg/models/v8/yolov8-cls.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/cfg/models/v8/yolov8-ghost-p2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/cfg/models/v8/yolov8-ghost-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/cfg/models/v8/yolov8-ghost.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/cfg/models/v8/yolov8-obb.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/cfg/models/v8/yolov8-p2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/cfg/models/v8/yolov8-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/cfg/models/v8/yolov8-pose-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/cfg/models/v8/yolov8-pose.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/cfg/models/v8/yolov8-rtdetr.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/cfg/models/v8/yolov8-seg-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/cfg/models/v8/yolov8-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/cfg/models/v8/yolov8-world.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/cfg/models/v8/yolov8-worldv2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/cfg/models/v8/yolov8.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:48:15.765806 ultralytics-8.2.4/ultralytics/cfg/models/v9/
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/cfg/models/v9/yolov9c-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/cfg/models/v9/yolov9c.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/cfg/models/v9/yolov9e-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/cfg/models/v9/yolov9e.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:48:15.765806 ultralytics-8.2.4/ultralytics/cfg/trackers/
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/cfg/trackers/botsort.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/cfg/trackers/bytetrack.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:48:15.769806 ultralytics-8.2.4/ultralytics/data/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/data/annotator.py
--rw-r--r--   0 runner    (1001) docker     (127)    57741 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/data/augment.py
--rw-r--r--   0 runner    (1001) docker     (127)    13481 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/data/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7266 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/data/build.py
--rw-r--r--   0 runner    (1001) docker     (127)    17528 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/data/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    22201 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/data/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:48:15.769806 ultralytics-8.2.4/ultralytics/data/explorer/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/data/explorer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18711 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/data/explorer/explorer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:48:15.769806 ultralytics-8.2.4/ultralytics/data/explorer/gui/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/data/explorer/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10087 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/data/explorer/gui/dash.py
--rw-r--r--   0 runner    (1001) docker     (127)     7085 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/data/explorer/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    23142 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/data/loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)    10010 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/data/split_dota.py
--rw-r--r--   0 runner    (1001) docker     (127)    30869 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:48:15.769806 ultralytics-8.2.4/ultralytics/engine/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    54507 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/engine/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)    40019 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/engine/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    17022 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/engine/predictor.py
--rw-r--r--   0 runner    (1001) docker     (127)    30667 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/engine/results.py
--rw-r--r--   0 runner    (1001) docker     (127)    34987 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/engine/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11844 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/engine/tuner.py
--rw-r--r--   0 runner    (1001) docker     (127)    14643 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/engine/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:48:15.769806 ultralytics-8.2.4/ultralytics/hub/
--rw-r--r--   0 runner    (1001) docker     (127)     5068 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/hub/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    15197 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/hub/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     9721 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/hub/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:48:15.773806 ultralytics-8.2.4/ultralytics/models/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:48:15.773806 ultralytics-8.2.4/ultralytics/models/fastsam/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/models/fastsam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/models/fastsam/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/models/fastsam/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)    16182 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/models/fastsam/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/models/fastsam/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/models/fastsam/val.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:48:15.773806 ultralytics-8.2.4/ultralytics/models/nas/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/models/nas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/models/nas/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/models/nas/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/models/nas/val.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:48:15.773806 ultralytics-8.2.4/ultralytics/models/rtdetr/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/models/rtdetr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/models/rtdetr/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/models/rtdetr/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/models/rtdetr/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/models/rtdetr/val.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:48:15.773806 ultralytics-8.2.4/ultralytics/models/sam/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/models/sam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/models/sam/amg.py
--rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/models/sam/build.py
--rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/models/sam/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:48:15.777806 ultralytics-8.2.4/ultralytics/models/sam/modules/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/models/sam/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7816 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/models/sam/modules/decoders.py
--rw-r--r--   0 runner    (1001) docker     (127)    24746 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/models/sam/modules/encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/models/sam/modules/sam.py
--rw-r--r--   0 runner    (1001) docker     (127)    29125 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/models/sam/modules/tiny_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    11164 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/models/sam/modules/transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)    23614 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/models/sam/predict.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:48:15.777806 ultralytics-8.2.4/ultralytics/models/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/models/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15135 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/models/utils/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    13244 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/models/utils/ops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:48:15.777806 ultralytics-8.2.4/ultralytics/models/yolo/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/models/yolo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:48:15.777806 ultralytics-8.2.4/ultralytics/models/yolo/classify/
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/models/yolo/classify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/models/yolo/classify/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     6888 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/models/yolo/classify/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/models/yolo/classify/val.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:48:15.777806 ultralytics-8.2.4/ultralytics/models/yolo/detect/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/models/yolo/detect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/models/yolo/detect/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     6353 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/models/yolo/detect/train.py
--rw-r--r--   0 runner    (1001) docker     (127)    14427 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/models/yolo/detect/val.py
--rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/models/yolo/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:48:15.777806 ultralytics-8.2.4/ultralytics/models/yolo/obb/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/models/yolo/obb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/models/yolo/obb/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/models/yolo/obb/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     8511 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/models/yolo/obb/val.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:48:15.777806 ultralytics-8.2.4/ultralytics/models/yolo/pose/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/models/yolo/pose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/models/yolo/pose/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/models/yolo/pose/train.py
--rw-r--r--   0 runner    (1001) docker     (127)    10607 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/models/yolo/pose/val.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:48:15.781806 ultralytics-8.2.4/ultralytics/models/yolo/segment/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/models/yolo/segment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/models/yolo/segment/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/models/yolo/segment/train.py
--rw-r--r--   0 runner    (1001) docker     (127)    11745 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/models/yolo/segment/val.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:48:15.781806 ultralytics-8.2.4/ultralytics/models/yolo/world/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/models/yolo/world/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/models/yolo/world/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/models/yolo/world/train_world.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:48:15.781806 ultralytics-8.2.4/ultralytics/nn/
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30864 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/nn/autobackend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:48:15.781806 ultralytics-8.2.4/ultralytics/nn/modules/
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/nn/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25251 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/nn/modules/block.py
--rw-r--r--   0 runner    (1001) docker     (127)    12722 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/nn/modules/conv.py
--rw-r--r--   0 runner    (1001) docker     (127)    22338 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/nn/modules/head.py
--rw-r--r--   0 runner    (1001) docker     (127)    17909 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/nn/modules/transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/nn/modules/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    43623 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/nn/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:48:15.781806 ultralytics-8.2.4/ultralytics/solutions/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/solutions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5696 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/solutions/ai_gym.py
--rw-r--r--   0 runner    (1001) docker     (127)     6334 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/solutions/distance_calculation.py
--rw-r--r--   0 runner    (1001) docker     (127)    12276 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/solutions/heatmap.py
--rw-r--r--   0 runner    (1001) docker     (127)    11558 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/solutions/object_counter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6684 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/solutions/queue_management.py
--rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/solutions/speed_estimation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:48:15.785806 ultralytics-8.2.4/ultralytics/trackers/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/trackers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/trackers/basetrack.py
--rw-r--r--   0 runner    (1001) docker     (127)     8601 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/trackers/bot_sort.py
--rw-r--r--   0 runner    (1001) docker     (127)    18857 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/trackers/byte_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/trackers/track.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:48:15.785806 ultralytics-8.2.4/ultralytics/trackers/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-27 19:46:54.000000 ultralytics-8.2.4/ultralytics/trackers/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13688 2024-04-27 19:46:55.000000 ultralytics-8.2.4/ultralytics/trackers/utils/gmc.py
--rw-r--r--   0 runner    (1001) docker     (127)    15168 2024-04-27 19:46:55.000000 ultralytics-8.2.4/ultralytics/trackers/utils/kalman_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5404 2024-04-27 19:46:55.000000 ultralytics-8.2.4/ultralytics/trackers/utils/matching.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:48:15.789806 ultralytics-8.2.4/ultralytics/utils/
--rw-r--r--   0 runner    (1001) docker     (127)    39286 2024-04-27 19:46:55.000000 ultralytics-8.2.4/ultralytics/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-04-27 19:46:55.000000 ultralytics-8.2.4/ultralytics/utils/autobatch.py
--rw-r--r--   0 runner    (1001) docker     (127)    23470 2024-04-27 19:46:55.000000 ultralytics-8.2.4/ultralytics/utils/benchmarks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:48:15.789806 ultralytics-8.2.4/ultralytics/utils/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-27 19:46:55.000000 ultralytics-8.2.4/ultralytics/utils/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-04-27 19:46:55.000000 ultralytics-8.2.4/ultralytics/utils/callbacks/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5923 2024-04-27 19:46:55.000000 ultralytics-8.2.4/ultralytics/utils/callbacks/clearml.py
--rw-r--r--   0 runner    (1001) docker     (127)    13744 2024-04-27 19:46:55.000000 ultralytics-8.2.4/ultralytics/utils/callbacks/comet.py
--rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-04-27 19:46:55.000000 ultralytics-8.2.4/ultralytics/utils/callbacks/dvc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-04-27 19:46:55.000000 ultralytics-8.2.4/ultralytics/utils/callbacks/hub.py
--rw-r--r--   0 runner    (1001) docker     (127)     5323 2024-04-27 19:46:55.000000 ultralytics-8.2.4/ultralytics/utils/callbacks/mlflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-04-27 19:46:55.000000 ultralytics-8.2.4/ultralytics/utils/callbacks/neptune.py
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-27 19:46:55.000000 ultralytics-8.2.4/ultralytics/utils/callbacks/raytune.py
--rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-04-27 19:46:55.000000 ultralytics-8.2.4/ultralytics/utils/callbacks/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     6674 2024-04-27 19:46:55.000000 ultralytics-8.2.4/ultralytics/utils/callbacks/wb.py
--rw-r--r--   0 runner    (1001) docker     (127)    27971 2024-04-27 19:46:55.000000 ultralytics-8.2.4/ultralytics/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-27 19:46:55.000000 ultralytics-8.2.4/ultralytics/utils/dist.py
--rw-r--r--   0 runner    (1001) docker     (127)    21496 2024-04-27 19:46:55.000000 ultralytics-8.2.4/ultralytics/utils/downloads.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-27 19:46:55.000000 ultralytics-8.2.4/ultralytics/utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     6761 2024-04-27 19:46:55.000000 ultralytics-8.2.4/ultralytics/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (127)    15575 2024-04-27 19:46:55.000000 ultralytics-8.2.4/ultralytics/utils/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)    32717 2024-04-27 19:46:55.000000 ultralytics-8.2.4/ultralytics/utils/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    53518 2024-04-27 19:46:55.000000 ultralytics-8.2.4/ultralytics/utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    33309 2024-04-27 19:46:55.000000 ultralytics-8.2.4/ultralytics/utils/ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-04-27 19:46:55.000000 ultralytics-8.2.4/ultralytics/utils/patches.py
--rw-r--r--   0 runner    (1001) docker     (127)    47332 2024-04-27 19:46:55.000000 ultralytics-8.2.4/ultralytics/utils/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)    16017 2024-04-27 19:46:55.000000 ultralytics-8.2.4/ultralytics/utils/tal.py
--rw-r--r--   0 runner    (1001) docker     (127)    25916 2024-04-27 19:46:55.000000 ultralytics-8.2.4/ultralytics/utils/torch_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-04-27 19:46:55.000000 ultralytics-8.2.4/ultralytics/utils/triton.py
--rw-r--r--   0 runner    (1001) docker     (127)     6171 2024-04-27 19:46:55.000000 ultralytics-8.2.4/ultralytics/utils/tuner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:48:15.789806 ultralytics-8.2.4/ultralytics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    40530 2024-04-27 19:48:15.000000 ultralytics-8.2.4/ultralytics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7684 2024-04-27 19:48:15.000000 ultralytics-8.2.4/ultralytics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 19:48:15.000000 ultralytics-8.2.4/ultralytics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-27 19:48:15.000000 ultralytics-8.2.4/ultralytics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-27 19:48:15.000000 ultralytics-8.2.4/ultralytics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-27 19:48:15.000000 ultralytics-8.2.4/ultralytics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:59:40.836780 ultralytics-8.2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-29 08:58:27.000000 ultralytics-8.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    40530 2024-04-29 08:59:40.836780 ultralytics-8.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    36782 2024-04-29 08:58:27.000000 ultralytics-8.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7334 2024-04-29 08:58:27.000000 ultralytics-8.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 08:59:40.836780 ultralytics-8.2.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:59:40.800779 ultralytics-8.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-04-29 08:58:27.000000 ultralytics-8.2.5/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-04-29 08:58:27.000000 ultralytics-8.2.5/tests/test_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-04-29 08:58:27.000000 ultralytics-8.2.5/tests/test_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-04-29 08:58:27.000000 ultralytics-8.2.5/tests/test_explorer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6053 2024-04-29 08:58:27.000000 ultralytics-8.2.5/tests/test_integrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23135 2024-04-29 08:58:27.000000 ultralytics-8.2.5/tests/test_python.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:59:40.800779 ultralytics-8.2.5/ultralytics/
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:59:40.800779 ultralytics-8.2.5/ultralytics/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)   137419 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/assets/bus.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    50427 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/assets/zidane.jpg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:59:40.800779 ultralytics-8.2.5/ultralytics/cfg/
+-rw-r--r--   0 runner    (1001) docker     (127)    21312 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/cfg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:59:40.804779 ultralytics-8.2.5/ultralytics/cfg/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/cfg/datasets/Argoverse.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/cfg/datasets/DOTAv1.5.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/cfg/datasets/DOTAv1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/cfg/datasets/GlobalWheat2020.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    42507 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/cfg/datasets/ImageNet.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     9324 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/cfg/datasets/Objects365.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/cfg/datasets/SKU-110K.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/cfg/datasets/VOC.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/cfg/datasets/VisDrone.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/cfg/datasets/african-wildlife.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/cfg/datasets/brain-tumor.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/cfg/datasets/carparts-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/cfg/datasets/coco-pose.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/cfg/datasets/coco.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/cfg/datasets/coco128-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/cfg/datasets/coco128.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/cfg/datasets/coco8-pose.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/cfg/datasets/coco8-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/cfg/datasets/coco8.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/cfg/datasets/crack-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/cfg/datasets/dota8.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    29705 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/cfg/datasets/lvis.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    12493 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/cfg/datasets/open-images-v7.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/cfg/datasets/package-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/cfg/datasets/tiger-pose.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/cfg/datasets/xView.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8211 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/cfg/default.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:59:40.792779 ultralytics-8.2.5/ultralytics/cfg/models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:59:40.804779 ultralytics-8.2.5/ultralytics/cfg/models/rt-detr/
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/cfg/models/rt-detr/rtdetr-l.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/cfg/models/rt-detr/rtdetr-resnet101.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/cfg/models/rt-detr/rtdetr-resnet50.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/cfg/models/rt-detr/rtdetr-x.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:59:40.804779 ultralytics-8.2.5/ultralytics/cfg/models/v3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/cfg/models/v3/yolov3-spp.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/cfg/models/v3/yolov3-tiny.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/cfg/models/v3/yolov3.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:59:40.808779 ultralytics-8.2.5/ultralytics/cfg/models/v5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/cfg/models/v5/yolov5-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/cfg/models/v5/yolov5.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:59:40.808779 ultralytics-8.2.5/ultralytics/cfg/models/v6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/cfg/models/v6/yolov6.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:59:40.808779 ultralytics-8.2.5/ultralytics/cfg/models/v8/
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/cfg/models/v8/yolov8-cls-resnet101.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/cfg/models/v8/yolov8-cls-resnet50.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/cfg/models/v8/yolov8-cls.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/cfg/models/v8/yolov8-ghost-p2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/cfg/models/v8/yolov8-ghost-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/cfg/models/v8/yolov8-ghost.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/cfg/models/v8/yolov8-obb.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/cfg/models/v8/yolov8-p2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/cfg/models/v8/yolov8-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/cfg/models/v8/yolov8-pose-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/cfg/models/v8/yolov8-pose.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/cfg/models/v8/yolov8-rtdetr.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/cfg/models/v8/yolov8-seg-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/cfg/models/v8/yolov8-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/cfg/models/v8/yolov8-world.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/cfg/models/v8/yolov8-worldv2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/cfg/models/v8/yolov8.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:59:40.808779 ultralytics-8.2.5/ultralytics/cfg/models/v9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/cfg/models/v9/yolov9c-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/cfg/models/v9/yolov9c.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/cfg/models/v9/yolov9e-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/cfg/models/v9/yolov9e.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:59:40.808779 ultralytics-8.2.5/ultralytics/cfg/trackers/
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/cfg/trackers/botsort.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/cfg/trackers/bytetrack.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:59:40.812780 ultralytics-8.2.5/ultralytics/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/data/annotator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57741 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/data/augment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13481 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/data/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7266 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/data/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17528 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/data/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22201 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/data/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:59:40.812780 ultralytics-8.2.5/ultralytics/data/explorer/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/data/explorer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18711 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/data/explorer/explorer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:59:40.812780 ultralytics-8.2.5/ultralytics/data/explorer/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/data/explorer/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10087 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/data/explorer/gui/dash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7085 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/data/explorer/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23142 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/data/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10010 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/data/split_dota.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30869 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:59:40.812780 ultralytics-8.2.5/ultralytics/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54507 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/engine/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40019 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/engine/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17022 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/engine/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30667 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/engine/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34987 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/engine/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11844 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/engine/tuner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14643 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/engine/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:59:40.816779 ultralytics-8.2.5/ultralytics/hub/
+-rw-r--r--   0 runner    (1001) docker     (127)     5068 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/hub/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15197 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/hub/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9721 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/hub/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:59:40.816779 ultralytics-8.2.5/ultralytics/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:59:40.816779 ultralytics-8.2.5/ultralytics/models/fastsam/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/models/fastsam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/models/fastsam/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/models/fastsam/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16182 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/models/fastsam/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/models/fastsam/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/models/fastsam/val.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:59:40.816779 ultralytics-8.2.5/ultralytics/models/nas/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/models/nas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/models/nas/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/models/nas/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/models/nas/val.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:59:40.816779 ultralytics-8.2.5/ultralytics/models/rtdetr/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/models/rtdetr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/models/rtdetr/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/models/rtdetr/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/models/rtdetr/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/models/rtdetr/val.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:59:40.816779 ultralytics-8.2.5/ultralytics/models/sam/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/models/sam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/models/sam/amg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/models/sam/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/models/sam/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:59:40.820779 ultralytics-8.2.5/ultralytics/models/sam/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/models/sam/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7816 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/models/sam/modules/decoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24746 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/models/sam/modules/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/models/sam/modules/sam.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29125 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/models/sam/modules/tiny_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11164 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/models/sam/modules/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23614 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/models/sam/predict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:59:40.820779 ultralytics-8.2.5/ultralytics/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/models/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15135 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/models/utils/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13244 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/models/utils/ops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:59:40.820779 ultralytics-8.2.5/ultralytics/models/yolo/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/models/yolo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:59:40.820779 ultralytics-8.2.5/ultralytics/models/yolo/classify/
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/models/yolo/classify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/models/yolo/classify/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6888 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/models/yolo/classify/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/models/yolo/classify/val.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:59:40.820779 ultralytics-8.2.5/ultralytics/models/yolo/detect/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/models/yolo/detect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/models/yolo/detect/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6353 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/models/yolo/detect/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14427 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/models/yolo/detect/val.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/models/yolo/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:59:40.820779 ultralytics-8.2.5/ultralytics/models/yolo/obb/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/models/yolo/obb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/models/yolo/obb/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/models/yolo/obb/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8511 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/models/yolo/obb/val.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:59:40.824780 ultralytics-8.2.5/ultralytics/models/yolo/pose/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/models/yolo/pose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/models/yolo/pose/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/models/yolo/pose/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10607 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/models/yolo/pose/val.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:59:40.824780 ultralytics-8.2.5/ultralytics/models/yolo/segment/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/models/yolo/segment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/models/yolo/segment/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/models/yolo/segment/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11745 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/models/yolo/segment/val.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:59:40.824780 ultralytics-8.2.5/ultralytics/models/yolo/world/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/models/yolo/world/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/models/yolo/world/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/models/yolo/world/train_world.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:59:40.824780 ultralytics-8.2.5/ultralytics/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30864 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/nn/autobackend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:59:40.824780 ultralytics-8.2.5/ultralytics/nn/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/nn/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25251 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/nn/modules/block.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12722 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/nn/modules/conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22338 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/nn/modules/head.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17909 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/nn/modules/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/nn/modules/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43623 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/nn/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:59:40.828780 ultralytics-8.2.5/ultralytics/solutions/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/solutions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5696 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/solutions/ai_gym.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6334 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/solutions/distance_calculation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11970 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/solutions/heatmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11287 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/solutions/object_counter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8656 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/solutions/parking_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6684 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/solutions/queue_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/solutions/speed_estimation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:59:40.828780 ultralytics-8.2.5/ultralytics/trackers/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/trackers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/trackers/basetrack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8601 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/trackers/bot_sort.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18857 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/trackers/byte_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/trackers/track.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:59:40.828780 ultralytics-8.2.5/ultralytics/trackers/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/trackers/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13688 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/trackers/utils/gmc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15168 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/trackers/utils/kalman_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5404 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/trackers/utils/matching.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:59:40.832780 ultralytics-8.2.5/ultralytics/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)    39286 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/utils/autobatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23470 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/utils/benchmarks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:59:40.832780 ultralytics-8.2.5/ultralytics/utils/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/utils/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/utils/callbacks/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5923 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/utils/callbacks/clearml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13744 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/utils/callbacks/comet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/utils/callbacks/dvc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/utils/callbacks/hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5323 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/utils/callbacks/mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/utils/callbacks/neptune.py
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/utils/callbacks/raytune.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/utils/callbacks/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6674 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/utils/callbacks/wb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27971 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/utils/dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21496 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/utils/downloads.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6761 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15575 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/utils/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32717 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/utils/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53518 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33309 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/utils/ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/utils/patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48315 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/utils/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16017 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/utils/tal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25916 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/utils/torch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/utils/triton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6171 2024-04-29 08:58:27.000000 ultralytics-8.2.5/ultralytics/utils/tuner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:59:40.832780 ultralytics-8.2.5/ultralytics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    40530 2024-04-29 08:59:40.000000 ultralytics-8.2.5/ultralytics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7728 2024-04-29 08:59:40.000000 ultralytics-8.2.5/ultralytics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 08:59:40.000000 ultralytics-8.2.5/ultralytics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-29 08:59:40.000000 ultralytics-8.2.5/ultralytics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-29 08:59:40.000000 ultralytics-8.2.5/ultralytics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-29 08:59:40.000000 ultralytics-8.2.5/ultralytics.egg-info/top_level.txt
```

### Comparing `ultralytics-8.2.4/LICENSE` & `ultralytics-8.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/PKG-INFO` & `ultralytics-8.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultralytics
-Version: 8.2.4
+Version: 8.2.5
 Summary: Ultralytics YOLOv8 for SOTA object detection, multi-object tracking, instance segmentation, pose estimation and image classification.
 Author: Glenn Jocher, Ayush Chaurasia, Jing Qiu
 Maintainer: Glenn Jocher, Ayush Chaurasia, Jing Qiu
 License: AGPL-3.0
 Project-URL: Bug Reports, https://github.com/ultralytics/ultralytics/issues
 Project-URL: Funding, https://ultralytics.com
 Project-URL: Source, https://github.com/ultralytics/ultralytics/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ultralytics Version: 8.2.4 Summary: Ultralytics
+Metadata-Version: 2.1 Name: ultralytics Version: 8.2.5 Summary: Ultralytics
 YOLOv8 for SOTA object detection, multi-object tracking, instance segmentation,
 pose estimation and image classification. Author: Glenn Jocher, Ayush
 Chaurasia, Jing Qiu Maintainer: Glenn Jocher, Ayush Chaurasia, Jing Qiu
 License: AGPL-3.0 Project-URL: Bug Reports, https://github.com/ultralytics/
 ultralytics/issues Project-URL: Funding, https://ultralytics.com Project-URL:
 Source, https://github.com/ultralytics/ultralytics/ Keywords: machine-
 learning,deep-learning,computer-
```

### Comparing `ultralytics-8.2.4/README.md` & `ultralytics-8.2.5/README.md`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/pyproject.toml` & `ultralytics-8.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/tests/test_cli.py` & `ultralytics-8.2.5/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/tests/test_cuda.py` & `ultralytics-8.2.5/tests/test_cuda.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/tests/test_engine.py` & `ultralytics-8.2.5/tests/test_engine.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/tests/test_explorer.py` & `ultralytics-8.2.5/tests/test_explorer.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/tests/test_integrations.py` & `ultralytics-8.2.5/tests/test_integrations.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/tests/test_python.py` & `ultralytics-8.2.5/tests/test_python.py`

 * *Files 0% similar despite different names*

```diff
@@ -633,14 +633,15 @@
     for batch in [SOURCE], [SOURCE, SOURCE]:  # test batch size 1 and 2
         assert len(model_detect.embed(source=batch, imgsz=32)) == len(batch)
         assert len(model_segment.embed(source=batch, imgsz=32)) == len(batch)
 
 
 @pytest.mark.skipif(checks.IS_PYTHON_3_12, reason="YOLOWorld with CLIP is not supported in Python 3.12")
 def test_yolo_world():
+    """Tests YOLO world models with different configurations, including classes, detection, and training scenarios."""
     model = YOLO("yolov8s-world.pt")  # no YOLOv8n-world model yet
     model.set_classes(["tree", "window"])
     model(ASSETS / "bus.jpg", conf=0.01)
 
     model = YOLO("yolov8s-worldv2.pt")  # no YOLOv8n-world model yet
     # Training from pretrain, evaluation process is included at the final stage of training.
     # Use dota8.yaml which has less categories to reduce the inference time of CLIP model
```

### Comparing `ultralytics-8.2.4/ultralytics/__init__.py` & `ultralytics-8.2.5/ultralytics/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Ultralytics YOLO 🚀, AGPL-3.0 license
 
-__version__ = "8.2.4"
+__version__ = "8.2.5"
 
 from ultralytics.data.explorer.explorer import Explorer
 from ultralytics.models import RTDETR, SAM, YOLO, YOLOWorld
 from ultralytics.models.fastsam import FastSAM
 from ultralytics.models.nas import NAS
 from ultralytics.utils import ASSETS, SETTINGS
 from ultralytics.utils.checks import check_yolo as checks
```

### Comparing `ultralytics-8.2.4/ultralytics/assets/bus.jpg` & `ultralytics-8.2.5/ultralytics/assets/bus.jpg`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/assets/zidane.jpg` & `ultralytics-8.2.5/ultralytics/assets/zidane.jpg`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/cfg/__init__.py` & `ultralytics-8.2.5/ultralytics/cfg/__init__.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/cfg/datasets/Argoverse.yaml` & `ultralytics-8.2.5/ultralytics/cfg/datasets/Argoverse.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/cfg/datasets/DOTAv1.5.yaml` & `ultralytics-8.2.5/ultralytics/cfg/datasets/DOTAv1.5.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/cfg/datasets/DOTAv1.yaml` & `ultralytics-8.2.5/ultralytics/cfg/datasets/DOTAv1.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/cfg/datasets/GlobalWheat2020.yaml` & `ultralytics-8.2.5/ultralytics/cfg/datasets/GlobalWheat2020.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/cfg/datasets/ImageNet.yaml` & `ultralytics-8.2.5/ultralytics/cfg/datasets/ImageNet.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/cfg/datasets/Objects365.yaml` & `ultralytics-8.2.5/ultralytics/cfg/datasets/Objects365.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/cfg/datasets/SKU-110K.yaml` & `ultralytics-8.2.5/ultralytics/cfg/datasets/SKU-110K.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/cfg/datasets/VOC.yaml` & `ultralytics-8.2.5/ultralytics/cfg/datasets/VOC.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/cfg/datasets/VisDrone.yaml` & `ultralytics-8.2.5/ultralytics/cfg/datasets/VisDrone.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/cfg/datasets/african-wildlife.yaml` & `ultralytics-8.2.5/ultralytics/cfg/datasets/african-wildlife.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/cfg/datasets/brain-tumor.yaml` & `ultralytics-8.2.5/ultralytics/cfg/datasets/brain-tumor.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/cfg/datasets/carparts-seg.yaml` & `ultralytics-8.2.5/ultralytics/cfg/datasets/carparts-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/cfg/datasets/coco-pose.yaml` & `ultralytics-8.2.5/ultralytics/cfg/datasets/coco-pose.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/cfg/datasets/coco.yaml` & `ultralytics-8.2.5/ultralytics/cfg/datasets/coco.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/cfg/datasets/coco128-seg.yaml` & `ultralytics-8.2.5/ultralytics/cfg/datasets/coco128-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/cfg/datasets/coco128.yaml` & `ultralytics-8.2.5/ultralytics/cfg/datasets/coco128.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/cfg/datasets/coco8-pose.yaml` & `ultralytics-8.2.5/ultralytics/cfg/datasets/coco8-pose.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/cfg/datasets/coco8-seg.yaml` & `ultralytics-8.2.5/ultralytics/cfg/datasets/coco8-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/cfg/datasets/coco8.yaml` & `ultralytics-8.2.5/ultralytics/cfg/datasets/coco8.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/cfg/datasets/crack-seg.yaml` & `ultralytics-8.2.5/ultralytics/cfg/datasets/crack-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/cfg/datasets/dota8.yaml` & `ultralytics-8.2.5/ultralytics/cfg/datasets/dota8.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/cfg/datasets/lvis.yaml` & `ultralytics-8.2.5/ultralytics/cfg/datasets/lvis.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/cfg/datasets/open-images-v7.yaml` & `ultralytics-8.2.5/ultralytics/cfg/datasets/open-images-v7.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/cfg/datasets/package-seg.yaml` & `ultralytics-8.2.5/ultralytics/cfg/datasets/package-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/cfg/datasets/tiger-pose.yaml` & `ultralytics-8.2.5/ultralytics/cfg/datasets/tiger-pose.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/cfg/datasets/xView.yaml` & `ultralytics-8.2.5/ultralytics/cfg/datasets/xView.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/cfg/default.yaml` & `ultralytics-8.2.5/ultralytics/cfg/default.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/cfg/models/rt-detr/rtdetr-l.yaml` & `ultralytics-8.2.5/ultralytics/cfg/models/rt-detr/rtdetr-l.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/cfg/models/rt-detr/rtdetr-resnet101.yaml` & `ultralytics-8.2.5/ultralytics/cfg/models/rt-detr/rtdetr-resnet101.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/cfg/models/rt-detr/rtdetr-resnet50.yaml` & `ultralytics-8.2.5/ultralytics/cfg/models/rt-detr/rtdetr-resnet50.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/cfg/models/rt-detr/rtdetr-x.yaml` & `ultralytics-8.2.5/ultralytics/cfg/models/rt-detr/rtdetr-x.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/cfg/models/v3/yolov3-spp.yaml` & `ultralytics-8.2.5/ultralytics/cfg/models/v3/yolov3-spp.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/cfg/models/v3/yolov3-tiny.yaml` & `ultralytics-8.2.5/ultralytics/cfg/models/v3/yolov3-tiny.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/cfg/models/v3/yolov3.yaml` & `ultralytics-8.2.5/ultralytics/cfg/models/v3/yolov3.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/cfg/models/v5/yolov5-p6.yaml` & `ultralytics-8.2.5/ultralytics/cfg/models/v5/yolov5-p6.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/cfg/models/v5/yolov5.yaml` & `ultralytics-8.2.5/ultralytics/cfg/models/v5/yolov5.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/cfg/models/v6/yolov6.yaml` & `ultralytics-8.2.5/ultralytics/cfg/models/v6/yolov6.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/cfg/models/v8/yolov8-cls-resnet101.yaml` & `ultralytics-8.2.5/ultralytics/cfg/models/v8/yolov8-cls-resnet101.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/cfg/models/v8/yolov8-cls-resnet50.yaml` & `ultralytics-8.2.5/ultralytics/cfg/models/v8/yolov8-cls-resnet50.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/cfg/models/v8/yolov8-cls.yaml` & `ultralytics-8.2.5/ultralytics/cfg/models/v8/yolov8-cls.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/cfg/models/v8/yolov8-ghost-p2.yaml` & `ultralytics-8.2.5/ultralytics/cfg/models/v8/yolov8-ghost-p2.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/cfg/models/v8/yolov8-ghost-p6.yaml` & `ultralytics-8.2.5/ultralytics/cfg/models/v8/yolov8-ghost-p6.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/cfg/models/v8/yolov8-ghost.yaml` & `ultralytics-8.2.5/ultralytics/cfg/models/v8/yolov8-ghost.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/cfg/models/v8/yolov8-obb.yaml` & `ultralytics-8.2.5/ultralytics/cfg/models/v8/yolov8-obb.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/cfg/models/v8/yolov8-p2.yaml` & `ultralytics-8.2.5/ultralytics/cfg/models/v8/yolov8-p2.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/cfg/models/v8/yolov8-p6.yaml` & `ultralytics-8.2.5/ultralytics/cfg/models/v8/yolov8-p6.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/cfg/models/v8/yolov8-pose-p6.yaml` & `ultralytics-8.2.5/ultralytics/cfg/models/v8/yolov8-pose-p6.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/cfg/models/v8/yolov8-pose.yaml` & `ultralytics-8.2.5/ultralytics/cfg/models/v8/yolov8-pose.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/cfg/models/v8/yolov8-rtdetr.yaml` & `ultralytics-8.2.5/ultralytics/cfg/models/v8/yolov8-rtdetr.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/cfg/models/v8/yolov8-seg-p6.yaml` & `ultralytics-8.2.5/ultralytics/cfg/models/v8/yolov8-seg-p6.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/cfg/models/v8/yolov8-seg.yaml` & `ultralytics-8.2.5/ultralytics/cfg/models/v8/yolov8-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/cfg/models/v8/yolov8-world.yaml` & `ultralytics-8.2.5/ultralytics/cfg/models/v8/yolov8-world.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/cfg/models/v8/yolov8-worldv2.yaml` & `ultralytics-8.2.5/ultralytics/cfg/models/v8/yolov8-worldv2.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/cfg/models/v8/yolov8.yaml` & `ultralytics-8.2.5/ultralytics/cfg/models/v8/yolov8.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/cfg/models/v9/yolov9c-seg.yaml` & `ultralytics-8.2.5/ultralytics/cfg/models/v9/yolov9c-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/cfg/models/v9/yolov9c.yaml` & `ultralytics-8.2.5/ultralytics/cfg/models/v9/yolov9c.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/cfg/models/v9/yolov9e-seg.yaml` & `ultralytics-8.2.5/ultralytics/cfg/models/v9/yolov9e-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/cfg/models/v9/yolov9e.yaml` & `ultralytics-8.2.5/ultralytics/cfg/models/v9/yolov9e.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/cfg/trackers/botsort.yaml` & `ultralytics-8.2.5/ultralytics/cfg/trackers/botsort.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/cfg/trackers/bytetrack.yaml` & `ultralytics-8.2.5/ultralytics/cfg/trackers/bytetrack.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/data/__init__.py` & `ultralytics-8.2.5/ultralytics/data/__init__.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/data/annotator.py` & `ultralytics-8.2.5/ultralytics/data/annotator.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/data/augment.py` & `ultralytics-8.2.5/ultralytics/data/augment.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/data/base.py` & `ultralytics-8.2.5/ultralytics/data/base.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/data/build.py` & `ultralytics-8.2.5/ultralytics/data/build.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/data/converter.py` & `ultralytics-8.2.5/ultralytics/data/converter.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/data/dataset.py` & `ultralytics-8.2.5/ultralytics/data/dataset.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/data/explorer/explorer.py` & `ultralytics-8.2.5/ultralytics/data/explorer/explorer.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/data/explorer/gui/dash.py` & `ultralytics-8.2.5/ultralytics/data/explorer/gui/dash.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/data/explorer/utils.py` & `ultralytics-8.2.5/ultralytics/data/explorer/utils.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/data/loaders.py` & `ultralytics-8.2.5/ultralytics/data/loaders.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/data/split_dota.py` & `ultralytics-8.2.5/ultralytics/data/split_dota.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/data/utils.py` & `ultralytics-8.2.5/ultralytics/data/utils.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/engine/exporter.py` & `ultralytics-8.2.5/ultralytics/engine/exporter.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/engine/model.py` & `ultralytics-8.2.5/ultralytics/engine/model.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/engine/predictor.py` & `ultralytics-8.2.5/ultralytics/engine/predictor.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/engine/results.py` & `ultralytics-8.2.5/ultralytics/engine/results.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/engine/trainer.py` & `ultralytics-8.2.5/ultralytics/engine/trainer.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/engine/tuner.py` & `ultralytics-8.2.5/ultralytics/engine/tuner.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/engine/validator.py` & `ultralytics-8.2.5/ultralytics/engine/validator.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/hub/__init__.py` & `ultralytics-8.2.5/ultralytics/hub/__init__.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/hub/auth.py` & `ultralytics-8.2.5/ultralytics/hub/auth.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/hub/session.py` & `ultralytics-8.2.5/ultralytics/hub/session.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/hub/utils.py` & `ultralytics-8.2.5/ultralytics/hub/utils.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/models/fastsam/model.py` & `ultralytics-8.2.5/ultralytics/models/fastsam/model.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/models/fastsam/predict.py` & `ultralytics-8.2.5/ultralytics/models/fastsam/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/models/fastsam/prompt.py` & `ultralytics-8.2.5/ultralytics/models/fastsam/prompt.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/models/fastsam/utils.py` & `ultralytics-8.2.5/ultralytics/models/fastsam/utils.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/models/fastsam/val.py` & `ultralytics-8.2.5/ultralytics/models/fastsam/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/models/nas/model.py` & `ultralytics-8.2.5/ultralytics/models/nas/model.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/models/nas/predict.py` & `ultralytics-8.2.5/ultralytics/models/nas/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/models/nas/val.py` & `ultralytics-8.2.5/ultralytics/models/nas/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/models/rtdetr/model.py` & `ultralytics-8.2.5/ultralytics/models/rtdetr/model.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/models/rtdetr/predict.py` & `ultralytics-8.2.5/ultralytics/models/rtdetr/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/models/rtdetr/train.py` & `ultralytics-8.2.5/ultralytics/models/rtdetr/train.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/models/rtdetr/val.py` & `ultralytics-8.2.5/ultralytics/models/rtdetr/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/models/sam/amg.py` & `ultralytics-8.2.5/ultralytics/models/sam/amg.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/models/sam/build.py` & `ultralytics-8.2.5/ultralytics/models/sam/build.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/models/sam/model.py` & `ultralytics-8.2.5/ultralytics/models/sam/model.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/models/sam/modules/decoders.py` & `ultralytics-8.2.5/ultralytics/models/sam/modules/decoders.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/models/sam/modules/encoders.py` & `ultralytics-8.2.5/ultralytics/models/sam/modules/encoders.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/models/sam/modules/sam.py` & `ultralytics-8.2.5/ultralytics/models/sam/modules/sam.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/models/sam/modules/tiny_encoder.py` & `ultralytics-8.2.5/ultralytics/models/sam/modules/tiny_encoder.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/models/sam/modules/transformer.py` & `ultralytics-8.2.5/ultralytics/models/sam/modules/transformer.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/models/sam/predict.py` & `ultralytics-8.2.5/ultralytics/models/sam/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/models/utils/loss.py` & `ultralytics-8.2.5/ultralytics/models/utils/loss.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/models/utils/ops.py` & `ultralytics-8.2.5/ultralytics/models/utils/ops.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/models/yolo/classify/predict.py` & `ultralytics-8.2.5/ultralytics/models/yolo/classify/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/models/yolo/classify/train.py` & `ultralytics-8.2.5/ultralytics/models/yolo/classify/train.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/models/yolo/classify/val.py` & `ultralytics-8.2.5/ultralytics/models/yolo/classify/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/models/yolo/detect/predict.py` & `ultralytics-8.2.5/ultralytics/models/yolo/detect/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/models/yolo/detect/train.py` & `ultralytics-8.2.5/ultralytics/models/yolo/detect/train.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/models/yolo/detect/val.py` & `ultralytics-8.2.5/ultralytics/models/yolo/detect/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/models/yolo/model.py` & `ultralytics-8.2.5/ultralytics/models/yolo/model.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/models/yolo/obb/predict.py` & `ultralytics-8.2.5/ultralytics/models/yolo/obb/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/models/yolo/obb/train.py` & `ultralytics-8.2.5/ultralytics/models/yolo/obb/train.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/models/yolo/obb/val.py` & `ultralytics-8.2.5/ultralytics/models/yolo/obb/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/models/yolo/pose/predict.py` & `ultralytics-8.2.5/ultralytics/models/yolo/pose/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/models/yolo/pose/train.py` & `ultralytics-8.2.5/ultralytics/models/yolo/pose/train.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/models/yolo/pose/val.py` & `ultralytics-8.2.5/ultralytics/models/yolo/pose/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/models/yolo/segment/predict.py` & `ultralytics-8.2.5/ultralytics/models/yolo/segment/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/models/yolo/segment/train.py` & `ultralytics-8.2.5/ultralytics/models/yolo/segment/train.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/models/yolo/segment/val.py` & `ultralytics-8.2.5/ultralytics/models/yolo/segment/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/models/yolo/world/train.py` & `ultralytics-8.2.5/ultralytics/models/yolo/world/train.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/models/yolo/world/train_world.py` & `ultralytics-8.2.5/ultralytics/models/yolo/world/train_world.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/nn/__init__.py` & `ultralytics-8.2.5/ultralytics/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/nn/autobackend.py` & `ultralytics-8.2.5/ultralytics/nn/autobackend.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/nn/modules/__init__.py` & `ultralytics-8.2.5/ultralytics/nn/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/nn/modules/block.py` & `ultralytics-8.2.5/ultralytics/nn/modules/block.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/nn/modules/conv.py` & `ultralytics-8.2.5/ultralytics/nn/modules/conv.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/nn/modules/head.py` & `ultralytics-8.2.5/ultralytics/nn/modules/head.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/nn/modules/transformer.py` & `ultralytics-8.2.5/ultralytics/nn/modules/transformer.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/nn/modules/utils.py` & `ultralytics-8.2.5/ultralytics/nn/modules/utils.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/nn/tasks.py` & `ultralytics-8.2.5/ultralytics/nn/tasks.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/solutions/ai_gym.py` & `ultralytics-8.2.5/ultralytics/solutions/ai_gym.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/solutions/distance_calculation.py` & `ultralytics-8.2.5/ultralytics/solutions/distance_calculation.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/solutions/heatmap.py` & `ultralytics-8.2.5/ultralytics/solutions/heatmap.py`

 * *Files 4% similar despite different names*

```diff
@@ -186,17 +186,15 @@
                 self.annotator.draw_region(
                     reg_pts=self.count_reg_pts, color=self.region_color, thickness=self.region_thickness
                 )
 
             for box, cls, track_id in zip(self.boxes, self.clss, self.track_ids):
                 # Store class info
                 if self.names[cls] not in self.class_wise_count:
-                    if len(self.names[cls]) > 5:
-                        self.names[cls] = self.names[cls][:5]
-                    self.class_wise_count[self.names[cls]] = {"in": 0, "out": 0}
+                    self.class_wise_count[self.names[cls]] = {"IN": 0, "OUT": 0}
 
                 if self.shape == "circle":
                     center = (int((box[0] + box[2]) // 2), int((box[1] + box[3]) // 2))
                     radius = min(int(box[2]) - int(box[0]), int(box[3]) - int(box[1])) // 2
 
                     y, x = np.ogrid[0 : self.heatmap.shape[0], 0 : self.heatmap.shape[1]]
                     mask = (x - center[0]) ** 2 + (y - center[1]) ** 2 <= radius**2
@@ -221,32 +219,32 @@
                     is_inside = self.counting_region.contains(Point(track_line[-1]))
 
                     if prev_position is not None and is_inside and track_id not in self.count_ids:
                         self.count_ids.append(track_id)
 
                         if (box[0] - prev_position[0]) * (self.counting_region.centroid.x - prev_position[0]) > 0:
                             self.in_counts += 1
-                            self.class_wise_count[self.names[cls]]["in"] += 1
+                            self.class_wise_count[self.names[cls]]["IN"] += 1
                         else:
                             self.out_counts += 1
-                            self.class_wise_count[self.names[cls]]["out"] += 1
+                            self.class_wise_count[self.names[cls]]["OUT"] += 1
 
                 # Count objects using line
                 elif len(self.count_reg_pts) == 2:
                     if prev_position is not None and track_id not in self.count_ids:
                         distance = Point(track_line[-1]).distance(self.counting_region)
                         if distance < self.line_dist_thresh and track_id not in self.count_ids:
                             self.count_ids.append(track_id)
 
                             if (box[0] - prev_position[0]) * (self.counting_region.centroid.x - prev_position[0]) > 0:
                                 self.in_counts += 1
-                                self.class_wise_count[self.names[cls]]["in"] += 1
+                                self.class_wise_count[self.names[cls]]["IN"] += 1
                             else:
                                 self.out_counts += 1
-                                self.class_wise_count[self.names[cls]]["out"] += 1
+                                self.class_wise_count[self.names[cls]]["OUT"] += 1
 
         else:
             for box, cls in zip(self.boxes, self.clss):
                 if self.shape == "circle":
                     center = (int((box[0] + box[2]) // 2), int((box[1] + box[3]) // 2))
                     radius = min(int(box[2]) - int(box[0]), int(box[3]) - int(box[1])) // 2
 
@@ -260,36 +258,29 @@
                 else:
                     self.heatmap[int(box[1]) : int(box[3]), int(box[0]) : int(box[2])] += 2
 
         # Normalize, apply colormap to heatmap and combine with original image
         heatmap_normalized = cv2.normalize(self.heatmap, None, 0, 255, cv2.NORM_MINMAX)
         heatmap_colored = cv2.applyColorMap(heatmap_normalized.astype(np.uint8), self.colormap)
 
-        label = "Ultralytics Analytics \t"
+        labels_dict = {}
 
         for key, value in self.class_wise_count.items():
-            if value["in"] != 0 or value["out"] != 0:
+            if value["IN"] != 0 or value["OUT"] != 0:
                 if not self.view_in_counts and not self.view_out_counts:
-                    label = None
+                    continue
                 elif not self.view_in_counts:
-                    label += f"{str.capitalize(key)}: IN {value['in']} \t"
+                    labels_dict[str.capitalize(key)] = f"OUT {value['OUT']}"
                 elif not self.view_out_counts:
-                    label += f"{str.capitalize(key)}: OUT {value['out']} \t"
+                    labels_dict[str.capitalize(key)] = f"IN {value['IN']}"
                 else:
-                    label += f"{str.capitalize(key)}: IN {value['in']} OUT {value['out']} \t"
+                    labels_dict[str.capitalize(key)] = f"IN {value['IN']} OUT {value['OUT']}"
 
-        label = label.rstrip()
-        label = label.split("\t")
-
-        if self.count_reg_pts is not None and label is not None:
-            self.annotator.display_counts(
-                counts=label,
-                count_txt_color=self.count_txt_color,
-                count_bg_color=self.count_bg_color,
-            )
+        if labels_dict is not None:
+            self.annotator.display_analytics(self.im0, labels_dict, self.count_txt_color, self.count_bg_color, 10)
 
         self.im0 = cv2.addWeighted(self.im0, 1 - self.heatmap_alpha, heatmap_colored, self.heatmap_alpha, 0)
 
         if self.env_check and self.view_img:
             self.display_frames()
 
         return self.im0
```

### Comparing `ultralytics-8.2.4/ultralytics/solutions/object_counter.py` & `ultralytics-8.2.5/ultralytics/solutions/object_counter.py`

 * *Files 4% similar despite different names*

```diff
@@ -177,17 +177,15 @@
             # Extract tracks
             for box, track_id, cls in zip(boxes, track_ids, clss):
                 # Draw bounding box
                 self.annotator.box_label(box, label=f"{self.names[cls]}#{track_id}", color=colors(int(track_id), True))
 
                 # Store class info
                 if self.names[cls] not in self.class_wise_count:
-                    if len(self.names[cls]) > 5:
-                        self.names[cls] = self.names[cls][:5]
-                    self.class_wise_count[self.names[cls]] = {"in": 0, "out": 0}
+                    self.class_wise_count[self.names[cls]] = {"IN": 0, "OUT": 0}
 
                 # Draw Tracks
                 track_line = self.track_history[track_id]
                 track_line.append((float((box[0] + box[2]) / 2), float((box[1] + box[3]) / 2)))
                 if len(track_line) > 30:
                     track_line.pop(0)
 
@@ -206,55 +204,48 @@
                     is_inside = self.counting_region.contains(Point(track_line[-1]))
 
                     if prev_position is not None and is_inside and track_id not in self.count_ids:
                         self.count_ids.append(track_id)
 
                         if (box[0] - prev_position[0]) * (self.counting_region.centroid.x - prev_position[0]) > 0:
                             self.in_counts += 1
-                            self.class_wise_count[self.names[cls]]["in"] += 1
+                            self.class_wise_count[self.names[cls]]["IN"] += 1
                         else:
                             self.out_counts += 1
-                            self.class_wise_count[self.names[cls]]["out"] += 1
+                            self.class_wise_count[self.names[cls]]["OUT"] += 1
 
                 # Count objects using line
                 elif len(self.reg_pts) == 2:
                     if prev_position is not None and track_id not in self.count_ids:
                         distance = Point(track_line[-1]).distance(self.counting_region)
                         if distance < self.line_dist_thresh and track_id not in self.count_ids:
                             self.count_ids.append(track_id)
 
                             if (box[0] - prev_position[0]) * (self.counting_region.centroid.x - prev_position[0]) > 0:
                                 self.in_counts += 1
-                                self.class_wise_count[self.names[cls]]["in"] += 1
+                                self.class_wise_count[self.names[cls]]["IN"] += 1
                             else:
                                 self.out_counts += 1
-                                self.class_wise_count[self.names[cls]]["out"] += 1
+                                self.class_wise_count[self.names[cls]]["OUT"] += 1
 
-        label = "Ultralytics Analytics \t"
+        labels_dict = {}
 
         for key, value in self.class_wise_count.items():
-            if value["in"] != 0 or value["out"] != 0:
+            if value["IN"] != 0 or value["OUT"] != 0:
                 if not self.view_in_counts and not self.view_out_counts:
-                    label = None
+                    continue
                 elif not self.view_in_counts:
-                    label += f"{str.capitalize(key)}: IN {value['in']} \t"
+                    labels_dict[str.capitalize(key)] = f"OUT {value['OUT']}"
                 elif not self.view_out_counts:
-                    label += f"{str.capitalize(key)}: OUT {value['out']} \t"
+                    labels_dict[str.capitalize(key)] = f"IN {value['IN']}"
                 else:
-                    label += f"{str.capitalize(key)}: IN {value['in']} OUT {value['out']} \t"
+                    labels_dict[str.capitalize(key)] = f"IN {value['IN']} OUT {value['OUT']}"
 
-        label = label.rstrip()
-        label = label.split("\t")
-
-        if label is not None:
-            self.annotator.display_counts(
-                counts=label,
-                count_txt_color=self.count_txt_color,
-                count_bg_color=self.count_bg_color,
-            )
+        if labels_dict is not None:
+            self.annotator.display_analytics(self.im0, labels_dict, self.count_txt_color, self.count_bg_color, 10)
 
     def display_frames(self):
         """Display frame."""
         if self.env_check:
             cv2.namedWindow(self.window_name)
             if len(self.reg_pts) == 4:  # only add mouse event If user drawn region
                 cv2.setMouseCallback(self.window_name, self.mouse_event_for_region, {"region_points": self.reg_pts})
```

### Comparing `ultralytics-8.2.4/ultralytics/solutions/queue_management.py` & `ultralytics-8.2.5/ultralytics/solutions/queue_management.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/solutions/speed_estimation.py` & `ultralytics-8.2.5/ultralytics/solutions/speed_estimation.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/trackers/basetrack.py` & `ultralytics-8.2.5/ultralytics/trackers/basetrack.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/trackers/bot_sort.py` & `ultralytics-8.2.5/ultralytics/trackers/bot_sort.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/trackers/byte_tracker.py` & `ultralytics-8.2.5/ultralytics/trackers/byte_tracker.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/trackers/track.py` & `ultralytics-8.2.5/ultralytics/trackers/track.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/trackers/utils/gmc.py` & `ultralytics-8.2.5/ultralytics/trackers/utils/gmc.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/trackers/utils/kalman_filter.py` & `ultralytics-8.2.5/ultralytics/trackers/utils/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/trackers/utils/matching.py` & `ultralytics-8.2.5/ultralytics/trackers/utils/matching.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/utils/__init__.py` & `ultralytics-8.2.5/ultralytics/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/utils/autobatch.py` & `ultralytics-8.2.5/ultralytics/utils/autobatch.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/utils/benchmarks.py` & `ultralytics-8.2.5/ultralytics/utils/benchmarks.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/utils/callbacks/base.py` & `ultralytics-8.2.5/ultralytics/utils/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/utils/callbacks/clearml.py` & `ultralytics-8.2.5/ultralytics/utils/callbacks/clearml.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/utils/callbacks/comet.py` & `ultralytics-8.2.5/ultralytics/utils/callbacks/comet.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/utils/callbacks/dvc.py` & `ultralytics-8.2.5/ultralytics/utils/callbacks/dvc.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/utils/callbacks/hub.py` & `ultralytics-8.2.5/ultralytics/utils/callbacks/hub.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/utils/callbacks/mlflow.py` & `ultralytics-8.2.5/ultralytics/utils/callbacks/mlflow.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/utils/callbacks/neptune.py` & `ultralytics-8.2.5/ultralytics/utils/callbacks/neptune.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/utils/callbacks/raytune.py` & `ultralytics-8.2.5/ultralytics/utils/callbacks/raytune.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/utils/callbacks/tensorboard.py` & `ultralytics-8.2.5/ultralytics/utils/callbacks/tensorboard.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/utils/callbacks/wb.py` & `ultralytics-8.2.5/ultralytics/utils/callbacks/wb.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/utils/checks.py` & `ultralytics-8.2.5/ultralytics/utils/checks.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/utils/dist.py` & `ultralytics-8.2.5/ultralytics/utils/dist.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/utils/downloads.py` & `ultralytics-8.2.5/ultralytics/utils/downloads.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/utils/errors.py` & `ultralytics-8.2.5/ultralytics/utils/errors.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/utils/files.py` & `ultralytics-8.2.5/ultralytics/utils/files.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/utils/instance.py` & `ultralytics-8.2.5/ultralytics/utils/instance.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/utils/loss.py` & `ultralytics-8.2.5/ultralytics/utils/loss.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/utils/metrics.py` & `ultralytics-8.2.5/ultralytics/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/utils/ops.py` & `ultralytics-8.2.5/ultralytics/utils/ops.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/utils/patches.py` & `ultralytics-8.2.5/ultralytics/utils/patches.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/utils/plotting.py` & `ultralytics-8.2.5/ultralytics/utils/plotting.py`

 * *Files 5% similar despite different names*

```diff
@@ -415,59 +415,71 @@
             0,
             fontScale=fontsize,
             color=txt_color,
             thickness=self.tf,
             lineType=cv2.LINE_AA,
         )
 
-    def display_counts(self, counts=None, count_bg_color=(0, 0, 0), count_txt_color=(255, 255, 255)):
+    ### Parking management utils
+    def display_objects_labels(self, im0, text, txt_color, bg_color, x_center, y_center, margin):
         """
-        Display counts on im0 with text background and border.
+        Display the bounding boxes labels in parking management app.
 
         Args:
-            counts (str): objects count data
-            count_bg_color (RGB Color): counts highlighter color
-            count_txt_color (RGB Color): counts display color
+            im0 (ndarray): inference image
+            text (str): object/class name
+            txt_color (bgr color): display color for text foreground
+            bg_color (bgr color): display color for text background
+            x_center (float): x position center point for bounding box
+            y_center (float): y position center point for bounding box
+            margin (int): gap between text and rectangle for better display
         """
 
-        tl = self.tf or round(0.002 * (self.im.shape[0] + self.im.shape[1]) / 2) + 1
-        tf = max(tl - 1, 1)
+        text_size = cv2.getTextSize(text, 0, fontScale=self.sf, thickness=self.tf)[0]
+        text_x = x_center - text_size[0] // 2
+        text_y = y_center + text_size[1] // 2
+
+        rect_x1 = text_x - margin
+        rect_y1 = text_y - text_size[1] - margin
+        rect_x2 = text_x + text_size[0] + margin
+        rect_y2 = text_y + margin
+        cv2.rectangle(im0, (rect_x1, rect_y1), (rect_x2, rect_y2), bg_color, -1)
+        cv2.putText(im0, text, (text_x, text_y), 0, self.sf, txt_color, self.tf, lineType=cv2.LINE_AA)
 
-        t_sizes = [cv2.getTextSize(str(count), 0, fontScale=self.sf, thickness=self.tf)[0] for count in counts]
+    # Parking lot and object counting app
+    def display_analytics(self, im0, text, txt_color, bg_color, margin):
+        """
+        Display the overall statistics for parking lots
+        Args:
+            im0 (ndarray): inference image
+            text (dict): labels dictionary
+            txt_color (bgr color): display color for text foreground
+            bg_color (bgr color): display color for text background
+            margin (int): gap between text and rectangle for better display
+        """
 
-        max_text_width = max([size[0] for size in t_sizes])
-        max_text_height = max([size[1] for size in t_sizes])
+        horizontal_gap = int(im0.shape[1] * 0.02)
+        vertical_gap = int(im0.shape[0] * 0.01)
 
-        text_x = self.im.shape[1] - int(self.im.shape[1] * 0.025 + max_text_width)
-        text_y = int(self.im.shape[0] * 0.025)
-
-        for i, count in enumerate(counts):
-            text_x_pos = text_x
-            text_y_pos = text_y + i * (max_text_height + 25 * tf)
-
-            # Draw the border
-            cv2.rectangle(
-                self.im,
-                (text_x_pos - (10 * tf), text_y_pos - (10 * tf)),
-                (text_x_pos + max_text_width + (10 * tf), text_y_pos + max_text_height + (10 * tf)),
-                count_bg_color,
-                -1,
-            )
+        text_y_offset = 0
 
-            # Draw the count text
+        for label, value in text.items():
+            txt = f"{label}: {value}"
+            text_size = cv2.getTextSize(txt, 0, int(self.sf * 1.5), int(self.tf * 1.5))[0]
+            text_x = im0.shape[1] - text_size[0] - margin * 2 - horizontal_gap
+            text_y = text_y_offset + text_size[1] + margin * 2 + vertical_gap
+            rect_x1 = text_x - margin * 2
+            rect_y1 = text_y - text_size[1] - margin * 2
+            rect_x2 = text_x + text_size[0] + margin * 2
+            rect_y2 = text_y + margin * 2
+            cv2.rectangle(im0, (rect_x1, rect_y1), (rect_x2, rect_y2), bg_color, -1)
             cv2.putText(
-                self.im,
-                str(count),
-                (text_x_pos, text_y_pos + max_text_height),
-                0,
-                fontScale=self.sf,
-                color=count_txt_color,
-                thickness=self.tf,
-                lineType=cv2.LINE_AA,
+                im0, txt, (text_x, text_y), 0, int(self.sf * 1.5), txt_color, int(self.tf * 1.5), lineType=cv2.LINE_AA
             )
+            text_y_offset = rect_y2
 
     @staticmethod
     def estimate_pose_angle(a, b, c):
         """
         Calculate the pose angle for object.
 
         Args:
```

### Comparing `ultralytics-8.2.4/ultralytics/utils/tal.py` & `ultralytics-8.2.5/ultralytics/utils/tal.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/utils/torch_utils.py` & `ultralytics-8.2.5/ultralytics/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/utils/triton.py` & `ultralytics-8.2.5/ultralytics/utils/triton.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics/utils/tuner.py` & `ultralytics-8.2.5/ultralytics/utils/tuner.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.4/ultralytics.egg-info/PKG-INFO` & `ultralytics-8.2.5/ultralytics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultralytics
-Version: 8.2.4
+Version: 8.2.5
 Summary: Ultralytics YOLOv8 for SOTA object detection, multi-object tracking, instance segmentation, pose estimation and image classification.
 Author: Glenn Jocher, Ayush Chaurasia, Jing Qiu
 Maintainer: Glenn Jocher, Ayush Chaurasia, Jing Qiu
 License: AGPL-3.0
 Project-URL: Bug Reports, https://github.com/ultralytics/ultralytics/issues
 Project-URL: Funding, https://ultralytics.com
 Project-URL: Source, https://github.com/ultralytics/ultralytics/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ultralytics Version: 8.2.4 Summary: Ultralytics
+Metadata-Version: 2.1 Name: ultralytics Version: 8.2.5 Summary: Ultralytics
 YOLOv8 for SOTA object detection, multi-object tracking, instance segmentation,
 pose estimation and image classification. Author: Glenn Jocher, Ayush
 Chaurasia, Jing Qiu Maintainer: Glenn Jocher, Ayush Chaurasia, Jing Qiu
 License: AGPL-3.0 Project-URL: Bug Reports, https://github.com/ultralytics/
 ultralytics/issues Project-URL: Funding, https://ultralytics.com Project-URL:
 Source, https://github.com/ultralytics/ultralytics/ Keywords: machine-
 learning,deep-learning,computer-
```

### Comparing `ultralytics-8.2.4/ultralytics.egg-info/SOURCES.txt` & `ultralytics-8.2.5/ultralytics.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -169,14 +169,15 @@
 ultralytics/nn/modules/transformer.py
 ultralytics/nn/modules/utils.py
 ultralytics/solutions/__init__.py
 ultralytics/solutions/ai_gym.py
 ultralytics/solutions/distance_calculation.py
 ultralytics/solutions/heatmap.py
 ultralytics/solutions/object_counter.py
+ultralytics/solutions/parking_management.py
 ultralytics/solutions/queue_management.py
 ultralytics/solutions/speed_estimation.py
 ultralytics/trackers/__init__.py
 ultralytics/trackers/basetrack.py
 ultralytics/trackers/bot_sort.py
 ultralytics/trackers/byte_tracker.py
 ultralytics/trackers/track.py
```

### Comparing `ultralytics-8.2.4/ultralytics.egg-info/requires.txt` & `ultralytics-8.2.5/ultralytics.egg-info/requires.txt`

 * *Files identical despite different names*

