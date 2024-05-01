# Comparing `tmp/awxkit-24.3.0.tar.gz` & `tmp/awxkit-24.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awxkit-24.3.0.tar", last modified: Tue Apr 23 19:12:39 2024, max compression
+gzip compressed data, was "awxkit-24.3.1.tar", last modified: Wed May  1 01:25:36 2024, max compression
```

## Comparing `awxkit-24.3.0.tar` & `awxkit-24.3.1.tar`

### file list

```diff
@@ -1,131 +1,131 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:12:39.739015 awxkit-24.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-23 19:12:19.000000 awxkit-24.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-23 19:12:19.000000 awxkit-24.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-23 19:12:39.739015 awxkit-24.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-23 19:12:19.000000 awxkit-24.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:12:39.723015 awxkit-24.3.0/awxkit/
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:12:39.723015 awxkit-24.3.0/awxkit/api/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5147 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/api/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:12:39.727015 awxkit-24.3.0/awxkit/api/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/api/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/api/mixins/has_copy.py
--rw-r--r--   0 runner    (1001) docker     (127)    16885 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/api/mixins/has_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/api/mixins/has_instance_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/api/mixins/has_notifications.py
--rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/api/mixins/has_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/api/mixins/has_survey.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/api/mixins/has_variables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:12:39.735015 awxkit-24.3.0/awxkit/api/pages/
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/api/pages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/api/pages/access_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/api/pages/activity_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/api/pages/ad_hoc_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)    18321 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/api/pages/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3275 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/api/pages/applications.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/api/pages/authtoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     9208 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/api/pages/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/api/pages/bulk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/api/pages/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/api/pages/credential_input_sources.py
--rw-r--r--   0 runner    (1001) docker     (127)    11525 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/api/pages/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/api/pages/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/api/pages/execution_environments.py
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/api/pages/host_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/api/pages/instance_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/api/pages/instances.py
--rw-r--r--   0 runner    (1001) docker     (127)    15890 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/api/pages/inventory.py
--rw-r--r--   0 runner    (1001) docker     (127)     7231 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/api/pages/job_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/api/pages/jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/api/pages/labels.py
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/api/pages/mesh_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/api/pages/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     7775 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/api/pages/notification_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/api/pages/notifications.py
--rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/api/pages/organizations.py
--rw-r--r--   0 runner    (1001) docker     (127)    20193 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/api/pages/page.py
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/api/pages/ping.py
--rw-r--r--   0 runner    (1001) docker     (127)     5965 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/api/pages/projects.py
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/api/pages/roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/api/pages/schedules.py
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/api/pages/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/api/pages/subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/api/pages/survey_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/api/pages/system_job_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/api/pages/system_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/api/pages/teams.py
--rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/api/pages/unified_job_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     6767 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/api/pages/unified_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/api/pages/users.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/api/pages/workflow_approval_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/api/pages/workflow_approvals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/api/pages/workflow_job_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5257 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/api/pages/workflow_job_template_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/api/pages/workflow_job_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/api/pages/workflow_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6687 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/api/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    15692 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/api/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:12:39.735015 awxkit-24.3.0/awxkit/awx/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/awx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4982 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/awx/inventory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/awx/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:12:39.735015 awxkit-24.3.0/awxkit/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/cli/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12767 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/cli/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    20311 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/cli/custom.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:12:39.735015 awxkit-24.3.0/awxkit/cli/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/cli/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/cli/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/cli/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:12:39.735015 awxkit-24.3.0/awxkit/cli/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/cli/docs/source/authentication.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/cli/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/cli/docs/source/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/cli/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/cli/docs/source/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/cli/docs/source/output.rst
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/cli/docs/source/reference.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/cli/docs/source/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6642 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/cli/format.py
--rw-r--r--   0 runner    (1001) docker     (127)    12584 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/cli/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     8793 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/cli/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/cli/sphinx.py
--rw-r--r--   0 runner    (1001) docker     (127)     3870 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/cli/stdout.py
--rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:12:39.739015 awxkit-24.3.0/awxkit/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3693 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/scripts/basic_session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:12:39.739015 awxkit-24.3.0/awxkit/utils/
--rw-r--r--   0 runner    (1001) docker     (127)    12963 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/utils/toposort.py
--rw-r--r--   0 runner    (1001) docker     (127)    21486 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/words.py
--rw-r--r--   0 runner    (1001) docker     (127)     9107 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/ws.py
--rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-04-23 19:12:19.000000 awxkit-24.3.0/awxkit/yaml_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:12:39.739015 awxkit-24.3.0/awxkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-23 19:12:39.000000 awxkit-24.3.0/awxkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-04-23 19:12:39.000000 awxkit-24.3.0/awxkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:12:39.000000 awxkit-24.3.0/awxkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-23 19:12:39.000000 awxkit-24.3.0/awxkit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-23 19:12:39.000000 awxkit-24.3.0/awxkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-23 19:12:39.000000 awxkit-24.3.0/awxkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-23 19:12:19.000000 awxkit-24.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 19:12:39.739015 awxkit-24.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-04-23 19:12:19.000000 awxkit-24.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:12:39.739015 awxkit-24.3.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:12:19.000000 awxkit-24.3.0/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:12:39.739015 awxkit-24.3.0/test/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-23 19:12:19.000000 awxkit-24.3.0/test/cli/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3554 2024-04-23 19:12:19.000000 awxkit-24.3.0/test/cli/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-23 19:12:19.000000 awxkit-24.3.0/test/cli/test_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     6872 2024-04-23 19:12:19.000000 awxkit-24.3.0/test/cli/test_options.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:12:19.000000 awxkit-24.3.0/test/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-23 19:12:19.000000 awxkit-24.3.0/test/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    21943 2024-04-23 19:12:19.000000 awxkit-24.3.0/test/test_dependency_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     9169 2024-04-23 19:12:19.000000 awxkit-24.3.0/test/test_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    13409 2024-04-23 19:12:19.000000 awxkit-24.3.0/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-23 19:12:19.000000 awxkit-24.3.0/test/test_ws.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-23 19:12:19.000000 awxkit-24.3.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:25:36.661775 awxkit-24.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-01 01:25:23.000000 awxkit-24.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-01 01:25:23.000000 awxkit-24.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-01 01:25:36.661775 awxkit-24.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-01 01:25:23.000000 awxkit-24.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:25:36.645775 awxkit-24.3.1/awxkit/
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:25:36.645775 awxkit-24.3.1/awxkit/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5147 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/api/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:25:36.649775 awxkit-24.3.1/awxkit/api/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/api/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/api/mixins/has_copy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16885 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/api/mixins/has_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/api/mixins/has_instance_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/api/mixins/has_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/api/mixins/has_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/api/mixins/has_survey.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/api/mixins/has_variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:25:36.657775 awxkit-24.3.1/awxkit/api/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/api/pages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/api/pages/access_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/api/pages/activity_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/api/pages/ad_hoc_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18164 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/api/pages/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3275 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/api/pages/applications.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/api/pages/authtoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9208 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/api/pages/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/api/pages/bulk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/api/pages/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/api/pages/credential_input_sources.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11525 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/api/pages/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/api/pages/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/api/pages/execution_environments.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/api/pages/host_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/api/pages/instance_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/api/pages/instances.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15890 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/api/pages/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7231 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/api/pages/job_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/api/pages/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/api/pages/labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/api/pages/mesh_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/api/pages/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7775 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/api/pages/notification_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/api/pages/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/api/pages/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21450 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/api/pages/page.py
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/api/pages/ping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5965 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/api/pages/projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/api/pages/roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/api/pages/schedules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/api/pages/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/api/pages/subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/api/pages/survey_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/api/pages/system_job_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/api/pages/system_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/api/pages/teams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/api/pages/unified_job_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6767 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/api/pages/unified_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/api/pages/users.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/api/pages/workflow_approval_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/api/pages/workflow_approvals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/api/pages/workflow_job_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5257 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/api/pages/workflow_job_template_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/api/pages/workflow_job_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/api/pages/workflow_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6687 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/api/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15692 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/api/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:25:36.657775 awxkit-24.3.1/awxkit/awx/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/awx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4982 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/awx/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/awx/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:25:36.657775 awxkit-24.3.1/awxkit/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/cli/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12767 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/cli/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20311 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/cli/custom.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:25:36.657775 awxkit-24.3.1/awxkit/cli/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/cli/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/cli/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/cli/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:25:36.657775 awxkit-24.3.1/awxkit/cli/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/cli/docs/source/authentication.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/cli/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/cli/docs/source/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/cli/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/cli/docs/source/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/cli/docs/source/output.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/cli/docs/source/reference.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/cli/docs/source/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6642 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/cli/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12584 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/cli/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8793 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/cli/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/cli/sphinx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3870 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/cli/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:25:36.657775 awxkit-24.3.1/awxkit/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3693 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/scripts/basic_session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:25:36.661775 awxkit-24.3.1/awxkit/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)    12963 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/utils/toposort.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21486 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/words.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9107 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/ws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-05-01 01:25:23.000000 awxkit-24.3.1/awxkit/yaml_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:25:36.661775 awxkit-24.3.1/awxkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-01 01:25:36.000000 awxkit-24.3.1/awxkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-05-01 01:25:36.000000 awxkit-24.3.1/awxkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 01:25:36.000000 awxkit-24.3.1/awxkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-01 01:25:36.000000 awxkit-24.3.1/awxkit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-01 01:25:36.000000 awxkit-24.3.1/awxkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-01 01:25:36.000000 awxkit-24.3.1/awxkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-01 01:25:23.000000 awxkit-24.3.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 01:25:36.661775 awxkit-24.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-05-01 01:25:23.000000 awxkit-24.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:25:36.661775 awxkit-24.3.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 01:25:23.000000 awxkit-24.3.1/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:25:36.661775 awxkit-24.3.1/test/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-01 01:25:23.000000 awxkit-24.3.1/test/cli/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3554 2024-05-01 01:25:23.000000 awxkit-24.3.1/test/cli/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-05-01 01:25:23.000000 awxkit-24.3.1/test/cli/test_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6872 2024-05-01 01:25:23.000000 awxkit-24.3.1/test/cli/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 01:25:23.000000 awxkit-24.3.1/test/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-05-01 01:25:23.000000 awxkit-24.3.1/test/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21943 2024-05-01 01:25:23.000000 awxkit-24.3.1/test/test_dependency_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9169 2024-05-01 01:25:23.000000 awxkit-24.3.1/test/test_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13409 2024-05-01 01:25:23.000000 awxkit-24.3.1/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-01 01:25:23.000000 awxkit-24.3.1/test/test_ws.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-01 01:25:23.000000 awxkit-24.3.1/tox.ini
```

### Comparing `awxkit-24.3.0/.gitignore` & `awxkit-24.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/PKG-INFO` & `awxkit-24.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awxkit
-Version: 24.3.0
+Version: 24.3.1
 Summary: The official command line interface for Ansible AWX
 Home-page: https://github.com/ansible/awx
 Author: Red Hat, Inc.
 Author-email: info@ansible.com
 License: Apache 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `awxkit-24.3.0/awxkit/api/client.py` & `awxkit-24.3.1/awxkit/api/client.py`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/awxkit/api/mixins/has_create.py` & `awxkit-24.3.1/awxkit/api/mixins/has_create.py`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/awxkit/api/mixins/has_instance_groups.py` & `awxkit-24.3.1/awxkit/api/mixins/has_instance_groups.py`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/awxkit/api/mixins/has_notifications.py` & `awxkit-24.3.1/awxkit/api/mixins/has_notifications.py`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/awxkit/api/mixins/has_status.py` & `awxkit-24.3.1/awxkit/api/mixins/has_status.py`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/awxkit/api/mixins/has_survey.py` & `awxkit-24.3.1/awxkit/api/mixins/has_survey.py`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/awxkit/api/pages/__init__.py` & `awxkit-24.3.1/awxkit/api/pages/__init__.py`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/awxkit/api/pages/ad_hoc_commands.py` & `awxkit-24.3.1/awxkit/api/pages/ad_hoc_commands.py`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/awxkit/api/pages/api.py` & `awxkit-24.3.1/awxkit/api/pages/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -230,15 +230,15 @@
                 identifier = 'or__id'
             else:
                 identifier = 'or__' + identifier
 
         return endpoint.get(**{identifier: value}, all_pages=True)
 
     def export_assets(self, **kwargs):
-        self._cache = page.PageCache()
+        self._cache = page.PageCache(self.connection)
 
         # If no resource kwargs are explicitly used, export everything.
         all_resources = all(kwargs.get(resource) is None for resource in EXPORTABLE_RESOURCES)
 
         data = {}
         for resource in EXPORTABLE_RESOURCES:
             value = kwargs.get(resource)
@@ -331,15 +331,15 @@
             # Queue up everything related to be either created or assigned.
             for name, S in asset.get('related', {}).items():
                 if not S:
                     continue
                 if name == 'roles':
                     indexed_roles = defaultdict(list)
                     for role in S:
-                        if 'content_object' not in role:
+                        if role.get('content_object') is None:
                             continue
                         indexed_roles[role['content_object']['type']].append(role)
                     self._roles.append((_page, indexed_roles))
                 else:
                     self._related.append((_page, name, S))
 
         return changed
@@ -407,28 +407,25 @@
             else:  # It is a create set
                 self._cache.get_page(endpoint)
                 self._import_list(endpoint, related_set)
 
             # FIXME: deal with pruning existing relations that do not match the import set
 
     def import_assets(self, data):
-        self._cache = page.PageCache()
+        self._cache = page.PageCache(self.connection)
         self._related = []
         self._roles = []
 
         changed = False
 
         for resource in self._dependent_resources():
             endpoint = getattr(self, resource)
 
-            # Load up existing objects, so that we can try to update or link to them
-            self._cache.get_page(endpoint)
             imported = self._import_list(endpoint, data.get(resource) or [])
             changed = changed or imported
-            # FIXME: should we delete existing unpatched assets?
 
         self._assign_related()
         self._assign_membership()
         self._assign_roles()
 
         return changed
```

### Comparing `awxkit-24.3.0/awxkit/api/pages/applications.py` & `awxkit-24.3.1/awxkit/api/pages/applications.py`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/awxkit/api/pages/base.py` & `awxkit-24.3.1/awxkit/api/pages/base.py`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/awxkit/api/pages/bulk.py` & `awxkit-24.3.1/awxkit/api/pages/bulk.py`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/awxkit/api/pages/config.py` & `awxkit-24.3.1/awxkit/api/pages/config.py`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/awxkit/api/pages/credentials.py` & `awxkit-24.3.1/awxkit/api/pages/credentials.py`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/awxkit/api/pages/execution_environments.py` & `awxkit-24.3.1/awxkit/api/pages/execution_environments.py`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/awxkit/api/pages/instance_groups.py` & `awxkit-24.3.1/awxkit/api/pages/instance_groups.py`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/awxkit/api/pages/instances.py` & `awxkit-24.3.1/awxkit/api/pages/instances.py`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/awxkit/api/pages/inventory.py` & `awxkit-24.3.1/awxkit/api/pages/inventory.py`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/awxkit/api/pages/job_templates.py` & `awxkit-24.3.1/awxkit/api/pages/job_templates.py`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/awxkit/api/pages/jobs.py` & `awxkit-24.3.1/awxkit/api/pages/jobs.py`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/awxkit/api/pages/labels.py` & `awxkit-24.3.1/awxkit/api/pages/labels.py`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/awxkit/api/pages/notification_templates.py` & `awxkit-24.3.1/awxkit/api/pages/notification_templates.py`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/awxkit/api/pages/notifications.py` & `awxkit-24.3.1/awxkit/api/pages/notifications.py`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/awxkit/api/pages/organizations.py` & `awxkit-24.3.1/awxkit/api/pages/organizations.py`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/awxkit/api/pages/page.py` & `awxkit-24.3.1/awxkit/api/pages/page.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from requests import Response
 import http.client as http
 
 from awxkit.utils import PseudoNamespace, is_relative_endpoint, are_same_endpoint, super_dir_set, is_list_or_tuple, to_str
 from awxkit.api import utils
 from awxkit.api.client import Connection
 from awxkit.api.registry import URLRegistry
+from awxkit.api.resources import resources
 from awxkit.config import config
 import awxkit.exceptions as exc
 
 
 log = logging.getLogger(__name__)
 
 
@@ -489,18 +490,19 @@
         return self.endpoint == other
 
     def __ne__(self, other):
         return self.endpoint != other
 
 
 class PageCache(object):
-    def __init__(self):
+    def __init__(self, connection=None):
         self.options = {}
         self.pages_by_url = {}
         self.pages_by_natural_key = {}
+        self.connection = connection or Connection(config.base_url, not config.assume_untrusted)
 
     def get_options(self, page):
         url = page.endpoint if isinstance(page, Page) else str(page)
         if url in self.options:
             return self.options[url]
 
         try:
@@ -546,11 +548,35 @@
             log.warning("This endpoint is deprecated: %s", url)
             return self.pages_by_url.setdefault(url, None)
 
         log.debug("get_page: %s", page.endpoint)
         return self.set_page(page)
 
     def get_by_natural_key(self, natural_key):
-        endpoint = self.pages_by_natural_key.get(utils.freeze(natural_key))
-        log.debug("get_by_natural_key: %s, endpoint: %s", repr(natural_key), endpoint)
-        if endpoint:
-            return self.get_page(endpoint)
+        page = self.pages_by_natural_key.get(utils.freeze(natural_key))
+        if page is None:
+            # We need some way to get ahold of the top-level resource
+            # list endpoint from the natural_key type.  The resources
+            # object more or less has that for each of the detail
+            # views.  Just chop off the /<id>/ bit.
+            endpoint = getattr(resources, natural_key['type'], None)
+            if endpoint is None:
+                return
+            endpoint = ''.join([endpoint.rsplit('/', 2)[0], '/'])
+            page_type = get_registered_page(endpoint)
+
+            kwargs = {}
+            for k, v in natural_key.items():
+                if isinstance(v, str) and k != 'type':
+                    kwargs[k] = v
+
+            # Do a filtered query against the list endpoint, usually
+            # with the name of the object but sometimes more.
+            list_page = page_type(self.connection, endpoint=endpoint).get(all_pages=True, **kwargs)
+            if 'results' in list_page:
+                for p in list_page.results:
+                    self.set_page(p)
+            page = self.pages_by_natural_key.get(utils.freeze(natural_key))
+
+        log.debug("get_by_natural_key: %s, endpoint: %s", repr(natural_key), page)
+        if page:
+            return self.get_page(page)
```

### Comparing `awxkit-24.3.0/awxkit/api/pages/projects.py` & `awxkit-24.3.1/awxkit/api/pages/projects.py`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/awxkit/api/pages/roles.py` & `awxkit-24.3.1/awxkit/api/pages/roles.py`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/awxkit/api/pages/schedules.py` & `awxkit-24.3.1/awxkit/api/pages/schedules.py`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/awxkit/api/pages/settings.py` & `awxkit-24.3.1/awxkit/api/pages/settings.py`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/awxkit/api/pages/survey_spec.py` & `awxkit-24.3.1/awxkit/api/pages/survey_spec.py`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/awxkit/api/pages/system_job_templates.py` & `awxkit-24.3.1/awxkit/api/pages/system_job_templates.py`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/awxkit/api/pages/teams.py` & `awxkit-24.3.1/awxkit/api/pages/teams.py`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/awxkit/api/pages/unified_job_templates.py` & `awxkit-24.3.1/awxkit/api/pages/unified_job_templates.py`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/awxkit/api/pages/unified_jobs.py` & `awxkit-24.3.1/awxkit/api/pages/unified_jobs.py`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/awxkit/api/pages/users.py` & `awxkit-24.3.1/awxkit/api/pages/users.py`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/awxkit/api/pages/workflow_approval_templates.py` & `awxkit-24.3.1/awxkit/api/pages/workflow_approval_templates.py`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/awxkit/api/pages/workflow_approvals.py` & `awxkit-24.3.1/awxkit/api/pages/workflow_approvals.py`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/awxkit/api/pages/workflow_job_nodes.py` & `awxkit-24.3.1/awxkit/api/pages/workflow_job_nodes.py`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/awxkit/api/pages/workflow_job_template_nodes.py` & `awxkit-24.3.1/awxkit/api/pages/workflow_job_template_nodes.py`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/awxkit/api/pages/workflow_job_templates.py` & `awxkit-24.3.1/awxkit/api/pages/workflow_job_templates.py`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/awxkit/api/pages/workflow_jobs.py` & `awxkit-24.3.1/awxkit/api/pages/workflow_jobs.py`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/awxkit/api/registry.py` & `awxkit-24.3.1/awxkit/api/registry.py`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/awxkit/api/resources.py` & `awxkit-24.3.1/awxkit/api/resources.py`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/awxkit/api/utils.py` & `awxkit-24.3.1/awxkit/api/utils.py`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/awxkit/awx/inventory.py` & `awxkit-24.3.1/awxkit/awx/inventory.py`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/awxkit/awx/utils.py` & `awxkit-24.3.1/awxkit/awx/utils.py`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/awxkit/cli/__init__.py` & `awxkit-24.3.1/awxkit/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/awxkit/cli/client.py` & `awxkit-24.3.1/awxkit/cli/client.py`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/awxkit/cli/custom.py` & `awxkit-24.3.1/awxkit/cli/custom.py`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/awxkit/cli/docs/Makefile` & `awxkit-24.3.1/awxkit/cli/docs/Makefile`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/awxkit/cli/docs/make.bat` & `awxkit-24.3.1/awxkit/cli/docs/make.bat`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/awxkit/cli/docs/source/authentication.rst` & `awxkit-24.3.1/awxkit/cli/docs/source/authentication.rst`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/awxkit/cli/docs/source/conf.py` & `awxkit-24.3.1/awxkit/cli/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/awxkit/cli/docs/source/examples.rst` & `awxkit-24.3.1/awxkit/cli/docs/source/examples.rst`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/awxkit/cli/docs/source/index.rst` & `awxkit-24.3.1/awxkit/cli/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/awxkit/cli/docs/source/output.rst` & `awxkit-24.3.1/awxkit/cli/docs/source/output.rst`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/awxkit/cli/docs/source/usage.rst` & `awxkit-24.3.1/awxkit/cli/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/awxkit/cli/format.py` & `awxkit-24.3.1/awxkit/cli/format.py`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/awxkit/cli/options.py` & `awxkit-24.3.1/awxkit/cli/options.py`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/awxkit/cli/resource.py` & `awxkit-24.3.1/awxkit/cli/resource.py`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/awxkit/cli/sphinx.py` & `awxkit-24.3.1/awxkit/cli/sphinx.py`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/awxkit/cli/stdout.py` & `awxkit-24.3.1/awxkit/cli/stdout.py`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/awxkit/cli/utils.py` & `awxkit-24.3.1/awxkit/cli/utils.py`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/awxkit/config.py` & `awxkit-24.3.1/awxkit/config.py`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/awxkit/exceptions.py` & `awxkit-24.3.1/awxkit/exceptions.py`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/awxkit/scripts/basic_session.py` & `awxkit-24.3.1/awxkit/scripts/basic_session.py`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/awxkit/utils/__init__.py` & `awxkit-24.3.1/awxkit/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/awxkit/utils/toposort.py` & `awxkit-24.3.1/awxkit/utils/toposort.py`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/awxkit/words.py` & `awxkit-24.3.1/awxkit/words.py`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/awxkit/ws.py` & `awxkit-24.3.1/awxkit/ws.py`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/awxkit/yaml_file.py` & `awxkit-24.3.1/awxkit/yaml_file.py`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/awxkit.egg-info/PKG-INFO` & `awxkit-24.3.1/awxkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awxkit
-Version: 24.3.0
+Version: 24.3.1
 Summary: The official command line interface for Ansible AWX
 Home-page: https://github.com/ansible/awx
 Author: Red Hat, Inc.
 Author-email: info@ansible.com
 License: Apache 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `awxkit-24.3.0/awxkit.egg-info/SOURCES.txt` & `awxkit-24.3.1/awxkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/setup.py` & `awxkit-24.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/test/cli/test_client.py` & `awxkit-24.3.1/test/cli/test_client.py`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/test/cli/test_config.py` & `awxkit-24.3.1/test/cli/test_config.py`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/test/cli/test_format.py` & `awxkit-24.3.1/test/cli/test_format.py`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/test/cli/test_options.py` & `awxkit-24.3.1/test/cli/test_options.py`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/test/test_credentials.py` & `awxkit-24.3.1/test/test_credentials.py`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/test/test_dependency_resolver.py` & `awxkit-24.3.1/test/test_dependency_resolver.py`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/test/test_registry.py` & `awxkit-24.3.1/test/test_registry.py`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/test/test_utils.py` & `awxkit-24.3.1/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/test/test_ws.py` & `awxkit-24.3.1/test/test_ws.py`

 * *Files identical despite different names*

### Comparing `awxkit-24.3.0/tox.ini` & `awxkit-24.3.1/tox.ini`

 * *Files identical despite different names*
