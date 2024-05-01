# Comparing `tmp/pybuilder-git-version-0.5.0.tar.gz` & `tmp/pybuilder-git-version-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybuilder-git-version-0.5.0.tar", last modified: Mon Dec 18 10:02:17 2023, max compression
+gzip compressed data, was "pybuilder-git-version-0.6.0.tar", last modified: Wed May  1 11:15:01 2024, max compression
```

## Comparing `pybuilder-git-version-0.5.0.tar` & `pybuilder-git-version-0.6.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jeffreysheehan   (501) staff       (20)        0 2023-12-18 10:02:17.028706 pybuilder-git-version-0.5.0/
--rw-r--r--   0 jeffreysheehan   (501) staff       (20)     2223 2023-12-18 10:02:17.028420 pybuilder-git-version-0.5.0/PKG-INFO
-drwxr-xr-x   0 jeffreysheehan   (501) staff       (20)        0 2023-12-18 10:02:17.025786 pybuilder-git-version-0.5.0/pybuilder_git_version/
--rw-r--r--   0 jeffreysheehan   (501) staff       (20)     1163 2023-12-17 12:24:58.000000 pybuilder-git-version-0.5.0/pybuilder_git_version/__init__.py
--rw-r--r--   0 jeffreysheehan   (501) staff       (20)     2342 2023-12-17 12:24:58.000000 pybuilder-git-version-0.5.0/pybuilder_git_version/util.py
-drwxr-xr-x   0 jeffreysheehan   (501) staff       (20)        0 2023-12-18 10:02:17.028029 pybuilder-git-version-0.5.0/pybuilder_git_version.egg-info/
--rw-r--r--   0 jeffreysheehan   (501) staff       (20)     2223 2023-12-18 10:02:16.000000 pybuilder-git-version-0.5.0/pybuilder_git_version.egg-info/PKG-INFO
--rw-r--r--   0 jeffreysheehan   (501) staff       (20)      390 2023-12-18 10:02:16.000000 pybuilder-git-version-0.5.0/pybuilder_git_version.egg-info/SOURCES.txt
--rw-r--r--   0 jeffreysheehan   (501) staff       (20)        1 2023-12-18 10:02:16.000000 pybuilder-git-version-0.5.0/pybuilder_git_version.egg-info/dependency_links.txt
--rw-r--r--   0 jeffreysheehan   (501) staff       (20)        1 2023-12-18 10:02:16.000000 pybuilder-git-version-0.5.0/pybuilder_git_version.egg-info/namespace_packages.txt
--rw-r--r--   0 jeffreysheehan   (501) staff       (20)       33 2023-12-18 10:02:16.000000 pybuilder-git-version-0.5.0/pybuilder_git_version.egg-info/requires.txt
--rw-r--r--   0 jeffreysheehan   (501) staff       (20)       22 2023-12-18 10:02:16.000000 pybuilder-git-version-0.5.0/pybuilder_git_version.egg-info/top_level.txt
--rw-r--r--   0 jeffreysheehan   (501) staff       (20)        1 2023-12-18 10:02:16.000000 pybuilder-git-version-0.5.0/pybuilder_git_version.egg-info/zip-safe
--rw-r--r--   0 jeffreysheehan   (501) staff       (20)       38 2023-12-18 10:02:17.028812 pybuilder-git-version-0.5.0/setup.cfg
--rwxr-xr-x   0 jeffreysheehan   (501) staff       (20)     3366 2023-12-18 10:02:16.000000 pybuilder-git-version-0.5.0/setup.py
+drwxr-xr-x   0 jeffreysheehan   (501) staff       (20)        0 2024-05-01 11:15:01.397236 pybuilder-git-version-0.6.0/
+-rw-r--r--   0 jeffreysheehan   (501) staff       (20)     2223 2024-05-01 11:15:01.396875 pybuilder-git-version-0.6.0/PKG-INFO
+drwxr-xr-x   0 jeffreysheehan   (501) staff       (20)        0 2024-05-01 11:15:01.393635 pybuilder-git-version-0.6.0/pybuilder_git_version/
+-rw-r--r--   0 jeffreysheehan   (501) staff       (20)     1364 2024-05-01 10:14:57.000000 pybuilder-git-version-0.6.0/pybuilder_git_version/__init__.py
+-rw-r--r--   0 jeffreysheehan   (501) staff       (20)     2491 2024-05-01 10:21:21.000000 pybuilder-git-version-0.6.0/pybuilder_git_version/util.py
+drwxr-xr-x   0 jeffreysheehan   (501) staff       (20)        0 2024-05-01 11:15:01.396456 pybuilder-git-version-0.6.0/pybuilder_git_version.egg-info/
+-rw-r--r--   0 jeffreysheehan   (501) staff       (20)     2223 2024-05-01 11:15:01.000000 pybuilder-git-version-0.6.0/pybuilder_git_version.egg-info/PKG-INFO
+-rw-r--r--   0 jeffreysheehan   (501) staff       (20)      390 2024-05-01 11:15:01.000000 pybuilder-git-version-0.6.0/pybuilder_git_version.egg-info/SOURCES.txt
+-rw-r--r--   0 jeffreysheehan   (501) staff       (20)        1 2024-05-01 11:15:01.000000 pybuilder-git-version-0.6.0/pybuilder_git_version.egg-info/dependency_links.txt
+-rw-r--r--   0 jeffreysheehan   (501) staff       (20)        1 2024-05-01 11:15:01.000000 pybuilder-git-version-0.6.0/pybuilder_git_version.egg-info/namespace_packages.txt
+-rw-r--r--   0 jeffreysheehan   (501) staff       (20)       33 2024-05-01 11:15:01.000000 pybuilder-git-version-0.6.0/pybuilder_git_version.egg-info/requires.txt
+-rw-r--r--   0 jeffreysheehan   (501) staff       (20)       22 2024-05-01 11:15:01.000000 pybuilder-git-version-0.6.0/pybuilder_git_version.egg-info/top_level.txt
+-rw-r--r--   0 jeffreysheehan   (501) staff       (20)        1 2024-05-01 11:15:01.000000 pybuilder-git-version-0.6.0/pybuilder_git_version.egg-info/zip-safe
+-rw-r--r--   0 jeffreysheehan   (501) staff       (20)       38 2024-05-01 11:15:01.397358 pybuilder-git-version-0.6.0/setup.cfg
+-rwxr-xr-x   0 jeffreysheehan   (501) staff       (20)     3366 2024-05-01 11:15:00.000000 pybuilder-git-version-0.6.0/setup.py
```

### Comparing `pybuilder-git-version-0.5.0/PKG-INFO` & `pybuilder-git-version-0.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybuilder-git-version
-Version: 0.5.0
+Version: 0.6.0
 Summary: A Git versioning plugin for PyBuilder
 Home-page: https://github.com/jlsheehan/pybuilder-git-version
 Author: Jeffrey Sheehan
 Author-email: jeff.sheehan7@gmail.com
 Maintainer: 
 Maintainer-email: 
 License: MIT License
```

### Comparing `pybuilder-git-version-0.5.0/pybuilder_git_version/__init__.py` & `pybuilder-git-version-0.6.0/pybuilder_git_version/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 from git import Repo
 from git.exc import InvalidGitRepositoryError
-from pybuilder.core import init, Project, Logger
+from pybuilder.core import init, Project, Logger, before
 
 from pybuilder_git_version.util import NoValidTagFoundError, find_latest_version
 
 
 @init
 def init_pybuilder_git_version(project: Project, logger: Logger):
     project.set_property_if_unset("use_git_version", True)
     project.set_property_if_unset("git_version_commit_distance_as_build_number", True)
     project.set_property_if_unset("git_version_master_branch", "master")
+
+
+@before("prepare", only_once=True)
+def update_version(project: Project, logger: Logger):
+    logger.info("Using master branch %s", project.get_property("git_version_master_branch"))
     if project.get_property("use_git_version"):
         try:
             repo = Repo(project.basedir)
             latest_tag = find_latest_version(repo, logger, master_branch_name=project.get_property("git_version_master_branch"))
             project.version = latest_tag
             project.set_property("dir_dist", f"$dir_target/dist/{project.name}-{project.version}")
             logger.info("Set project version to %s", project.version)
         except InvalidGitRepositoryError:
             logger.warn("No git repository found")
         except NoValidTagFoundError:
             logger.warn("No git tags found")
     else:
-        logger.debug("Not using git version")
+        logger.info("Not using git version, disabled")
```

### Comparing `pybuilder-git-version-0.5.0/pybuilder_git_version/util.py` & `pybuilder-git-version-0.6.0/pybuilder_git_version/util.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 
 def find_latest_version(repo: Repo, logger: Logger, master_branch_name: str = 'master') -> str:
     # valid_tags = [t for t in repo.tags if semver.VersionInfo.isvalid(t.name)]
     # logger.debug("Valid tags are: %s", [t.name for t in valid_tags])
     latest_tag, distance, branch_name = find_latest_tag_in_path(repo, logger)
     detached_head = branch_name is None
+    logger.debug("latest tag = %s, distance = %s, branch_name = %s, master_branch_name = %s", latest_tag, distance, branch_name, master_branch_name)
     on_master_branch = not detached_head and branch_name == master_branch_name
     repo_dirty = repo.is_dirty()
     if distance == 0 and (on_master_branch or detached_head) and not repo_dirty:
         logger.info("Using unmodified tag %s", latest_tag)
         return latest_tag.name
     else:
         logger.debug("Bumping patch and adding build")
@@ -42,15 +43,15 @@
         for valid_tag in valid_tags:
             logger.debug("Checking if %s in %s", valid_tag.commit, commits)
             if valid_tag.commit in commits:
                 latest_tag = valid_tag
                 distance = commits.index(latest_tag.commit)
                 return latest_tag, distance, branch_name
     # didnt find anything...
-    logger.warn("No valid tags found")
+    logger.info("No valid tags found")
     raise NoValidTagFoundError("No valid version tag found")
 
 
 def sane_branch_name(branch_name):
     if '/' in branch_name:
         branch_part = branch_name.split('/')[-1]
     else:
```

### Comparing `pybuilder-git-version-0.5.0/pybuilder_git_version.egg-info/PKG-INFO` & `pybuilder-git-version-0.6.0/pybuilder_git_version.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybuilder-git-version
-Version: 0.5.0
+Version: 0.6.0
 Summary: A Git versioning plugin for PyBuilder
 Home-page: https://github.com/jlsheehan/pybuilder-git-version
 Author: Jeffrey Sheehan
 Author-email: jeff.sheehan7@gmail.com
 Maintainer: 
 Maintainer-email: 
 License: MIT License
```

### Comparing `pybuilder-git-version-0.5.0/setup.py` & `pybuilder-git-version-0.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         _install.run(self)
 
         self.post_install_script()
 
 if __name__ == '__main__':
     setup(
         name = 'pybuilder-git-version',
-        version = '0.5.0',
+        version = '0.6.0',
         description = 'A Git versioning plugin for PyBuilder',
         long_description = "PyBuilder Git Version Plugin\n============================\n\nSummary\n-------\n\nThis project is a plugin for [PyBuilder](https://pybuilder.io) that sets the\nproject version based on git tags.\n\nUsage\n-----\n\nTo use the plugin put the following in the plugins section of `build.py`:\n\n```python\nuse_plugin('pybuilder_git_version')\n```\n\nThe possible properties for use are:\n\n| Property                                    | Value        | Default | Usage                                      |\n|---------------------------------------------|--------------|---------|--------------------------------------------|\n| use_git_version                             | True / False | True    | Turns off pybuilder_git_version            |\n| git_version_commit_distance_as_build_number | True / False | True    | Uses commit count from tag as build number |\n\n\nExamples\n--------\n\nThe following table has examples of repo state and corresponding version\nnumber produced.\n\n| Tag        | Branch             | Clean / Dirty | Number of commits since tag | Version                |\n|------------|--------------------|---------------|-----------------------------|------------------------|\n| 0.0.1      | master             | clean         | 0                           | 0.0.1                  |\n| 0.0.1      | master             | dirty         | 0                           | 0.0.2+build.0          |\n| 0.2.2      | develop            | clean         | 5                           | 0.2.3+develop.5        |\n| 1.2.3      | develop            | dirty         | 3                           | 1.2.4+develop.3        |\n| 1.0.0-rc.1 | feature/TICKET-100 | clean         | 5                           | 1.0.0-rc.1+ticket100.5 |\n| 0.0.1      | hotfix/BUG-20      | clean         | 0                           | 0.0.2+bug20.0          |",
         long_description_content_type = 'text/markdown',
         classifiers = [
             'Development Status :: 3 - Alpha',
             'Programming Language :: Python'
         ],
@@ -45,15 +45,15 @@
         packages = ['pybuilder_git_version'],
         namespace_packages = [],
         py_modules = [],
         entry_points = {},
         data_files = [],
         package_data = {},
         install_requires = [
-            'gitpython==3.1.24',
+            'gitpython==3.1.43',
             'semver==2.13.0'
         ],
         dependency_links = [],
         zip_safe = True,
         cmdclass = {'install': install},
         python_requires = '',
         obsoletes = [],
```

