# Comparing `tmp/lecert-1.0.tar.gz` & `tmp/lecert-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lecert-1.0.tar", last modified: Fri Apr 26 09:47:17 2024, max compression
+gzip compressed data, was "lecert-1.1.tar", last modified: Wed May  1 09:19:43 2024, max compression
```

## Comparing `lecert-1.0.tar` & `lecert-1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 09:47:17.984317 lecert-1.0/
--rw-rw-rw-   0        0        0     2912 2024-04-26 09:47:17.984317 lecert-1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2463 2024-04-26 09:46:02.000000 lecert-1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-26 09:47:17.960317 lecert-1.0/lecert/
--rw-rw-rw-   0        0        0     5601 2024-04-26 09:01:58.000000 lecert-1.0/lecert/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-26 09:47:17.983316 lecert-1.0/lecert.egg-info/
--rw-rw-rw-   0        0        0     2912 2024-04-26 09:47:17.000000 lecert-1.0/lecert.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      186 2024-04-26 09:47:17.000000 lecert-1.0/lecert.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 09:47:17.000000 lecert-1.0/lecert.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-04-26 09:47:17.000000 lecert-1.0/lecert.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-26 09:47:17.000000 lecert-1.0/lecert.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-26 09:47:17.984317 lecert-1.0/setup.cfg
--rw-rw-rw-   0        0        0      714 2024-04-26 09:41:30.000000 lecert-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 09:19:43.958261 lecert-1.1/
+-rw-rw-rw-   0        0        0     2912 2024-05-01 09:19:43.957290 lecert-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2463 2024-04-26 09:46:02.000000 lecert-1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-01 09:19:43.930777 lecert-1.1/lecert/
+-rw-rw-rw-   0        0        0     6363 2024-05-01 09:18:02.000000 lecert-1.1/lecert/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 09:19:43.956289 lecert-1.1/lecert.egg-info/
+-rw-rw-rw-   0        0        0     2912 2024-05-01 09:19:43.000000 lecert-1.1/lecert.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      186 2024-05-01 09:19:43.000000 lecert-1.1/lecert.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 09:19:43.000000 lecert-1.1/lecert.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-01 09:19:43.000000 lecert-1.1/lecert.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-01 09:19:43.000000 lecert-1.1/lecert.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-01 09:19:43.958261 lecert-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      714 2024-05-01 09:18:11.000000 lecert-1.1/setup.py
```

### Comparing `lecert-1.0/PKG-INFO` & `lecert-1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lecert
-Version: 1.0
+Version: 1.1
 Summary: Python module for obtaining SSL certificates from Let's Encrypt for self-service projects
 Home-page: https://github.com/EightShift/lecert
 Author: EightShift
 Author-email: the8shift@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lecert-1.0/README.md` & `lecert-1.1/README.md`

 * *Files identical despite different names*

### Comparing `lecert-1.0/lecert/__init__.py` & `lecert-1.1/lecert/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,36 @@
 import os
+import sys
 from datetime import datetime, timedelta
 from contextlib import contextmanager
 import shutil
 
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives.asymmetric import rsa
 import josepy as jose
 import OpenSSL
 
 from acme import challenges
 from acme import client
 from acme import crypto_util
 from acme import messages
+import logging
+
+
+logger = logging.getLogger('lecert')
+
+formatter = logging.Formatter(
+    '%(asctime)s (%(filename)s:%(lineno)d %(threadName)s) %(levelname)s - %(name)s: "%(message)s"'
+)
+
+console_output_handler = logging.StreamHandler(sys.stderr)
+console_output_handler.setFormatter(formatter)
+logger.addHandler(console_output_handler)
+
+logger.setLevel(logging.ERROR)
 
 
 KEY_SIZE = 2048
 DIRECTORY_URL = 'https://acme-v02.api.letsencrypt.org/directory'
 ACME_CHALLENGE_DIR_NAME = '__acme-challenge__'
 
 
@@ -31,32 +46,39 @@
 		created = os.path.getctime(cert_path)
 		if datetime.now() - datetime.fromtimestamp(created) < timedelta(days=cert_lifetime):
 			return False
 	
 	return True
 
 
-def _backup_saving(file_path, data):
-	old_file_path = file_path + '.old'
-	if os.path.exists(file_path):
-		if os.path.exists(old_file_path):
-			os.remove(old_file_path)
+def _backup_saving(certs_dir, cert_name_data, privkey_name_data, backup_time_format='%Y-%m-%d_%H-%M-%S'):
+	current_datetime = datetime.now().strftime(backup_time_format)
+	created_datetime = None
+
+	backups_dir = os.path.join(certs_dir, 'backups')
+	os.makedirs(backups_dir, exist_ok=True)
+
+	for name, data in (cert_name_data, privkey_name_data):
+		path = os.path.join(certs_dir, name)
+
+		if os.path.exists(path):
+			if not created_datetime:
+				created_datetime = datetime.fromtimestamp(os.path.getctime(path)).strftime(backup_time_format)
+			
+			backup_dir = os.path.join(backups_dir, f'{created_datetime}~{current_datetime}')
+			os.makedirs(backup_dir, exist_ok=True)
 
-		os.rename(file_path, old_file_path)
+			backup_path = os.path.join(backup_dir, path)
+			try:
+				shutil.move(path, backup_path)
+			except:
+				pass
 
-	try:
-		with open(file_path, 'w') as _file:
+		with open(path, 'w') as _file:
 			_file.write(data)
-	except:
-		if os.path.exists(old_file_path):
-			os.rename(old_file_path, file_path)
-
-		return False
-	
-	return True
 
 
 def _select_http01_challb(auths):
 	for chall_body in auths.body.challenges:
 		if isinstance(chall_body.chall, challenges.HTTP01):
 			return chall_body
 
@@ -78,23 +100,14 @@
 		with open(challenge_token_path, 'w') as challenge_token_file:
 			challenge_token_file.write(validation)
 
 		# Let the CA server know that we are ready for the challenge.
 		client_acme.answer_challenge(challb, response)
 
 
-def _save_cert(privkey_path, cert_path, privkey_pem, finalized_order):
-	if not _backup_saving(privkey_path, privkey_pem.decode()):  # saving privkey.pem file
-		return False
-
-	if not _backup_saving(cert_path, finalized_order.fullchain_pem): # saving cert.pem file
-		return False
-	
-	return True
-
 
 @contextmanager
 def _get_acme_challenge_dir(certs_dir):
 	acme_challenge_dir = os.path.join(certs_dir, ACME_CHALLENGE_DIR_NAME)
 	try:
 		os.makedirs(acme_challenge_dir, exist_ok=True)
 
@@ -115,35 +128,35 @@
 	try:
 		yield client_acme
 	finally:
 		client_acme.deactivate_registration(regr)
 
 
 
-def get_cert(certs_dir, email, domains, www=True, cert_lifetime=30, timeout=150, force=False, privkey_file_name='privkey.pem', cert_file_name='cert.pem'):
+def get_cert(certs_dir, email, domains, www=True, cert_lifetime=30, timeout=150, force=False, privkey_file_name='privkey.pem', cert_file_name='cert.pem', backup_time_format='%Y-%m-%d_%H-%M-%S'):
 	"""Obtains a new certificate from Let's Encrypt.
 
 	Args:
 		certs_dir (str): The directory where the certificates are stored.
 		email (str): The email address of the account.
 		domains (list): The list of domains to include in the certificate.
 		www (bool): Whether to include the www subdomain in the certificate.
 		cert_lifetime (int): The lifetime of the certificate in days.
 		timeout (int): The timeout in seconds for the certificate issuance process.
 		force (bool): Whether to force the certificate issuance even if the current certificate is still valid.
 		privkey_file_name (str): The name of the private key file.
 		cert_file_name (str): The name of the certificate file.
+		backup_time_format (str): Time format for backup directories.
 
 	Returns:
 		bool: True if the certificate was obtained successfully, False otherwise.
 	"""
-	privkey_path = os.path.join(certs_dir, privkey_file_name)
+	
 	cert_path = os.path.join(certs_dir, cert_file_name)
-
-	if not force and not _time_to_get_cert(cert_path, cert_lifetime): # force or checking __created__ file
+	if not force and not _time_to_get_cert(cert_path, cert_lifetime): # force or checking file creation time
 		return
 
 	try:
 		with _get_client_acme(email) as client_acme:
 			# Create private key
 			privkey_pem = _generate_privkey_pem()
 			
@@ -156,10 +169,15 @@
 
 			with _get_acme_challenge_dir(certs_dir) as acme_challenge_dir:
 				_accept_challenges(acme_challenge_dir, client_acme, order)
 
 				# Wait for challenge status and then issue a certificate.
 				finalized_order = client_acme.poll_and_finalize(order, datetime.now() + timedelta(seconds=timeout))
 
-			return _save_cert(privkey_path, cert_path, privkey_pem, finalized_order)
-	except:
-		return False
+			_backup_saving(certs_dir, (cert_file_name, finalized_order.fullchain_pem), (privkey_file_name, privkey_pem.decode()), backup_time_format) # saving private key and certificate with backup
+
+			return True
+
+	except Exception as e:
+		logger.error(e)
+
+	return False
```

### Comparing `lecert-1.0/lecert.egg-info/PKG-INFO` & `lecert-1.1/lecert.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lecert
-Version: 1.0
+Version: 1.1
 Summary: Python module for obtaining SSL certificates from Let's Encrypt for self-service projects
 Home-page: https://github.com/EightShift/lecert
 Author: EightShift
 Author-email: the8shift@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lecert-1.0/setup.py` & `lecert-1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='lecert',
-    version='1.0',
+    version='1.1',
     description='Python module for obtaining SSL certificates from Let\'s Encrypt for self-service projects',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='EightShift',
     author_email='the8shift@gmail.com',
     url='https://github.com/EightShift/lecert',
     packages=find_packages(),
```

