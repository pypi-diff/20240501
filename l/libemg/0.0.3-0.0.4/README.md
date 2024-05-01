# Comparing `tmp/libemg-0.0.3.tar.gz` & `tmp/libemg-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/libemg-0.0.3.tar", last modified: Mon Feb  5 18:56:10 2024, max compression
+gzip compressed data, was "libemg-0.0.4.tar", last modified: Wed May  1 11:25:14 2024, max compression
```

## Comparing `libemg-0.0.3.tar` & `libemg-0.0.4.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxr-xr-x   0 ethaneddy   (501) staff       (20)        0 2024-02-05 18:56:10.000000 libemg-0.0.3/
--rw-r--r--   0 ethaneddy   (501) staff       (20)     1951 2024-02-05 18:56:10.000000 libemg-0.0.3/PKG-INFO
-drwxr-xr-x   0 ethaneddy   (501) staff       (20)        0 2024-02-05 18:56:10.000000 libemg-0.0.3/libemg.egg-info/
--rw-r--r--   0 ethaneddy   (501) staff       (20)     1951 2024-02-05 18:56:10.000000 libemg-0.0.3/libemg.egg-info/PKG-INFO
--rw-r--r--   0 ethaneddy   (501) staff       (20)     3151 2024-02-05 18:56:10.000000 libemg-0.0.3/libemg.egg-info/SOURCES.txt
--rw-r--r--   0 ethaneddy   (501) staff       (20)       76 2024-02-05 18:56:10.000000 libemg-0.0.3/libemg.egg-info/requires.txt
--rw-r--r--   0 ethaneddy   (501) staff       (20)        7 2024-02-05 18:56:10.000000 libemg-0.0.3/libemg.egg-info/top_level.txt
--rw-r--r--   0 ethaneddy   (501) staff       (20)        1 2024-02-05 18:56:10.000000 libemg-0.0.3/libemg.egg-info/dependency_links.txt
--rw-r--r--   0 ethaneddy   (501) staff       (20)     1201 2023-08-08 16:27:23.000000 libemg-0.0.3/LICENSE
--rw-r--r--   0 ethaneddy   (501) staff       (20)      335 2024-02-05 18:55:40.000000 libemg-0.0.3/requirements.txt
-drwxr-xr-x   0 ethaneddy   (501) staff       (20)        0 2024-02-05 18:56:10.000000 libemg-0.0.3/libemg/
--rw-r--r--   0 ethaneddy   (501) staff       (20)    28265 2024-02-05 18:55:40.000000 libemg-0.0.3/libemg/data_handler.py
--rw-r--r--   0 ethaneddy   (501) staff       (20)    30005 2023-08-08 16:27:23.000000 libemg-0.0.3/libemg/feature_selector.py
--rw-r--r--   0 ethaneddy   (501) staff       (20)    12312 2023-08-08 16:27:23.000000 libemg-0.0.3/libemg/offline_metrics.py
--rw-r--r--   0 ethaneddy   (501) staff       (20)    13822 2023-08-08 16:27:23.000000 libemg-0.0.3/libemg/filtering.py
--rw-r--r--   0 ethaneddy   (501) staff       (20)    18886 2024-01-16 13:05:46.000000 libemg-0.0.3/libemg/screen_guided_training.py
--rw-r--r--   0 ethaneddy   (501) staff       (20)    29317 2024-02-05 18:55:40.000000 libemg-0.0.3/libemg/emg_classifier.py
--rw-r--r--   0 ethaneddy   (501) staff       (20)    18538 2023-08-12 13:31:23.000000 libemg-0.0.3/libemg/datasets.py
--rw-r--r--   0 ethaneddy   (501) staff       (20)      326 2023-08-08 16:27:23.000000 libemg-0.0.3/libemg/__init__.py
--rw-r--r--   0 ethaneddy   (501) staff       (20)    12461 2024-02-05 18:55:40.000000 libemg-0.0.3/libemg/streamers.py
--rw-r--r--   0 ethaneddy   (501) staff       (20)     2504 2024-01-16 13:05:46.000000 libemg-0.0.3/libemg/utils.py
--rw-r--r--   0 ethaneddy   (501) staff       (20)    72973 2024-01-26 14:48:56.000000 libemg-0.0.3/libemg/feature_extractor.py
-drwxr-xr-x   0 ethaneddy   (501) staff       (20)        0 2024-02-05 18:56:10.000000 libemg-0.0.3/libemg/_streamers/
--rw-r--r--   0 ethaneddy   (501) staff       (20)    18031 2024-01-16 13:05:46.000000 libemg-0.0.3/libemg/_streamers/_myo_streamer.py
--rw-r--r--   0 ethaneddy   (501) staff       (20)     4307 2023-08-08 16:27:23.000000 libemg-0.0.3/libemg/_streamers/_delsys_streamer.py
--rw-r--r--   0 ethaneddy   (501) staff       (20)    13282 2024-02-05 18:55:40.000000 libemg-0.0.3/libemg/_streamers/_OTB_Syncstation.py
--rw-r--r--   0 ethaneddy   (501) staff       (20)    17850 2024-02-05 18:55:40.000000 libemg-0.0.3/libemg/_streamers/_oymotion_windows_streamer.py
--rw-r--r--   0 ethaneddy   (501) staff       (20)      480 2024-02-05 18:55:40.000000 libemg-0.0.3/libemg/_streamers/__init__.py
--rw-r--r--   0 ethaneddy   (501) staff       (20)     3073 2023-08-08 16:27:23.000000 libemg-0.0.3/libemg/_streamers/_sifi_streamer.py
--rw-r--r--   0 ethaneddy   (501) staff       (20)     7870 2024-01-16 13:05:46.000000 libemg-0.0.3/libemg/_streamers/_sifi_bridge_streamer.py
--rw-r--r--   0 ethaneddy   (501) staff       (20)     3709 2023-08-08 16:27:23.000000 libemg-0.0.3/libemg/_streamers/_emager_streamer.py
--rw-r--r--   0 ethaneddy   (501) staff       (20)     8303 2024-02-05 18:55:40.000000 libemg-0.0.3/libemg/_streamers/_OTB_MuoviPlus.py
--rw-r--r--   0 ethaneddy   (501) staff       (20)    25110 2024-01-26 14:48:56.000000 libemg-0.0.3/libemg/_streamers/_oymotion_streamer.py
--rw-r--r--   0 ethaneddy   (501) staff       (20)     8287 2024-02-05 18:55:40.000000 libemg-0.0.3/libemg/_streamers/_OTB_Muovi.py
--rw-r--r--   0 ethaneddy   (501) staff       (20)     9576 2024-02-05 18:55:40.000000 libemg-0.0.3/libemg/_streamers/_OTB_SessantaquattroPlus.py
--rw-r--r--   0 ethaneddy   (501) staff       (20)     1589 2024-01-16 13:05:46.000000 libemg-0.0.3/libemg/raw_data.py
-drwxr-xr-x   0 ethaneddy   (501) staff       (20)        0 2024-02-05 18:56:10.000000 libemg-0.0.3/tests/
--rw-r--r--   0 ethaneddy   (501) staff       (20)     5972 2024-01-26 14:48:56.000000 libemg-0.0.3/tests/test_feature_extractor.py
--rw-r--r--   0 ethaneddy   (501) staff       (20)     2607 2023-08-08 17:15:49.000000 libemg-0.0.3/tests/test_stream_architecture.py
--rw-r--r--   0 ethaneddy   (501) staff       (20)        0 2023-08-08 17:15:49.000000 libemg-0.0.3/tests/__init__.py
-drwxr-xr-x   0 ethaneddy   (501) staff       (20)        0 2024-02-05 18:56:10.000000 libemg-0.0.3/tests/feature_tests/
--rw-r--r--   0 ethaneddy   (501) staff       (20)      868 2023-08-08 17:15:49.000000 libemg-0.0.3/tests/feature_tests/test_mav_feature.py
--rw-r--r--   0 ethaneddy   (501) staff       (20)      810 2023-08-08 17:15:49.000000 libemg-0.0.3/tests/feature_tests/test_zc_feature.py
--rw-r--r--   0 ethaneddy   (501) staff       (20)     2120 2023-08-08 17:15:49.000000 libemg-0.0.3/tests/test_offline_metrics.py
--rw-r--r--   0 ethaneddy   (501) staff       (20)     2482 2024-01-22 15:52:05.000000 libemg-0.0.3/tests/test_feature_verification.py
--rw-r--r--   0 ethaneddy   (501) staff       (20)     2872 2023-08-08 17:15:49.000000 libemg-0.0.3/tests/test_online_classifier.py
--rw-r--r--   0 ethaneddy   (501) staff       (20)     1282 2024-01-22 15:51:47.000000 libemg-0.0.3/tests/get_feature_values.m
-drwxr-xr-x   0 ethaneddy   (501) staff       (20)        0 2024-02-05 18:56:10.000000 libemg-0.0.3/tests/data/
--rw-r--r--   0 ethaneddy   (501) staff       (20)      816 2023-08-08 17:15:49.000000 libemg-0.0.3/tests/data/matlab_MNP.csv
--rw-r--r--   0 ethaneddy   (501) staff       (20)    11479 2023-08-08 17:15:49.000000 libemg-0.0.3/tests/data/emg_data_myo.csv
--rw-r--r--   0 ethaneddy   (501) staff       (20)      718 2023-08-08 17:15:49.000000 libemg-0.0.3/tests/data/matlab_MNF.csv
--rw-r--r--   0 ethaneddy   (501) staff       (20)      715 2023-08-08 17:15:49.000000 libemg-0.0.3/tests/data/matlab_DASDV.csv
--rw-r--r--   0 ethaneddy   (501) staff       (20)     3775 2023-08-08 17:15:49.000000 libemg-0.0.3/tests/data/test_labels
--rw-r--r--   0 ethaneddy   (501) staff       (20)     1128 2023-08-08 17:15:49.000000 libemg-0.0.3/tests/data/matlab_SM.csv
--rw-r--r--   0 ethaneddy   (501) staff       (20)     8690 2023-08-08 17:15:49.000000 libemg-0.0.3/tests/data/emg_data_zeros.csv
--rw-r--r--   0 ethaneddy   (501) staff       (20)      712 2023-08-08 17:15:49.000000 libemg-0.0.3/tests/data/matlab_MZP.csv
--rw-r--r--   0 ethaneddy   (501) staff       (20)      701 2023-08-08 17:15:49.000000 libemg-0.0.3/tests/data/matlab_TM.csv
--rw-r--r--   0 ethaneddy   (501) staff       (20)      416 2023-08-08 17:15:49.000000 libemg-0.0.3/tests/data/matlab_WAMP.csv
--rw-r--r--   0 ethaneddy   (501) staff       (20)      726 2023-08-08 17:15:49.000000 libemg-0.0.3/tests/data/matlab_MDF.csv
--rw-r--r--   0 ethaneddy   (501) staff       (20)      717 2023-08-08 17:15:49.000000 libemg-0.0.3/tests/data/matlab_MFL.csv
--rw-r--r--   0 ethaneddy   (501) staff       (20)      578 2023-08-08 17:15:49.000000 libemg-0.0.3/tests/data/matlab_MAVSLP.csv
--rw-r--r--   0 ethaneddy   (501) staff       (20)     5757 2023-08-08 17:15:49.000000 libemg-0.0.3/tests/data/matlab_RMSPHASOR.csv
--rw-r--r--   0 ethaneddy   (501) staff       (20)      876 2023-08-08 17:15:49.000000 libemg-0.0.3/tests/data/matlab_SKEW.csv
--rw-r--r--   0 ethaneddy   (501) staff       (20)      727 2023-08-08 17:15:49.000000 libemg-0.0.3/tests/data/matlab_FUZZYEN.csv
--rw-r--r--   0 ethaneddy   (501) staff       (20)     3824 2023-08-08 17:15:49.000000 libemg-0.0.3/tests/data/matlab_CC.csv
--rw-r--r--   0 ethaneddy   (501) staff       (20)     5755 2023-08-08 17:15:49.000000 libemg-0.0.3/tests/data/matlab_WLPHASOR.csv
--rw-r--r--   0 ethaneddy   (501) staff       (20)      372 2023-08-08 17:15:49.000000 libemg-0.0.3/tests/data/matlab_ZC.csv
--rw-r--r--   0 ethaneddy   (501) staff       (20)      312 2023-08-08 17:15:49.000000 libemg-0.0.3/tests/data/matlab_MPK.csv
--rw-r--r--   0 ethaneddy   (501) staff       (20)      875 2023-08-08 17:15:49.000000 libemg-0.0.3/tests/data/matlab_M0.csv
--rw-r--r--   0 ethaneddy   (501) staff       (20)     3665 2023-08-08 17:15:49.000000 libemg-0.0.3/tests/data/matlab_AR.csv
--rw-r--r--   0 ethaneddy   (501) staff       (20)      906 2023-08-08 17:15:49.000000 libemg-0.0.3/tests/data/matlab_IRF.csv
--rw-r--r--   0 ethaneddy   (501) staff       (20)      922 2023-08-08 17:15:49.000000 libemg-0.0.3/tests/data/matlab_WLF.csv
--rw-r--r--   0 ethaneddy   (501) staff       (20)      717 2023-08-08 17:15:49.000000 libemg-0.0.3/tests/data/matlab_MAVFD.csv
--rw-r--r--   0 ethaneddy   (501) staff       (20)      921 2023-08-08 17:15:49.000000 libemg-0.0.3/tests/data/matlab_M2.csv
--rw-r--r--   0 ethaneddy   (501) staff       (20)      718 2023-08-08 17:15:49.000000 libemg-0.0.3/tests/data/matlab_MSR.csv
--rw-r--r--   0 ethaneddy   (501) staff       (20)      709 2023-08-08 17:15:49.000000 libemg-0.0.3/tests/data/matlab_LD.csv
--rw-r--r--   0 ethaneddy   (501) staff       (20)      714 2023-08-08 17:15:49.000000 libemg-0.0.3/tests/data/matlab_LS.csv
--rw-r--r--   0 ethaneddy   (501) staff       (20)   183694 2023-08-08 17:15:49.000000 libemg-0.0.3/tests/data/stream_data_tester.csv
--rw-r--r--   0 ethaneddy   (501) staff       (20)      496 2023-08-08 17:15:49.000000 libemg-0.0.3/tests/data/matlab_WL.csv
--rw-r--r--   0 ethaneddy   (501) staff       (20)      925 2023-08-08 17:15:49.000000 libemg-0.0.3/tests/data/matlab_M4.csv
-drwxr-xr-x   0 ethaneddy   (501) staff       (20)        0 2024-02-05 18:56:10.000000 libemg-0.0.3/tests/data/myo_dataset/
--rw-r--r--   0 ethaneddy   (501) staff       (20)    13896 2023-08-08 17:15:49.000000 libemg-0.0.3/tests/data/myo_dataset/R_0_C_3_EMG.csv
--rw-r--r--   0 ethaneddy   (501) staff       (20)    13514 2023-08-08 17:15:49.000000 libemg-0.0.3/tests/data/myo_dataset/R_3_C_1_EMG.csv
--rw-r--r--   0 ethaneddy   (501) staff       (20)    13471 2023-08-08 17:15:49.000000 libemg-0.0.3/tests/data/myo_dataset/R_3_C_0_EMG.csv
--rw-r--r--   0 ethaneddy   (501) staff       (20)    13588 2023-08-08 17:15:49.000000 libemg-0.0.3/tests/data/myo_dataset/R_1_C_4_EMG.csv
--rw-r--r--   0 ethaneddy   (501) staff       (20)    13088 2023-08-08 17:15:49.000000 libemg-0.0.3/tests/data/myo_dataset/R_0_C_2_EMG.csv
--rw-r--r--   0 ethaneddy   (501) staff       (20)    13016 2023-08-08 17:15:49.000000 libemg-0.0.3/tests/data/myo_dataset/R_3_C_2_EMG.csv
--rw-r--r--   0 ethaneddy   (501) staff       (20)    13712 2023-08-08 17:15:49.000000 libemg-0.0.3/tests/data/myo_dataset/R_2_C_4_EMG.csv
--rw-r--r--   0 ethaneddy   (501) staff       (20)    13783 2023-08-08 17:15:49.000000 libemg-0.0.3/tests/data/myo_dataset/R_0_C_0_EMG.csv
--rw-r--r--   0 ethaneddy   (501) staff       (20)    13490 2023-08-08 17:15:49.000000 libemg-0.0.3/tests/data/myo_dataset/R_0_C_1_EMG.csv
--rw-r--r--   0 ethaneddy   (501) staff       (20)    14121 2023-08-08 17:15:49.000000 libemg-0.0.3/tests/data/myo_dataset/R_3_C_3_EMG.csv
--rw-r--r--   0 ethaneddy   (501) staff       (20)    13170 2023-08-08 17:15:49.000000 libemg-0.0.3/tests/data/myo_dataset/R_1_C_2_EMG.csv
--rw-r--r--   0 ethaneddy   (501) staff       (20)    13562 2023-08-08 17:15:49.000000 libemg-0.0.3/tests/data/myo_dataset/R_0_C_4_EMG.csv
--rw-r--r--   0 ethaneddy   (501) staff       (20)    13585 2023-08-08 17:15:49.000000 libemg-0.0.3/tests/data/myo_dataset/R_2_C_0_EMG.csv
--rw-r--r--   0 ethaneddy   (501) staff       (20)    13923 2023-08-08 17:15:49.000000 libemg-0.0.3/tests/data/myo_dataset/R_2_C_1_EMG.csv
--rw-r--r--   0 ethaneddy   (501) staff       (20)    13900 2023-08-08 17:15:49.000000 libemg-0.0.3/tests/data/myo_dataset/R_1_C_3_EMG.csv
--rw-r--r--   0 ethaneddy   (501) staff       (20)    14084 2023-08-08 17:15:49.000000 libemg-0.0.3/tests/data/myo_dataset/R_2_C_3_EMG.csv
--rw-r--r--   0 ethaneddy   (501) staff       (20)    13977 2023-08-08 17:15:49.000000 libemg-0.0.3/tests/data/myo_dataset/R_1_C_1_EMG.csv
--rw-r--r--   0 ethaneddy   (501) staff       (20)    13643 2023-08-08 17:15:49.000000 libemg-0.0.3/tests/data/myo_dataset/R_1_C_0_EMG.csv
--rw-r--r--   0 ethaneddy   (501) staff       (20)    13254 2023-08-08 17:15:49.000000 libemg-0.0.3/tests/data/myo_dataset/R_3_C_4_EMG.csv
--rw-r--r--   0 ethaneddy   (501) staff       (20)    13187 2023-08-08 17:15:49.000000 libemg-0.0.3/tests/data/myo_dataset/R_2_C_2_EMG.csv
--rw-r--r--   0 ethaneddy   (501) staff       (20)      580 2023-08-08 17:15:49.000000 libemg-0.0.3/tests/data/matlab_MAV.csv
--rw-r--r--   0 ethaneddy   (501) staff       (20)      717 2023-08-08 17:15:49.000000 libemg-0.0.3/tests/data/matlab_PAP.csv
--rw-r--r--   0 ethaneddy   (501) staff       (20)      416 2023-08-08 17:15:49.000000 libemg-0.0.3/tests/data/matlab_SSC.csv
--rw-r--r--   0 ethaneddy   (501) staff       (20)      720 2023-08-08 17:15:49.000000 libemg-0.0.3/tests/data/matlab_RMS.csv
--rw-r--r--   0 ethaneddy   (501) staff       (20)      713 2023-08-08 17:15:49.000000 libemg-0.0.3/tests/data/matlab_KURT.csv
--rw-r--r--   0 ethaneddy   (501) staff       (20)     1951 2023-08-08 17:15:49.000000 libemg-0.0.3/tests/data/predictions
--rw-r--r--   0 ethaneddy   (501) staff       (20)      755 2023-08-08 17:15:49.000000 libemg-0.0.3/tests/data/matlab_SAMPEN.csv
--rw-r--r--   0 ethaneddy   (501) staff       (20)      490 2023-08-08 17:15:49.000000 libemg-0.0.3/tests/data/matlab_IAV.csv
--rw-r--r--   0 ethaneddy   (501) staff       (20)      686 2023-08-08 17:15:49.000000 libemg-0.0.3/tests/data/matlab_VAR.csv
--rw-r--r--   0 ethaneddy   (501) staff       (20)      918 2023-08-08 17:15:49.000000 libemg-0.0.3/tests/data/matlab_SPARSI.csv
--rw-r--r--   0 ethaneddy   (501) staff       (20)     1058 2024-02-05 18:55:40.000000 libemg-0.0.3/README.md
--rw-r--r--   0 ethaneddy   (501) staff       (20)     1852 2024-02-05 18:55:40.000000 libemg-0.0.3/setup.py
--rw-r--r--   0 ethaneddy   (501) staff       (20)      575 2024-01-16 13:05:46.000000 libemg-0.0.3/.gitignore
-drwxr-xr-x   0 ethaneddy   (501) staff       (20)        0 2024-02-05 18:56:10.000000 libemg-0.0.3/.github/
-drwxr-xr-x   0 ethaneddy   (501) staff       (20)        0 2024-02-05 18:56:10.000000 libemg-0.0.3/.github/workflows/
--rw-r--r--   0 ethaneddy   (501) staff       (20)      842 2024-02-05 17:48:06.000000 libemg-0.0.3/.github/workflows/ci.yaml
--rw-r--r--   0 ethaneddy   (501) staff       (20)       38 2024-02-05 18:56:10.000000 libemg-0.0.3/setup.cfg
+drwxr-xr-x   0 ethaneddy   (501) staff       (20)        0 2024-05-01 11:25:14.855158 libemg-0.0.4/
+drwxr-xr-x   0 ethaneddy   (501) staff       (20)        0 2024-05-01 11:25:14.827831 libemg-0.0.4/.github/
+drwxr-xr-x   0 ethaneddy   (501) staff       (20)        0 2024-05-01 11:25:14.830405 libemg-0.0.4/.github/workflows/
+-rw-r--r--   0 ethaneddy   (501) staff       (20)      842 2024-02-05 17:48:06.000000 libemg-0.0.4/.github/workflows/ci.yaml
+-rw-r--r--   0 ethaneddy   (501) staff       (20)      575 2024-04-30 23:24:17.000000 libemg-0.0.4/.gitignore
+-rw-r--r--   0 ethaneddy   (501) staff       (20)     1201 2023-08-08 16:27:23.000000 libemg-0.0.4/LICENSE
+-rw-r--r--   0 ethaneddy   (501) staff       (20)     1877 2024-05-01 11:25:14.854749 libemg-0.0.4/PKG-INFO
+-rw-r--r--   0 ethaneddy   (501) staff       (20)     1058 2024-04-30 23:24:17.000000 libemg-0.0.4/README.md
+drwxr-xr-x   0 ethaneddy   (501) staff       (20)        0 2024-05-01 11:25:14.833345 libemg-0.0.4/libemg/
+-rw-r--r--   0 ethaneddy   (501) staff       (20)      326 2024-04-30 23:24:17.000000 libemg-0.0.4/libemg/__init__.py
+drwxr-xr-x   0 ethaneddy   (501) staff       (20)        0 2024-05-01 11:25:14.837985 libemg-0.0.4/libemg/_streamers/
+-rw-r--r--   0 ethaneddy   (501) staff       (20)     8287 2024-04-30 23:24:17.000000 libemg-0.0.4/libemg/_streamers/_OTB_Muovi.py
+-rw-r--r--   0 ethaneddy   (501) staff       (20)     8303 2024-04-30 23:24:17.000000 libemg-0.0.4/libemg/_streamers/_OTB_MuoviPlus.py
+-rw-r--r--   0 ethaneddy   (501) staff       (20)     9576 2024-04-30 23:24:17.000000 libemg-0.0.4/libemg/_streamers/_OTB_SessantaquattroPlus.py
+-rw-r--r--   0 ethaneddy   (501) staff       (20)    13282 2024-04-30 23:24:17.000000 libemg-0.0.4/libemg/_streamers/_OTB_Syncstation.py
+-rw-r--r--   0 ethaneddy   (501) staff       (20)      480 2024-04-30 23:24:17.000000 libemg-0.0.4/libemg/_streamers/__init__.py
+-rw-r--r--   0 ethaneddy   (501) staff       (20)     4307 2023-08-08 16:27:23.000000 libemg-0.0.4/libemg/_streamers/_delsys_streamer.py
+-rw-r--r--   0 ethaneddy   (501) staff       (20)     3709 2024-04-30 23:24:17.000000 libemg-0.0.4/libemg/_streamers/_emager_streamer.py
+-rw-r--r--   0 ethaneddy   (501) staff       (20)    18031 2024-04-30 23:24:17.000000 libemg-0.0.4/libemg/_streamers/_myo_streamer.py
+-rw-r--r--   0 ethaneddy   (501) staff       (20)    25110 2024-04-30 23:24:17.000000 libemg-0.0.4/libemg/_streamers/_oymotion_streamer.py
+-rw-r--r--   0 ethaneddy   (501) staff       (20)    17850 2024-04-30 23:24:17.000000 libemg-0.0.4/libemg/_streamers/_oymotion_windows_streamer.py
+-rw-r--r--   0 ethaneddy   (501) staff       (20)     7870 2024-04-30 23:24:17.000000 libemg-0.0.4/libemg/_streamers/_sifi_bridge_streamer.py
+-rw-r--r--   0 ethaneddy   (501) staff       (20)     3073 2024-04-30 23:24:17.000000 libemg-0.0.4/libemg/_streamers/_sifi_streamer.py
+-rw-r--r--   0 ethaneddy   (501) staff       (20)    28503 2024-05-01 11:23:55.000000 libemg-0.0.4/libemg/data_handler.py
+-rw-r--r--   0 ethaneddy   (501) staff       (20)    18538 2024-03-26 17:23:51.000000 libemg-0.0.4/libemg/datasets.py
+-rw-r--r--   0 ethaneddy   (501) staff       (20)    29317 2024-04-30 23:24:17.000000 libemg-0.0.4/libemg/emg_classifier.py
+-rw-r--r--   0 ethaneddy   (501) staff       (20)    72973 2024-04-30 23:24:17.000000 libemg-0.0.4/libemg/feature_extractor.py
+-rw-r--r--   0 ethaneddy   (501) staff       (20)    30005 2023-08-08 16:27:23.000000 libemg-0.0.4/libemg/feature_selector.py
+-rw-r--r--   0 ethaneddy   (501) staff       (20)    13822 2023-08-08 16:27:23.000000 libemg-0.0.4/libemg/filtering.py
+-rw-r--r--   0 ethaneddy   (501) staff       (20)    12312 2023-08-08 16:27:23.000000 libemg-0.0.4/libemg/offline_metrics.py
+-rw-r--r--   0 ethaneddy   (501) staff       (20)     1589 2024-04-30 23:24:17.000000 libemg-0.0.4/libemg/raw_data.py
+-rw-r--r--   0 ethaneddy   (501) staff       (20)    18886 2024-04-30 23:24:17.000000 libemg-0.0.4/libemg/screen_guided_training.py
+-rw-r--r--   0 ethaneddy   (501) staff       (20)    12507 2024-05-01 11:23:55.000000 libemg-0.0.4/libemg/streamers.py
+-rw-r--r--   0 ethaneddy   (501) staff       (20)     2504 2024-04-30 23:24:17.000000 libemg-0.0.4/libemg/utils.py
+drwxr-xr-x   0 ethaneddy   (501) staff       (20)        0 2024-05-01 11:25:14.854245 libemg-0.0.4/libemg.egg-info/
+-rw-r--r--   0 ethaneddy   (501) staff       (20)     1877 2024-05-01 11:25:14.000000 libemg-0.0.4/libemg.egg-info/PKG-INFO
+-rw-r--r--   0 ethaneddy   (501) staff       (20)     3151 2024-05-01 11:25:14.000000 libemg-0.0.4/libemg.egg-info/SOURCES.txt
+-rw-r--r--   0 ethaneddy   (501) staff       (20)        1 2024-05-01 11:25:14.000000 libemg-0.0.4/libemg.egg-info/dependency_links.txt
+-rw-r--r--   0 ethaneddy   (501) staff       (20)       76 2024-05-01 11:25:14.000000 libemg-0.0.4/libemg.egg-info/requires.txt
+-rw-r--r--   0 ethaneddy   (501) staff       (20)        7 2024-05-01 11:25:14.000000 libemg-0.0.4/libemg.egg-info/top_level.txt
+-rw-r--r--   0 ethaneddy   (501) staff       (20)      335 2024-04-30 23:24:17.000000 libemg-0.0.4/requirements.txt
+-rw-r--r--   0 ethaneddy   (501) staff       (20)       38 2024-05-01 11:25:14.855230 libemg-0.0.4/setup.cfg
+-rw-r--r--   0 ethaneddy   (501) staff       (20)     1852 2024-05-01 11:24:43.000000 libemg-0.0.4/setup.py
+drwxr-xr-x   0 ethaneddy   (501) staff       (20)        0 2024-05-01 11:25:14.839534 libemg-0.0.4/tests/
+-rw-r--r--   0 ethaneddy   (501) staff       (20)        0 2023-08-08 17:15:49.000000 libemg-0.0.4/tests/__init__.py
+drwxr-xr-x   0 ethaneddy   (501) staff       (20)        0 2024-05-01 11:25:14.848981 libemg-0.0.4/tests/data/
+-rw-r--r--   0 ethaneddy   (501) staff       (20)    11479 2023-08-08 17:15:49.000000 libemg-0.0.4/tests/data/emg_data_myo.csv
+-rw-r--r--   0 ethaneddy   (501) staff       (20)     8690 2023-08-08 17:15:49.000000 libemg-0.0.4/tests/data/emg_data_zeros.csv
+-rw-r--r--   0 ethaneddy   (501) staff       (20)     3665 2023-08-08 17:15:49.000000 libemg-0.0.4/tests/data/matlab_AR.csv
+-rw-r--r--   0 ethaneddy   (501) staff       (20)     3824 2023-08-08 17:15:49.000000 libemg-0.0.4/tests/data/matlab_CC.csv
+-rw-r--r--   0 ethaneddy   (501) staff       (20)      715 2023-08-08 17:15:49.000000 libemg-0.0.4/tests/data/matlab_DASDV.csv
+-rw-r--r--   0 ethaneddy   (501) staff       (20)      727 2023-08-08 17:15:49.000000 libemg-0.0.4/tests/data/matlab_FUZZYEN.csv
+-rw-r--r--   0 ethaneddy   (501) staff       (20)      490 2023-08-08 17:15:49.000000 libemg-0.0.4/tests/data/matlab_IAV.csv
+-rw-r--r--   0 ethaneddy   (501) staff       (20)      906 2023-08-08 17:15:49.000000 libemg-0.0.4/tests/data/matlab_IRF.csv
+-rw-r--r--   0 ethaneddy   (501) staff       (20)      713 2023-08-08 17:15:49.000000 libemg-0.0.4/tests/data/matlab_KURT.csv
+-rw-r--r--   0 ethaneddy   (501) staff       (20)      709 2023-08-08 17:15:49.000000 libemg-0.0.4/tests/data/matlab_LD.csv
+-rw-r--r--   0 ethaneddy   (501) staff       (20)      714 2023-08-08 17:15:49.000000 libemg-0.0.4/tests/data/matlab_LS.csv
+-rw-r--r--   0 ethaneddy   (501) staff       (20)      875 2023-08-08 17:15:49.000000 libemg-0.0.4/tests/data/matlab_M0.csv
+-rw-r--r--   0 ethaneddy   (501) staff       (20)      921 2023-08-08 17:15:49.000000 libemg-0.0.4/tests/data/matlab_M2.csv
+-rw-r--r--   0 ethaneddy   (501) staff       (20)      925 2023-08-08 17:15:49.000000 libemg-0.0.4/tests/data/matlab_M4.csv
+-rw-r--r--   0 ethaneddy   (501) staff       (20)      580 2023-08-08 17:15:49.000000 libemg-0.0.4/tests/data/matlab_MAV.csv
+-rw-r--r--   0 ethaneddy   (501) staff       (20)      717 2023-08-08 17:15:49.000000 libemg-0.0.4/tests/data/matlab_MAVFD.csv
+-rw-r--r--   0 ethaneddy   (501) staff       (20)      578 2023-08-08 17:15:49.000000 libemg-0.0.4/tests/data/matlab_MAVSLP.csv
+-rw-r--r--   0 ethaneddy   (501) staff       (20)      726 2023-08-08 17:15:49.000000 libemg-0.0.4/tests/data/matlab_MDF.csv
+-rw-r--r--   0 ethaneddy   (501) staff       (20)      717 2023-08-08 17:15:49.000000 libemg-0.0.4/tests/data/matlab_MFL.csv
+-rw-r--r--   0 ethaneddy   (501) staff       (20)      718 2023-08-08 17:15:49.000000 libemg-0.0.4/tests/data/matlab_MNF.csv
+-rw-r--r--   0 ethaneddy   (501) staff       (20)      816 2023-08-08 17:15:49.000000 libemg-0.0.4/tests/data/matlab_MNP.csv
+-rw-r--r--   0 ethaneddy   (501) staff       (20)      312 2023-08-08 17:15:49.000000 libemg-0.0.4/tests/data/matlab_MPK.csv
+-rw-r--r--   0 ethaneddy   (501) staff       (20)      718 2023-08-08 17:15:49.000000 libemg-0.0.4/tests/data/matlab_MSR.csv
+-rw-r--r--   0 ethaneddy   (501) staff       (20)      712 2023-08-08 17:15:49.000000 libemg-0.0.4/tests/data/matlab_MZP.csv
+-rw-r--r--   0 ethaneddy   (501) staff       (20)      717 2023-08-08 17:15:49.000000 libemg-0.0.4/tests/data/matlab_PAP.csv
+-rw-r--r--   0 ethaneddy   (501) staff       (20)      720 2023-08-08 17:15:49.000000 libemg-0.0.4/tests/data/matlab_RMS.csv
+-rw-r--r--   0 ethaneddy   (501) staff       (20)     5757 2023-08-08 17:15:49.000000 libemg-0.0.4/tests/data/matlab_RMSPHASOR.csv
+-rw-r--r--   0 ethaneddy   (501) staff       (20)      755 2023-08-08 17:15:49.000000 libemg-0.0.4/tests/data/matlab_SAMPEN.csv
+-rw-r--r--   0 ethaneddy   (501) staff       (20)      876 2023-08-08 17:15:49.000000 libemg-0.0.4/tests/data/matlab_SKEW.csv
+-rw-r--r--   0 ethaneddy   (501) staff       (20)     1128 2023-08-08 17:15:49.000000 libemg-0.0.4/tests/data/matlab_SM.csv
+-rw-r--r--   0 ethaneddy   (501) staff       (20)      918 2023-08-08 17:15:49.000000 libemg-0.0.4/tests/data/matlab_SPARSI.csv
+-rw-r--r--   0 ethaneddy   (501) staff       (20)      416 2023-08-08 17:15:49.000000 libemg-0.0.4/tests/data/matlab_SSC.csv
+-rw-r--r--   0 ethaneddy   (501) staff       (20)      701 2023-08-08 17:15:49.000000 libemg-0.0.4/tests/data/matlab_TM.csv
+-rw-r--r--   0 ethaneddy   (501) staff       (20)      686 2023-08-08 17:15:49.000000 libemg-0.0.4/tests/data/matlab_VAR.csv
+-rw-r--r--   0 ethaneddy   (501) staff       (20)      416 2023-08-08 17:15:49.000000 libemg-0.0.4/tests/data/matlab_WAMP.csv
+-rw-r--r--   0 ethaneddy   (501) staff       (20)      496 2023-08-08 17:15:49.000000 libemg-0.0.4/tests/data/matlab_WL.csv
+-rw-r--r--   0 ethaneddy   (501) staff       (20)      922 2023-08-08 17:15:49.000000 libemg-0.0.4/tests/data/matlab_WLF.csv
+-rw-r--r--   0 ethaneddy   (501) staff       (20)     5755 2023-08-08 17:15:49.000000 libemg-0.0.4/tests/data/matlab_WLPHASOR.csv
+-rw-r--r--   0 ethaneddy   (501) staff       (20)      372 2023-08-08 17:15:49.000000 libemg-0.0.4/tests/data/matlab_ZC.csv
+drwxr-xr-x   0 ethaneddy   (501) staff       (20)        0 2024-05-01 11:25:14.853508 libemg-0.0.4/tests/data/myo_dataset/
+-rw-r--r--   0 ethaneddy   (501) staff       (20)    13783 2023-08-08 17:15:49.000000 libemg-0.0.4/tests/data/myo_dataset/R_0_C_0_EMG.csv
+-rw-r--r--   0 ethaneddy   (501) staff       (20)    13490 2023-08-08 17:15:49.000000 libemg-0.0.4/tests/data/myo_dataset/R_0_C_1_EMG.csv
+-rw-r--r--   0 ethaneddy   (501) staff       (20)    13088 2023-08-08 17:15:49.000000 libemg-0.0.4/tests/data/myo_dataset/R_0_C_2_EMG.csv
+-rw-r--r--   0 ethaneddy   (501) staff       (20)    13896 2023-08-08 17:15:49.000000 libemg-0.0.4/tests/data/myo_dataset/R_0_C_3_EMG.csv
+-rw-r--r--   0 ethaneddy   (501) staff       (20)    13562 2023-08-08 17:15:49.000000 libemg-0.0.4/tests/data/myo_dataset/R_0_C_4_EMG.csv
+-rw-r--r--   0 ethaneddy   (501) staff       (20)    13643 2023-08-08 17:15:49.000000 libemg-0.0.4/tests/data/myo_dataset/R_1_C_0_EMG.csv
+-rw-r--r--   0 ethaneddy   (501) staff       (20)    13977 2023-08-08 17:15:49.000000 libemg-0.0.4/tests/data/myo_dataset/R_1_C_1_EMG.csv
+-rw-r--r--   0 ethaneddy   (501) staff       (20)    13170 2023-08-08 17:15:49.000000 libemg-0.0.4/tests/data/myo_dataset/R_1_C_2_EMG.csv
+-rw-r--r--   0 ethaneddy   (501) staff       (20)    13900 2023-08-08 17:15:49.000000 libemg-0.0.4/tests/data/myo_dataset/R_1_C_3_EMG.csv
+-rw-r--r--   0 ethaneddy   (501) staff       (20)    13588 2023-08-08 17:15:49.000000 libemg-0.0.4/tests/data/myo_dataset/R_1_C_4_EMG.csv
+-rw-r--r--   0 ethaneddy   (501) staff       (20)    13585 2023-08-08 17:15:49.000000 libemg-0.0.4/tests/data/myo_dataset/R_2_C_0_EMG.csv
+-rw-r--r--   0 ethaneddy   (501) staff       (20)    13923 2023-08-08 17:15:49.000000 libemg-0.0.4/tests/data/myo_dataset/R_2_C_1_EMG.csv
+-rw-r--r--   0 ethaneddy   (501) staff       (20)    13187 2023-08-08 17:15:49.000000 libemg-0.0.4/tests/data/myo_dataset/R_2_C_2_EMG.csv
+-rw-r--r--   0 ethaneddy   (501) staff       (20)    14084 2023-08-08 17:15:49.000000 libemg-0.0.4/tests/data/myo_dataset/R_2_C_3_EMG.csv
+-rw-r--r--   0 ethaneddy   (501) staff       (20)    13712 2023-08-08 17:15:49.000000 libemg-0.0.4/tests/data/myo_dataset/R_2_C_4_EMG.csv
+-rw-r--r--   0 ethaneddy   (501) staff       (20)    13471 2023-08-08 17:15:49.000000 libemg-0.0.4/tests/data/myo_dataset/R_3_C_0_EMG.csv
+-rw-r--r--   0 ethaneddy   (501) staff       (20)    13514 2023-08-08 17:15:49.000000 libemg-0.0.4/tests/data/myo_dataset/R_3_C_1_EMG.csv
+-rw-r--r--   0 ethaneddy   (501) staff       (20)    13016 2023-08-08 17:15:49.000000 libemg-0.0.4/tests/data/myo_dataset/R_3_C_2_EMG.csv
+-rw-r--r--   0 ethaneddy   (501) staff       (20)    14121 2023-08-08 17:15:49.000000 libemg-0.0.4/tests/data/myo_dataset/R_3_C_3_EMG.csv
+-rw-r--r--   0 ethaneddy   (501) staff       (20)    13254 2023-08-08 17:15:49.000000 libemg-0.0.4/tests/data/myo_dataset/R_3_C_4_EMG.csv
+-rw-r--r--   0 ethaneddy   (501) staff       (20)     1951 2023-08-08 17:15:49.000000 libemg-0.0.4/tests/data/predictions
+-rw-r--r--   0 ethaneddy   (501) staff       (20)   183694 2023-08-08 17:15:49.000000 libemg-0.0.4/tests/data/stream_data_tester.csv
+-rw-r--r--   0 ethaneddy   (501) staff       (20)     3775 2023-08-08 17:15:49.000000 libemg-0.0.4/tests/data/test_labels
+drwxr-xr-x   0 ethaneddy   (501) staff       (20)        0 2024-05-01 11:25:14.853932 libemg-0.0.4/tests/feature_tests/
+-rw-r--r--   0 ethaneddy   (501) staff       (20)      868 2023-08-08 17:15:49.000000 libemg-0.0.4/tests/feature_tests/test_mav_feature.py
+-rw-r--r--   0 ethaneddy   (501) staff       (20)      810 2023-08-08 17:15:49.000000 libemg-0.0.4/tests/feature_tests/test_zc_feature.py
+-rw-r--r--   0 ethaneddy   (501) staff       (20)     1282 2024-01-22 15:51:47.000000 libemg-0.0.4/tests/get_feature_values.m
+-rw-r--r--   0 ethaneddy   (501) staff       (20)     5972 2024-04-30 23:24:17.000000 libemg-0.0.4/tests/test_feature_extractor.py
+-rw-r--r--   0 ethaneddy   (501) staff       (20)     2482 2024-01-22 15:52:05.000000 libemg-0.0.4/tests/test_feature_verification.py
+-rw-r--r--   0 ethaneddy   (501) staff       (20)     2120 2023-08-08 17:15:49.000000 libemg-0.0.4/tests/test_offline_metrics.py
+-rw-r--r--   0 ethaneddy   (501) staff       (20)     2872 2023-08-08 17:15:49.000000 libemg-0.0.4/tests/test_online_classifier.py
+-rw-r--r--   0 ethaneddy   (501) staff       (20)     2607 2023-08-08 17:15:49.000000 libemg-0.0.4/tests/test_stream_architecture.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `libemg-0.0.3/PKG-INFO` & `libemg-0.0.4/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,47 +1,54 @@
 Metadata-Version: 2.1
 Name: libemg
-Version: 0.0.3
+Version: 0.0.4
 Summary: LibEMG - Myoelectric Control Library
-Home-page: UNKNOWN
 Author: Ethan Eddy, Evan Campbell, Angkoon Phinyomark, Scott Bateman, and Erik Scheme
-License: UNKNOWN
-Description: 
-        ![LibEMG](docs/source/libemg_logo.png)
-        
-        The goal of this library is to provide an easy to use and feature-rich API for developing robust real-time EMG-based interactions, and performing thorough offline analysis.
-        
-        **Authors**: Ethan Eddy, Evan Campbell, Angkoon Phinyomark, Scott Bateman, and Erik Scheme
-        
-        ## Documentation
-        All documentation can be found at: [Library Documentation](https://libemg.github.io/libemg/)
-        
-        ## Install 
-        `pip install libemg`
-        
-        ## Questions
-        Check out our discord server if you have questions, comments, or feature requests: https://discord.gg/NeqTTXmM4F
-        
-        ## Citing
-        We ask that if you leverage this library for any research-related purposes please cite the following publication:
-        
-        ```
-        @ARTICLE{10214558,
-          author={Eddy, Ethan and Campbell, Evan and Phinyomark, Angkoon and Bateman, Scott and Scheme, Erik},
-          journal={IEEE Access}, 
-          title={LibEMG: An Open Source Library to Facilitate the Exploration of Myoelectric Control}, 
-          year={2023},
-          volume={11},
-          number={},
-          pages={87380-87397},
-          doi={10.1109/ACCESS.2023.3304544}}
-        ```
-        
 Keywords: emg,myoelectric_control,pattern_recognition,muscle-based input
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable  
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: scikit-learn
+Requires-Dist: pillow
+Requires-Dist: matplotlib
+Requires-Dist: librosa
+Requires-Dist: wfdb
+Requires-Dist: pyserial
+Requires-Dist: PyWavelets
+
+
+![LibEMG](docs/source/libemg_logo.png)
+
+The goal of this library is to provide an easy to use and feature-rich API for developing robust real-time EMG-based interactions, and performing thorough offline analysis.
+
+**Authors**: Ethan Eddy, Evan Campbell, Angkoon Phinyomark, Scott Bateman, and Erik Scheme
+
+## Documentation
+All documentation can be found at: [Library Documentation](https://libemg.github.io/libemg/)
+
+## Install 
+`pip install libemg`
+
+## Questions
+Check out our discord server if you have questions, comments, or feature requests: https://discord.gg/NeqTTXmM4F
+
+## Citing
+We ask that if you leverage this library for any research-related purposes please cite the following publication:
+
+```
+@ARTICLE{10214558,
+  author={Eddy, Ethan and Campbell, Evan and Phinyomark, Angkoon and Bateman, Scott and Scheme, Erik},
+  journal={IEEE Access}, 
+  title={LibEMG: An Open Source Library to Facilitate the Exploration of Myoelectric Control}, 
+  year={2023},
+  volume={11},
+  number={},
+  pages={87380-87397},
+  doi={10.1109/ACCESS.2023.3304544}}
+```
```

### Comparing `libemg-0.0.3/libemg.egg-info/PKG-INFO` & `libemg-0.0.4/libemg.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,47 +1,54 @@
 Metadata-Version: 2.1
 Name: libemg
-Version: 0.0.3
+Version: 0.0.4
 Summary: LibEMG - Myoelectric Control Library
-Home-page: UNKNOWN
 Author: Ethan Eddy, Evan Campbell, Angkoon Phinyomark, Scott Bateman, and Erik Scheme
-License: UNKNOWN
-Description: 
-        ![LibEMG](docs/source/libemg_logo.png)
-        
-        The goal of this library is to provide an easy to use and feature-rich API for developing robust real-time EMG-based interactions, and performing thorough offline analysis.
-        
-        **Authors**: Ethan Eddy, Evan Campbell, Angkoon Phinyomark, Scott Bateman, and Erik Scheme
-        
-        ## Documentation
-        All documentation can be found at: [Library Documentation](https://libemg.github.io/libemg/)
-        
-        ## Install 
-        `pip install libemg`
-        
-        ## Questions
-        Check out our discord server if you have questions, comments, or feature requests: https://discord.gg/NeqTTXmM4F
-        
-        ## Citing
-        We ask that if you leverage this library for any research-related purposes please cite the following publication:
-        
-        ```
-        @ARTICLE{10214558,
-          author={Eddy, Ethan and Campbell, Evan and Phinyomark, Angkoon and Bateman, Scott and Scheme, Erik},
-          journal={IEEE Access}, 
-          title={LibEMG: An Open Source Library to Facilitate the Exploration of Myoelectric Control}, 
-          year={2023},
-          volume={11},
-          number={},
-          pages={87380-87397},
-          doi={10.1109/ACCESS.2023.3304544}}
-        ```
-        
 Keywords: emg,myoelectric_control,pattern_recognition,muscle-based input
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable  
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: scikit-learn
+Requires-Dist: pillow
+Requires-Dist: matplotlib
+Requires-Dist: librosa
+Requires-Dist: wfdb
+Requires-Dist: pyserial
+Requires-Dist: PyWavelets
+
+
+![LibEMG](docs/source/libemg_logo.png)
+
+The goal of this library is to provide an easy to use and feature-rich API for developing robust real-time EMG-based interactions, and performing thorough offline analysis.
+
+**Authors**: Ethan Eddy, Evan Campbell, Angkoon Phinyomark, Scott Bateman, and Erik Scheme
+
+## Documentation
+All documentation can be found at: [Library Documentation](https://libemg.github.io/libemg/)
+
+## Install 
+`pip install libemg`
+
+## Questions
+Check out our discord server if you have questions, comments, or feature requests: https://discord.gg/NeqTTXmM4F
+
+## Citing
+We ask that if you leverage this library for any research-related purposes please cite the following publication:
+
+```
+@ARTICLE{10214558,
+  author={Eddy, Ethan and Campbell, Evan and Phinyomark, Angkoon and Bateman, Scott and Scheme, Erik},
+  journal={IEEE Access}, 
+  title={LibEMG: An Open Source Library to Facilitate the Exploration of Myoelectric Control}, 
+  year={2023},
+  volume={11},
+  number={},
+  pages={87380-87397},
+  doi={10.1109/ACCESS.2023.3304544}}
+```
```

### Comparing `libemg-0.0.3/libemg.egg-info/SOURCES.txt` & `libemg-0.0.4/libemg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/LICENSE` & `libemg-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/libemg/data_handler.py` & `libemg-0.0.4/libemg/data_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,26 +61,28 @@
     The purpose of this class is to facilitate the process of accumulating offline training
     and testing data. This class is extensible to a wide range of file and folder structures. 
     """
     def __init__(self):
         super().__init__()
     
 
-    def get_data(self, folder_location="", filename_dic={}, delimiter=",", mrdf_key='p_signal'):
+    def get_data(self, folder_location="", filename_dic={}, delimiter=",", mrdf_key='p_signal', skiprows=0):
         """Method to collect data from a folder into the OfflineDataHandler object. Metadata can be collected either from the filename
         specifying <tag>_regex keys in the filename_dic, or from within the .csv or .txt files specifying <tag>_columns in the filename_dic.
 
         Parameters
         ----------
         folder_location: str
             Location of the dataset relative to current file path
         filename_dic: dict
             dictionary containing the values of the metadata and the regex or columns associated with that metadata.
         delimiter: char
             How the columns of the files are separated in the .txt or .csv files.
+        skiprows: int
+            The number of rows in the CSV file to skip (from the top).
         """
         # you can insert custom member variables that will be collected from the filename using the dictionary
         # this gives at least a tiny bit of flexibility around what is recorded aside from the data
         dictionary_keys = filename_dic.keys()
         keys = [k for k in dictionary_keys if not (k.endswith("_regex") or k.endswith("_column"))]
         for k in keys:
             if not hasattr(self, k):
@@ -103,20 +105,22 @@
         self._check_file_regex(files, regex_keys)
 
         for f in files:
             if '.hea' in f:
                 # The key is the emg key that is in the mrdf file
                 file_data = (wfdb.rdrecord(f.replace('.hea',''))).__getattribute__(mrdf_key)
             else:
-                file_data = np.genfromtxt(f,delimiter=delimiter)
+                file_data = np.genfromtxt(f,delimiter=delimiter, skip_header=skiprows)
             # collect the data from the file
             if "data_column" in dictionary_keys:
                 self.data.append(file_data[:, filename_dic["data_column"]])
             else:
                 self.data.append(file_data)
+            if len(self.data[-1].shape) == 1:
+                self.data[-1] = np.expand_dims(self.data[-1], 1)
             # also collect the metadata from the filename
             for k in keys:
                 if k + "_regex" in dictionary_keys:
                     k_val = re.findall(filename_dic[k+"_regex"],f)[0]
                     k_id  = filename_dic[k].index(k_val)
                     metadata_column = k_id * np.ones((file_data.shape[0],1), dtype=int)
                     setattr(self, k, getattr(self,k)+[metadata_column])
```

### Comparing `libemg-0.0.3/libemg/feature_selector.py` & `libemg-0.0.4/libemg/feature_selector.py`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/libemg/offline_metrics.py` & `libemg-0.0.4/libemg/offline_metrics.py`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/libemg/filtering.py` & `libemg-0.0.4/libemg/filtering.py`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/libemg/screen_guided_training.py` & `libemg-0.0.4/libemg/screen_guided_training.py`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/libemg/emg_classifier.py` & `libemg-0.0.4/libemg/emg_classifier.py`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/libemg/datasets.py` & `libemg-0.0.4/libemg/datasets.py`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/libemg/streamers.py` & `libemg-0.0.4/libemg/streamers.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,14 +107,15 @@
     version: string optional, default = '1.2'
         The version for the sifi streamer.
     Examples
     ---------
     >>> sifibridge_streamer()
     """
     sb = SiFiBridgeStreamer(ip, port,notch_on=notch_on,
+                            version=version,
                             ecg=ecg,
                             emg=emg,
                             eda=eda,
                             imu=imu,
                             ppg=ppg,
                             notch_freq=notch_freq,
                             emgfir_on=emg_fir_on,
```

### Comparing `libemg-0.0.3/libemg/utils.py` & `libemg-0.0.4/libemg/utils.py`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/libemg/feature_extractor.py` & `libemg-0.0.4/libemg/feature_extractor.py`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/libemg/_streamers/_myo_streamer.py` & `libemg-0.0.4/libemg/_streamers/_myo_streamer.py`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/libemg/_streamers/_delsys_streamer.py` & `libemg-0.0.4/libemg/_streamers/_delsys_streamer.py`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/libemg/_streamers/_OTB_Syncstation.py` & `libemg-0.0.4/libemg/_streamers/_OTB_Syncstation.py`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/libemg/_streamers/_oymotion_windows_streamer.py` & `libemg-0.0.4/libemg/_streamers/_oymotion_windows_streamer.py`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/libemg/_streamers/_sifi_streamer.py` & `libemg-0.0.4/libemg/_streamers/_sifi_streamer.py`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/libemg/_streamers/_sifi_bridge_streamer.py` & `libemg-0.0.4/libemg/_streamers/_sifi_bridge_streamer.py`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/libemg/_streamers/_emager_streamer.py` & `libemg-0.0.4/libemg/_streamers/_emager_streamer.py`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/libemg/_streamers/_OTB_MuoviPlus.py` & `libemg-0.0.4/libemg/_streamers/_OTB_MuoviPlus.py`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/libemg/_streamers/_oymotion_streamer.py` & `libemg-0.0.4/libemg/_streamers/_oymotion_streamer.py`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/libemg/_streamers/_OTB_Muovi.py` & `libemg-0.0.4/libemg/_streamers/_OTB_Muovi.py`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/libemg/_streamers/_OTB_SessantaquattroPlus.py` & `libemg-0.0.4/libemg/_streamers/_OTB_SessantaquattroPlus.py`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/libemg/raw_data.py` & `libemg-0.0.4/libemg/raw_data.py`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/tests/test_feature_extractor.py` & `libemg-0.0.4/tests/test_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/tests/test_stream_architecture.py` & `libemg-0.0.4/tests/test_stream_architecture.py`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/tests/feature_tests/test_mav_feature.py` & `libemg-0.0.4/tests/feature_tests/test_mav_feature.py`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/tests/feature_tests/test_zc_feature.py` & `libemg-0.0.4/tests/feature_tests/test_zc_feature.py`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/tests/test_offline_metrics.py` & `libemg-0.0.4/tests/test_offline_metrics.py`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/tests/test_feature_verification.py` & `libemg-0.0.4/tests/test_feature_verification.py`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/tests/test_online_classifier.py` & `libemg-0.0.4/tests/test_online_classifier.py`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/tests/get_feature_values.m` & `libemg-0.0.4/tests/get_feature_values.m`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/tests/data/matlab_MNP.csv` & `libemg-0.0.4/tests/data/matlab_MNP.csv`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/tests/data/emg_data_myo.csv` & `libemg-0.0.4/tests/data/emg_data_myo.csv`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/tests/data/matlab_MNF.csv` & `libemg-0.0.4/tests/data/matlab_MNF.csv`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/tests/data/matlab_DASDV.csv` & `libemg-0.0.4/tests/data/matlab_DASDV.csv`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/tests/data/test_labels` & `libemg-0.0.4/tests/data/test_labels`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/tests/data/matlab_SM.csv` & `libemg-0.0.4/tests/data/matlab_SM.csv`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/tests/data/emg_data_zeros.csv` & `libemg-0.0.4/tests/data/emg_data_zeros.csv`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/tests/data/matlab_MZP.csv` & `libemg-0.0.4/tests/data/matlab_MZP.csv`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/tests/data/matlab_TM.csv` & `libemg-0.0.4/tests/data/matlab_TM.csv`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/tests/data/matlab_MDF.csv` & `libemg-0.0.4/tests/data/matlab_MDF.csv`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/tests/data/matlab_MFL.csv` & `libemg-0.0.4/tests/data/matlab_MFL.csv`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/tests/data/matlab_MAVSLP.csv` & `libemg-0.0.4/tests/data/matlab_MAVSLP.csv`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/tests/data/matlab_RMSPHASOR.csv` & `libemg-0.0.4/tests/data/matlab_RMSPHASOR.csv`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/tests/data/matlab_SKEW.csv` & `libemg-0.0.4/tests/data/matlab_SKEW.csv`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/tests/data/matlab_FUZZYEN.csv` & `libemg-0.0.4/tests/data/matlab_FUZZYEN.csv`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/tests/data/matlab_CC.csv` & `libemg-0.0.4/tests/data/matlab_CC.csv`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/tests/data/matlab_WLPHASOR.csv` & `libemg-0.0.4/tests/data/matlab_WLPHASOR.csv`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/tests/data/matlab_M0.csv` & `libemg-0.0.4/tests/data/matlab_M0.csv`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/tests/data/matlab_AR.csv` & `libemg-0.0.4/tests/data/matlab_AR.csv`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/tests/data/matlab_IRF.csv` & `libemg-0.0.4/tests/data/matlab_IRF.csv`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/tests/data/matlab_WLF.csv` & `libemg-0.0.4/tests/data/matlab_WLF.csv`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/tests/data/matlab_MAVFD.csv` & `libemg-0.0.4/tests/data/matlab_MAVFD.csv`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/tests/data/matlab_M2.csv` & `libemg-0.0.4/tests/data/matlab_M2.csv`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/tests/data/matlab_MSR.csv` & `libemg-0.0.4/tests/data/matlab_MSR.csv`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/tests/data/matlab_LD.csv` & `libemg-0.0.4/tests/data/matlab_LD.csv`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/tests/data/matlab_LS.csv` & `libemg-0.0.4/tests/data/matlab_LS.csv`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/tests/data/stream_data_tester.csv` & `libemg-0.0.4/tests/data/stream_data_tester.csv`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/tests/data/matlab_M4.csv` & `libemg-0.0.4/tests/data/matlab_M4.csv`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/tests/data/myo_dataset/R_0_C_3_EMG.csv` & `libemg-0.0.4/tests/data/myo_dataset/R_0_C_3_EMG.csv`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/tests/data/myo_dataset/R_3_C_1_EMG.csv` & `libemg-0.0.4/tests/data/myo_dataset/R_3_C_1_EMG.csv`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/tests/data/myo_dataset/R_3_C_0_EMG.csv` & `libemg-0.0.4/tests/data/myo_dataset/R_3_C_0_EMG.csv`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/tests/data/myo_dataset/R_1_C_4_EMG.csv` & `libemg-0.0.4/tests/data/myo_dataset/R_1_C_4_EMG.csv`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/tests/data/myo_dataset/R_0_C_2_EMG.csv` & `libemg-0.0.4/tests/data/myo_dataset/R_0_C_2_EMG.csv`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/tests/data/myo_dataset/R_3_C_2_EMG.csv` & `libemg-0.0.4/tests/data/myo_dataset/R_3_C_2_EMG.csv`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/tests/data/myo_dataset/R_2_C_4_EMG.csv` & `libemg-0.0.4/tests/data/myo_dataset/R_2_C_4_EMG.csv`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/tests/data/myo_dataset/R_0_C_0_EMG.csv` & `libemg-0.0.4/tests/data/myo_dataset/R_0_C_0_EMG.csv`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/tests/data/myo_dataset/R_0_C_1_EMG.csv` & `libemg-0.0.4/tests/data/myo_dataset/R_0_C_1_EMG.csv`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/tests/data/myo_dataset/R_3_C_3_EMG.csv` & `libemg-0.0.4/tests/data/myo_dataset/R_3_C_3_EMG.csv`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/tests/data/myo_dataset/R_1_C_2_EMG.csv` & `libemg-0.0.4/tests/data/myo_dataset/R_1_C_2_EMG.csv`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/tests/data/myo_dataset/R_0_C_4_EMG.csv` & `libemg-0.0.4/tests/data/myo_dataset/R_0_C_4_EMG.csv`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/tests/data/myo_dataset/R_2_C_0_EMG.csv` & `libemg-0.0.4/tests/data/myo_dataset/R_2_C_0_EMG.csv`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/tests/data/myo_dataset/R_2_C_1_EMG.csv` & `libemg-0.0.4/tests/data/myo_dataset/R_2_C_1_EMG.csv`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/tests/data/myo_dataset/R_1_C_3_EMG.csv` & `libemg-0.0.4/tests/data/myo_dataset/R_1_C_3_EMG.csv`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/tests/data/myo_dataset/R_2_C_3_EMG.csv` & `libemg-0.0.4/tests/data/myo_dataset/R_2_C_3_EMG.csv`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/tests/data/myo_dataset/R_1_C_1_EMG.csv` & `libemg-0.0.4/tests/data/myo_dataset/R_1_C_1_EMG.csv`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/tests/data/myo_dataset/R_1_C_0_EMG.csv` & `libemg-0.0.4/tests/data/myo_dataset/R_1_C_0_EMG.csv`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/tests/data/myo_dataset/R_3_C_4_EMG.csv` & `libemg-0.0.4/tests/data/myo_dataset/R_3_C_4_EMG.csv`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/tests/data/myo_dataset/R_2_C_2_EMG.csv` & `libemg-0.0.4/tests/data/myo_dataset/R_2_C_2_EMG.csv`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/tests/data/matlab_MAV.csv` & `libemg-0.0.4/tests/data/matlab_MAV.csv`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/tests/data/matlab_PAP.csv` & `libemg-0.0.4/tests/data/matlab_PAP.csv`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/tests/data/matlab_RMS.csv` & `libemg-0.0.4/tests/data/matlab_RMS.csv`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/tests/data/matlab_KURT.csv` & `libemg-0.0.4/tests/data/matlab_KURT.csv`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/tests/data/predictions` & `libemg-0.0.4/tests/data/predictions`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/tests/data/matlab_SAMPEN.csv` & `libemg-0.0.4/tests/data/matlab_SAMPEN.csv`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/tests/data/matlab_VAR.csv` & `libemg-0.0.4/tests/data/matlab_VAR.csv`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/tests/data/matlab_SPARSI.csv` & `libemg-0.0.4/tests/data/matlab_SPARSI.csv`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/README.md` & `libemg-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/setup.py` & `libemg-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     long_description = "\n" + fh.read()
 
 # To release:
 # python setup.py sdist
 # python -m twine upload --repository testpypi dist/* --verbose  <------ testpypi
 # 
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'LibEMG - Myoelectric Control Library'
 LONG_DESCRIPTION = 'A library for designing and exploring real-time and offline myoelectric control systems.'
 
 setup(
     name="libemg",
     version=VERSION,
     author="Ethan Eddy, Evan Campbell, Angkoon Phinyomark, Scott Bateman, and Erik Scheme",
```

### Comparing `libemg-0.0.3/.gitignore` & `libemg-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `libemg-0.0.3/.github/workflows/ci.yaml` & `libemg-0.0.4/.github/workflows/ci.yaml`

 * *Files identical despite different names*

