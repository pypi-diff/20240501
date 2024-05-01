# Comparing `tmp/deadline_cloud_for_unreal_engine-0.2.0.tar.gz` & `tmp/deadline_cloud_for_unreal_engine-0.2.1.tar.gz`

## Comparing `deadline_cloud_for_unreal_engine-0.2.0.tar` & `deadline_cloud_for_unreal_engine-0.2.1.tar`

### file list

```diff
@@ -1,83 +1,83 @@
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/_version.py
--rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/hatch_custom_hook.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/src/deadline/unreal_adaptor/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/src/deadline/unreal_adaptor/_version.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/src/deadline/unreal_adaptor/UnrealAdaptor/__init__.py
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/src/deadline/unreal_adaptor/UnrealAdaptor/__main__.py
--rw-r--r--   0        0        0    17700 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/src/deadline/unreal_adaptor/UnrealAdaptor/adaptor.py
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/src/deadline/unreal_adaptor/UnrealAdaptor/common.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/src/deadline/unreal_adaptor/UnrealAdaptor/py.typed
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/src/deadline/unreal_adaptor/UnrealAdaptor/schemas/init_data.schema.json
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/src/deadline/unreal_adaptor/UnrealAdaptor/schemas/run_data.schema.json
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/src/deadline/unreal_adaptor/UnrealClient/__init__.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/src/deadline/unreal_adaptor/UnrealClient/py.typed
--rw-r--r--   0        0        0     4234 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/src/deadline/unreal_adaptor/UnrealClient/unreal_client.py
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/src/deadline/unreal_adaptor/UnrealClient/step_handlers/__init__.py
--rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/src/deadline/unreal_adaptor/UnrealClient/step_handlers/base_step_handler.py
--rw-r--r--   0        0        0     3144 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/src/deadline/unreal_adaptor/UnrealClient/step_handlers/unreal_custom_step_handler.py
--rw-r--r--   0        0        0    10032 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/src/deadline/unreal_adaptor/UnrealClient/step_handlers/unreal_render_step_handler.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/src/deadline/unreal_submitter/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/src/deadline/unreal_submitter/_version.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/src/deadline/unreal_submitter/common.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/src/deadline/unreal_submitter/settings.py
--rw-r--r--   0        0        0     8419 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/src/deadline/unreal_submitter/submitter.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/src/deadline/unreal_submitter/templates/default_unreal_job_template_v04.yaml
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/src/deadline/unreal_submitter/templates/default_unreal_job_template_v05.yaml
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/src/deadline/unreal_submitter/templates/default_unreal_job_template_v06.yaml
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/src/deadline/unreal_submitter/templates/default_unreal_step_template_v04.yaml
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/src/deadline/unreal_submitter/templates/default_unreal_step_template_v05.yaml
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/src/deadline/unreal_submitter/unreal_dependency_collector/__init__.py
--rw-r--r--   0        0        0     5715 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/src/deadline/unreal_submitter/unreal_dependency_collector/collector.py
--rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/src/deadline/unreal_submitter/unreal_dependency_collector/common.py
--rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/src/deadline/unreal_submitter/unreal_dependency_collector/dependency_search_options.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/src/deadline/unreal_submitter/unreal_open_job/__init__.py
--rw-r--r--   0        0        0    14727 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/src/deadline/unreal_submitter/unreal_open_job/job_step.py
--rw-r--r--   0        0        0    15473 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/src/deadline/unreal_submitter/unreal_open_job/open_job_description.py
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/DEVELOPMENT.md
--rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/LICENSE
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/NOTICE
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/README.md
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/UnrealDeadlineCloudService.uplugin
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/Config/DefaultUnrealDeadlineCloudService.ini
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/Content/Python/init_unreal.py
--rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/Content/Python/job_library.py
--rw-r--r--   0        0        0     3603 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/Content/Python/remote_executor.py
--rw-r--r--   0        0        0    14845 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/Content/Python/settings.py
--rw-r--r--   0        0        0   114392 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/Documentation/Doxyfile
--rw-r--r--   0        0        0     3069 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/Documentation/doxygen-awesome-sidebar-only.css
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/Documentation/doxygen-awesome.LICENSE
--rw-r--r--   0        0        0    35480 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/Documentation/doxygen-awesome.css
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/Resources/Icon128.png
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/Source/UnrealDeadlineCloudService/UnrealDeadlineCloudService.Build.cs
--rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/Source/UnrealDeadlineCloudService/Private/UnrealDeadlineCloudServiceModule.cpp
--rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/Source/UnrealDeadlineCloudService/Private/DeadlineCloudJobSettings/DeadlineCloudDeveloperSettings.cpp
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/Source/UnrealDeadlineCloudService/Private/DeadlineCloudJobSettings/DeadlineCloudJobDataAsset.cpp
--rw-r--r--   0        0        0    16560 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/Source/UnrealDeadlineCloudService/Private/DeadlineCloudJobSettings/DeadlineCloudJobPresetDetailsCustomization.cpp
--rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/Source/UnrealDeadlineCloudService/Private/DeadlineCloudJobSettings/DeadlineCloudSettingsDetails.cpp
--rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/Source/UnrealDeadlineCloudService/Private/DeadlineCloudJobSettings/DeadlineCloudStatusHandler.cpp
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/Source/UnrealDeadlineCloudService/Private/MovieRenderPipeline/DeadlineCloudRenderStepSetting.cpp
--rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/Source/UnrealDeadlineCloudService/Private/MovieRenderPipeline/DeadlineCloudStepBaseSetting.cpp
--rw-r--r--   0        0        0     9084 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/Source/UnrealDeadlineCloudService/Private/MovieRenderPipeline/MoviePipelineDeadlineCloudExecutorJob.cpp
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/Source/UnrealDeadlineCloudService/Private/PythonAPILibraries/DeadlineCloudJobBundleLibrary.cpp
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/Source/UnrealDeadlineCloudService/Private/PythonAPILibraries/PythonAPILibrary.cpp
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/Source/UnrealDeadlineCloudService/Private/PythonAPILibraries/PythonGameThreadExecutor.cpp
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/Source/UnrealDeadlineCloudService/Public/UnrealDeadlineCloudServiceModule.h
--rw-r--r--   0        0        0     7691 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/Source/UnrealDeadlineCloudService/Public/DeadlineCloudJobSettings/DeadlineCloudDeveloperSettings.h
--rw-r--r--   0        0        0     8579 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/Source/UnrealDeadlineCloudService/Public/DeadlineCloudJobSettings/DeadlineCloudJobDataAsset.h
--rw-r--r--   0        0        0     8194 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/Source/UnrealDeadlineCloudService/Public/DeadlineCloudJobSettings/DeadlineCloudJobPresetDetailsCustomization.h
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/Source/UnrealDeadlineCloudService/Public/DeadlineCloudJobSettings/DeadlineCloudSettingsDetails.h
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/Source/UnrealDeadlineCloudService/Public/DeadlineCloudJobSettings/DeadlineCloudStatusHandler.h
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/Source/UnrealDeadlineCloudService/Public/MovieRenderPipeline/DeadlineCloudCustomScriptStepSetting.h
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/Source/UnrealDeadlineCloudService/Public/MovieRenderPipeline/DeadlineCloudRenderStepSetting.h
--rw-r--r--   0        0        0     3057 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/Source/UnrealDeadlineCloudService/Public/MovieRenderPipeline/DeadlineCloudStepBaseSetting.h
--rw-r--r--   0        0        0     3393 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/Source/UnrealDeadlineCloudService/Public/MovieRenderPipeline/MoviePipelineDeadlineCloudExecutorJob.h
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/Source/UnrealDeadlineCloudService/Public/PythonAPILibraries/DeadlineCloudJobBundleLibrary.h
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/Source/UnrealDeadlineCloudService/Public/PythonAPILibraries/PythonAPILibrary.h
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/Source/UnrealDeadlineCloudService/Public/PythonAPILibraries/PythonGameThreadExecutor.h
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/.gitignore
--rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/LICENSE
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/NOTICE
--rw-r--r--   0        0        0     3673 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/README.md
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/hatch.toml
--rw-r--r--   0        0        0     3981 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4781 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/_version.py
+-rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/hatch_custom_hook.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/src/deadline/unreal_adaptor/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/src/deadline/unreal_adaptor/_version.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/src/deadline/unreal_adaptor/UnrealAdaptor/__init__.py
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/src/deadline/unreal_adaptor/UnrealAdaptor/__main__.py
+-rw-r--r--   0        0        0    17700 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/src/deadline/unreal_adaptor/UnrealAdaptor/adaptor.py
+-rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/src/deadline/unreal_adaptor/UnrealAdaptor/common.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/src/deadline/unreal_adaptor/UnrealAdaptor/py.typed
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/src/deadline/unreal_adaptor/UnrealAdaptor/schemas/init_data.schema.json
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/src/deadline/unreal_adaptor/UnrealAdaptor/schemas/run_data.schema.json
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/src/deadline/unreal_adaptor/UnrealClient/__init__.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/src/deadline/unreal_adaptor/UnrealClient/py.typed
+-rw-r--r--   0        0        0     4234 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/src/deadline/unreal_adaptor/UnrealClient/unreal_client.py
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/src/deadline/unreal_adaptor/UnrealClient/step_handlers/__init__.py
+-rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/src/deadline/unreal_adaptor/UnrealClient/step_handlers/base_step_handler.py
+-rw-r--r--   0        0        0     3144 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/src/deadline/unreal_adaptor/UnrealClient/step_handlers/unreal_custom_step_handler.py
+-rw-r--r--   0        0        0    10032 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/src/deadline/unreal_adaptor/UnrealClient/step_handlers/unreal_render_step_handler.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/src/deadline/unreal_submitter/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/src/deadline/unreal_submitter/_version.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/src/deadline/unreal_submitter/common.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/src/deadline/unreal_submitter/settings.py
+-rw-r--r--   0        0        0     8419 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/src/deadline/unreal_submitter/submitter.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/src/deadline/unreal_submitter/templates/default_unreal_job_template_v04.yaml
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/src/deadline/unreal_submitter/templates/default_unreal_job_template_v05.yaml
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/src/deadline/unreal_submitter/templates/default_unreal_job_template_v06.yaml
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/src/deadline/unreal_submitter/templates/default_unreal_step_template_v04.yaml
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/src/deadline/unreal_submitter/templates/default_unreal_step_template_v05.yaml
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/src/deadline/unreal_submitter/unreal_dependency_collector/__init__.py
+-rw-r--r--   0        0        0     5715 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/src/deadline/unreal_submitter/unreal_dependency_collector/collector.py
+-rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/src/deadline/unreal_submitter/unreal_dependency_collector/common.py
+-rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/src/deadline/unreal_submitter/unreal_dependency_collector/dependency_search_options.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/src/deadline/unreal_submitter/unreal_open_job/__init__.py
+-rw-r--r--   0        0        0    14727 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/src/deadline/unreal_submitter/unreal_open_job/job_step.py
+-rw-r--r--   0        0        0    15473 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/src/deadline/unreal_submitter/unreal_open_job/open_job_description.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/DEVELOPMENT.md
+-rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/LICENSE
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/NOTICE
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/README.md
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/UnrealDeadlineCloudService.uplugin
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/Config/DefaultUnrealDeadlineCloudService.ini
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/Content/Python/init_unreal.py
+-rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/Content/Python/job_library.py
+-rw-r--r--   0        0        0     3603 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/Content/Python/remote_executor.py
+-rw-r--r--   0        0        0    14845 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/Content/Python/settings.py
+-rw-r--r--   0        0        0   114392 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/Documentation/Doxyfile
+-rw-r--r--   0        0        0     3069 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/Documentation/doxygen-awesome-sidebar-only.css
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/Documentation/doxygen-awesome.LICENSE
+-rw-r--r--   0        0        0    35480 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/Documentation/doxygen-awesome.css
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/Resources/Icon128.png
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/Source/UnrealDeadlineCloudService/UnrealDeadlineCloudService.Build.cs
+-rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/Source/UnrealDeadlineCloudService/Private/UnrealDeadlineCloudServiceModule.cpp
+-rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/Source/UnrealDeadlineCloudService/Private/DeadlineCloudJobSettings/DeadlineCloudDeveloperSettings.cpp
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/Source/UnrealDeadlineCloudService/Private/DeadlineCloudJobSettings/DeadlineCloudJobDataAsset.cpp
+-rw-r--r--   0        0        0    16560 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/Source/UnrealDeadlineCloudService/Private/DeadlineCloudJobSettings/DeadlineCloudJobPresetDetailsCustomization.cpp
+-rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/Source/UnrealDeadlineCloudService/Private/DeadlineCloudJobSettings/DeadlineCloudSettingsDetails.cpp
+-rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/Source/UnrealDeadlineCloudService/Private/DeadlineCloudJobSettings/DeadlineCloudStatusHandler.cpp
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/Source/UnrealDeadlineCloudService/Private/MovieRenderPipeline/DeadlineCloudRenderStepSetting.cpp
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/Source/UnrealDeadlineCloudService/Private/MovieRenderPipeline/DeadlineCloudStepBaseSetting.cpp
+-rw-r--r--   0        0        0     9084 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/Source/UnrealDeadlineCloudService/Private/MovieRenderPipeline/MoviePipelineDeadlineCloudExecutorJob.cpp
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/Source/UnrealDeadlineCloudService/Private/PythonAPILibraries/DeadlineCloudJobBundleLibrary.cpp
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/Source/UnrealDeadlineCloudService/Private/PythonAPILibraries/PythonAPILibrary.cpp
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/Source/UnrealDeadlineCloudService/Private/PythonAPILibraries/PythonGameThreadExecutor.cpp
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/Source/UnrealDeadlineCloudService/Public/UnrealDeadlineCloudServiceModule.h
+-rw-r--r--   0        0        0     7691 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/Source/UnrealDeadlineCloudService/Public/DeadlineCloudJobSettings/DeadlineCloudDeveloperSettings.h
+-rw-r--r--   0        0        0     8579 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/Source/UnrealDeadlineCloudService/Public/DeadlineCloudJobSettings/DeadlineCloudJobDataAsset.h
+-rw-r--r--   0        0        0     8194 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/Source/UnrealDeadlineCloudService/Public/DeadlineCloudJobSettings/DeadlineCloudJobPresetDetailsCustomization.h
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/Source/UnrealDeadlineCloudService/Public/DeadlineCloudJobSettings/DeadlineCloudSettingsDetails.h
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/Source/UnrealDeadlineCloudService/Public/DeadlineCloudJobSettings/DeadlineCloudStatusHandler.h
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/Source/UnrealDeadlineCloudService/Public/MovieRenderPipeline/DeadlineCloudCustomScriptStepSetting.h
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/Source/UnrealDeadlineCloudService/Public/MovieRenderPipeline/DeadlineCloudRenderStepSetting.h
+-rw-r--r--   0        0        0     3057 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/Source/UnrealDeadlineCloudService/Public/MovieRenderPipeline/DeadlineCloudStepBaseSetting.h
+-rw-r--r--   0        0        0     3393 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/Source/UnrealDeadlineCloudService/Public/MovieRenderPipeline/MoviePipelineDeadlineCloudExecutorJob.h
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/Source/UnrealDeadlineCloudService/Public/PythonAPILibraries/DeadlineCloudJobBundleLibrary.h
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/Source/UnrealDeadlineCloudService/Public/PythonAPILibraries/PythonAPILibrary.h
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/Source/UnrealDeadlineCloudService/Public/PythonAPILibraries/PythonGameThreadExecutor.h
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/.gitignore
+-rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/LICENSE
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/NOTICE
+-rw-r--r--   0        0        0     3673 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/README.md
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/hatch.toml
+-rw-r--r--   0        0        0     3981 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4781 2020-02-02 00:00:00.000000 deadline_cloud_for_unreal_engine-0.2.1/PKG-INFO
```

### Comparing `deadline_cloud_for_unreal_engine-0.2.0/hatch_custom_hook.py` & `deadline_cloud_for_unreal_engine-0.2.1/hatch_custom_hook.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_unreal_engine-0.2.0/src/deadline/unreal_adaptor/UnrealAdaptor/__main__.py` & `deadline_cloud_for_unreal_engine-0.2.1/src/deadline/unreal_adaptor/UnrealAdaptor/__main__.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_unreal_engine-0.2.0/src/deadline/unreal_adaptor/UnrealAdaptor/adaptor.py` & `deadline_cloud_for_unreal_engine-0.2.1/src/deadline/unreal_adaptor/UnrealAdaptor/adaptor.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_unreal_engine-0.2.0/src/deadline/unreal_adaptor/UnrealAdaptor/common.py` & `deadline_cloud_for_unreal_engine-0.2.1/src/deadline/unreal_adaptor/UnrealAdaptor/common.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_unreal_engine-0.2.0/src/deadline/unreal_adaptor/UnrealClient/unreal_client.py` & `deadline_cloud_for_unreal_engine-0.2.1/src/deadline/unreal_adaptor/UnrealClient/unreal_client.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_unreal_engine-0.2.0/src/deadline/unreal_adaptor/UnrealClient/step_handlers/__init__.py` & `deadline_cloud_for_unreal_engine-0.2.1/src/deadline/unreal_adaptor/UnrealClient/step_handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_unreal_engine-0.2.0/src/deadline/unreal_adaptor/UnrealClient/step_handlers/base_step_handler.py` & `deadline_cloud_for_unreal_engine-0.2.1/src/deadline/unreal_adaptor/UnrealClient/step_handlers/base_step_handler.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_unreal_engine-0.2.0/src/deadline/unreal_adaptor/UnrealClient/step_handlers/unreal_custom_step_handler.py` & `deadline_cloud_for_unreal_engine-0.2.1/src/deadline/unreal_adaptor/UnrealClient/step_handlers/unreal_custom_step_handler.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_unreal_engine-0.2.0/src/deadline/unreal_adaptor/UnrealClient/step_handlers/unreal_render_step_handler.py` & `deadline_cloud_for_unreal_engine-0.2.1/src/deadline/unreal_adaptor/UnrealClient/step_handlers/unreal_render_step_handler.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_unreal_engine-0.2.0/src/deadline/unreal_submitter/common.py` & `deadline_cloud_for_unreal_engine-0.2.1/src/deadline/unreal_submitter/common.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_unreal_engine-0.2.0/src/deadline/unreal_submitter/submitter.py` & `deadline_cloud_for_unreal_engine-0.2.1/src/deadline/unreal_submitter/submitter.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_unreal_engine-0.2.0/src/deadline/unreal_submitter/templates/default_unreal_job_template_v04.yaml` & `deadline_cloud_for_unreal_engine-0.2.1/src/deadline/unreal_submitter/templates/default_unreal_job_template_v04.yaml`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_unreal_engine-0.2.0/src/deadline/unreal_submitter/templates/default_unreal_job_template_v06.yaml` & `deadline_cloud_for_unreal_engine-0.2.1/src/deadline/unreal_submitter/templates/default_unreal_job_template_v06.yaml`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_unreal_engine-0.2.0/src/deadline/unreal_submitter/templates/default_unreal_step_template_v04.yaml` & `deadline_cloud_for_unreal_engine-0.2.1/src/deadline/unreal_submitter/templates/default_unreal_step_template_v04.yaml`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_unreal_engine-0.2.0/src/deadline/unreal_submitter/templates/default_unreal_step_template_v05.yaml` & `deadline_cloud_for_unreal_engine-0.2.1/src/deadline/unreal_submitter/templates/default_unreal_step_template_v05.yaml`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_unreal_engine-0.2.0/src/deadline/unreal_submitter/unreal_dependency_collector/collector.py` & `deadline_cloud_for_unreal_engine-0.2.1/src/deadline/unreal_submitter/unreal_dependency_collector/collector.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_unreal_engine-0.2.0/src/deadline/unreal_submitter/unreal_dependency_collector/common.py` & `deadline_cloud_for_unreal_engine-0.2.1/src/deadline/unreal_submitter/unreal_dependency_collector/common.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_unreal_engine-0.2.0/src/deadline/unreal_submitter/unreal_dependency_collector/dependency_search_options.py` & `deadline_cloud_for_unreal_engine-0.2.1/src/deadline/unreal_submitter/unreal_dependency_collector/dependency_search_options.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_unreal_engine-0.2.0/src/deadline/unreal_submitter/unreal_open_job/job_step.py` & `deadline_cloud_for_unreal_engine-0.2.1/src/deadline/unreal_submitter/unreal_open_job/job_step.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_unreal_engine-0.2.0/src/deadline/unreal_submitter/unreal_open_job/open_job_description.py` & `deadline_cloud_for_unreal_engine-0.2.1/src/deadline/unreal_submitter/unreal_open_job/open_job_description.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/DEVELOPMENT.md` & `deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/DEVELOPMENT.md`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/LICENSE` & `deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/LICENSE`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/README.md` & `deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/README.md`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/UnrealDeadlineCloudService.uplugin` & `deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/UnrealDeadlineCloudService.uplugin`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/Config/DefaultUnrealDeadlineCloudService.ini` & `deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/Config/DefaultUnrealDeadlineCloudService.ini`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/Content/Python/init_unreal.py` & `deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/Content/Python/init_unreal.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/Content/Python/job_library.py` & `deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/Content/Python/job_library.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/Content/Python/remote_executor.py` & `deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/Content/Python/remote_executor.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/Content/Python/settings.py` & `deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/Content/Python/settings.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/Documentation/Doxyfile` & `deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/Documentation/Doxyfile`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/Documentation/doxygen-awesome-sidebar-only.css` & `deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/Documentation/doxygen-awesome-sidebar-only.css`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/Documentation/doxygen-awesome.LICENSE` & `deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/Documentation/doxygen-awesome.LICENSE`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/Documentation/doxygen-awesome.css` & `deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/Documentation/doxygen-awesome.css`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/Source/UnrealDeadlineCloudService/UnrealDeadlineCloudService.Build.cs` & `deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/Source/UnrealDeadlineCloudService/UnrealDeadlineCloudService.Build.cs`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/Source/UnrealDeadlineCloudService/Private/UnrealDeadlineCloudServiceModule.cpp` & `deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/Source/UnrealDeadlineCloudService/Private/UnrealDeadlineCloudServiceModule.cpp`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/Source/UnrealDeadlineCloudService/Private/DeadlineCloudJobSettings/DeadlineCloudDeveloperSettings.cpp` & `deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/Source/UnrealDeadlineCloudService/Private/DeadlineCloudJobSettings/DeadlineCloudDeveloperSettings.cpp`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/Source/UnrealDeadlineCloudService/Private/DeadlineCloudJobSettings/DeadlineCloudJobDataAsset.cpp` & `deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/Source/UnrealDeadlineCloudService/Private/DeadlineCloudJobSettings/DeadlineCloudJobDataAsset.cpp`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/Source/UnrealDeadlineCloudService/Private/DeadlineCloudJobSettings/DeadlineCloudJobPresetDetailsCustomization.cpp` & `deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/Source/UnrealDeadlineCloudService/Private/DeadlineCloudJobSettings/DeadlineCloudJobPresetDetailsCustomization.cpp`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/Source/UnrealDeadlineCloudService/Private/DeadlineCloudJobSettings/DeadlineCloudSettingsDetails.cpp` & `deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/Source/UnrealDeadlineCloudService/Private/DeadlineCloudJobSettings/DeadlineCloudSettingsDetails.cpp`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/Source/UnrealDeadlineCloudService/Private/DeadlineCloudJobSettings/DeadlineCloudStatusHandler.cpp` & `deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/Source/UnrealDeadlineCloudService/Private/DeadlineCloudJobSettings/DeadlineCloudStatusHandler.cpp`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/Source/UnrealDeadlineCloudService/Private/MovieRenderPipeline/DeadlineCloudStepBaseSetting.cpp` & `deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/Source/UnrealDeadlineCloudService/Private/MovieRenderPipeline/DeadlineCloudStepBaseSetting.cpp`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/Source/UnrealDeadlineCloudService/Private/MovieRenderPipeline/MoviePipelineDeadlineCloudExecutorJob.cpp` & `deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/Source/UnrealDeadlineCloudService/Private/MovieRenderPipeline/MoviePipelineDeadlineCloudExecutorJob.cpp`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/Source/UnrealDeadlineCloudService/Public/UnrealDeadlineCloudServiceModule.h` & `deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/Source/UnrealDeadlineCloudService/Public/UnrealDeadlineCloudServiceModule.h`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/Source/UnrealDeadlineCloudService/Public/DeadlineCloudJobSettings/DeadlineCloudDeveloperSettings.h` & `deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/Source/UnrealDeadlineCloudService/Public/DeadlineCloudJobSettings/DeadlineCloudDeveloperSettings.h`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/Source/UnrealDeadlineCloudService/Public/DeadlineCloudJobSettings/DeadlineCloudJobDataAsset.h` & `deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/Source/UnrealDeadlineCloudService/Public/DeadlineCloudJobSettings/DeadlineCloudJobDataAsset.h`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/Source/UnrealDeadlineCloudService/Public/DeadlineCloudJobSettings/DeadlineCloudJobPresetDetailsCustomization.h` & `deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/Source/UnrealDeadlineCloudService/Public/DeadlineCloudJobSettings/DeadlineCloudJobPresetDetailsCustomization.h`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/Source/UnrealDeadlineCloudService/Public/DeadlineCloudJobSettings/DeadlineCloudSettingsDetails.h` & `deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/Source/UnrealDeadlineCloudService/Public/DeadlineCloudJobSettings/DeadlineCloudSettingsDetails.h`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/Source/UnrealDeadlineCloudService/Public/DeadlineCloudJobSettings/DeadlineCloudStatusHandler.h` & `deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/Source/UnrealDeadlineCloudService/Public/DeadlineCloudJobSettings/DeadlineCloudStatusHandler.h`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/Source/UnrealDeadlineCloudService/Public/MovieRenderPipeline/DeadlineCloudCustomScriptStepSetting.h` & `deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/Source/UnrealDeadlineCloudService/Public/MovieRenderPipeline/DeadlineCloudCustomScriptStepSetting.h`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/Source/UnrealDeadlineCloudService/Public/MovieRenderPipeline/DeadlineCloudRenderStepSetting.h` & `deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/Source/UnrealDeadlineCloudService/Public/MovieRenderPipeline/DeadlineCloudRenderStepSetting.h`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/Source/UnrealDeadlineCloudService/Public/MovieRenderPipeline/DeadlineCloudStepBaseSetting.h` & `deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/Source/UnrealDeadlineCloudService/Public/MovieRenderPipeline/DeadlineCloudStepBaseSetting.h`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/Source/UnrealDeadlineCloudService/Public/MovieRenderPipeline/MoviePipelineDeadlineCloudExecutorJob.h` & `deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/Source/UnrealDeadlineCloudService/Public/MovieRenderPipeline/MoviePipelineDeadlineCloudExecutorJob.h`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/Source/UnrealDeadlineCloudService/Public/PythonAPILibraries/DeadlineCloudJobBundleLibrary.h` & `deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/Source/UnrealDeadlineCloudService/Public/PythonAPILibraries/DeadlineCloudJobBundleLibrary.h`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/Source/UnrealDeadlineCloudService/Public/PythonAPILibraries/PythonAPILibrary.h` & `deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/Source/UnrealDeadlineCloudService/Public/PythonAPILibraries/PythonAPILibrary.h`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_unreal_engine-0.2.0/src/unreal_plugin/Source/UnrealDeadlineCloudService/Public/PythonAPILibraries/PythonGameThreadExecutor.h` & `deadline_cloud_for_unreal_engine-0.2.1/src/unreal_plugin/Source/UnrealDeadlineCloudService/Public/PythonAPILibraries/PythonGameThreadExecutor.h`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_unreal_engine-0.2.0/.gitignore` & `deadline_cloud_for_unreal_engine-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_unreal_engine-0.2.0/LICENSE` & `deadline_cloud_for_unreal_engine-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_unreal_engine-0.2.0/README.md` & `deadline_cloud_for_unreal_engine-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_unreal_engine-0.2.0/hatch.toml` & `deadline_cloud_for_unreal_engine-0.2.1/hatch.toml`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_unreal_engine-0.2.0/pyproject.toml` & `deadline_cloud_for_unreal_engine-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
   "Operating System :: Microsoft :: Windows",
   "License :: OSI Approved :: Apache Software License",
   "Intended Audience :: Developers",
   "Intended Audience :: End Users/Desktop"
 ]
 
 dependencies = [
-    "deadline == 0.47.*",
+    "deadline == 0.48.*",
     "openjd-adaptor-runtime == 0.7.*",
 ]
 
 [project.urls]
 Homepage = "https://github.com/aws-deadline/deadline-cloud-for-unreal-engine"
 Source = "https://github.com/aws-deadline/deadline-cloud-for-unreal-engine"
```

### Comparing `deadline_cloud_for_unreal_engine-0.2.0/PKG-INFO` & `deadline_cloud_for_unreal_engine-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: deadline-cloud-for-unreal-engine
-Version: 0.2.0
+Version: 0.2.1
 Summary: AWS Deadline Cloud for Unreal Engine
 Project-URL: Homepage, https://github.com/aws-deadline/deadline-cloud-for-unreal-engine
 Project-URL: Source, https://github.com/aws-deadline/deadline-cloud-for-unreal-engine
 Author: Amazon Web Services
 License-Expression: Apache-2.0
 License-File: LICENSE
 License-File: NOTICE
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
-Requires-Dist: deadline==0.47.*
+Requires-Dist: deadline==0.48.*
 Requires-Dist: openjd-adaptor-runtime==0.7.*
 Description-Content-Type: text/markdown
 
 # AWS Deadline Cloud for Unreal Engine
 
 [![pypi](https://img.shields.io/pypi/v/deadline-cloud-for-unreal-engine.svg?style=flat)](https://pypi.python.org/pypi/deadline-cloud-for-unreal-engine)
 [![python](https://img.shields.io/pypi/pyversions/deadline-cloud-for-unreal-engine.svg?style=flat)](https://pypi.python.org/pypi/deadline-cloud-for-unreal-engine)
```

