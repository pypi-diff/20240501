# Comparing `tmp/deadline_cloud_worker_agent-0.27.0.tar.gz` & `tmp/deadline_cloud_worker_agent-0.27.1.tar.gz`

## Comparing `deadline_cloud_worker_agent-0.27.0.tar` & `deadline_cloud_worker_agent-0.27.1.tar`

### file list

```diff
@@ -1,80 +1,80 @@
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/_version.py
--rw-r--r--   0        0        0     5654 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/hatch_version_hook.py
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/__init__.py
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/__main__.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/_version.py
--rw-r--r--   0        0        0    11897 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/api_models.py
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/errors.py
--rw-r--r--   0        0        0     6205 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/file_system_operations.py
--rw-r--r--   0        0        0    19728 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/log_messages.py
--rw-r--r--   0        0        0     4433 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/metrics.py
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/progress.py
--rw-r--r--   0        0        0    21274 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/session_events.py
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/utils.py
--rw-r--r--   0        0        0    20244 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/worker.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/aws/__init__.py
--rw-r--r--   0        0        0    36140 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/aws/deadline/__init__.py
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/aws_credentials/__init__.py
--rw-r--r--   0        0        0     7198 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/aws_credentials/aws_configs.py
--rw-r--r--   0        0        0     6313 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/aws_credentials/boto3_sessions.py
--rw-r--r--   0        0        0     8937 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/aws_credentials/credentials_refresher.py
--rw-r--r--   0        0        0    23258 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/aws_credentials/queue_boto3_session.py
--rw-r--r--   0        0        0     9018 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/aws_credentials/temporary_credentials.py
--rw-r--r--   0        0        0     4957 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/aws_credentials/worker_boto3_session.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/boto/__init__.py
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/boto/config.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/boto/logger.py
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/boto/retries.py
--rw-r--r--   0        0        0    18821 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/boto/shim.py
--rw-r--r--   0        0        0     9301 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/installer/__init__.py
--rwxr-xr-x   0        0        0    18766 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/installer/install.sh
--rw-r--r--   0        0        0    38437 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/installer/win_installer.py
--rw-r--r--   0        0        0    12555 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/installer/worker.toml.example
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/log_sync/__init__.py
--rw-r--r--   0        0        0    27033 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/log_sync/cloudwatch.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/log_sync/loggers.py
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/scheduler/__init__.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/scheduler/log.py
--rw-r--r--   0        0        0    64684 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/scheduler/scheduler.py
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/scheduler/session_action_status.py
--rw-r--r--   0        0        0     6914 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/scheduler/session_cleanup.py
--rw-r--r--   0        0        0    19792 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/scheduler/session_queue.py
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/sessions/__init__.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/sessions/active_action.py
--rw-r--r--   0        0        0     2283 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/sessions/errors.py
--rw-r--r--   0        0        0    10611 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/sessions/log_config.py
--rw-r--r--   0        0        0    54231 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/sessions/session.py
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/sessions/actions/__init__.py
--rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/sessions/actions/action_definition.py
--rw-r--r--   0        0        0     3595 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/sessions/actions/enter_env.py
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/sessions/actions/exit_env.py
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/sessions/actions/openjd_action.py
--rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/sessions/actions/run_step_task.py
--rw-r--r--   0        0        0     5962 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/sessions/actions/sync_input_job_attachments.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/sessions/job_entities/__init__.py
--rw-r--r--   0        0        0     3149 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/sessions/job_entities/environment_details.py
--rw-r--r--   0        0        0     6166 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/sessions/job_entities/job_attachment_details.py
--rw-r--r--   0        0        0    18435 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/sessions/job_entities/job_details.py
--rw-r--r--   0        0        0    15220 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/sessions/job_entities/job_entities.py
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/sessions/job_entities/job_entity_type.py
--rw-r--r--   0        0        0     4587 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/sessions/job_entities/step_details.py
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/sessions/job_entities/validation.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/startup/__init__.py
--rw-r--r--   0        0        0    20997 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/startup/bootstrap.py
--rw-r--r--   0        0        0     8344 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/startup/capabilities.py
--rw-r--r--   0        0        0     4861 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/startup/cli_args.py
--rw-r--r--   0        0        0    10967 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/startup/config.py
--rw-r--r--   0        0        0     6108 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/startup/config_file.py
--rw-r--r--   0        0        0    16187 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/startup/entrypoint.py
--rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/startup/host_properties.py
--rw-r--r--   0        0        0     8384 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/startup/settings.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/windows/__init__.py
--rw-r--r--   0        0        0    12818 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/windows/win_credentials_resolver.py
--rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/windows/win_service.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/.gitignore
--rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/LICENSE
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/NOTICE
--rw-r--r--   0        0        0     7110 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/README.md
--rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/hatch.toml
--rw-r--r--   0        0        0     6460 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/pyproject.toml
--rw-r--r--   0        0        0     8558 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.0/PKG-INFO
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/_version.py
+-rw-r--r--   0        0        0     5654 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/hatch_version_hook.py
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/__init__.py
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/__main__.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/_version.py
+-rw-r--r--   0        0        0    11897 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/api_models.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/errors.py
+-rw-r--r--   0        0        0     6205 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/file_system_operations.py
+-rw-r--r--   0        0        0    19728 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/log_messages.py
+-rw-r--r--   0        0        0     4433 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/metrics.py
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/progress.py
+-rw-r--r--   0        0        0    21274 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/session_events.py
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/utils.py
+-rw-r--r--   0        0        0    20244 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/worker.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/aws/__init__.py
+-rw-r--r--   0        0        0    36140 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/aws/deadline/__init__.py
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/aws_credentials/__init__.py
+-rw-r--r--   0        0        0     7198 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/aws_credentials/aws_configs.py
+-rw-r--r--   0        0        0     6313 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/aws_credentials/boto3_sessions.py
+-rw-r--r--   0        0        0     8937 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/aws_credentials/credentials_refresher.py
+-rw-r--r--   0        0        0    23258 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/aws_credentials/queue_boto3_session.py
+-rw-r--r--   0        0        0     9018 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/aws_credentials/temporary_credentials.py
+-rw-r--r--   0        0        0     4957 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/aws_credentials/worker_boto3_session.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/boto/__init__.py
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/boto/config.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/boto/logger.py
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/boto/retries.py
+-rw-r--r--   0        0        0    18821 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/boto/shim.py
+-rw-r--r--   0        0        0     9301 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/installer/__init__.py
+-rwxr-xr-x   0        0        0    18766 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/installer/install.sh
+-rw-r--r--   0        0        0    38437 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/installer/win_installer.py
+-rw-r--r--   0        0        0    12555 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/installer/worker.toml.example
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/log_sync/__init__.py
+-rw-r--r--   0        0        0    27033 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/log_sync/cloudwatch.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/log_sync/loggers.py
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/scheduler/__init__.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/scheduler/log.py
+-rw-r--r--   0        0        0    64684 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/scheduler/scheduler.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/scheduler/session_action_status.py
+-rw-r--r--   0        0        0     6914 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/scheduler/session_cleanup.py
+-rw-r--r--   0        0        0    19792 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/scheduler/session_queue.py
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/sessions/__init__.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/sessions/active_action.py
+-rw-r--r--   0        0        0     2283 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/sessions/errors.py
+-rw-r--r--   0        0        0    10611 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/sessions/log_config.py
+-rw-r--r--   0        0        0    54231 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/sessions/session.py
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/sessions/actions/__init__.py
+-rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/sessions/actions/action_definition.py
+-rw-r--r--   0        0        0     3595 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/sessions/actions/enter_env.py
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/sessions/actions/exit_env.py
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/sessions/actions/openjd_action.py
+-rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/sessions/actions/run_step_task.py
+-rw-r--r--   0        0        0     5962 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/sessions/actions/sync_input_job_attachments.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/sessions/job_entities/__init__.py
+-rw-r--r--   0        0        0     3149 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/sessions/job_entities/environment_details.py
+-rw-r--r--   0        0        0     6166 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/sessions/job_entities/job_attachment_details.py
+-rw-r--r--   0        0        0    18435 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/sessions/job_entities/job_details.py
+-rw-r--r--   0        0        0    15220 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/sessions/job_entities/job_entities.py
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/sessions/job_entities/job_entity_type.py
+-rw-r--r--   0        0        0     4587 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/sessions/job_entities/step_details.py
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/sessions/job_entities/validation.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/startup/__init__.py
+-rw-r--r--   0        0        0    20997 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/startup/bootstrap.py
+-rw-r--r--   0        0        0     8344 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/startup/capabilities.py
+-rw-r--r--   0        0        0     4861 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/startup/cli_args.py
+-rw-r--r--   0        0        0    10967 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/startup/config.py
+-rw-r--r--   0        0        0     6108 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/startup/config_file.py
+-rw-r--r--   0        0        0    16187 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/startup/entrypoint.py
+-rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/startup/host_properties.py
+-rw-r--r--   0        0        0     8384 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/startup/settings.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/windows/__init__.py
+-rw-r--r--   0        0        0    12818 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/windows/win_credentials_resolver.py
+-rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/windows/win_service.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/.gitignore
+-rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/LICENSE
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/NOTICE
+-rw-r--r--   0        0        0     7110 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/README.md
+-rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/hatch.toml
+-rw-r--r--   0        0        0     6460 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/pyproject.toml
+-rw-r--r--   0        0        0     8558 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.27.1/PKG-INFO
```

### Comparing `deadline_cloud_worker_agent-0.27.0/hatch_version_hook.py` & `deadline_cloud_worker_agent-0.27.1/hatch_version_hook.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/api_models.py` & `deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/api_models.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/file_system_operations.py` & `deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/file_system_operations.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/log_messages.py` & `deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/log_messages.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/metrics.py` & `deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/metrics.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/progress.py` & `deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/progress.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/session_events.py` & `deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/session_events.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/utils.py` & `deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/utils.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/worker.py` & `deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/worker.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/aws/deadline/__init__.py` & `deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/aws/deadline/__init__.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/aws_credentials/aws_configs.py` & `deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/aws_credentials/aws_configs.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/aws_credentials/boto3_sessions.py` & `deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/aws_credentials/boto3_sessions.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/aws_credentials/credentials_refresher.py` & `deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/aws_credentials/credentials_refresher.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/aws_credentials/queue_boto3_session.py` & `deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/aws_credentials/queue_boto3_session.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/aws_credentials/temporary_credentials.py` & `deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/aws_credentials/temporary_credentials.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/aws_credentials/worker_boto3_session.py` & `deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/aws_credentials/worker_boto3_session.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/boto/config.py` & `deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/boto/config.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/boto/retries.py` & `deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/boto/retries.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/boto/shim.py` & `deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/boto/shim.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/installer/__init__.py` & `deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/installer/__init__.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/installer/install.sh` & `deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/installer/install.sh`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/installer/win_installer.py` & `deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/installer/win_installer.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/installer/worker.toml.example` & `deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/installer/worker.toml.example`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/log_sync/cloudwatch.py` & `deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/log_sync/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/scheduler/scheduler.py` & `deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/scheduler/session_action_status.py` & `deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/scheduler/session_action_status.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/scheduler/session_cleanup.py` & `deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/scheduler/session_cleanup.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/scheduler/session_queue.py` & `deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/scheduler/session_queue.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/sessions/errors.py` & `deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/sessions/errors.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/sessions/log_config.py` & `deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/sessions/log_config.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/sessions/session.py` & `deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/sessions/session.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/sessions/actions/__init__.py` & `deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/sessions/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/sessions/actions/action_definition.py` & `deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/sessions/actions/action_definition.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/sessions/actions/enter_env.py` & `deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/sessions/actions/enter_env.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/sessions/actions/exit_env.py` & `deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/sessions/actions/exit_env.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/sessions/actions/openjd_action.py` & `deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/sessions/actions/openjd_action.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/sessions/actions/run_step_task.py` & `deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/sessions/actions/run_step_task.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/sessions/actions/sync_input_job_attachments.py` & `deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/sessions/actions/sync_input_job_attachments.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/sessions/job_entities/environment_details.py` & `deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/sessions/job_entities/environment_details.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/sessions/job_entities/job_attachment_details.py` & `deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/sessions/job_entities/job_attachment_details.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/sessions/job_entities/job_details.py` & `deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/sessions/job_entities/job_details.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/sessions/job_entities/job_entities.py` & `deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/sessions/job_entities/job_entities.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/sessions/job_entities/step_details.py` & `deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/sessions/job_entities/step_details.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/sessions/job_entities/validation.py` & `deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/sessions/job_entities/validation.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/startup/bootstrap.py` & `deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/startup/bootstrap.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/startup/capabilities.py` & `deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/startup/capabilities.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/startup/cli_args.py` & `deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/startup/cli_args.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/startup/config.py` & `deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/startup/config.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/startup/config_file.py` & `deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/startup/config_file.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/startup/entrypoint.py` & `deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/startup/entrypoint.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/startup/host_properties.py` & `deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/startup/host_properties.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/startup/settings.py` & `deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/startup/settings.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/windows/win_credentials_resolver.py` & `deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/windows/win_credentials_resolver.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.27.0/src/deadline_worker_agent/windows/win_service.py` & `deadline_cloud_worker_agent-0.27.1/src/deadline_worker_agent/windows/win_service.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.27.0/LICENSE` & `deadline_cloud_worker_agent-0.27.1/LICENSE`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.27.0/README.md` & `deadline_cloud_worker_agent-0.27.1/README.md`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.27.0/hatch.toml` & `deadline_cloud_worker_agent-0.27.1/hatch.toml`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.27.0/pyproject.toml` & `deadline_cloud_worker_agent-0.27.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 ]
 dynamic = ["version"]
 readme = "README.md"
 license = "Apache-2.0"
 dependencies = [
     "requests ~= 2.31",
     "boto3 >= 1.34.75",
-    "deadline == 0.47.*",
+    "deadline == 0.48.*",
     "openjd-sessions == 0.7.*",
     # tomli became tomllib in standard library in Python 3.11
     "tomli == 2.0.* ; python_version<'3.11'",
     "typing_extensions ~= 4.8",
     "psutil ~= 5.9",
     "pydantic ~= 1.10.0",
     "pywin32 == 306; platform_system == 'Windows'",
```

### Comparing `deadline_cloud_worker_agent-0.27.0/PKG-INFO` & `deadline_cloud_worker_agent-0.27.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: deadline-cloud-worker-agent
-Version: 0.27.0
+Version: 0.27.1
 Summary: The AWS Deadline Cloud worker agent can be used to run a worker in an AWS Deadline Cloud fleet
 Project-URL: Homepage, https://github.com/aws-deadline/deadline-cloud-worker-agent
 Project-URL: Source, https://github.com/aws-deadline/deadline-cloud-worker-agent
 Author: Amazon Web Services
 License-Expression: Apache-2.0
 License-File: LICENSE
 License-File: NOTICE
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
 Requires-Dist: boto3>=1.34.75
-Requires-Dist: deadline==0.47.*
+Requires-Dist: deadline==0.48.*
 Requires-Dist: openjd-sessions==0.7.*
 Requires-Dist: psutil~=5.9
 Requires-Dist: pydantic~=1.10.0
 Requires-Dist: pywin32==306; platform_system == 'Windows'
 Requires-Dist: requests==2.31.*
 Requires-Dist: requests~=2.31
 Requires-Dist: tomli==2.0.*; python_version < '3.11'
```

