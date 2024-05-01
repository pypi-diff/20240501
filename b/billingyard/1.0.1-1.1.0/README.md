# Comparing `tmp/billingyard-1.0.1.tar.gz` & `tmp/billingyard-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "billingyard-1.0.1.tar", last modified: Thu Jul  1 17:24:02 2021, max compression
+gzip compressed data, was "billingyard-1.1.0.tar", last modified: Wed May  1 15:54:40 2024, max compression
```

## Comparing `billingyard-1.0.1.tar` & `billingyard-1.1.0.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxr-xr-x   0 martinvondrak   (501) staff       (20)        0 2021-07-01 17:24:02.316997 billingyard-1.0.1/
--rw-r--r--   0 martinvondrak   (501) staff       (20)    12064 2021-07-01 17:24:02.316833 billingyard-1.0.1/PKG-INFO
--rw-r--r--   0 martinvondrak   (501) staff       (20)     9430 2021-02-24 19:29:26.000000 billingyard-1.0.1/README.md
-drwxr-xr-x   0 martinvondrak   (501) staff       (20)        0 2021-07-01 17:24:02.314628 billingyard-1.0.1/billingyard/
--rw-r--r--   0 martinvondrak   (501) staff       (20)       40 2021-01-24 20:07:39.000000 billingyard-1.0.1/billingyard/__init__.py
--rw-r--r--   0 martinvondrak   (501) staff       (20)       60 2021-02-03 16:38:24.000000 billingyard-1.0.1/billingyard/__main__.py
--rw-r--r--   0 martinvondrak   (501) staff       (20)     1034 2021-02-14 21:30:25.000000 billingyard-1.0.1/billingyard/billingyard.py
--rw-r--r--   0 martinvondrak   (501) staff       (20)      802 2021-02-14 22:10:47.000000 billingyard-1.0.1/billingyard/cli.py
--rw-r--r--   0 martinvondrak   (501) staff       (20)     2577 2021-02-14 22:33:58.000000 billingyard-1.0.1/billingyard/invoice_processors.py
--rw-r--r--   0 martinvondrak   (501) staff       (20)     4137 2021-02-15 20:19:55.000000 billingyard-1.0.1/billingyard/models.py
--rw-r--r--   0 martinvondrak   (501) staff       (20)     3462 2021-02-14 20:32:31.000000 billingyard-1.0.1/billingyard/parser.py
-drwxr-xr-x   0 martinvondrak   (501) staff       (20)        0 2021-07-01 17:24:02.316420 billingyard-1.0.1/billingyard/templates/
--rw-r--r--   0 martinvondrak   (501) staff       (20)     6256 2021-02-14 21:58:50.000000 billingyard-1.0.1/billingyard/templates/invoice.html
--rw-r--r--   0 martinvondrak   (501) staff       (20)     8902 2021-07-01 17:13:37.000000 billingyard-1.0.1/billingyard/templates/vat_invoice.html
-drwxr-xr-x   0 martinvondrak   (501) staff       (20)        0 2021-07-01 17:24:02.315956 billingyard-1.0.1/billingyard.egg-info/
--rw-r--r--   0 martinvondrak   (501) staff       (20)    12064 2021-07-01 17:24:02.000000 billingyard-1.0.1/billingyard.egg-info/PKG-INFO
--rw-r--r--   0 martinvondrak   (501) staff       (20)      510 2021-07-01 17:24:02.000000 billingyard-1.0.1/billingyard.egg-info/SOURCES.txt
--rw-r--r--   0 martinvondrak   (501) staff       (20)        1 2021-07-01 17:24:02.000000 billingyard-1.0.1/billingyard.egg-info/dependency_links.txt
--rw-r--r--   0 martinvondrak   (501) staff       (20)       59 2021-07-01 17:24:02.000000 billingyard-1.0.1/billingyard.egg-info/entry_points.txt
--rw-r--r--   0 martinvondrak   (501) staff       (20)        1 2021-02-17 21:41:53.000000 billingyard-1.0.1/billingyard.egg-info/not-zip-safe
--rw-r--r--   0 martinvondrak   (501) staff       (20)       55 2021-07-01 17:24:02.000000 billingyard-1.0.1/billingyard.egg-info/requires.txt
--rw-r--r--   0 martinvondrak   (501) staff       (20)       12 2021-07-01 17:24:02.000000 billingyard-1.0.1/billingyard.egg-info/top_level.txt
--rw-r--r--   0 martinvondrak   (501) staff       (20)       38 2021-07-01 17:24:02.317043 billingyard-1.0.1/setup.cfg
--rw-r--r--   0 martinvondrak   (501) staff       (20)     1179 2021-07-01 17:22:10.000000 billingyard-1.0.1/setup.py
+drwxr-xr-x   0 martinvondrak   (501) staff       (20)        0 2024-05-01 15:54:40.895085 billingyard-1.1.0/
+-rw-r--r--   0 martinvondrak   (501) staff       (20)     1072 2021-01-19 19:12:52.000000 billingyard-1.1.0/LICENSE
+-rw-r--r--   0 martinvondrak   (501) staff       (20)    10250 2024-05-01 15:54:40.894865 billingyard-1.1.0/PKG-INFO
+-rw-r--r--   0 martinvondrak   (501) staff       (20)     9441 2024-05-01 14:45:14.000000 billingyard-1.1.0/README.md
+drwxr-xr-x   0 martinvondrak   (501) staff       (20)        0 2024-05-01 15:54:40.892764 billingyard-1.1.0/billingyard/
+-rw-r--r--   0 martinvondrak   (501) staff       (20)       40 2021-01-24 20:07:39.000000 billingyard-1.1.0/billingyard/__init__.py
+-rw-r--r--   0 martinvondrak   (501) staff       (20)       60 2021-02-03 16:38:24.000000 billingyard-1.1.0/billingyard/__main__.py
+-rw-r--r--   0 martinvondrak   (501) staff       (20)     1034 2021-02-14 21:30:25.000000 billingyard-1.1.0/billingyard/billingyard.py
+-rw-r--r--   0 martinvondrak   (501) staff       (20)      802 2021-02-14 22:10:47.000000 billingyard-1.1.0/billingyard/cli.py
+-rw-r--r--   0 martinvondrak   (501) staff       (20)     2577 2021-02-14 22:33:58.000000 billingyard-1.1.0/billingyard/invoice_processors.py
+-rw-r--r--   0 martinvondrak   (501) staff       (20)     4137 2021-02-15 20:19:55.000000 billingyard-1.1.0/billingyard/models.py
+-rw-r--r--   0 martinvondrak   (501) staff       (20)     3462 2021-02-14 20:32:31.000000 billingyard-1.1.0/billingyard/parser.py
+drwxr-xr-x   0 martinvondrak   (501) staff       (20)        0 2024-05-01 15:54:40.894231 billingyard-1.1.0/billingyard/templates/
+-rw-r--r--   0 martinvondrak   (501) staff       (20)     6256 2021-02-14 21:58:50.000000 billingyard-1.1.0/billingyard/templates/invoice.html
+-rw-r--r--   0 martinvondrak   (501) staff       (20)     8902 2021-07-01 17:13:37.000000 billingyard-1.1.0/billingyard/templates/vat_invoice.html
+drwxr-xr-x   0 martinvondrak   (501) staff       (20)        0 2024-05-01 15:54:40.894668 billingyard-1.1.0/billingyard.egg-info/
+-rw-r--r--   0 martinvondrak   (501) staff       (20)    10250 2024-05-01 15:54:40.000000 billingyard-1.1.0/billingyard.egg-info/PKG-INFO
+-rw-r--r--   0 martinvondrak   (501) staff       (20)      533 2024-05-01 15:54:40.000000 billingyard-1.1.0/billingyard.egg-info/SOURCES.txt
+-rw-r--r--   0 martinvondrak   (501) staff       (20)        1 2024-05-01 15:54:40.000000 billingyard-1.1.0/billingyard.egg-info/dependency_links.txt
+-rw-r--r--   0 martinvondrak   (501) staff       (20)       58 2024-05-01 15:54:40.000000 billingyard-1.1.0/billingyard.egg-info/entry_points.txt
+-rw-r--r--   0 martinvondrak   (501) staff       (20)        1 2021-02-17 21:41:53.000000 billingyard-1.1.0/billingyard.egg-info/not-zip-safe
+-rw-r--r--   0 martinvondrak   (501) staff       (20)       54 2024-05-01 15:54:40.000000 billingyard-1.1.0/billingyard.egg-info/requires.txt
+-rw-r--r--   0 martinvondrak   (501) staff       (20)       12 2024-05-01 15:54:40.000000 billingyard-1.1.0/billingyard.egg-info/top_level.txt
+-rw-r--r--   0 martinvondrak   (501) staff       (20)       80 2024-05-01 15:19:42.000000 billingyard-1.1.0/pyproject.toml
+-rw-r--r--   0 martinvondrak   (501) staff       (20)       38 2024-05-01 15:54:40.895122 billingyard-1.1.0/setup.cfg
+-rw-r--r--   0 martinvondrak   (501) staff       (20)     1261 2024-05-01 15:16:12.000000 billingyard-1.1.0/setup.py
```

### Comparing `billingyard-1.0.1/PKG-INFO` & `billingyard-1.1.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,265 +1,275 @@
 Metadata-Version: 2.1
 Name: billingyard
-Version: 1.0.1
+Version: 1.1.0
 Summary: CLI invoice generator for business entities in the Czech republic
 Home-page: https://github.com/MartinVondrak/billing-yard
 Author: Martin Vondrák
-Author-email: martinvondrak@icloud.com
-License: UNKNOWN
-Description: # Billing Yard
-        
-        Billing Yard is an open source CLI tool written in Python 3.9 for generating invoices from [JSON](https://www.json.org)
-        for business entities in the Czech republic. It supports invoices for both VAT payers and non VAT payers.
-        
-        If you like this software, please [buy me a coffee](https://www.buymeacoffee.com/martinvondrak).
-        
-        ## Installation
-        
-        First, please note that the software has [WeasyPrint](https://weasyprint.org)
-        as a dependency and WeasyPrint needs some external third party libraries for correct functioning. The way to install
-        these libraries will differ based on your operating system. So first you need to install these dependencies according to
-        the manual below, then you can install Billing Yard itself.
-        
-        The installation manual below expects you to know and understand how to work with [pip](https://pip.pypa.io)
-        and [Virtual Environment](https://docs.python.org/3/tutorial/venv.html).
-        
-        ### Linux
-        
-        Below, you can find how to install external third party libraries on different Linux distributions.
-        
-        #### Debian / Ubuntu
-        
-        Debian 10 Buster or newer / Ubuntu 18.04 Bionic Beaver or newer
-        
-        ```shell
-        sudo apt-get install build-essential python3-dev python3-pip python3-setuptools python3-wheel python3-cffi libcairo2 libpango-1.0-0 libpangocairo-1.0-0 libgdk-pixbuf2.0-0 libffi-dev shared-mime-info
-        ```
-        
-        #### Fedora
-        
-        ```shell
-        sudo yum install redhat-rpm-config python-devel python-pip python-setuptools python-wheel python-cffi libffi-devel cairo pango gdk-pixbuf2
-        ```
-        
-        #### Archlinux
-        
-        ```shell
-        sudo pacman -S python-pip python-setuptools python-wheel cairo pango gdk-pixbuf2 libffi pkg-config
-        ```
-        
-        #### Gentoo
-        
-        ```shell
-        emerge pip setuptools wheel cairo pango gdk-pixbuf cffi
-        ```
-        
-        #### Alpine
-        
-        Alpine Linux 3.6 or newer
-        
-        ```shell
-        apk --update --upgrade add gcc musl-dev jpeg-dev zlib-dev libffi-dev cairo-dev pango-dev gdk-pixbuf-dev
-        ```
-        
-        ### macOS
-        
-        Installation on macOS is recommended via [Homebrew](https://brew.sh).
-        
-        ```shell
-        brew install python3 cairo pango gdk-pixbuf libffi
-        ```
-        
-        ### Windows and further support
-        
-        For installation on Windows or further support, please see the
-        official [WeasyPrint installation guide](https://weasyprint.readthedocs.io/en/latest/install.html).
-        
-        ### Installing Billing Yard
-        
-        First you need to decide whether you want to use Virtual Environment or install Billing Yard globally. But note that
-        installing in Virtual Environment is always preferred way. Then just make sure you are using Python 3.9 or newer and run
-        following command, and you are done.
-        
-        ```shell
-        pip install billingyard
-        ```
-        
-        ## Basic usage
-        
-        First step is to create configuration and data source files for generating an invoice. All configuration and data
-        sources for an invoice are stored in JSON files. There are three schemas of JSON files, one for business entity (sender,
-        receiver), one for an invoice without VAT and one for an invoice with VAT. Then you can generate the invoice itself.
-        
-        ### Business entity
-        
-        We create two business entities, sender (entity which issues the invoice) and receiver (entity which pays the invoice).
-        
-        ```json
-        {
-          "company": "Company s.r.o.",
-          "street": "Ulice 38",
-          "city": "Praha",
-          "zip_code": "100 00",
-          "country": "Česká republika",
-          "company_id": "00011000",
-          "vat_id": "CZ00011000"
-        }
-        ```
-        
-        * **company** - the business name of the business entity
-        * **street** - the street in the address of the business entity
-        * **city** - the city in the address of the business entity
-        * **zip_code** - the zip code in the address of the business entity
-        * **country** - the country in the address of the business entity
-        * **company** - the identifier given by Czech authority of the business entity
-        * **street** - the identifier for VAT purpose of the business entity
-            * optional if business entity is not a VAT payer
-        
-        ### Invoice for a non VAT payer
-        
-        Below you can find the self explaining example of a non VAT payer invoice with further description.
-        
-        ```json
-        {
-          "invoice_number": "2021001",
-          "issue_date": "01. 01. 2021",
-          "due_date": "31. 01. 2021",
-          "currency": "Kč",
-          "bank": "Bank a.s.",
-          "bank_account": "1234567890/1234",
-          "payment_method": "bank transfer",
-          "register_info": "Fyzická osoba zapsaná v živnostenském rejstříku.",
-          "invoice_lines": [
-            {
-              "description": "software development",
-              "unit": "hr",
-              "quantity": 20,
-              "unit_price": 1500
-            }
-          ]
-        }
-        ```
-        
-        * **invoice_number** - a unique identifier of the invoice
-            * completely up to you, but keep in mind local policies from governmane
-        * **issue_date** - the date of issue of the invoice
-            * optional, if not set current date is used
-        * **due_date** - the last day, when the invoice must be paid
-        * **currency** - the currency in which is the invoice issued
-        * **bank** - the bank of the sender business entity
-        * **bank_account** - the bank account number of the sender business entity
-        * **payment_method** - the agreed instrument to pay the invoice
-            * e.g. bank transfer, cash, credit card
-            * this text is directly rendered in the invoice
-        * **register_info** - the info about record in government registers of the sender business entity
-            * the typical examples in Czech are "Fyzická osoba zapsaná v živnostenském rejstříku." or "Společnost je zapsána v
-              obchodním rejstříku vedeném u Městského soudu v Praze, oddílu C, vložce 2396."
-        * **invoice_lines** - the list of items that are invoiced
-        
-        Each invoice line consists of following properties.
-        
-        * **description** - the name or more exhaustive description of the invoiced item
-        * **unit** - the unit which we can use to count the invoiced item
-            * e.g. hour, piece, meter, square meter etc
-        * **quantity** - the amount of invoiced items in previously specified unit
-        * **unit_price** - the price of the invoiced item for one unit
-        
-        All dates have `DD. MM. YYYY` format.
-        
-        ### Invoice for a VAT payer
-        
-        Below you can find the self explaining example of a VAT payer invoice with further description.
-        
-        ```json
-        {
-          "invoice_number": "2021001",
-          "issue_date": "01. 01. 2021",
-          "supply_date": "01. 01. 2021",
-          "due_date": "31. 01. 2021",
-          "currency": "Kč",
-          "bank": "Bank a.s.",
-          "bank_account": "1234567890/1234",
-          "payment_method": "bank transfer",
-          "register_info": "Fyzická osoba zapsaná v živnostenském rejstříku.",
-          "invoice_lines": [
-            {
-              "description": "software development",
-              "unit": "hr",
-              "quantity": 20,
-              "unit_price": 1500,
-              "vat_rate": 0.21
-            }
-          ]
-        }
-        ```
-        
-        * **invoice_number** - a unique identifier of the invoice
-            * completely up to you, but keep in mind local policies from governmane
-        * **issue_date** - the date of issue of the invoice
-            * optional, if not set current date is used
-        * **supply_date** - the date of taxable supply
-            * optional, if not set current date is used
-        * **due_date** - the last day, when the invoice must be paid
-        * **currency** - the currency in which is the invoice issued
-        * **bank** - the bank of the sender business entity
-        * **bank_account** - the bank account number of the sender business entity
-        * **payment_method** - the agreed instrument to pay the invoice
-            * e.g. bank transfer, cash, credit card
-            * this text is directly rendered in the invoice
-        * **register_info** - the info about record in government registers of the sender business entity
-            * the typical examples in Czech are "Fyzická osoba zapsaná v živnostenském rejstříku." or "Společnost je zapsána v
-              obchodním rejstříku vedeném u Městského soudu v Praze, oddílu C, vložce 2396."
-        * **invoice_lines** - the list of items that are invoiced
-        
-        Each invoice line consists of following properties.
-        
-        * **description** - the name or more exhaustive description of the invoiced item
-        * **unit** - the unit which we can use to count the invoiced item
-            * e.g. hour, piece, meter, square meter etc
-        * **quantity** - the amount of invoiced items in previously specified unit
-        * **unit_price** - the price of the invoiced item for one unit without VAT
-        * **vat_rate** - the rate of VAT for this invoiced item
-        
-        All dates have `DD. MM. YYYY` format.
-        
-        ### Generating an invoice
-        
-        If you installed Billing Yard using Virtual Environment, just activate this environment and run one of the following
-        commands, depending on whether you are a VAT payer or not. If you installed Billing Yard globally, just run one of the
-        commands.
-        
-        ```shell
-        billingyard -s sender.json issue-invoice -i invoice.json -r receiver.json
-        ```
-        
-        The option `-s` expects path to JSON data file with information about a sender business entity. It can be omitted, if
-        its name is `sender.json` and it is located in the same directory from which is the command executed.
-        
-        The option `-i` expects path to JSON data file with the invoice data.
-        
-        The option `-r` expects path to JSON data file with information about a sender business entity.
-        
-        ```shell
-        billingyard -s sender.json issue-invoice -i invoice_vat.json -r receiver.json --vat
-        ```
-        
-        The option `--vat` is used to generate an invoice for a VAT payer sender business entity. Please do not forget, that in
-        this case, you have to also provide correct invoice JSON data file with all needed attributes.
-        
-        ## License
-        
-        This software is released under MIT License and use other third party software.
-        
-        * [Click](https://github.com/pallets/click/blob/master/LICENSE.rst)
-        * [Jinja2](https://github.com/pallets/jinja/blob/master/LICENSE.rst)
-        * [WeasyPrint](https://github.com/Kozea/WeasyPrint/blob/master/LICENSE)
-        
+Author-email: martin@martinvondrak.cz
 Keywords: invoice,cli,generator
-Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: Czech
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Office/Business :: Financial :: Accounting
+Classifier: Development Status :: 5 - Production/Stable
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: Click<9,>=8.1.7
+Requires-Dist: Jinja2<4,>=3.1.3
+Requires-Dist: WeasyPrint<63,>=62.0
+
+# Billing Yard
+
+Billing Yard is an open source CLI tool written in Python 3 for generating invoices from [JSON](https://www.json.org)
+for business entities in the Czech republic. It supports invoices for both VAT payers and non VAT payers.
+
+If you like this software, please [buy me a coffee](https://www.buymeacoffee.com/martinvondrak).
+
+## Installation
+
+First, please note that the software has [WeasyPrint](https://weasyprint.org) as a dependency and WeasyPrint needs some
+external third party libraries for correct functioning. The way to install these libraries will differ based on your
+operating system. So first you need to install these dependencies according to the manual below, then you can install
+Billing Yard itself.
+
+The installation manual below expects you to know and understand how to work with [pip](https://pip.pypa.io)
+and [Virtual Environment](https://docs.python.org/3/tutorial/venv.html).
+
+### Linux
+
+Below, you can find how to install external third party libraries on different Linux distributions.
+
+#### Debian
+
+Debian 11 Bullseye or newer
+
+```shell
+apt install python3-pip libpango-1.0-0 libpangoft2-1.0-0 libjpeg-dev libopenjp2-7-dev libffi-dev
+```
+
+#### Ubuntu
+
+Ubuntu 20.04 Focal Fossa or newer
+
+```shell
+apt install python3-pip libpango-1.0-0 libharfbuzz0b libpangoft2-1.0-0 libffi-dev libjpeg-dev libopenjp2-7-dev
+```
+
+#### Fedora
+
+Fedora 34 or newer
+
+```shell
+dnf install python3-pip pango gcc python3-devel gcc-c++ zlib-devel libjpeg-devel openjpeg2-devel libffi-devel
+```
+
+#### Archlinux
+
+```shell
+pacman -S python-pip pango gcc libjpeg-turbo openjpeg2
+```
+
+#### Alpine
+
+Alpine Linux 3.14 or newer
+
+```shell
+apk add py3-pip gcc musl-dev python3-dev pango zlib-dev jpeg-dev openjpeg-dev g++ libffi-dev
+```
+
+### macOS
+
+Installation on macOS is recommended via [Homebrew](https://brew.sh).
+
+```shell
+brew install python3 pango libffi
+```
+
+### Windows and further support
+
+For installation on Windows or further support, please see the
+official [WeasyPrint installation guide](https://doc.courtbouillon.org/weasyprint/stable/first_steps.html#windows). But
+please keep in mind that WeasyPrint must be installed as a dependency of Billing Yard and not directly using your OS
+package manager.
+
+### Installing Billing Yard
+
+First you need to decide whether you want to use Virtual Environment or install Billing Yard globally. But note that
+installing in Virtual Environment is always preferred way. Then just make sure you are using Python 3.9 or newer and
+run following command, and you are done.
+
+```shell
+pip install billingyard
+```
+
+## Basic usage
+
+First step is to create configuration and data source files for generating an invoice. All configuration and data
+sources for an invoice are stored in JSON files. There are three schemas of JSON files, one for business entity (sender,
+receiver), one for an invoice without VAT and one for an invoice with VAT. Then you can generate the invoice itself.
+
+### Business entity
+
+We create two business entities, sender (entity which issues the invoice) and receiver (entity which pays the invoice).
+
+```json
+{
+  "company": "Company s.r.o.",
+  "street": "Ulice 38",
+  "city": "Praha",
+  "zip_code": "100 00",
+  "country": "Česká republika",
+  "company_id": "00011000",
+  "vat_id": "CZ00011000"
+}
+```
+
+* **company** - the business name of the business entity
+* **street** - the street in the address of the business entity
+* **city** - the city in the address of the business entity
+* **zip_code** - the zip code in the address of the business entity
+* **country** - the country in the address of the business entity
+* **company** - the identifier given by Czech authority of the business entity
+* **vat_id** - the identifier for VAT purpose of the business entity
+    * optional if business entity is not a VAT payer
+
+### Invoice for a non VAT payer
+
+Below you can find the self explaining example of a non VAT payer invoice with further description.
+
+```json
+{
+  "invoice_number": "2021001",
+  "issue_date": "01. 01. 2021",
+  "due_date": "31. 01. 2021",
+  "currency": "Kč",
+  "bank": "Bank a.s.",
+  "bank_account": "1234567890/1234",
+  "payment_method": "bank transfer",
+  "register_info": "Fyzická osoba zapsaná v živnostenském rejstříku.",
+  "invoice_lines": [
+    {
+      "description": "software development",
+      "unit": "hr",
+      "quantity": 20,
+      "unit_price": 1500
+    }
+  ]
+}
+```
+
+* **invoice_number** - a unique identifier of the invoice
+    * completely up to you, but keep in mind local policies from government
+* **issue_date** - the date of issue of the invoice
+    * optional, if not set current date is used
+* **due_date** - the last day, when the invoice must be paid
+* **currency** - the currency in which is the invoice issued
+* **bank** - the bank of the sender business entity
+* **bank_account** - the bank account number of the sender business entity
+* **payment_method** - the agreed instrument to pay the invoice
+    * e.g. bank transfer, cash, credit card
+    * this text is directly rendered in the invoice
+* **register_info** - the info about record in government registers of the sender business entity
+    * the typical examples in Czech are "Fyzická osoba zapsaná v živnostenském rejstříku." or "Společnost je zapsána v
+      obchodním rejstříku vedeném u Městského soudu v Praze, oddílu C, vložce 2396."
+* **invoice_lines** - the list of items that are invoiced
+
+Each invoice line consists of following properties.
+
+* **description** - the name or more exhaustive description of the invoiced item
+* **unit** - the unit which we can use to count the invoiced item
+    * e.g. hour, piece, meter, square meter etc
+* **quantity** - the amount of invoiced items in previously specified unit
+* **unit_price** - the price of the invoiced item for one unit
+
+All dates have `DD. MM. YYYY` format.
+
+### Invoice for a VAT payer
+
+Below you can find the self explaining example of a VAT payer invoice with further description.
+
+```json
+{
+  "invoice_number": "2021001",
+  "issue_date": "01. 01. 2021",
+  "supply_date": "01. 01. 2021",
+  "due_date": "31. 01. 2021",
+  "currency": "Kč",
+  "bank": "Bank a.s.",
+  "bank_account": "1234567890/1234",
+  "payment_method": "bank transfer",
+  "register_info": "Fyzická osoba zapsaná v živnostenském rejstříku.",
+  "invoice_lines": [
+    {
+      "description": "software development",
+      "unit": "hr",
+      "quantity": 20,
+      "unit_price": 1500,
+      "vat_rate": 0.21
+    }
+  ]
+}
+```
+
+* **invoice_number** - a unique identifier of the invoice
+    * completely up to you, but keep in mind local policies from government
+* **issue_date** - the date of issue of the invoice
+    * optional, if not set current date is used
+* **supply_date** - the date of taxable supply
+    * optional, if not set current date is used
+* **due_date** - the last day, when the invoice must be paid
+* **currency** - the currency in which is the invoice issued
+* **bank** - the bank of the sender business entity
+* **bank_account** - the bank account number of the sender business entity
+* **payment_method** - the agreed instrument to pay the invoice
+    * e.g. bank transfer, cash, credit card
+    * this text is directly rendered in the invoice
+* **register_info** - the info about record in government registers of the sender business entity
+    * the typical examples in Czech are "Fyzická osoba zapsaná v živnostenském rejstříku." or "Společnost je zapsána v
+      obchodním rejstříku vedeném u Městského soudu v Praze, oddílu C, vložce 2396."
+* **invoice_lines** - the list of items that are invoiced
+
+Each invoice line consists of following properties.
+
+* **description** - the name or more exhaustive description of the invoiced item
+* **unit** - the unit which we can use to count the invoiced item
+    * e.g. hour, piece, meter, square meter etc
+* **quantity** - the amount of invoiced items in previously specified unit
+* **unit_price** - the price of the invoiced item for one unit without VAT
+* **vat_rate** - the rate of VAT for this invoiced item
+
+All dates have `DD. MM. YYYY` format.
+
+### Generating an invoice
+
+If you installed Billing Yard using Virtual Environment, just activate this environment and run one of the following
+commands, depending on whether you are a VAT payer or not. If you installed Billing Yard globally, just run one of the
+commands.
+
+```shell
+billingyard -s sender.json issue-invoice -i invoice.json -r receiver.json
+```
+
+The option `-s` expects path to JSON data file with information about a sender business entity. It can be omitted, if
+its name is `sender.json` and it is located in the same directory from which is the command executed.
+
+The option `-i` expects path to JSON data file with the invoice data.
+
+The option `-r` expects path to JSON data file with information about a sender business entity.
+
+```shell
+billingyard -s sender.json issue-invoice -i invoice_vat.json -r receiver.json --vat
+```
+
+The option `--vat` is used to generate an invoice for a VAT payer sender business entity. Please do not forget, that in
+this case, you have to also provide correct invoice JSON data file with all needed attributes.
+
+## License
+
+This software is released under MIT License and use other third party software.
+
+* [Click](https://github.com/pallets/click/blob/main/LICENSE.txt)
+* [Jinja2](https://github.com/pallets/jinja/blob/main/LICENSE.txt)
+* [WeasyPrint](https://github.com/Kozea/WeasyPrint/blob/master/LICENSE)
```

### Comparing `billingyard-1.0.1/README.md` & `billingyard-1.1.0/billingyard.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,80 +1,108 @@
+Metadata-Version: 2.1
+Name: billingyard
+Version: 1.1.0
+Summary: CLI invoice generator for business entities in the Czech republic
+Home-page: https://github.com/MartinVondrak/billing-yard
+Author: Martin Vondrák
+Author-email: martin@martinvondrak.cz
+Keywords: invoice,cli,generator
+Classifier: Environment :: Console
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: Czech
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Office/Business :: Financial :: Accounting
+Classifier: Development Status :: 5 - Production/Stable
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: Click<9,>=8.1.7
+Requires-Dist: Jinja2<4,>=3.1.3
+Requires-Dist: WeasyPrint<63,>=62.0
+
 # Billing Yard
 
-Billing Yard is an open source CLI tool written in Python 3.9 for generating invoices from [JSON](https://www.json.org)
+Billing Yard is an open source CLI tool written in Python 3 for generating invoices from [JSON](https://www.json.org)
 for business entities in the Czech republic. It supports invoices for both VAT payers and non VAT payers.
 
 If you like this software, please [buy me a coffee](https://www.buymeacoffee.com/martinvondrak).
 
 ## Installation
 
-First, please note that the software has [WeasyPrint](https://weasyprint.org)
-as a dependency and WeasyPrint needs some external third party libraries for correct functioning. The way to install
-these libraries will differ based on your operating system. So first you need to install these dependencies according to
-the manual below, then you can install Billing Yard itself.
+First, please note that the software has [WeasyPrint](https://weasyprint.org) as a dependency and WeasyPrint needs some
+external third party libraries for correct functioning. The way to install these libraries will differ based on your
+operating system. So first you need to install these dependencies according to the manual below, then you can install
+Billing Yard itself.
 
 The installation manual below expects you to know and understand how to work with [pip](https://pip.pypa.io)
 and [Virtual Environment](https://docs.python.org/3/tutorial/venv.html).
 
 ### Linux
 
 Below, you can find how to install external third party libraries on different Linux distributions.
 
-#### Debian / Ubuntu
+#### Debian
 
-Debian 10 Buster or newer / Ubuntu 18.04 Bionic Beaver or newer
+Debian 11 Bullseye or newer
 
 ```shell
-sudo apt-get install build-essential python3-dev python3-pip python3-setuptools python3-wheel python3-cffi libcairo2 libpango-1.0-0 libpangocairo-1.0-0 libgdk-pixbuf2.0-0 libffi-dev shared-mime-info
+apt install python3-pip libpango-1.0-0 libpangoft2-1.0-0 libjpeg-dev libopenjp2-7-dev libffi-dev
 ```
 
-#### Fedora
+#### Ubuntu
+
+Ubuntu 20.04 Focal Fossa or newer
 
 ```shell
-sudo yum install redhat-rpm-config python-devel python-pip python-setuptools python-wheel python-cffi libffi-devel cairo pango gdk-pixbuf2
+apt install python3-pip libpango-1.0-0 libharfbuzz0b libpangoft2-1.0-0 libffi-dev libjpeg-dev libopenjp2-7-dev
 ```
 
-#### Archlinux
+#### Fedora
+
+Fedora 34 or newer
 
 ```shell
-sudo pacman -S python-pip python-setuptools python-wheel cairo pango gdk-pixbuf2 libffi pkg-config
+dnf install python3-pip pango gcc python3-devel gcc-c++ zlib-devel libjpeg-devel openjpeg2-devel libffi-devel
 ```
 
-#### Gentoo
+#### Archlinux
 
 ```shell
-emerge pip setuptools wheel cairo pango gdk-pixbuf cffi
+pacman -S python-pip pango gcc libjpeg-turbo openjpeg2
 ```
 
 #### Alpine
 
-Alpine Linux 3.6 or newer
+Alpine Linux 3.14 or newer
 
 ```shell
-apk --update --upgrade add gcc musl-dev jpeg-dev zlib-dev libffi-dev cairo-dev pango-dev gdk-pixbuf-dev
+apk add py3-pip gcc musl-dev python3-dev pango zlib-dev jpeg-dev openjpeg-dev g++ libffi-dev
 ```
 
 ### macOS
 
 Installation on macOS is recommended via [Homebrew](https://brew.sh).
 
 ```shell
-brew install python3 cairo pango gdk-pixbuf libffi
+brew install python3 pango libffi
 ```
 
 ### Windows and further support
 
 For installation on Windows or further support, please see the
-official [WeasyPrint installation guide](https://weasyprint.readthedocs.io/en/latest/install.html).
+official [WeasyPrint installation guide](https://doc.courtbouillon.org/weasyprint/stable/first_steps.html#windows). But
+please keep in mind that WeasyPrint must be installed as a dependency of Billing Yard and not directly using your OS
+package manager.
 
 ### Installing Billing Yard
 
 First you need to decide whether you want to use Virtual Environment or install Billing Yard globally. But note that
-installing in Virtual Environment is always preferred way. Then just make sure you are using Python 3.9 or newer and run
-following command, and you are done.
+installing in Virtual Environment is always preferred way. Then just make sure you are using Python 3.9 or newer and
+run following command, and you are done.
 
 ```shell
 pip install billingyard
 ```
 
 ## Basic usage
 
@@ -100,15 +128,15 @@
 
 * **company** - the business name of the business entity
 * **street** - the street in the address of the business entity
 * **city** - the city in the address of the business entity
 * **zip_code** - the zip code in the address of the business entity
 * **country** - the country in the address of the business entity
 * **company** - the identifier given by Czech authority of the business entity
-* **street** - the identifier for VAT purpose of the business entity
+* **vat_id** - the identifier for VAT purpose of the business entity
     * optional if business entity is not a VAT payer
 
 ### Invoice for a non VAT payer
 
 Below you can find the self explaining example of a non VAT payer invoice with further description.
 
 ```json
@@ -129,15 +157,15 @@
       "unit_price": 1500
     }
   ]
 }
 ```
 
 * **invoice_number** - a unique identifier of the invoice
-    * completely up to you, but keep in mind local policies from governmane
+    * completely up to you, but keep in mind local policies from government
 * **issue_date** - the date of issue of the invoice
     * optional, if not set current date is used
 * **due_date** - the last day, when the invoice must be paid
 * **currency** - the currency in which is the invoice issued
 * **bank** - the bank of the sender business entity
 * **bank_account** - the bank account number of the sender business entity
 * **payment_method** - the agreed instrument to pay the invoice
@@ -182,15 +210,15 @@
       "vat_rate": 0.21
     }
   ]
 }
 ```
 
 * **invoice_number** - a unique identifier of the invoice
-    * completely up to you, but keep in mind local policies from governmane
+    * completely up to you, but keep in mind local policies from government
 * **issue_date** - the date of issue of the invoice
     * optional, if not set current date is used
 * **supply_date** - the date of taxable supply
     * optional, if not set current date is used
 * **due_date** - the last day, when the invoice must be paid
 * **currency** - the currency in which is the invoice issued
 * **bank** - the bank of the sender business entity
@@ -238,10 +266,10 @@
 The option `--vat` is used to generate an invoice for a VAT payer sender business entity. Please do not forget, that in
 this case, you have to also provide correct invoice JSON data file with all needed attributes.
 
 ## License
 
 This software is released under MIT License and use other third party software.
 
-* [Click](https://github.com/pallets/click/blob/master/LICENSE.rst)
-* [Jinja2](https://github.com/pallets/jinja/blob/master/LICENSE.rst)
+* [Click](https://github.com/pallets/click/blob/main/LICENSE.txt)
+* [Jinja2](https://github.com/pallets/jinja/blob/main/LICENSE.txt)
 * [WeasyPrint](https://github.com/Kozea/WeasyPrint/blob/master/LICENSE)
```

### Comparing `billingyard-1.0.1/billingyard/billingyard.py` & `billingyard-1.1.0/billingyard/billingyard.py`

 * *Files identical despite different names*

### Comparing `billingyard-1.0.1/billingyard/cli.py` & `billingyard-1.1.0/billingyard/cli.py`

 * *Files identical despite different names*

### Comparing `billingyard-1.0.1/billingyard/invoice_processors.py` & `billingyard-1.1.0/billingyard/invoice_processors.py`

 * *Files identical despite different names*

### Comparing `billingyard-1.0.1/billingyard/models.py` & `billingyard-1.1.0/billingyard/models.py`

 * *Files identical despite different names*

### Comparing `billingyard-1.0.1/billingyard/parser.py` & `billingyard-1.1.0/billingyard/parser.py`

 * *Files identical despite different names*

### Comparing `billingyard-1.0.1/billingyard/templates/invoice.html` & `billingyard-1.1.0/billingyard/templates/invoice.html`

 * *Files identical despite different names*

### Comparing `billingyard-1.0.1/billingyard/templates/vat_invoice.html` & `billingyard-1.1.0/billingyard/templates/vat_invoice.html`

 * *Files identical despite different names*

### Comparing `billingyard-1.0.1/setup.py` & `billingyard-1.1.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='billingyard',
-    version='1.0.1',
+    version='1.1.0',
     author='Martin Vondrák',
-    author_email='martinvondrak@icloud.com',
+    author_email='martin@martinvondrak.cz',
     description='CLI invoice generator for business entities in the Czech republic',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/MartinVondrak/billing-yard',
     keywords='invoice,cli,generator',
     classifiers=[
         'Environment :: Console',
         'Intended Audience :: End Users/Desktop',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: Czech',
         'Programming Language :: Python :: 3',
         'Topic :: Office/Business :: Financial :: Accounting',
+        'Development Status :: 5 - Production/Stable',
     ],
     packages=find_packages(),
     package_data={'billingyard': ['templates/*.html']},
+    python_requires='>=3.9',
     install_requires=[
-        'Click>=7.1.2,<8',
-        'Jinja2>=2.11.3,<3',
-        'WeasyPrint>=52.2,<53'
+        'Click>=8.1.7,<9',
+        'Jinja2>=3.1.3,<4',
+        'WeasyPrint>=62.0,<63'
     ],
     entry_points={
         'console_scripts': [
             'billingyard = billingyard.__main__:main',
         ],
     },
     zip_safe=False,
```

