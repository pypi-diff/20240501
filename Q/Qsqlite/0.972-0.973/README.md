# Comparing `tmp/Qsqlite-0.972.tar.gz` & `tmp/Qsqlite-0.973.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Qsqlite-0.972.tar", last modified: Tue May  3 15:29:44 2022, max compression
+gzip compressed data, was "Qsqlite-0.973.tar", last modified: Wed May  1 03:48:08 2024, max compression
```

## Comparing `Qsqlite-0.972.tar` & `Qsqlite-0.973.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 laicj      (501) staff       (20)        0 2022-05-03 15:29:44.987917 Qsqlite-0.972/
--rw-r--r--   0 laicj      (501) staff       (20)     1130 2022-03-12 04:41:00.000000 Qsqlite-0.972/LICENSE
--rw-r--r--   0 laicj      (501) staff       (20)    40500 2022-05-03 15:29:44.987781 Qsqlite-0.972/PKG-INFO
-drwxr-xr-x   0 laicj      (501) staff       (20)        0 2022-05-03 15:29:44.986894 Qsqlite-0.972/Qsqlite/
--rw-r--r--   0 laicj      (501) staff       (20)    90880 2022-05-03 15:29:12.000000 Qsqlite-0.972/Qsqlite/Qsqlite.py
--rw-r--r--   0 laicj      (501) staff       (20)      168 2022-03-27 14:05:41.000000 Qsqlite-0.972/Qsqlite/__init__.py
-drwxr-xr-x   0 laicj      (501) staff       (20)        0 2022-05-03 15:29:44.987610 Qsqlite-0.972/Qsqlite.egg-info/
--rw-r--r--   0 laicj      (501) staff       (20)    40500 2022-05-03 15:29:44.000000 Qsqlite-0.972/Qsqlite.egg-info/PKG-INFO
--rw-r--r--   0 laicj      (501) staff       (20)      213 2022-05-03 15:29:44.000000 Qsqlite-0.972/Qsqlite.egg-info/SOURCES.txt
--rw-r--r--   0 laicj      (501) staff       (20)        1 2022-05-03 15:29:44.000000 Qsqlite-0.972/Qsqlite.egg-info/dependency_links.txt
--rw-r--r--   0 laicj      (501) staff       (20)       42 2022-05-03 15:29:44.000000 Qsqlite-0.972/Qsqlite.egg-info/entry_points.txt
--rw-r--r--   0 laicj      (501) staff       (20)        8 2022-05-03 15:29:44.000000 Qsqlite-0.972/Qsqlite.egg-info/top_level.txt
--rw-r--r--   0 laicj      (501) staff       (20)       38 2022-05-03 15:29:44.987952 Qsqlite-0.972/setup.cfg
--rw-r--r--   0 laicj      (501) staff       (20)      758 2022-05-03 15:29:19.000000 Qsqlite-0.972/setup.py
+drwxr-xr-x   0 laicj      (501) staff       (20)        0 2024-05-01 03:48:08.826836 Qsqlite-0.973/
+-rw-r--r--   0 laicj      (501) staff       (20)     1130 2022-03-12 04:41:00.000000 Qsqlite-0.973/LICENSE
+-rw-r--r--   0 laicj      (501) staff       (20)    41114 2024-05-01 03:48:08.826711 Qsqlite-0.973/PKG-INFO
+drwxr-xr-x   0 laicj      (501) staff       (20)        0 2024-05-01 03:48:08.825815 Qsqlite-0.973/Qsqlite/
+-rw-r--r--   0 laicj      (501) staff       (20)    93480 2024-04-30 09:45:22.000000 Qsqlite-0.973/Qsqlite/Qsqlite.py
+-rw-r--r--   0 laicj      (501) staff       (20)      168 2022-03-27 14:05:41.000000 Qsqlite-0.973/Qsqlite/__init__.py
+drwxr-xr-x   0 laicj      (501) staff       (20)        0 2024-05-01 03:48:08.826536 Qsqlite-0.973/Qsqlite.egg-info/
+-rw-r--r--   0 laicj      (501) staff       (20)    41114 2024-05-01 03:48:08.000000 Qsqlite-0.973/Qsqlite.egg-info/PKG-INFO
+-rw-r--r--   0 laicj      (501) staff       (20)      213 2024-05-01 03:48:08.000000 Qsqlite-0.973/Qsqlite.egg-info/SOURCES.txt
+-rw-r--r--   0 laicj      (501) staff       (20)        1 2024-05-01 03:48:08.000000 Qsqlite-0.973/Qsqlite.egg-info/dependency_links.txt
+-rw-r--r--   0 laicj      (501) staff       (20)       42 2024-05-01 03:48:08.000000 Qsqlite-0.973/Qsqlite.egg-info/entry_points.txt
+-rw-r--r--   0 laicj      (501) staff       (20)        8 2024-05-01 03:48:08.000000 Qsqlite-0.973/Qsqlite.egg-info/top_level.txt
+-rw-r--r--   0 laicj      (501) staff       (20)       38 2024-05-01 03:48:08.826879 Qsqlite-0.973/setup.cfg
+-rw-r--r--   0 laicj      (501) staff       (20)      758 2024-04-25 04:09:22.000000 Qsqlite-0.973/setup.py
```

### Comparing `Qsqlite-0.972/LICENSE` & `Qsqlite-0.973/LICENSE`

 * *Files identical despite different names*

### Comparing `Qsqlite-0.972/PKG-INFO` & `Qsqlite-0.973/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Qsqlite
-Version: 0.972
+Version: 0.973
 Summary: Quick Sqlite Tools
 Home-page: https://github.com/wolf71/Qsqlite
 Author: Charles Lai
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -15,27 +15,27 @@
 
 # Quick SQLite Cmd/Script Tools
 
 ## Introduction to Qsqlite
 - A **command line tool** to interactively manipulate sqlite or mysql databases for fast data processing, analysis, statistics, and graphical presentation;
   - General sqlite operations (just like the sqlite cmd tools); can be easily manipulated using sql statements.
   - Support sqlite and sqlite memory database (:memory:), support mysql database, copy whole mysql database to sqlite, copy tables between different sqlite databases.
-  - Load csv or json data, or export select results to csv file.
+  - Load csv/tsv or json data, or export select results to csv/tsv file.
   - Draw graphs with the data obtained by select statement, such as: scatter, line, histogram (distribution), violin graph (based on data distribution).
   - Provide a series of extended sqlite functions, supporting regular operations, text-based sum operations, Chinese ID recognition, and other extended functions.
 - A **script interpreter** that can write script files to batch and automate a series of operations to achieve data processing, analysis, and report output;
   - Provides sql statement-based scripting capabilities, allowing you to automate batch operations and output the results to an html file.
   - Support extended loop/lend with nested support for loop statements, which is convenient for some operations that can't be handled by sql statements.
   - Support for formatting the output syntax of select results, to facilitate the generation of formatted reports.
   - The graphs are saved inline in the output html file, so that only a single html file can be sent to show all the graphs in their entirety.
 - A **Web Server** and **Job Server** that can provide web or scheduled task processing backend services based on a database;
   - The web server can be scripted to enable data query and data insertion operations to facilitate the interaction of data statistics and analysis results in a browser-based.
   - Job server can be defined by scripts to achieve regular data cleaning, data aggregation, analysis, report generation, and output as local files or send emails to share the results.
 - A **python libray**  Can be imported using: from Qsqlite import Qexec , for use in python or jupyter/ipython ipynb notebooks using Qexec(cmds) calls, cmds can be a string with newlines,including a series of commands or a command.
-- **Summary**: With sqlite's powerful sql syntax and high performance, Qsqlite hopes to enable you to efficiently use the power of sqlite and sql syntax to **quickly** organize, analyze, aggregation, and show result; and collaborate with Excel by exporting/importing csv files when needed to achieve greater efficiency.
+- **Summary**: With sqlite's powerful sql syntax and high performance, Qsqlite hopes to enable you to efficiently use the power of sqlite and sql syntax to **quickly** organize, analyze, aggregation, and show result; and collaborate with Excel by exporting/importing csv/tsv files when needed to achieve greater efficiency.
 
 ![Draw function demo](https://github.com/wolf71/Qsqlite/blob/master/draw.jpeg?raw=true)
 
 ## Quickly start
 1. install
   - pip3 install Qsqlite , and then open cmd/Term enter: Qsqlite 
   - Copy Qsqlite.py to local directory, and then open cmd/Term **python Qsqlite.py** (please using python3)
@@ -70,14 +70,15 @@
   - **open :memory:** open sqlite memory database file; can use memory database for temporary data processing, transit.
   - **db** show current open database name.
   - If the provided file name does not exist, a new database file will be created.
 - 1.2 MySQL Database Support
   1. create a MySQL database connection with **mysql dbname server user password**
     - For example: mysql test 127.0.0.1 root pwd (To set the MySQL port number, use: mysql test 127.0.0.1:3308 root pwd)
     - You can set multiple MySQL databases with mysql command and then switch them with open;
+    - Enter mysql will display currently mysql server list; if none setup, a reminder will show;
   2. Use **open #dbname#** to open/switch the MySQL database;
   3. some MySQL commands
     - show databases     Lists all databases on the database server
     - show tables        Lists all tables in the current database
     - show keys from tb  Lists the indexes contained in a table
 - 1.3 Common Commands
   - **?** Show help info, or **? str** search help str.
@@ -129,16 +130,19 @@
     - tab01 ( "r1" text, "r2" text, "r3" text )
   - If the csv file contains table header information (the first line of the csv file), the parameter 1 can be added at the end for correct identification.
     - using: **loadcsv filecsv tab01 1**
     - Set the table information based on the csv table header information, for example
       - tab01 ( "ID" text, "Name" text, "Tele" text )
   - loadcsv also support **tsv format** file (\t split type), just using: loadcsv test.tsv tb1 1
   - loadcsv also support **bioinformatics .maf/.vcf/.sam/.gtf/.gff/.gpd file**, just using: loadcsv test.maf tb1   or  loadcsv test.vcf tb1
-- 2.2 Exporting csv
-  - Use **>csv csv file name 0/1** (The parameter 0/1 indicates whether to export the table header information. 0-no export, 1-export)
+  - loadcsv support gzip / zip file, Judging by file extension; etc: test.tsv.gz / test.gtf.gz / test.csv.zip
+- 2.2 Exporting csv/tsv
+  - Use **>csv csv/tsv file name 0/1** (The parameter 0/1 indicates whether to export the table header information. 0-no export, 1-export)
+  - if file name has xxx.tsv will export tsv format, otherwise csv format.
+  - if file name has xxx.tsv.gz or xxx.csv.gz , will be exported in the corresponding format and gzip compressed.
   - Example: select * from table1 where n=300 >csv user1.csv 1 , export the contents of a table to user1.csv file by select and export the table header information (the first line of the exported csv file is the database table header information)
   - Example: select ID, name, sum(val) as val from tab1 group by ID limit 100 >csv test1.csv 0
 - 2.3 Load Simply json data, Example: JSON file t1.json like this:
 ```json
 [{"Corp": "Apple", "ID": 123}, {"Corp": "Microsoft", "ID": 456}, {"Corp": "IBM", "ID": 789}]
 ```
   - using: **loadjson t1.json corp**
@@ -166,14 +170,15 @@
         - locus text, locusinfo text, reference text, accession text, version text, dblink text, keywords text, source text, organism text, comment text			
       - (03) tb01_ref (table name add _ref, corresponding to all the contents of each LOCUS' REFERENCE description)
         - locus text, reference text, title text, authors text, journal text, pubmed text, remark text
     - A GenBank file may contain more than one Features block, which can be distinguished by locus;
     - start, end content only for (123..345) Simple location, for join/complement such complex location, fill in 0, 0, real content in the location field.
     - The note field is a compound field that aggregates all other contents of Features here, using item1=value1;item2=value2 ... Schema expression.
     - The translation content of Features, the file's sequence information ORIGIN are ignored.
+    - Support xxx.gb.gz or xxx.gbff.gz, if file name last .gz , will open it's as gzip format.
 - 2.6 Crawl website data, parse and write to database
   - using: **loop loadweb url=https://xxx.xxx.com/xxx re=<a href="/search:(.+?)">(\d+)</a>**, base on python regular module, Qsqlite loop nesting function, can achieve complex web data crawling and content extraction, and then write to the database.
   - loadweb parameter:
     - Required: url=web url address, include https:// or http://. Qsqlite will crawl the web page, and then extract the content using the pythone regular module.
     - Required: re=the regular expression. This expression using by Python re.findall against the fetched page, get data.
     - Optional: ext=additional parameter to pass the parameters from the previous loop to the next, e.g. ext=_^1_, _^3_
   - Example: (For more detailed and complete examples, please refer to the demo directory qCrawlWeb.txt script.)
@@ -536,14 +541,15 @@
 - 2022/03/08   V0.89 BugFix and add ls cmd and optimize loadcsv/>csv function.
 - 2022/03/13   V0.9  BugFix and add some demo.
 - 2022/03/14   V0.91 Add navg, rdelta sqlite ext-function and rewrite help.
 - 2022/03/27   V0.93 Add draw bar function, SQLite median, Qselect function.
 - 2022/04/02   V0.95 Add tsv/maf/vcf file support on loadcsv, load Chinese font for draw.
 - 2022/04/08   V0.96 Add .sam/.gtf/.gff/.gpd file support on loadcsv, add loadgb / exec function.
 - 2022/04/20   V0.97 Add ext-sql function: summary, and loop loadweb, download function.
+- 2024/04/25   V0.973 fix summary std function bug, add >csv support tsv format. add .gz/.zip support.
 
 ## sqlite references
 - SQlite3 Doc
   - https://docs.python.org/zh-cn/3/library/sqlite3.html
 - SQlite3 System Function Ref
   - https://www.sqlite.org/lang_corefunc.html
 - SQlit Ext
```

### Comparing `Qsqlite-0.972/Qsqlite/Qsqlite.py` & `Qsqlite-0.973/Qsqlite/Qsqlite.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 '''
   Qsqlite Quick sqlite Tools
            (c) 2020 - 2022
            By: Charles Lai
 '''
 
-__version__ = 0.972
+__version__ = 0.973
 __author__ = 'Charles Lai'
 
 help_str = '''
-====== Qsqlite (Quick Sqlite Tools) Help (V0.972) ======
+====== Qsqlite (Quick Sqlite Tools) Help (V0.973) ======
 # command
  @ q - quit
  @ ?/h - help    or  ? querystr    etc: ? draw;    cls / clear - clear screen. (windows-cls, mac/linux-clear)
  @ #/-  comment;  three ' for block comment;    { } for multi-lines block code.  ( { and } on new line )
  @ l - List last 12 cmd History; la - List all History; l0 - run last cmd; l8 - run #8 cmd; l> file / l< file (save/load cmd History to/from file )
  @ exec script - Execute a Qsqlite Script, etc: exec qInit.txt
  @ ls - List current dir files; ls *.csv or ls city
@@ -23,18 +23,19 @@
  @ db - Show open database name  / @ dinfo on/off - debug info on/off or using dinfo show status
  @ info 0/1/2/3 - show database info; 0-table / 1-index (for MySQL 2-tables; 3-table struct)
  @ >[ _@1_, _@2_, ...] select result reformat. (_@0_ for order id)
  @ copy dbname table_insert sqlcmd (insert select data to table_insert)
  - etc: copy new.db tb01 select * from tb00 where age < 100 limit 10
  - !same db,can using: insert into tb01 select a,b,c from tb00 where a<10
  @ dump #mysqldb# sqlitedb (Dump mysql database to sqlite with data.)
- @ loadcsv - load csv file and copy to new table (and support .tsv file, bioinformatics .maf/.vcf/.sam/.gtf/.gff/.gpd file)
+ @ loadcsv - load csv file and copy to new table (and support .tsv file, bioinformatics .maf/.vcf/.sam/.gtf/.gff/.gpd file; support .gz or .zip file)
  - etc: loadcsv file.csv table1	 or loadcsv file.csv table1 1 (csv line 1 as title)
+ - etc: loadcsv file.tsv.gz table1 or loadcsv file.gtf.zip
  @ loadgb - load bioinformatics genbank file features info to table. (etc: loadgb file tb01)
- @ >csv file.csv 1/0  export select result to csv file (0/1 - with/without rowinfo)
+ @ >csv file.csv 1/0  export select result to csv/tsv file (0/1 - with/without rowinfo; file.tsv export tsv format; file.csv.gz export csv file and gzip.)
  @ loadjson - load json file and copy to new table
  - etc: loadjson file.json table1 item (when item set, it's will select data on json item.)
  @ loop/lend function . Etc: select i1,i2 from tab / select * from tab where a = _^1_ and b = '_^2_' /lend
  - or : loop [(1,2,...),(1,2,...)...] / echo _^0_ _^1_ / lend
  @ loop loadweb function. Etc: loop loadweb url=https://xxx.xxx/xxx re=href="/searc/(.+?)" ext=_^1_
  @ loop [ i for i in loadweb('url=https://xxx.xxx/xxx re=href="/searc/(.+?)" ext=_^1_')[:1] ] , using in [ ]
  @ loop [i for i in getTableCols('c')[4:]]  using getTableCols function transform table cols to rows
@@ -90,23 +91,23 @@
  - Sqlite String add using : 'a' || 'b' ; select 'a' || x'0d' || x'0a' || 'apple'
  - cast(x as int) or cast(7/2.0 as int) or x+0 or x+0.0 / substr(str,begin,len)
  - select rowid, * from c (select system rowid); select last_insert_rowid()
  - with recursive xx(x) as (select 1 union select x+1 from xx where x<(select max(regfn(',',fn)) from tb1)) select id,regfind('(.+?)(?:,|$)',fn,x) as s from tb1, xx where s != '')  --> let a fn col like 'fun1,fun2,fun3,fun4' to row: fun1 / fun2 / fun3 / fun4 4 rows. (col to rows)
  - SQlite system function: count, max, min, avg, sum, substr, random, abs, upper, lower, length, trim, ltrim, rtrim, replace('apple','app','*'), typeof, hex, like('%12%',name) or like('23_33',tel) or like('100\%F%', name, '\'), iif(c,x,y), coalesce(t1,t2,t3...), hex(randomblob(16)), printf('%08d is %.2fs on %-10s %,d', 34123, 3123.334, 'apple',12345) ... 
  - Convert 1/22/20 date string to Sqlite format 2020-01-22 using: date(printf('20%d-%02d-%02d', regfind('(\d+?)(?:/|$)',d,3), regfind('(\d+?)(?:/|$)',d,1), regfind('(\d+?)(?:/|$)',d,2)))
  - Explain to see the SQLite execution policy: explain select ID from Room where m > 15
+ - loadcsv xxx.gtf gene , And then: select regfind('gene_id "(.+?)";',attributes,1) as id, regfind('gene_name "(.+?)";',attributes,1) as gene, regfind('gene_type "(.+?)";',attributes,1) as type from gene
  - VACUUM : optimize the database file (small size) / pragma table_info(tb1)  will list all tb1 cols info.
 '''
 
-import os, sys, math, re, time, base64, csv
+import os, sys, math, re, time, base64, csv, gzip, zipfile
 import sqlite3
 from http.server import BaseHTTPRequestHandler, HTTPServer
 from urllib.parse import urlparse, unquote
-from io import BytesIO,StringIO
-from random import random
+from io import BytesIO, StringIO, TextIOWrapper
 
 # for Linux/MacOS input() can get history by arrow key
 try:
   import readline
 except:
   pass
 
@@ -682,15 +683,18 @@
 class Cstd:
   def __init__(self):
     self.count = []
 
     # 每一行数据会调用这里
   def step(self, *value):
     for i in value:
-      self.count.append(i)
+      try:
+        self.count.append(float(i))
+      except:
+        pass
 
     # 最后返回结果
   def finalize(self):
     # 计算均值
     m = sum(self.count)/len(self.count)
     # 计算方差
     z = [(m-i)**2 for i in self.count]
@@ -766,18 +770,19 @@
       # 计算中位数 (对于偶数个数需要计算两个数的均值)
       med = sum(v) / len(v)
       # 计算 max, min
       max, min = self.count[-1], self.count[0]
       # 计算均值
       avg = sum(self.count) / s
       # 计算方差
-      z = [(med-i)**2 for i in self.count]
-      # 汇总方差，而后开平方得到标准差
-      std = ( sum(z)/s ) ** 0.5
-      # 计算 直方图
+      z = [(avg-i)**2 for i in self.count]
+      # 汇总方差，而后开平方得到 标准方差 (这里计算的是总体标准差)
+      # 如果要计算样本标准差: std = ( sum(z)/(s-1 if s > 1 else s) ) ** 0.5
+      std = ( sum(z)/ s ) ** 0.5
+      # 计算 直方图 (把数据根据 最大-最小 值均分为 hn 段, 而后看看大致落在哪段的数量)
       d = (max - min) / (hn - 1)
       o = [0 for i in range(hn)]
       # 避免 d=0 引发错误
       if d > 0:
         for i in self.count:
           o[ round( (i - min) / d ) ] += 1
       else:
@@ -953,19 +958,29 @@
 
 #
 # load csv file to new table
 #		参数：数据库, csv文件名, 表名, ftype是否第一行过滤掉(1表示过滤掉), 是否 tsv 格式(\t分割的csv)
 #
 def loadCSV(dbname, fname, tname, ftype, tsv=0):
   # 默认用 utf-8 打开文件，如果出错，则改用默认方式
-  wt = 2				# 默认尝试2次，一次用UTF-8解码，一次GBK
-  bt = time.time()	
+  wt = ['GBM','utf-8-sig']				# 默认尝试2次，一次用UTF-8解码，一次GBK; wt.pop(), 顺序反写
+  bt = time.time()
+  fname = fname.strip()
+  # 根据文件名判断压缩文件类别 (z_type: 0-非压缩, 1-gzip, 2-zip)
+  if fname[-3:].upper() == '.GZ':
+    z_type = 1
+    l_ext = fname[-7:-3].upper()
+  elif fname[-4:].upper() == '.ZIP':
+    z_type = 2
+    l_ext = fname[-8:-4].upper()
+  else:
+    z_type = 0
+    l_ext = fname[-4:].upper()
   # 根据文件名, 判断 CSV or TSV
   # 对于 .maf / .vcf 文件, 需要跳过前面部分(p_ext) #/## 的注释, p_n 表示 p_ext 的长度
-  l_ext = fname.strip()[-4:].upper()
   if l_ext == '.TSV':
     tsv = 1
     p_ext, p_n = '', 0
   elif l_ext == '.MAF':
     ftype, tsv = 1, 1
     p_ext, p_n = '#', 1
   elif l_ext == '.VCF':
@@ -979,21 +994,27 @@
     p_ext, p_n = '#', 1
   elif l_ext == '.GPD':
     ftype, tsv = 0, 1
     p_ext, p_n = '#', 1
   else:
     p_ext, p_n = '', 0
   # 读取文件, 检查是否符合要求
-  while wt > 0:
-    wt -= 1
+  while wt:
+    en_code = wt.pop()
     try:
-      if wt == 1:	# 先用 UTF-8 读取
-        f = open(fname, 'r', encoding='utf-8-sig', newline='')	#utf-8-sig也能解析utf-8内容
-      else:		# 否则改用 GBK
-        f = open(fname, 'r', encoding='GBK', newline='')
+      # 根据文件压缩类型, 使用不同的文件打开方式 (1-gzip, 2-zip, 0-normal)
+      # utf-8-sig也能解析utf-8内容
+      if z_type == 1:
+        f = gzip.open(fname, 'rt', encoding = en_code)
+      elif z_type == 2:
+        gz_f = zipfile.ZipFile(fname, 'r')
+        # 获取 ZIP 文件中的第一个文件, 并且通过 io.TextIOWrapper 方式来解码
+        f = TextIOWrapper(gz_f.open(gz_f.namelist()[0], 'r'), encoding = en_code)
+      else:
+        f = open(fname, 'r', encoding = en_code, newline = '')	
       # 读取文件 (cnt - 列数, rsize - 行数, skip_r - 跳过前面 行数, i_note: maf/vcf 文件注释 )
       cnt, err, rsize, skip_r = 0, 0, 0, 0
       i_note = []
       # 如果是 TSV 格式, 按照 \t 分割
       if tsv:
         r = csv.reader(f, delimiter='\t')
       else:
@@ -1057,16 +1078,29 @@
     # 针对 SQLite/MySQL 不同构建插入语句
     if check_mysql(dbname):
       rcnt = ','.join(['%s' for i in range(cnt)])
     else:
       rcnt = ','.join(['?' for i in range(cnt)])
     # create new table
     cu.execute('create table if not exists %s (%s);'%(tname,row))
-    # 文件指针回到开头位置
-    f.seek(0, 0)
+    # 文件指针回到开头位置(因为 zipfile 不支持 seek 功能, 因此需要重新打开)
+    if z_type == 2:
+      # 先关闭之前打开的文件，而后再打开
+      f.close()
+      gz_f.close()
+      # 重新打开文件
+      gz_f = zipfile.ZipFile(fname, 'r')
+      # 获取 ZIP 文件中的第一个文件, 并且通过 io.TextIOWrapper 方式来解码
+      f = TextIOWrapper(gz_f.open(gz_f.namelist()[0], 'r'), encoding = en_code)
+      if tsv:
+        r = csv.reader(f, delimiter='\t')
+      else:
+        r = csv.reader(f) #, delimiter=' ', quotechar='|')
+    else:
+      f.seek(0, 0)
     # 如果第一行是表头, 则递增 跳过计数器
     if ftype == 1: skip_r += 1
     # 跳过 头部 注释记录
     while skip_r:
       next(r)
       skip_r -= 1
     # 批量写入数据 (对于 非 csv/tsv 的生物信息学文件, 可能中间包含注释, 因此需要用逐行解析方式)
@@ -1269,16 +1303,19 @@
   # 搜寻 /Qualifiers 内容, 格式: 21个空格 + /xxx=xxx , 例如: /gene="ORF1ab"
   re_fval = re.compile('^ {21}/(.+)=(.+)$')
   # 确认 Location 是否有效 (2 / 2..30 / 2.30 / <2..30 / <2..>30 / 2^3 )
   re_location = re.compile('^(?:\<*|.+?\:)\d+(?:$|(?:\.{1,2}\>?|\^)\d+$)$')
   # 简单的 Location 提取 (33..456 / 33.456) -> start,end
   re_slocation = re.compile('^(\d+)(?:\.{1,2})(\d+)$')
 
-  # 读取文件
-  f = open(f_name, 'r',  encoding='utf-8')
+  # 读取文件(如果后缀.gz, 则以 gzip 方式打开)
+  if f_name[-3:].upper() == '.GZ':
+    f = gzip.open(f_name, 'rt', encoding='utf-8')
+  else:
+    f = open(f_name, 'rt', encoding='utf-8')
   for i in f:
     # 初始化已解析标志
     r_ok = 0
     # 如果已找到 Feature 部分, 则进行解析
     if f_flag:
       # 1. 搜寻 item 内容  (例如: /gene="ORF1ab" )
       if r_ok == 0:
@@ -1524,16 +1561,26 @@
       csv_flag = 1 + int(csv_p[0][2]) if csv_p[0][2] else 2
       # 判断文件名有效性
       if len(csv_file) < 3 or len(sql) < 10:
         print('!!!CSV File name error. or SQL Command Error')
         return -1
       # 输出到csv文件
       else:
-        f = open(csv_file, 'w', encoding='utf_8_sig', newline='')		#excel 用utf-8 有问题
-        csv_f = csv.writer(f)
+        # 判断是否需要使用 gzip 压缩输出文件
+        if csv_file[-3:].upper() == '.GZ':
+          f = gzip.open(csv_file, 'wt', encoding='utf_8_sig', newline='')
+          ext_flag = csv_file[-7:-3]
+        else:
+          f = open(csv_file, 'wt', encoding='utf_8_sig', newline='')		#excel 用utf-8 有问题
+          ext_flag = csv_file[-4:]
+        # 根据文件后缀判断(.csv or .tsv)来设置参数
+        if ext_flag.upper() == '.TSV':
+          csv_f = csv.writer(f, delimiter='\t')
+        else:
+          csv_f = csv.writer(f)
   # Connect SQLite
   bt = time.time()
   cx, cxt = dbconn(sqlite_db)
   cu = cx.cursor()
   Sqlite_ext_reset()
   cu.execute(sql)
   # 统计查询耗时
@@ -1570,15 +1617,15 @@
   # 表示 结果集 为空, 可能是update/del等语句，从 cu.rowcount 获取影响行数
   if cnt == 1:
     cnt = cu.rowcount
   else:
     cnt -= 1
   if csv_flag:
     f.close()
-    if o_disp: print('-- Total Write %d lines to csv file.'%(cnt))
+    if o_disp: print('-- Total Write %d lines to %s .'%(cnt, csv_file))
   elif not o:
     if o_disp: print('------ Total: %d ------ '%(cnt))
   cx.commit()
   cu.close()
   if cxt: cx.close()		# 如非内存连接，则关闭
   # 返回执行的结果 (列信息, 数据集)
   return rcol, retv
@@ -1885,15 +1932,20 @@
       elif not os.path.exists(db):
         print('@ %s Not Found, Create it.'%(db))
     elif cmd[:5] == 'MYSQL':
       s = re.findall('(.+?) (.+?) (.+?) (.+$)',cmd0[6:])
       if s:
         mysql_srv[s[0][0]] = [s[0][1],s[0][2],s[0][3]]
       else:
-        print('!!! Please using: mysql dbname serverip user password')
+        # 显示 当前存储的 mysql 列表
+        if mysql_srv:
+          for t_mysql in mysql_srv:
+            print(f'- MySQL Server: [{t_mysql}], {mysql_srv[t_mysql]}')
+        else:
+          print('!!! Please using: mysql dbname serverip user password')
     elif cmd[:2] == 'DB':
       print('- SQLite Version: %s'%(sqlite3.sqlite_version))
       if db:
         print('Database: %s '%(db))
       else:
         print('!!! Not Open Database, Using open dbname to open.')
     elif cmd[:4] == 'ECHO':
```

### Comparing `Qsqlite-0.972/Qsqlite.egg-info/PKG-INFO` & `Qsqlite-0.973/Qsqlite.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Qsqlite
-Version: 0.972
+Version: 0.973
 Summary: Quick Sqlite Tools
 Home-page: https://github.com/wolf71/Qsqlite
 Author: Charles Lai
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -15,27 +15,27 @@
 
 # Quick SQLite Cmd/Script Tools
 
 ## Introduction to Qsqlite
 - A **command line tool** to interactively manipulate sqlite or mysql databases for fast data processing, analysis, statistics, and graphical presentation;
   - General sqlite operations (just like the sqlite cmd tools); can be easily manipulated using sql statements.
   - Support sqlite and sqlite memory database (:memory:), support mysql database, copy whole mysql database to sqlite, copy tables between different sqlite databases.
-  - Load csv or json data, or export select results to csv file.
+  - Load csv/tsv or json data, or export select results to csv/tsv file.
   - Draw graphs with the data obtained by select statement, such as: scatter, line, histogram (distribution), violin graph (based on data distribution).
   - Provide a series of extended sqlite functions, supporting regular operations, text-based sum operations, Chinese ID recognition, and other extended functions.
 - A **script interpreter** that can write script files to batch and automate a series of operations to achieve data processing, analysis, and report output;
   - Provides sql statement-based scripting capabilities, allowing you to automate batch operations and output the results to an html file.
   - Support extended loop/lend with nested support for loop statements, which is convenient for some operations that can't be handled by sql statements.
   - Support for formatting the output syntax of select results, to facilitate the generation of formatted reports.
   - The graphs are saved inline in the output html file, so that only a single html file can be sent to show all the graphs in their entirety.
 - A **Web Server** and **Job Server** that can provide web or scheduled task processing backend services based on a database;
   - The web server can be scripted to enable data query and data insertion operations to facilitate the interaction of data statistics and analysis results in a browser-based.
   - Job server can be defined by scripts to achieve regular data cleaning, data aggregation, analysis, report generation, and output as local files or send emails to share the results.
 - A **python libray**  Can be imported using: from Qsqlite import Qexec , for use in python or jupyter/ipython ipynb notebooks using Qexec(cmds) calls, cmds can be a string with newlines,including a series of commands or a command.
-- **Summary**: With sqlite's powerful sql syntax and high performance, Qsqlite hopes to enable you to efficiently use the power of sqlite and sql syntax to **quickly** organize, analyze, aggregation, and show result; and collaborate with Excel by exporting/importing csv files when needed to achieve greater efficiency.
+- **Summary**: With sqlite's powerful sql syntax and high performance, Qsqlite hopes to enable you to efficiently use the power of sqlite and sql syntax to **quickly** organize, analyze, aggregation, and show result; and collaborate with Excel by exporting/importing csv/tsv files when needed to achieve greater efficiency.
 
 ![Draw function demo](https://github.com/wolf71/Qsqlite/blob/master/draw.jpeg?raw=true)
 
 ## Quickly start
 1. install
   - pip3 install Qsqlite , and then open cmd/Term enter: Qsqlite 
   - Copy Qsqlite.py to local directory, and then open cmd/Term **python Qsqlite.py** (please using python3)
@@ -70,14 +70,15 @@
   - **open :memory:** open sqlite memory database file; can use memory database for temporary data processing, transit.
   - **db** show current open database name.
   - If the provided file name does not exist, a new database file will be created.
 - 1.2 MySQL Database Support
   1. create a MySQL database connection with **mysql dbname server user password**
     - For example: mysql test 127.0.0.1 root pwd (To set the MySQL port number, use: mysql test 127.0.0.1:3308 root pwd)
     - You can set multiple MySQL databases with mysql command and then switch them with open;
+    - Enter mysql will display currently mysql server list; if none setup, a reminder will show;
   2. Use **open #dbname#** to open/switch the MySQL database;
   3. some MySQL commands
     - show databases     Lists all databases on the database server
     - show tables        Lists all tables in the current database
     - show keys from tb  Lists the indexes contained in a table
 - 1.3 Common Commands
   - **?** Show help info, or **? str** search help str.
@@ -129,16 +130,19 @@
     - tab01 ( "r1" text, "r2" text, "r3" text )
   - If the csv file contains table header information (the first line of the csv file), the parameter 1 can be added at the end for correct identification.
     - using: **loadcsv filecsv tab01 1**
     - Set the table information based on the csv table header information, for example
       - tab01 ( "ID" text, "Name" text, "Tele" text )
   - loadcsv also support **tsv format** file (\t split type), just using: loadcsv test.tsv tb1 1
   - loadcsv also support **bioinformatics .maf/.vcf/.sam/.gtf/.gff/.gpd file**, just using: loadcsv test.maf tb1   or  loadcsv test.vcf tb1
-- 2.2 Exporting csv
-  - Use **>csv csv file name 0/1** (The parameter 0/1 indicates whether to export the table header information. 0-no export, 1-export)
+  - loadcsv support gzip / zip file, Judging by file extension; etc: test.tsv.gz / test.gtf.gz / test.csv.zip
+- 2.2 Exporting csv/tsv
+  - Use **>csv csv/tsv file name 0/1** (The parameter 0/1 indicates whether to export the table header information. 0-no export, 1-export)
+  - if file name has xxx.tsv will export tsv format, otherwise csv format.
+  - if file name has xxx.tsv.gz or xxx.csv.gz , will be exported in the corresponding format and gzip compressed.
   - Example: select * from table1 where n=300 >csv user1.csv 1 , export the contents of a table to user1.csv file by select and export the table header information (the first line of the exported csv file is the database table header information)
   - Example: select ID, name, sum(val) as val from tab1 group by ID limit 100 >csv test1.csv 0
 - 2.3 Load Simply json data, Example: JSON file t1.json like this:
 ```json
 [{"Corp": "Apple", "ID": 123}, {"Corp": "Microsoft", "ID": 456}, {"Corp": "IBM", "ID": 789}]
 ```
   - using: **loadjson t1.json corp**
@@ -166,14 +170,15 @@
         - locus text, locusinfo text, reference text, accession text, version text, dblink text, keywords text, source text, organism text, comment text			
       - (03) tb01_ref (table name add _ref, corresponding to all the contents of each LOCUS' REFERENCE description)
         - locus text, reference text, title text, authors text, journal text, pubmed text, remark text
     - A GenBank file may contain more than one Features block, which can be distinguished by locus;
     - start, end content only for (123..345) Simple location, for join/complement such complex location, fill in 0, 0, real content in the location field.
     - The note field is a compound field that aggregates all other contents of Features here, using item1=value1;item2=value2 ... Schema expression.
     - The translation content of Features, the file's sequence information ORIGIN are ignored.
+    - Support xxx.gb.gz or xxx.gbff.gz, if file name last .gz , will open it's as gzip format.
 - 2.6 Crawl website data, parse and write to database
   - using: **loop loadweb url=https://xxx.xxx.com/xxx re=<a href="/search:(.+?)">(\d+)</a>**, base on python regular module, Qsqlite loop nesting function, can achieve complex web data crawling and content extraction, and then write to the database.
   - loadweb parameter:
     - Required: url=web url address, include https:// or http://. Qsqlite will crawl the web page, and then extract the content using the pythone regular module.
     - Required: re=the regular expression. This expression using by Python re.findall against the fetched page, get data.
     - Optional: ext=additional parameter to pass the parameters from the previous loop to the next, e.g. ext=_^1_, _^3_
   - Example: (For more detailed and complete examples, please refer to the demo directory qCrawlWeb.txt script.)
@@ -536,14 +541,15 @@
 - 2022/03/08   V0.89 BugFix and add ls cmd and optimize loadcsv/>csv function.
 - 2022/03/13   V0.9  BugFix and add some demo.
 - 2022/03/14   V0.91 Add navg, rdelta sqlite ext-function and rewrite help.
 - 2022/03/27   V0.93 Add draw bar function, SQLite median, Qselect function.
 - 2022/04/02   V0.95 Add tsv/maf/vcf file support on loadcsv, load Chinese font for draw.
 - 2022/04/08   V0.96 Add .sam/.gtf/.gff/.gpd file support on loadcsv, add loadgb / exec function.
 - 2022/04/20   V0.97 Add ext-sql function: summary, and loop loadweb, download function.
+- 2024/04/25   V0.973 fix summary std function bug, add >csv support tsv format. add .gz/.zip support.
 
 ## sqlite references
 - SQlite3 Doc
   - https://docs.python.org/zh-cn/3/library/sqlite3.html
 - SQlite3 System Function Ref
   - https://www.sqlite.org/lang_corefunc.html
 - SQlit Ext
```

### Comparing `Qsqlite-0.972/setup.py` & `Qsqlite-0.973/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('Readme.md', 'r') as f:
     long_description = f.read()
 
 setuptools.setup(
     name = 'Qsqlite',
-    version = '0.972',
+    version = '0.973',
     author = 'Charles Lai',
     author_email = '',
     description = 'Quick Sqlite Tools',
     long_description = long_description,
     long_description_content_type = 'text/markdown',
     url = 'https://github.com/wolf71/Qsqlite',
     packages = ['Qsqlite'],   #setuptools.find_packages(),
```

