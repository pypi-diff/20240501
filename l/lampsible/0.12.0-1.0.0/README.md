# Comparing `tmp/lampsible-0.12.0.tar.gz` & `tmp/lampsible-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lampsible-0.12.0.tar", last modified: Sun Apr 14 18:43:00 2024, max compression
+gzip compressed data, was "lampsible-1.0.0.tar", last modified: Wed May  1 19:11:14 2024, max compression
```

## Comparing `lampsible-0.12.0.tar` & `lampsible-1.0.0.tar`

### file list

```diff
@@ -1,79 +1,91 @@
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-14 18:43:00.527672 lampsible-0.12.0/
--rw-rw-r--   0 brian     (1000) brian     (1000)       54 2024-04-14 18:38:32.000000 lampsible-0.12.0/.gitignore
--rw-rw-r--   0 brian     (1000) brian     (1000)    11358 2024-04-14 18:38:32.000000 lampsible-0.12.0/LICENSE
--rw-r--r--   0 brian     (1000) brian     (1000)     3831 2024-04-14 18:43:00.527672 lampsible-0.12.0/PKG-INFO
--rw-rw-r--   0 brian     (1000) brian     (1000)     2977 2024-04-14 18:38:32.000000 lampsible-0.12.0/README.md
--rw-rw-r--   0 brian     (1000) brian     (1000)     1135 2024-04-14 18:38:32.000000 lampsible-0.12.0/pyproject.toml
--rw-rw-r--   0 brian     (1000) brian     (1000)       38 2024-04-14 18:43:00.527672 lampsible-0.12.0/setup.cfg
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-14 18:43:00.519672 lampsible-0.12.0/src/
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-14 18:43:00.523672 lampsible-0.12.0/src/lampsible/
--rw-rw-r--   0 brian     (1000) brian     (1000)        0 2024-04-14 18:38:32.000000 lampsible-0.12.0/src/lampsible/__init__.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    13680 2024-04-14 18:38:32.000000 lampsible-0.12.0/src/lampsible/arg_validator.py
--rw-rw-r--   0 brian     (1000) brian     (1000)      681 2024-04-14 18:38:32.000000 lampsible-0.12.0/src/lampsible/constants.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    17401 2024-04-14 18:38:32.000000 lampsible-0.12.0/src/lampsible/lampsible.py
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-14 18:43:00.523672 lampsible-0.12.0/src/lampsible/project/
--rw-rw-r--   0 brian     (1000) brian     (1000)       94 2024-04-14 18:38:32.000000 lampsible-0.12.0/src/lampsible/project/ansible-galaxy-requirements.yml
--rw-rw-r--   0 brian     (1000) brian     (1000)      944 2024-04-14 18:38:32.000000 lampsible-0.12.0/src/lampsible/project/apache.yml
--rw-rw-r--   0 brian     (1000) brian     (1000)      987 2024-04-14 18:38:32.000000 lampsible-0.12.0/src/lampsible/project/lamp-stack.yml
--rw-rw-r--   0 brian     (1000) brian     (1000)      383 2024-04-14 18:38:32.000000 lampsible-0.12.0/src/lampsible/project/mysql.yml
--rw-rw-r--   0 brian     (1000) brian     (1000)      331 2024-04-14 18:38:32.000000 lampsible-0.12.0/src/lampsible/project/php.yml
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-14 18:43:00.523672 lampsible-0.12.0/src/lampsible/project/roles/
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-14 18:43:00.519672 lampsible-0.12.0/src/lampsible/project/roles/apache-conf/
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-14 18:43:00.527672 lampsible-0.12.0/src/lampsible/project/roles/apache-conf/tasks/
--rw-rw-r--   0 brian     (1000) brian     (1000)      391 2024-04-14 18:38:32.000000 lampsible-0.12.0/src/lampsible/project/roles/apache-conf/tasks/main.yml
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-14 18:43:00.527672 lampsible-0.12.0/src/lampsible/project/roles/apache-conf/templates/
--rw-rw-r--   0 brian     (1000) brian     (1000)      948 2024-04-14 18:38:32.000000 lampsible-0.12.0/src/lampsible/project/roles/apache-conf/templates/ssl-params.conf.j2
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-14 18:43:00.523672 lampsible-0.12.0/src/lampsible/project/roles/apache-vhosts/
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-14 18:43:00.527672 lampsible-0.12.0/src/lampsible/project/roles/apache-vhosts/tasks/
--rw-rw-r--   0 brian     (1000) brian     (1000)      517 2024-04-14 18:38:32.000000 lampsible-0.12.0/src/lampsible/project/roles/apache-vhosts/tasks/main.yml
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-14 18:43:00.527672 lampsible-0.12.0/src/lampsible/project/roles/apache-vhosts/templates/
--rw-rw-r--   0 brian     (1000) brian     (1000)     1507 2024-04-14 18:38:32.000000 lampsible-0.12.0/src/lampsible/project/roles/apache-vhosts/templates/000-default.conf.j2
--rw-rw-r--   0 brian     (1000) brian     (1000)     6434 2024-04-14 18:38:32.000000 lampsible-0.12.0/src/lampsible/project/roles/apache-vhosts/templates/default-ssl.conf.j2
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-14 18:43:00.523672 lampsible-0.12.0/src/lampsible/project/roles/apache2/
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-14 18:43:00.527672 lampsible-0.12.0/src/lampsible/project/roles/apache2/tasks/
--rw-rw-r--   0 brian     (1000) brian     (1000)      322 2024-04-14 18:38:32.000000 lampsible-0.12.0/src/lampsible/project/roles/apache2/tasks/main.yml
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-14 18:43:00.523672 lampsible-0.12.0/src/lampsible/project/roles/apt-update/
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-14 18:43:00.527672 lampsible-0.12.0/src/lampsible/project/roles/apt-update/tasks/
--rw-rw-r--   0 brian     (1000) brian     (1000)       67 2024-04-14 18:38:32.000000 lampsible-0.12.0/src/lampsible/project/roles/apt-update/tasks/main.yaml
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-14 18:43:00.523672 lampsible-0.12.0/src/lampsible/project/roles/domain-for-wordpress/
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-14 18:43:00.527672 lampsible-0.12.0/src/lampsible/project/roles/domain-for-wordpress/tasks/
--rw-rw-r--   0 brian     (1000) brian     (1000)      752 2024-04-14 18:38:32.000000 lampsible-0.12.0/src/lampsible/project/roles/domain-for-wordpress/tasks/main.yml
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-14 18:43:00.523672 lampsible-0.12.0/src/lampsible/project/roles/fail2ban/
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-14 18:43:00.527672 lampsible-0.12.0/src/lampsible/project/roles/fail2ban/tasks/
--rw-rw-r--   0 brian     (1000) brian     (1000)      299 2024-04-14 18:38:32.000000 lampsible-0.12.0/src/lampsible/project/roles/fail2ban/tasks/main.yml
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-14 18:43:00.527672 lampsible-0.12.0/src/lampsible/project/roles/fail2ban/templates/
--rw-rw-r--   0 brian     (1000) brian     (1000)      971 2024-04-14 18:38:32.000000 lampsible-0.12.0/src/lampsible/project/roles/fail2ban/templates/jail.local.j2
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-14 18:43:00.523672 lampsible-0.12.0/src/lampsible/project/roles/mysql/
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-14 18:43:00.527672 lampsible-0.12.0/src/lampsible/project/roles/mysql/tasks/
--rw-rw-r--   0 brian     (1000) brian     (1000)     1371 2024-04-14 18:38:32.000000 lampsible-0.12.0/src/lampsible/project/roles/mysql/tasks/main.yml
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-14 18:43:00.523672 lampsible-0.12.0/src/lampsible/project/roles/php/
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-14 18:43:00.527672 lampsible-0.12.0/src/lampsible/project/roles/php/tasks/
--rw-rw-r--   0 brian     (1000) brian     (1000)      969 2024-04-14 18:38:32.000000 lampsible-0.12.0/src/lampsible/project/roles/php/tasks/main.yml
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-14 18:43:00.523672 lampsible-0.12.0/src/lampsible/project/roles/phpmyadmin/
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-14 18:43:00.527672 lampsible-0.12.0/src/lampsible/project/roles/phpmyadmin/tasks/
--rw-rw-r--   0 brian     (1000) brian     (1000)      495 2024-04-14 18:38:32.000000 lampsible-0.12.0/src/lampsible/project/roles/phpmyadmin/tasks/main.yml
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-14 18:43:00.527672 lampsible-0.12.0/src/lampsible/project/roles/phpmyadmin/templates/
--rw-rw-r--   0 brian     (1000) brian     (1000)     7260 2024-04-14 18:38:32.000000 lampsible-0.12.0/src/lampsible/project/roles/phpmyadmin/templates/apache2.conf
--rw-rw-r--   0 brian     (1000) brian     (1000)    73018 2024-04-14 18:38:32.000000 lampsible-0.12.0/src/lampsible/project/roles/phpmyadmin/templates/php.ini
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-14 18:43:00.523672 lampsible-0.12.0/src/lampsible/project/roles/pip/
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-14 18:43:00.527672 lampsible-0.12.0/src/lampsible/project/roles/pip/tasks/
--rw-rw-r--   0 brian     (1000) brian     (1000)       63 2024-04-14 18:38:32.000000 lampsible-0.12.0/src/lampsible/project/roles/pip/tasks/main.yaml
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-14 18:43:00.523672 lampsible-0.12.0/src/lampsible/project/roles/ssl-certbot/
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-14 18:43:00.527672 lampsible-0.12.0/src/lampsible/project/roles/ssl-certbot/tasks/
--rw-rw-r--   0 brian     (1000) brian     (1000)      265 2024-04-14 18:38:32.000000 lampsible-0.12.0/src/lampsible/project/roles/ssl-certbot/tasks/main.yml
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-14 18:43:00.523672 lampsible-0.12.0/src/lampsible/project/roles/ssl-selfsigned/
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-14 18:43:00.527672 lampsible-0.12.0/src/lampsible/project/roles/ssl-selfsigned/tasks/
--rw-rw-r--   0 brian     (1000) brian     (1000)      881 2024-04-14 18:38:32.000000 lampsible-0.12.0/src/lampsible/project/roles/ssl-selfsigned/tasks/main.yml
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-14 18:43:00.523672 lampsible-0.12.0/src/lampsible/project/roles/wordpress/
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-14 18:43:00.527672 lampsible-0.12.0/src/lampsible/project/roles/wordpress/tasks/
--rw-rw-r--   0 brian     (1000) brian     (1000)     3268 2024-04-14 18:38:32.000000 lampsible-0.12.0/src/lampsible/project/roles/wordpress/tasks/main.yml
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-14 18:43:00.527672 lampsible-0.12.0/src/lampsible/project/roles/wordpress/templates/
--rw-rw-r--   0 brian     (1000) brian     (1000)      582 2024-04-14 18:38:32.000000 lampsible-0.12.0/src/lampsible/project/roles/wordpress/templates/.htaccess
--rw-rw-r--   0 brian     (1000) brian     (1000)     1651 2024-04-14 18:38:32.000000 lampsible-0.12.0/src/lampsible/project/wordpress.yml
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-14 18:43:00.527672 lampsible-0.12.0/src/lampsible.egg-info/
--rw-r--r--   0 brian     (1000) brian     (1000)     3831 2024-04-14 18:43:00.000000 lampsible-0.12.0/src/lampsible.egg-info/PKG-INFO
--rw-rw-r--   0 brian     (1000) brian     (1000)     1749 2024-04-14 18:43:00.000000 lampsible-0.12.0/src/lampsible.egg-info/SOURCES.txt
--rw-rw-r--   0 brian     (1000) brian     (1000)        1 2024-04-14 18:43:00.000000 lampsible-0.12.0/src/lampsible.egg-info/dependency_links.txt
--rw-rw-r--   0 brian     (1000) brian     (1000)       55 2024-04-14 18:43:00.000000 lampsible-0.12.0/src/lampsible.egg-info/entry_points.txt
--rw-rw-r--   0 brian     (1000) brian     (1000)       33 2024-04-14 18:43:00.000000 lampsible-0.12.0/src/lampsible.egg-info/requires.txt
--rw-rw-r--   0 brian     (1000) brian     (1000)       10 2024-04-14 18:43:00.000000 lampsible-0.12.0/src/lampsible.egg-info/top_level.txt
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.293008 lampsible-1.0.0/
+-rw-rw-r--   0 brian     (1000) brian     (1000)       54 2024-05-01 19:10:38.000000 lampsible-1.0.0/.gitignore
+-rw-rw-r--   0 brian     (1000) brian     (1000)    11358 2024-05-01 19:10:38.000000 lampsible-1.0.0/LICENSE
+-rw-r--r--   0 brian     (1000) brian     (1000)     2694 2024-05-01 19:11:14.293008 lampsible-1.0.0/PKG-INFO
+-rw-rw-r--   0 brian     (1000) brian     (1000)     1817 2024-05-01 19:10:38.000000 lampsible-1.0.0/README.md
+-rw-rw-r--   0 brian     (1000) brian     (1000)     1069 2024-05-01 19:10:38.000000 lampsible-1.0.0/pyproject.toml
+-rw-rw-r--   0 brian     (1000) brian     (1000)       38 2024-05-01 19:11:14.293008 lampsible-1.0.0/setup.cfg
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.249013 lampsible-1.0.0/src/
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.253013 lampsible-1.0.0/src/lampsible/
+-rw-rw-r--   0 brian     (1000) brian     (1000)       22 2024-05-01 19:10:38.000000 lampsible-1.0.0/src/lampsible/__init__.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    21636 2024-05-01 19:10:38.000000 lampsible-1.0.0/src/lampsible/arg_validator.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     2137 2024-05-01 19:10:38.000000 lampsible-1.0.0/src/lampsible/constants.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    16544 2024-05-01 19:10:38.000000 lampsible-1.0.0/src/lampsible/lampsible.py
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.285009 lampsible-1.0.0/src/lampsible/project/
+-rw-rw-r--   0 brian     (1000) brian     (1000)       94 2024-05-01 19:10:38.000000 lampsible-1.0.0/src/lampsible/project/ansible-galaxy-requirements.yml
+-rw-rw-r--   0 brian     (1000) brian     (1000)      659 2024-05-01 19:10:38.000000 lampsible-1.0.0/src/lampsible/project/apache.yml
+-rw-rw-r--   0 brian     (1000) brian     (1000)      702 2024-05-01 19:10:38.000000 lampsible-1.0.0/src/lampsible/project/lamp-stack.yml
+-rw-rw-r--   0 brian     (1000) brian     (1000)      720 2024-05-01 19:10:38.000000 lampsible-1.0.0/src/lampsible/project/laravel.yml
+-rw-rw-r--   0 brian     (1000) brian     (1000)      291 2024-05-01 19:10:38.000000 lampsible-1.0.0/src/lampsible/project/mysql.yml
+-rw-rw-r--   0 brian     (1000) brian     (1000)      239 2024-05-01 19:10:38.000000 lampsible-1.0.0/src/lampsible/project/php.yml
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.253013 lampsible-1.0.0/src/lampsible/project/roles/
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.249013 lampsible-1.0.0/src/lampsible/project/roles/apache-conf/
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.285009 lampsible-1.0.0/src/lampsible/project/roles/apache-conf/tasks/
+-rw-rw-r--   0 brian     (1000) brian     (1000)      391 2024-05-01 19:10:38.000000 lampsible-1.0.0/src/lampsible/project/roles/apache-conf/tasks/main.yml
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.285009 lampsible-1.0.0/src/lampsible/project/roles/apache-conf/templates/
+-rw-rw-r--   0 brian     (1000) brian     (1000)      832 2024-05-01 19:10:38.000000 lampsible-1.0.0/src/lampsible/project/roles/apache-conf/templates/ssl-params.conf.j2
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.249013 lampsible-1.0.0/src/lampsible/project/roles/apache-vhosts/
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.285009 lampsible-1.0.0/src/lampsible/project/roles/apache-vhosts/tasks/
+-rw-rw-r--   0 brian     (1000) brian     (1000)      517 2024-05-01 19:10:38.000000 lampsible-1.0.0/src/lampsible/project/roles/apache-vhosts/tasks/main.yml
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.285009 lampsible-1.0.0/src/lampsible/project/roles/apache-vhosts/templates/
+-rw-rw-r--   0 brian     (1000) brian     (1000)     1507 2024-05-01 19:10:38.000000 lampsible-1.0.0/src/lampsible/project/roles/apache-vhosts/templates/000-default.conf.j2
+-rw-rw-r--   0 brian     (1000) brian     (1000)     6434 2024-05-01 19:10:38.000000 lampsible-1.0.0/src/lampsible/project/roles/apache-vhosts/templates/default-ssl.conf.j2
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.249013 lampsible-1.0.0/src/lampsible/project/roles/apache2/
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.285009 lampsible-1.0.0/src/lampsible/project/roles/apache2/tasks/
+-rw-rw-r--   0 brian     (1000) brian     (1000)      322 2024-05-01 19:10:38.000000 lampsible-1.0.0/src/lampsible/project/roles/apache2/tasks/main.yml
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.253013 lampsible-1.0.0/src/lampsible/project/roles/apt-update/
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.289009 lampsible-1.0.0/src/lampsible/project/roles/apt-update/tasks/
+-rw-rw-r--   0 brian     (1000) brian     (1000)      175 2024-05-01 19:10:38.000000 lampsible-1.0.0/src/lampsible/project/roles/apt-update/tasks/main.yaml
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.253013 lampsible-1.0.0/src/lampsible/project/roles/domain-for-wordpress/
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.289009 lampsible-1.0.0/src/lampsible/project/roles/domain-for-wordpress/tasks/
+-rw-rw-r--   0 brian     (1000) brian     (1000)      409 2024-05-01 19:10:38.000000 lampsible-1.0.0/src/lampsible/project/roles/domain-for-wordpress/tasks/main.yml
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.253013 lampsible-1.0.0/src/lampsible/project/roles/fail2ban/
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.289009 lampsible-1.0.0/src/lampsible/project/roles/fail2ban/tasks/
+-rw-rw-r--   0 brian     (1000) brian     (1000)      299 2024-05-01 19:10:38.000000 lampsible-1.0.0/src/lampsible/project/roles/fail2ban/tasks/main.yml
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.289009 lampsible-1.0.0/src/lampsible/project/roles/fail2ban/templates/
+-rw-rw-r--   0 brian     (1000) brian     (1000)      971 2024-05-01 19:10:38.000000 lampsible-1.0.0/src/lampsible/project/roles/fail2ban/templates/jail.local.j2
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.253013 lampsible-1.0.0/src/lampsible/project/roles/laravel/
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.289009 lampsible-1.0.0/src/lampsible/project/roles/laravel/tasks/
+-rw-rw-r--   0 brian     (1000) brian     (1000)      798 2024-05-01 19:10:38.000000 lampsible-1.0.0/src/lampsible/project/roles/laravel/tasks/main.yml
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.289009 lampsible-1.0.0/src/lampsible/project/roles/laravel/templates/
+-rw-rw-r--   0 brian     (1000) brian     (1000)     1068 2024-05-01 19:10:38.000000 lampsible-1.0.0/src/lampsible/project/roles/laravel/templates/.env.j2
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.253013 lampsible-1.0.0/src/lampsible/project/roles/mysql/
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.289009 lampsible-1.0.0/src/lampsible/project/roles/mysql/tasks/
+-rw-rw-r--   0 brian     (1000) brian     (1000)     1368 2024-05-01 19:10:38.000000 lampsible-1.0.0/src/lampsible/project/roles/mysql/tasks/main.yml
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.253013 lampsible-1.0.0/src/lampsible/project/roles/php/
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.289009 lampsible-1.0.0/src/lampsible/project/roles/php/tasks/
+-rw-rw-r--   0 brian     (1000) brian     (1000)      241 2024-05-01 19:10:38.000000 lampsible-1.0.0/src/lampsible/project/roles/php/tasks/main.yml
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.253013 lampsible-1.0.0/src/lampsible/project/roles/phpmyadmin/
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.289009 lampsible-1.0.0/src/lampsible/project/roles/phpmyadmin/tasks/
+-rw-rw-r--   0 brian     (1000) brian     (1000)      495 2024-05-01 19:10:38.000000 lampsible-1.0.0/src/lampsible/project/roles/phpmyadmin/tasks/main.yml
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.289009 lampsible-1.0.0/src/lampsible/project/roles/phpmyadmin/templates/
+-rw-rw-r--   0 brian     (1000) brian     (1000)     7260 2024-05-01 19:10:38.000000 lampsible-1.0.0/src/lampsible/project/roles/phpmyadmin/templates/apache2.conf
+-rw-rw-r--   0 brian     (1000) brian     (1000)    73018 2024-05-01 19:10:38.000000 lampsible-1.0.0/src/lampsible/project/roles/phpmyadmin/templates/php.ini
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.253013 lampsible-1.0.0/src/lampsible/project/roles/pip/
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.289009 lampsible-1.0.0/src/lampsible/project/roles/pip/tasks/
+-rw-rw-r--   0 brian     (1000) brian     (1000)       62 2024-05-01 19:10:38.000000 lampsible-1.0.0/src/lampsible/project/roles/pip/tasks/main.yaml
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.253013 lampsible-1.0.0/src/lampsible/project/roles/ssl-certbot/
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.293008 lampsible-1.0.0/src/lampsible/project/roles/ssl-certbot/tasks/
+-rw-rw-r--   0 brian     (1000) brian     (1000)      264 2024-05-01 19:10:38.000000 lampsible-1.0.0/src/lampsible/project/roles/ssl-certbot/tasks/main.yml
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.253013 lampsible-1.0.0/src/lampsible/project/roles/ssl-selfsigned/
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.293008 lampsible-1.0.0/src/lampsible/project/roles/ssl-selfsigned/tasks/
+-rw-rw-r--   0 brian     (1000) brian     (1000)      837 2024-05-01 19:10:38.000000 lampsible-1.0.0/src/lampsible/project/roles/ssl-selfsigned/tasks/main.yml
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.253013 lampsible-1.0.0/src/lampsible/project/roles/wordpress-block-xmlrpc/
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.293008 lampsible-1.0.0/src/lampsible/project/roles/wordpress-block-xmlrpc/tasks/
+-rw-rw-r--   0 brian     (1000) brian     (1000)      262 2024-05-01 19:10:38.000000 lampsible-1.0.0/src/lampsible/project/roles/wordpress-block-xmlrpc/tasks/main.yml
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.293008 lampsible-1.0.0/src/lampsible/project/roles/wordpress-block-xmlrpc/templates/
+-rw-rw-r--   0 brian     (1000) brian     (1000)      582 2024-05-01 19:10:38.000000 lampsible-1.0.0/src/lampsible/project/roles/wordpress-block-xmlrpc/templates/.htaccess
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.253013 lampsible-1.0.0/src/lampsible/project/roles/wordpress-cli/
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.293008 lampsible-1.0.0/src/lampsible/project/roles/wordpress-cli/tasks/
+-rw-rw-r--   0 brian     (1000) brian     (1000)     2644 2024-05-01 19:10:38.000000 lampsible-1.0.0/src/lampsible/project/roles/wordpress-cli/tasks/main.yml
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.253013 lampsible-1.0.0/src/lampsible/project/roles/wordpress-manual/
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.293008 lampsible-1.0.0/src/lampsible/project/roles/wordpress-manual/tasks/
+-rw-rw-r--   0 brian     (1000) brian     (1000)     2416 2024-05-01 19:10:38.000000 lampsible-1.0.0/src/lampsible/project/roles/wordpress-manual/tasks/main.yml
+-rw-rw-r--   0 brian     (1000) brian     (1000)     1657 2024-05-01 19:10:38.000000 lampsible-1.0.0/src/lampsible/project/wordpress.yml
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-01 19:11:14.293008 lampsible-1.0.0/src/lampsible.egg-info/
+-rw-r--r--   0 brian     (1000) brian     (1000)     2694 2024-05-01 19:11:14.000000 lampsible-1.0.0/src/lampsible.egg-info/PKG-INFO
+-rw-rw-r--   0 brian     (1000) brian     (1000)     2031 2024-05-01 19:11:14.000000 lampsible-1.0.0/src/lampsible.egg-info/SOURCES.txt
+-rw-rw-r--   0 brian     (1000) brian     (1000)        1 2024-05-01 19:11:14.000000 lampsible-1.0.0/src/lampsible.egg-info/dependency_links.txt
+-rw-rw-r--   0 brian     (1000) brian     (1000)       55 2024-05-01 19:11:14.000000 lampsible-1.0.0/src/lampsible.egg-info/entry_points.txt
+-rw-rw-r--   0 brian     (1000) brian     (1000)       42 2024-05-01 19:11:14.000000 lampsible-1.0.0/src/lampsible.egg-info/requires.txt
+-rw-rw-r--   0 brian     (1000) brian     (1000)       10 2024-05-01 19:11:14.000000 lampsible-1.0.0/src/lampsible.egg-info/top_level.txt
```

### Comparing `lampsible-0.12.0/LICENSE` & `lampsible-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lampsible-0.12.0/pyproject.toml` & `lampsible-1.0.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -3,43 +3,42 @@
     "setuptools>=69.0",
     "setuptools-scm>=8.0"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lampsible"
-version = "0.12.0"
+version = "1.0.0"
 authors = [
     {name="Brian St. Hilaire", email="brian.st-hilaire@sanctus-tech.com"}
 ]
 description = "Deploy and set up LAMP stacks with Ansible"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
     "ansible-core",
     "ansible-runner",
+    "requests",
     "fqdn",
 ]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Framework :: Ansible",
     "Programming Language :: Python :: 3",
     "Intended Audience :: Developers",
     "Intended Audience :: Information Technology",
     "Intended Audience :: System Administrators",
     "License :: OSI Approved :: Apache Software License",
 ]
 
 [project.scripts]
-# TODO: Improve this.
 lampsible = "lampsible:lampsible.main"
 
 [project.urls]
 Homepage = "https://github.com/saint-hilaire/lampsible"
 Issues = "https://github.com/saint-hilaire/lampsible/issues"
 
-# TODO: It may be possible without the following 2 tables.
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.setuptools_scm]
```

### Comparing `lampsible-0.12.0/src/lampsible/project/apache.yml` & `lampsible-1.0.0/src/lampsible/project/lamp-stack.yml`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,34 @@
 ---
 - hosts: all
   become: true
   gather_facts: true
-
   tasks:
-    - name: "Include standard Ansible role"
-      include_role:
+    - include_role:
         name: "{{ item }}"
       loop:
         - apt-update
         - apache2
+        - php
+        - pip
+        - mysql
 
-    - name: Conditionally include SSL role
-      include_role:
+    - include_role:
         name: ssl-selfsigned
       when: ssl_selfsigned
 
     # It's important that this runs after the selfsigned certificates,
     # if those are being used, but before Certbot, if that's being used.
-    - name: Include Apache virtual host role
-      include_role:
+    - include_role:
         name: apache-vhosts
 
-    - name: Conditionally include SSL role
-      include_role:
+    - include_role:
         name: ssl-certbot
       when: ssl_certbot
 
-    - name: Conditionally include custom Apache configuration
-      include_role:
+    - include_role:
         name: apache-conf
       when: ssl_selfsigned
 
-    - name: Conditionally include fail2ban role
-      include_role:
+    - include_role:
         name: fail2ban
       when: not insecure_skip_fail2ban
```

### Comparing `lampsible-0.12.0/src/lampsible/project/lamp-stack.yml` & `lampsible-1.0.0/src/lampsible/project/laravel.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,35 @@
 ---
 - hosts: all
   become: true
   gather_facts: true
   tasks:
-    - name: "Include standard Ansible role"
-      include_role:
+    - include_role:
         name: "{{ item }}"
       loop:
         - apt-update
         - apache2
         - php
         - pip
         - mysql
+        - laravel
 
-    - name: Conditionally include SSL role
-      include_role:
+    - include_role:
         name: ssl-selfsigned
       when: ssl_selfsigned
 
     # It's important that this runs after the selfsigned certificates,
     # if those are being used, but before Certbot, if that's being used.
-    - name: Include Apache virtual host role
-      include_role:
+    - include_role:
         name: apache-vhosts
 
-    - name: Conditionally include SSL role
-      include_role:
+    - include_role:
         name: ssl-certbot
       when: ssl_certbot
 
-    - name: Conditionally include custom Apache configuration
-      include_role:
+    - include_role:
         name: apache-conf
       when: ssl_selfsigned
 
-    - name: Conditionally include fail2ban role
-      include_role:
+    - include_role:
         name: fail2ban
       when: not insecure_skip_fail2ban
```

### Comparing `lampsible-0.12.0/src/lampsible/project/roles/apache-conf/templates/ssl-params.conf.j2` & `lampsible-1.0.0/src/lampsible/project/roles/apache-conf/templates/ssl-params.conf.j2`

 * *Files 21% similar despite different names*

```diff
@@ -12,10 +12,8 @@
 Header always set X-Content-Type-Options nosniff
 # Requires Apache >= 2.4
 SSLCompression off
 SSLSessionTickets Off
 SSLUseStapling on
 SSLStaplingCache "shmcb:logs/stapling-cache(150000)"
 
-# TODO: This has caused bugs in the past in other projects...
-# This whole thing needs to be refactored altogether.
 SSLOpenSSLConfCmd DHParameters "/etc/ssl/certs/dhparam.pem"
```

### Comparing `lampsible-0.12.0/src/lampsible/project/roles/apache-vhosts/tasks/main.yml` & `lampsible-1.0.0/src/lampsible/project/roles/apache-vhosts/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `lampsible-0.12.0/src/lampsible/project/roles/apache-vhosts/templates/000-default.conf.j2` & `lampsible-1.0.0/src/lampsible/project/roles/apache-vhosts/templates/000-default.conf.j2`

 * *Files identical despite different names*

### Comparing `lampsible-0.12.0/src/lampsible/project/roles/apache-vhosts/templates/default-ssl.conf.j2` & `lampsible-1.0.0/src/lampsible/project/roles/apache-vhosts/templates/default-ssl.conf.j2`

 * *Files identical despite different names*

### Comparing `lampsible-0.12.0/src/lampsible/project/roles/fail2ban/templates/jail.local.j2` & `lampsible-1.0.0/src/lampsible/project/roles/fail2ban/templates/jail.local.j2`

 * *Files identical despite different names*

### Comparing `lampsible-0.12.0/src/lampsible/project/roles/mysql/tasks/main.yml` & `lampsible-1.0.0/src/lampsible/project/roles/mysql/tasks/main.yml`

 * *Files 15% similar despite different names*

```diff
@@ -12,34 +12,34 @@
 #     login_unix_socket: /run/mysqld/mysqld.sock
 # - name: Removes all anonymous user accounts
 #   community.mysql.mysql_user:
 #     name: ''
 #     host_all: true
 #     state: absent
 
-- name: Install Python package pymysql.
+- name: Install Python package pymysql
   pip:
     name: pymysql
     # TODO: Necessary for Ubuntu versions 23 or newer, but there
     # might be more elegant ways to deal with this.
     extra_args: "{{ '--break-system-packages' if ansible_facts['distribution'] == 'Ubuntu' and ansible_facts['distribution_major_version'] == '23' else '' }}"
 
-- name: Create database user.
+- name: Create database user
   community.mysql.mysql_user:
     name:     "{{ database_username }}"
     password: "{{ database_password }}"
     # TODO: Consider using this along with a hashed password.
     # encrypted: true
     priv: '*.*:ALL'
     state: present
     login_unix_socket: /run/mysqld/mysqld.sock
     # TODO: Some other options to consider:
     # host: localhost
     # host_all: true
   when: database_username
 
-- name: Create database.
+- name: Create database
   community.mysql.mysql_db:
     name: "{{ database_name }}"
     state: present
     login_unix_socket: /run/mysqld/mysqld.sock
   when: database_name
```

### Comparing `lampsible-0.12.0/src/lampsible/project/roles/phpmyadmin/templates/apache2.conf` & `lampsible-1.0.0/src/lampsible/project/roles/phpmyadmin/templates/apache2.conf`

 * *Files identical despite different names*

### Comparing `lampsible-0.12.0/src/lampsible/project/roles/phpmyadmin/templates/php.ini` & `lampsible-1.0.0/src/lampsible/project/roles/phpmyadmin/templates/php.ini`

 * *Files identical despite different names*

### Comparing `lampsible-0.12.0/src/lampsible/project/roles/ssl-selfsigned/tasks/main.yml` & `lampsible-1.0.0/src/lampsible/project/roles/ssl-selfsigned/tasks/main.yml`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 ---
 - name: Prepare directories
   file:
     path: "{{ item }}"
     state: directory
-    # TODO: Are these the right permissions
     owner: root
     group: root
     mode: '0755'
   loop:
     - /etc/ssl/certs
     - /etc/ssl/private
     - /etc/ssl/csr
```

### Comparing `lampsible-0.12.0/src/lampsible/project/roles/wordpress/tasks/main.yml` & `lampsible-1.0.0/src/lampsible/project/roles/wordpress-manual/tasks/main.yml`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,10 @@
 ---
-#################################################################
-# TODO: There are some open source Ansible playbooks/methods/etc. for
-# dealing with WordPress. It is particularly challenging that WordPress needs
-# to be 'installed' by the user by submitting the usual '5 Minute Install'
-# form, that is, HTML form via HTTP... But maybe the options that WordPress
-# expects from that form submission can also somehow be supplied via
-# Ansible parameters... This would solve a lot of problems!
-#################################################################
+# DEPRECATED
+# Installing WordPress manually
 
 - name: Download WordPress
   unarchive:
     src: "https://wordpress.org/wordpress-{{ wordpress_version }}.tar.gz"
     dest: "/var/www/html/"
     remote_src: yes
 
@@ -68,22 +62,7 @@
 - name: Set file ownership for wp-content/
   file:
     path: /var/www/html/wordpress/wp-content/
     state: directory
     recurse: yes
     owner: www-data
     group: www-data
-
-- name: Block the insecure endpoint xmlrpc.php
-  template:
-    src: .htaccess
-    dest: /var/www/html/wordpress/.htaccess
-    # TODO: Maybe this is not secure...
-    owner: www-data
-    group: www-data
-    mode: '0644'
-  when: not wordpress_insecure_allow_xmlrpc
-
-- name: Restart Apache
-  service:
-    name: apache2
-    state: reloaded
```

### Comparing `lampsible-0.12.0/src/lampsible/project/roles/wordpress/templates/.htaccess` & `lampsible-1.0.0/src/lampsible/project/roles/wordpress-block-xmlrpc/templates/.htaccess`

 * *Files identical despite different names*

### Comparing `lampsible-0.12.0/src/lampsible.egg-info/SOURCES.txt` & `lampsible-1.0.0/src/lampsible.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -11,30 +11,35 @@
 src/lampsible.egg-info/dependency_links.txt
 src/lampsible.egg-info/entry_points.txt
 src/lampsible.egg-info/requires.txt
 src/lampsible.egg-info/top_level.txt
 src/lampsible/project/ansible-galaxy-requirements.yml
 src/lampsible/project/apache.yml
 src/lampsible/project/lamp-stack.yml
+src/lampsible/project/laravel.yml
 src/lampsible/project/mysql.yml
 src/lampsible/project/php.yml
 src/lampsible/project/wordpress.yml
 src/lampsible/project/roles/apache-conf/tasks/main.yml
 src/lampsible/project/roles/apache-conf/templates/ssl-params.conf.j2
 src/lampsible/project/roles/apache-vhosts/tasks/main.yml
 src/lampsible/project/roles/apache-vhosts/templates/000-default.conf.j2
 src/lampsible/project/roles/apache-vhosts/templates/default-ssl.conf.j2
 src/lampsible/project/roles/apache2/tasks/main.yml
 src/lampsible/project/roles/apt-update/tasks/main.yaml
 src/lampsible/project/roles/domain-for-wordpress/tasks/main.yml
 src/lampsible/project/roles/fail2ban/tasks/main.yml
 src/lampsible/project/roles/fail2ban/templates/jail.local.j2
+src/lampsible/project/roles/laravel/tasks/main.yml
+src/lampsible/project/roles/laravel/templates/.env.j2
 src/lampsible/project/roles/mysql/tasks/main.yml
 src/lampsible/project/roles/php/tasks/main.yml
 src/lampsible/project/roles/phpmyadmin/tasks/main.yml
 src/lampsible/project/roles/phpmyadmin/templates/apache2.conf
 src/lampsible/project/roles/phpmyadmin/templates/php.ini
 src/lampsible/project/roles/pip/tasks/main.yaml
 src/lampsible/project/roles/ssl-certbot/tasks/main.yml
 src/lampsible/project/roles/ssl-selfsigned/tasks/main.yml
-src/lampsible/project/roles/wordpress/tasks/main.yml
-src/lampsible/project/roles/wordpress/templates/.htaccess
+src/lampsible/project/roles/wordpress-block-xmlrpc/tasks/main.yml
+src/lampsible/project/roles/wordpress-block-xmlrpc/templates/.htaccess
+src/lampsible/project/roles/wordpress-cli/tasks/main.yml
+src/lampsible/project/roles/wordpress-manual/tasks/main.yml
```

