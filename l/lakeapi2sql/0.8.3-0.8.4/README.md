# Comparing `tmp/lakeapi2sql-0.8.3.tar.gz` & `tmp/lakeapi2sql-0.8.4.tar.gz`

## Comparing `lakeapi2sql-0.8.3.tar` & `lakeapi2sql-0.8.4.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0     1420 1970-01-01 00:00:00.000000 lakeapi2sql-0.8.3/Cargo.toml
--rw-r--r--   0     1001      127      118 2024-04-29 09:22:42.000000 lakeapi2sql-0.8.3/.editorconfig
--rw-r--r--   0     1001      127     2966 2024-04-29 09:22:42.000000 lakeapi2sql-0.8.3/.github/workflows/CI.yml
--rw-r--r--   0     1001      127     3110 2024-04-29 09:22:42.000000 lakeapi2sql-0.8.3/.gitignore
--rw-r--r--   0     1001      127       76 2024-04-29 09:22:42.000000 lakeapi2sql-0.8.3/.vscode/settings.json
--rw-r--r--   0     1001      127     1081 2024-04-29 09:22:42.000000 lakeapi2sql-0.8.3/LICENSE
--rw-r--r--   0     1001      127     1388 2024-04-29 09:22:42.000000 lakeapi2sql-0.8.3/README.md
--rw-r--r--   0     1001      127        0 2024-04-29 09:22:42.000000 lakeapi2sql-0.8.3/lakeapi2sql/__init__.py
--rw-r--r--   0     1001      127     3102 2024-04-29 09:22:42.000000 lakeapi2sql-0.8.3/lakeapi2sql/bulk_insert.py
--rw-r--r--   0     1001      127        0 2024-04-29 09:22:42.000000 lakeapi2sql-0.8.3/py.typed
--rw-r--r--   0     1001      127    22898 2024-04-29 09:22:42.000000 lakeapi2sql-0.8.3/src/arrow_convert.rs
--rw-r--r--   0     1001      127     6809 2024-04-29 09:22:42.000000 lakeapi2sql-0.8.3/src/bulk_insert.rs
--rw-r--r--   0     1001      127     1519 2024-04-29 09:22:42.000000 lakeapi2sql-0.8.3/src/connect.rs
--rw-r--r--   0     1001      127     5190 2024-04-29 09:22:42.000000 lakeapi2sql-0.8.3/src/lib.rs
--rw-r--r--   0     1001      127        0 2024-04-29 09:22:42.000000 lakeapi2sql-0.8.3/test/__init__.py
--rw-r--r--   0     1001      127     1649 2024-04-29 09:22:42.000000 lakeapi2sql-0.8.3/test/test_insert.py
--rw-r--r--   0     1001      127     1663 2024-04-29 09:22:42.000000 lakeapi2sql-0.8.3/test/test_insert_reader.py
--rw-r--r--   0     1001      127    69775 2024-04-29 09:22:52.000000 lakeapi2sql-0.8.3/Cargo.lock
--rw-r--r--   0     1001      127      693 2024-04-29 09:22:42.000000 lakeapi2sql-0.8.3/pyproject.toml
--rw-r--r--   0        0        0     1852 1970-01-01 00:00:00.000000 lakeapi2sql-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0     1461 1970-01-01 00:00:00.000000 lakeapi2sql-0.8.4/Cargo.toml
+-rw-r--r--   0     1001      127      118 2024-05-01 09:04:08.000000 lakeapi2sql-0.8.4/.editorconfig
+-rw-r--r--   0     1001      127     2966 2024-05-01 09:04:08.000000 lakeapi2sql-0.8.4/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127     3110 2024-05-01 09:04:08.000000 lakeapi2sql-0.8.4/.gitignore
+-rw-r--r--   0     1001      127       76 2024-05-01 09:04:08.000000 lakeapi2sql-0.8.4/.vscode/settings.json
+-rw-r--r--   0     1001      127     1081 2024-05-01 09:04:08.000000 lakeapi2sql-0.8.4/LICENSE
+-rw-r--r--   0     1001      127     1388 2024-05-01 09:04:08.000000 lakeapi2sql-0.8.4/README.md
+-rw-r--r--   0     1001      127        0 2024-05-01 09:04:08.000000 lakeapi2sql-0.8.4/lakeapi2sql/__init__.py
+-rw-r--r--   0     1001      127     3102 2024-05-01 09:04:08.000000 lakeapi2sql-0.8.4/lakeapi2sql/bulk_insert.py
+-rw-r--r--   0     1001      127        0 2024-05-01 09:04:08.000000 lakeapi2sql-0.8.4/py.typed
+-rw-r--r--   0     1001      127    22276 2024-05-01 09:04:08.000000 lakeapi2sql-0.8.4/src/arrow_convert.rs
+-rw-r--r--   0     1001      127     5134 2024-05-01 09:04:08.000000 lakeapi2sql-0.8.4/src/bulk_insert.rs
+-rw-r--r--   0     1001      127     2123 2024-05-01 09:04:08.000000 lakeapi2sql-0.8.4/src/connect.rs
+-rw-r--r--   0     1001      127     1705 2024-05-01 09:04:08.000000 lakeapi2sql-0.8.4/src/error.rs
+-rw-r--r--   0     1001      127     4862 2024-05-01 09:04:08.000000 lakeapi2sql-0.8.4/src/lib.rs
+-rw-r--r--   0     1001      127        0 2024-05-01 09:04:08.000000 lakeapi2sql-0.8.4/test/__init__.py
+-rw-r--r--   0     1001      127     1649 2024-05-01 09:04:08.000000 lakeapi2sql-0.8.4/test/test_insert.py
+-rw-r--r--   0     1001      127     1667 2024-05-01 09:04:08.000000 lakeapi2sql-0.8.4/test/test_insert_reader.py
+-rw-r--r--   0     1001      127    70255 2024-05-01 09:04:13.000000 lakeapi2sql-0.8.4/Cargo.lock
+-rw-r--r--   0     1001      127      693 2024-05-01 09:04:08.000000 lakeapi2sql-0.8.4/pyproject.toml
+-rw-r--r--   0        0        0     1852 1970-01-01 00:00:00.000000 lakeapi2sql-0.8.4/PKG-INFO
```

### Comparing `lakeapi2sql-0.8.3/Cargo.toml` & `lakeapi2sql-0.8.4/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -5,41 +5,42 @@
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "lake2sql"
 crate-type = ["lib", "cdylib"]
 
 [dependencies]
-arrow = { version = "48.0.0", features = ["ipc_compression", "pyarrow"] }
+arrow = { version = "51.0.0", features = ["ipc_compression", "pyarrow"] }
 futures = "0.3.28"
 log = "0.4.19"
 pyo3-asyncio = { version = "0.20", features = ["attributes", "tokio-runtime"] }
 pyo3-log = "0.9.0"
 rust_decimal = "1.32.0"
+thiserror = "1.0.59"
 
 time = "0.3.22"
 tokio = { version = "1.28.2", features = ["net", "macros"] }
 tokio-util = { version = "0.7.8", features = ["compat", "io-util", "io"] }
 
 [target.'cfg(target_os="linux")'.dependencies]
 reqwest = { version = "0.11.18", features = [
     "stream",
     "rustls-tls-native-roots",
 ], default-features = false }
-tiberius = { git = "https://github.com/aersam/tiberius.git", branch = "bulk", features = [
+tiberius = { git = "https://github.com/aersam/tiberius.git", branch = "expose_ado_net", features = [
     "time",
     "sql-browser-tokio",
     "rust_decimal",
     "tds73",
     "rustls",
 ], default-features = false }
 
 [target.'cfg(not(target_os="linux"))'.dependencies]
 reqwest = { version = "0.11.18", features = ["stream"] }
-tiberius = { git = "https://github.com/aersam/tiberius.git", branch = "bulk", features = [
+tiberius = { git = "https://github.com/aersam/tiberius.git", branch = "expose_ado_net", features = [
     "time",
     "sql-browser-tokio",
     "rust_decimal",
 ] }
 
 [dependencies.pyo3]
 version = "0.20.0"
```

### Comparing `lakeapi2sql-0.8.3/.github/workflows/CI.yml` & `lakeapi2sql-0.8.4/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.8.3/.gitignore` & `lakeapi2sql-0.8.4/.gitignore`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.8.3/LICENSE` & `lakeapi2sql-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.8.3/README.md` & `lakeapi2sql-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.8.3/lakeapi2sql/bulk_insert.py` & `lakeapi2sql-0.8.4/lakeapi2sql/bulk_insert.py`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.8.3/src/arrow_convert.rs` & `lakeapi2sql-0.8.4/src/arrow_convert.rs`

 * *Files 6% similar despite different names*

```diff
@@ -34,58 +34,36 @@
 use tiberius::time::time::PrimitiveDateTime;
 use tiberius::time::time::Time;
 use tiberius::ColumnData;
 use tiberius::ColumnType;
 use tiberius::ToSql;
 use tiberius::TokenRow;
 
-#[derive(Debug)]
-pub(crate) struct NotSupportedError {
-    dtype: DataType,
-    column_type: ColumnType,
-}
-impl Display for NotSupportedError {
-    fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
-        f.write_fmt(format_args!(
-            "Cannot use data type {}. Sql Type: {:?}",
-            self.dtype, self.column_type
-        ))
-    }
-}
-impl std::error::Error for NotSupportedError {
-    fn source(&self) -> Option<&(dyn std::error::Error + 'static)> {
-        None
-    }
-
-    fn description(&self) -> &str {
-        "description() is deprecated; use Display"
-    }
-
-    fn cause(&self) -> Option<&dyn std::error::Error> {
-        self.source()
-    }
-}
+use crate::error::LakeApi2SqlError;
 
 fn to_col_dt<'a>(d: ColumnData<'_>) -> ColumnData<'a> {
     match d {
         ColumnData::DateTime2(dt) => ColumnData::DateTime2(dt),
         ColumnData::DateTime(dt) => ColumnData::DateTime(dt),
         ColumnData::Time(dt) => ColumnData::Time(dt),
         _ => panic!("Not a time field"),
     }
 }
 
 pub(crate) fn get_token_rows<'a, 'b>(
     batch: &'a RecordBatch,
     colsnames: &'b Vec<(String, ColumnType)>,
-) -> Result<Vec<TokenRow<'a>>, Box<dyn std::error::Error + Send + Sync>> {
-    let unix_min_date = Date::from_calendar_date(1970, tiberius::time::time::Month::January, 1)?;
-    let sql_min_date = Date::from_calendar_date(1, tiberius::time::time::Month::January, 1)?;
-    let sql_min_datetime = Date::from_calendar_date(1900, tiberius::time::time::Month::January, 1)?;
-    let unix_min: PrimitiveDateTime = unix_min_date.with_time(Time::from_hms(0, 0, 0)?);
+) -> Result<Vec<TokenRow<'a>>, LakeApi2SqlError> {
+    let unix_min_date =
+        Date::from_calendar_date(1970, tiberius::time::time::Month::January, 1).unwrap();
+    let sql_min_date =
+        Date::from_calendar_date(1, tiberius::time::time::Month::January, 1).unwrap();
+    let sql_min_datetime =
+        Date::from_calendar_date(1900, tiberius::time::time::Month::January, 1).unwrap();
+    let unix_min: PrimitiveDateTime = unix_min_date.with_time(Time::from_hms(0, 0, 0).unwrap());
     let sql_min_to_unix_min = (unix_min_date - sql_min_date).whole_days();
     let sql_min_dt_to_unix_min = (unix_min_date - sql_min_datetime).whole_days();
     let rows = batch.num_rows();
     //let mut token_rows: Vec<TokenRow> = vec![TokenRow::new(); rows.try_into()?];
     let mut token_rows: Vec<TokenRow<'a>> = Vec::with_capacity(rows);
     for _ in 0..rows {
         token_rows.push(TokenRow::with_capacity(colsnames.len()));
@@ -499,15 +477,15 @@
                 for val in ba.iter() {
                     token_rows[rowindex].push(ColumnData::Binary(val.map(|x| Cow::from(x))));
                     rowindex += 1;
                 }
             }
             arrow::datatypes::DataType::Decimal128(_, s) => {
                 let ba = col.as_any().downcast_ref::<Decimal128Array>().unwrap();
-                let scale: u8 = s.clone().try_into()?;
+                let scale: u8 = s.clone().try_into().unwrap();
                 let mut rowindex = 0;
                 match coltype {
                     ColumnType::Numericn | ColumnType::Decimaln => {
                         for val in ba.iter() {
                             token_rows[rowindex].push(ColumnData::Numeric(
                                 val.map(|x| Numeric::new_with_scale(x, scale)),
                             ));
@@ -521,24 +499,24 @@
                                     .to_f64()
                                     .unwrap()
                             })));
                             rowindex += 1;
                         }
                     }
                     _ => {
-                        return Err(Box::new(NotSupportedError {
+                        return Err(LakeApi2SqlError::NotSupported {
                             dtype: col.data_type().clone(),
                             column_type: coltype.clone(),
-                        }))
+                        })
                     } //other => panic!("Not supported {:?}", other),
                 }
             }
             dt => {
-                return Err(Box::new(NotSupportedError {
+                return Err(LakeApi2SqlError::NotSupported {
                     dtype: dt.clone(),
                     column_type: coltype.clone(),
-                }))
+                })
             } //other => panic!("Not supported {:?}", other),
         }
     }
     Ok(token_rows)
 }
```

### Comparing `lakeapi2sql-0.8.3/src/bulk_insert.rs` & `lakeapi2sql-0.8.4/src/bulk_insert.rs`

 * *Files 21% similar despite different names*

```diff
@@ -1,80 +1,33 @@
 use std::{fmt::Display, sync::Arc};
 
 use arrow::ffi_stream::ArrowArrayStreamReader;
 use arrow::record_batch::RecordBatchReader;
-use arrow::{
-    datatypes::Schema, error::ArrowError, ipc::reader::StreamReader, record_batch::RecordBatch,
-};
+use arrow::{datatypes::Schema, ipc::reader::StreamReader, record_batch::RecordBatch};
 use futures::stream::TryStreamExt;
 use log::info;
 use tiberius::Client;
 use tiberius::ColumnType;
 use tiberius::SqlBulkCopyOptions;
 use tokio::net::TcpStream;
 use tokio_util::compat::Compat;
 use tokio_util::compat::FuturesAsyncReadCompatExt;
 use tokio_util::io::SyncIoBridge;
 
 use tokio::sync::mpsc;
 use tokio::task;
 
 use crate::arrow_convert::get_token_rows;
-
-#[derive(Debug)]
-pub(crate) struct ArrowErrorWrap {
-    error: ArrowError,
-}
-impl Display for ArrowErrorWrap {
-    fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
-        f.write_fmt(format_args!("arrow error {}", self.error))
-    }
-}
-impl std::error::Error for ArrowErrorWrap {
-    fn source(&self) -> Option<&(dyn std::error::Error + 'static)> {
-        None
-    }
-
-    fn description(&self) -> &str {
-        "description() is deprecated; use Display"
-    }
-
-    fn cause(&self) -> Option<&dyn std::error::Error> {
-        self.source()
-    }
-}
-
-#[derive(Debug)]
-pub(crate) struct SendErrorWrap {
-    error: String,
-}
-impl Display for SendErrorWrap {
-    fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
-        f.write_fmt(format_args!("send error {}", self.error))
-    }
-}
-impl std::error::Error for SendErrorWrap {
-    fn source(&self) -> Option<&(dyn std::error::Error + 'static)> {
-        None
-    }
-
-    fn description(&self) -> &str {
-        "description() is deprecated; use Display"
-    }
-
-    fn cause(&self) -> Option<&dyn std::error::Error> {
-        self.source()
-    }
-}
+use crate::error::LakeApi2SqlError;
 
 async fn get_cols_from_table(
     db_client: &mut Client<Compat<TcpStream>>,
     table_name: &str,
     column_names: &[&str],
-) -> Result<Vec<(String, ColumnType)>, Box<dyn std::error::Error + Send + Sync>> {
+) -> Result<Vec<(String, ColumnType)>, LakeApi2SqlError> {
     let cols_sql = match column_names.len() {
         0 => "*".to_owned(),
         _ => column_names
             .iter()
             .map(|c| format!("[{}]", c))
             .collect::<Vec<String>>()
             .join(", "),
@@ -91,15 +44,15 @@
 }
 
 pub async fn bulk_insert_batch<'a>(
     table_name: &str,
     blk: &mut tiberius::BulkLoadRequest<'a, Compat<TcpStream>>,
     batch: &'a RecordBatch,
     collist: &'a Vec<(String, ColumnType)>,
-) -> Result<(), Box<dyn std::error::Error + Send + Sync>> {
+) -> Result<(), LakeApi2SqlError> {
     let nrows = batch.num_rows();
     info!("{table_name}: received {nrows}");
     let rows = task::block_in_place(|| get_token_rows(batch, &collist))?;
     info!("{table_name}: converted {nrows}");
     for rowdt in rows {
         blk.send(rowdt).await?;
     }
@@ -110,15 +63,15 @@
 pub async fn bulk_insert<'a>(
     db_client: &'a mut Client<Compat<TcpStream>>,
     table_name: &str,
     column_names: &'a [&'a str],
     url: &str,
     user: &str,
     password: &str,
-) -> Result<Arc<Schema>, Box<dyn std::error::Error + Send + Sync>> {
+) -> Result<Arc<Schema>, LakeApi2SqlError> {
     //let mut row = TokenRow::new();
     //row.push(1.into_sql());
     //blk.send(row).await?;
     //blk.finalize().await?;
 
     let collist = get_cols_from_table(db_client, table_name, column_names).await?;
     log::debug!("{:?}", collist);
@@ -137,40 +90,30 @@
     let res = res
         .bytes_stream()
         .map_err(|e| futures::io::Error::new(futures::io::ErrorKind::Other, e))
         .into_async_read()
         .compat();
     let (tx, mut rx) = mpsc::channel::<RecordBatch>(2);
     let syncstr = SyncIoBridge::new(res);
-    let worker = tokio::task::spawn_blocking(
-        move || -> Result<Arc<Schema>, Box<dyn std::error::Error + Send + Sync>> {
-            let reader = StreamReader::try_new(syncstr, None);
-            if let Err(err) = reader {
-                return Err(Box::new(ArrowErrorWrap { error: err }));
-            }
-            let mut reader = reader.unwrap();
-            let schema = reader.schema();
-            loop {
-                match reader.next() {
-                    Some(x) => match x {
-                        Ok(b) => {
-                            tx.blocking_send(b).map_err(|e| {
-                                Box::new(SendErrorWrap {
-                                    error: e.to_string(),
-                                })
-                            })?;
-                        }
-                        Err(l) => println!("{:?}", l),
-                    },
-                    None => break,
-                };
-            }
-            Ok(schema)
-        },
-    );
+    let worker = tokio::task::spawn_blocking(move || -> Result<Arc<Schema>, LakeApi2SqlError> {
+        let mut reader = StreamReader::try_new(syncstr, None)?;
+        let schema = reader.schema();
+        loop {
+            match reader.next() {
+                Some(x) => match x {
+                    Ok(b) => {
+                        tx.blocking_send(b)?;
+                    }
+                    Err(l) => println!("{:?}", l),
+                },
+                None => break,
+            };
+        }
+        Ok(schema)
+    });
     while let Some(v) = rx.recv().await {
         let mut blk = db_client
             .bulk_insert_with_options(
                 table_name,
                 &column_names,
                 SqlBulkCopyOptions::TableLock,
                 &[],
@@ -184,15 +127,15 @@
 }
 
 pub async fn bulk_insert_reader(
     db_client: &mut Client<Compat<TcpStream>>,
     table_name: &str,
     column_names: &[&str],
     reader: &mut ArrowArrayStreamReader,
-) -> Result<Arc<Schema>, Box<dyn std::error::Error + Send + Sync>> {
+) -> Result<Arc<Schema>, LakeApi2SqlError> {
     //let mut row = TokenRow::new();
     //row.push(1.into_sql());
     //blk.send(row).await?;
     //blk.finalize().await?;
 
     let collist = get_cols_from_table(db_client, table_name, column_names).await?;
     log::debug!("{:?}", collist);
```

### Comparing `lakeapi2sql-0.8.3/src/connect.rs` & `lakeapi2sql-0.8.4/src/connect.rs`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,24 @@
+use tiberius::client::AdoNetConfig;
+use tiberius::client::ConfigString;
 use tiberius::error::Error;
 use tiberius::AuthMethod;
 use tiberius::Client;
 use tiberius::Config;
 use tiberius::SqlBrowser;
 use tokio::net::TcpStream;
 use tokio_util::compat::Compat;
 use tokio_util::compat::TokioAsyncWriteCompatExt;
 
+use crate::error::LakeApi2SqlError;
+
 pub async fn connect_sql(
     con_str: &str,
     aad_token: Option<String>,
-) -> Result<Client<Compat<TcpStream>>, Box<dyn std::error::Error + Send + Sync>> {
+) -> Result<Client<Compat<TcpStream>>, LakeApi2SqlError> {
     let mut config = Config::from_ado_string(con_str)?;
     if let Some(tv) = aad_token.clone() {
         config.authentication(AuthMethod::AADToken(tv));
     }
 
     config.encryption(tiberius::EncryptionLevel::Required);
 
@@ -22,24 +26,36 @@
     tcp.set_nodelay(true)?;
 
     let client = match Client::connect(config, tcp.compat_write()).await {
         // Connection successful.
         Ok(client) => client,
         // The server wants us to redirect to a different address
         Err(Error::Routing { host, port }) => {
-            let mut config = Config::from_ado_string(con_str)?;
+            let ado_cfg: AdoNetConfig = con_str.parse()?;
+            let ado_cfg2: AdoNetConfig = con_str.parse()?;
+
+            let mut config = Config::from_config_string(ado_cfg)?;
             if let Some(tv) = aad_token {
                 config.authentication(AuthMethod::AADToken(tv));
             }
             config.host(&host);
             config.port(port);
+            let instance = match ado_cfg2.server() {
+                Ok(v) => v.instance,
+                Err(_) => None,
+            };
+            if instance.is_some() {
+                let tcp = TcpStream::connect_named(&config).await?;
+                tcp.set_nodelay(true)?;
+                Client::connect(config, tcp.compat_write()).await?
+            } else {
+                let tcp = TcpStream::connect(config.get_addr()).await?;
+                tcp.set_nodelay(true)?;
 
-            let tcp = TcpStream::connect(config.get_addr()).await?;
-            tcp.set_nodelay(true)?;
-
-            // we should not have more than one redirect, so we'll short-circuit here.
-            Client::connect(config, tcp.compat_write()).await?
+                // we should not have more than one redirect, so we'll short-circuit here.
+                Client::connect(config, tcp.compat_write()).await?
+            }
         }
         Err(e) => Err(e)?,
     };
     Ok(client)
 }
```

### Comparing `lakeapi2sql-0.8.3/src/lib.rs` & `lakeapi2sql-0.8.4/src/lib.rs`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 use arrow::pyarrow::FromPyArrow;
 use pyo3::exceptions::{PyConnectionError, PyIOError};
 use pyo3::prelude::*;
 use pyo3::types::{PyDict, PyString};
 mod arrow_convert;
 pub mod bulk_insert;
 pub mod connect;
+pub mod error;
 use tokio::net::TcpStream;
 
 fn field_into_dict<'a>(py: Python<'a>, field: &'a Field) -> &'a PyDict {
     let d = PyDict::new(py);
     d.set_item("name", field.name().clone()).unwrap();
     d.set_item("arrow_type", field.data_type().to_string())
         .unwrap();
@@ -137,38 +138,28 @@
     column_names: Vec<String>,
     aad_token: Option<String>,
 ) -> PyResult<&'a PyAny> {
     let mut reader: ArrowArrayStreamReader =
         ArrowArrayStreamReader::from_pyarrow(record_batch_reader)?;
 
     pyo3_asyncio::tokio::future_into_py(py, async move {
-        let db_client = connect::connect_sql(&connection_string, aad_token).await;
-        if let Err(er) = db_client {
-            return Err(PyErr::new::<PyConnectionError, _>(format!(
-                "Error connecting: {er}"
-            )));
-        }
+        let mut db_client = connect::connect_sql(&connection_string, aad_token).await?;
         let bres = bulk_insert::bulk_insert_reader(
-            &mut db_client.unwrap(),
+            &mut db_client,
             &table_name,
             &column_names
                 .iter()
                 .map(|x| x.as_str())
                 .collect::<Vec<&str>>(),
             &mut reader,
         )
-        .await;
+        .await?;
 
-        if let Err(er) = bres {
-            return Err(PyErr::new::<PyIOError, _>(format!(
-                "Error connecting: {er}"
-            )));
-        }
         Ok(Python::with_gil(|py| {
-            let d: Py<PyDict> = into_dict(py, bres.unwrap()).into();
+            let d: Py<PyDict> = into_dict(py, bres).into();
             d
         }))
     })
 }
 
 /// A Python module implemented in Rust.
 #[pymodule]
```

### Comparing `lakeapi2sql-0.8.3/test/test_insert.py` & `lakeapi2sql-0.8.4/test/test_insert.py`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.8.3/test/test_insert_reader.py` & `lakeapi2sql-0.8.4/test/test_insert_reader.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pyarrow as pa
 import pyodbc
 import pytest
 import lakeapi2sql.bulk_insert
 import os
 from dotenv import load_dotenv
 
-data = [pa.array([1, 2, 3, 4]), pa.array(["foo", "bar", "baz", None]), pa.array([True, None, False, True])]
+data = [pa.array([1, 2, 3, 4]), pa.array(["foo", "bar", "$ä,àE", None]), pa.array([True, None, False, True])]
 
 
 batch = pa.record_batch(data, names=["f0", "f1", "f2"])
 
 batchreader = pa.RecordBatchReader.from_batches(batch.schema, [batch])
 load_dotenv()
 ## in order to use sql express, be sure to enable tcp for sql express and to start sql browser service
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `lakeapi2sql-0.8.3/Cargo.lock` & `lakeapi2sql-0.8.4/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -76,19 +76,18 @@
 name = "arrayvec"
 version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "96d30a06541fbafbc7f82ed10c06164cfbd2c401138f6addd8404629c4b16711"
 
 [[package]]
 name = "arrow"
-version = "48.0.1"
+version = "51.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a8919668503a4f2d8b6da96fa7c16e93046bfb3412ffcfa1e5dc7d2e3adcb378"
+checksum = "219d05930b81663fd3b32e3bde8ce5bff3c4d23052a99f11a8fa50a3b47b2658"
 dependencies = [
- "ahash 0.8.11",
  "arrow-arith",
  "arrow-array",
  "arrow-buffer",
  "arrow-cast",
  "arrow-csv",
  "arrow-data",
  "arrow-ipc",
@@ -99,76 +98,79 @@
  "arrow-select",
  "arrow-string",
  "pyo3",
 ]
 
 [[package]]
 name = "arrow-arith"
-version = "48.0.1"
+version = "51.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ef983914f477d4278b068f13b3224b7d19eb2b807ac9048544d3bfebdf2554c4"
+checksum = "0272150200c07a86a390be651abdd320a2d12e84535f0837566ca87ecd8f95e0"
 dependencies = [
  "arrow-array",
  "arrow-buffer",
  "arrow-data",
  "arrow-schema",
  "chrono",
  "half",
  "num",
 ]
 
 [[package]]
 name = "arrow-array"
-version = "48.0.1"
+version = "51.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d6eaf89041fa5937940ae390294ece29e1db584f46d995608d6e5fe65a2e0e9b"
+checksum = "8010572cf8c745e242d1b632bd97bd6d4f40fefed5ed1290a8f433abaa686fea"
 dependencies = [
  "ahash 0.8.11",
  "arrow-buffer",
  "arrow-data",
  "arrow-schema",
  "chrono",
  "half",
  "hashbrown 0.14.5",
  "num",
 ]
 
 [[package]]
 name = "arrow-buffer"
-version = "48.0.1"
+version = "51.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "55512d988c6fbd76e514fd3ff537ac50b0a675da5a245e4fdad77ecfd654205f"
+checksum = "0d0a2432f0cba5692bf4cb757469c66791394bac9ec7ce63c1afe74744c37b27"
 dependencies = [
  "bytes",
  "half",
  "num",
 ]
 
 [[package]]
 name = "arrow-cast"
-version = "48.0.1"
+version = "51.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "655ee51a2156ba5375931ce21c1b2494b1d9260e6dcdc6d4db9060c37dc3325b"
+checksum = "9abc10cd7995e83505cc290df9384d6e5412b207b79ce6bdff89a10505ed2cba"
 dependencies = [
  "arrow-array",
  "arrow-buffer",
  "arrow-data",
  "arrow-schema",
  "arrow-select",
+ "atoi",
+ "base64 0.22.1",
  "chrono",
  "half",
  "lexical-core",
  "num",
+ "ryu",
 ]
 
 [[package]]
 name = "arrow-csv"
-version = "48.0.1"
+version = "51.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "258bb689997ad5b6660b3ce3638bd6b383d668ec555ed41ad7c6559cbb2e4f91"
+checksum = "95cbcba196b862270bf2a5edb75927380a7f3a163622c61d40cbba416a6305f2"
 dependencies = [
  "arrow-array",
  "arrow-buffer",
  "arrow-cast",
  "arrow-data",
  "arrow-schema",
  "chrono",
@@ -177,45 +179,45 @@
  "lazy_static",
  "lexical-core",
  "regex",
 ]
 
 [[package]]
 name = "arrow-data"
-version = "48.0.1"
+version = "51.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6dc2b9fec74763427e2e5575b8cc31ce96ba4c9b4eb05ce40e0616d9fad12461"
+checksum = "2742ac1f6650696ab08c88f6dd3f0eb68ce10f8c253958a18c943a68cd04aec5"
 dependencies = [
  "arrow-buffer",
  "arrow-schema",
  "half",
  "num",
 ]
 
 [[package]]
 name = "arrow-ipc"
-version = "48.0.1"
+version = "51.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6eaa6ab203cc6d89b7eaa1ac781c1dfeef325454c5d5a0419017f95e6bafc03c"
+checksum = "a42ea853130f7e78b9b9d178cb4cd01dee0f78e64d96c2949dc0a915d6d9e19d"
 dependencies = [
  "arrow-array",
  "arrow-buffer",
  "arrow-cast",
  "arrow-data",
  "arrow-schema",
  "flatbuffers",
  "lz4_flex",
  "zstd",
 ]
 
 [[package]]
 name = "arrow-json"
-version = "48.0.1"
+version = "51.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fb64e30d9b73f66fdc5c52d5f4cf69bbf03d62f64ffeafa0715590a5320baed7"
+checksum = "eaafb5714d4e59feae964714d724f880511500e3569cc2a94d02456b403a2a49"
 dependencies = [
  "arrow-array",
  "arrow-buffer",
  "arrow-cast",
  "arrow-data",
  "arrow-schema",
  "chrono",
@@ -225,76 +227,77 @@
  "num",
  "serde",
  "serde_json",
 ]
 
 [[package]]
 name = "arrow-ord"
-version = "48.0.1"
+version = "51.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f9a818951c0d11c428dda03e908175969c262629dd20bd0850bd6c7a8c3bfe48"
+checksum = "e3e6b61e3dc468f503181dccc2fc705bdcc5f2f146755fa5b56d0a6c5943f412"
 dependencies = [
  "arrow-array",
  "arrow-buffer",
  "arrow-data",
  "arrow-schema",
  "arrow-select",
  "half",
  "num",
 ]
 
 [[package]]
 name = "arrow-row"
-version = "48.0.1"
+version = "51.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a5d664318bc05f930559fc088888f0f7174d3c5bc888c0f4f9ae8f23aa398ba3"
+checksum = "848ee52bb92eb459b811fb471175ea3afcf620157674c8794f539838920f9228"
 dependencies = [
  "ahash 0.8.11",
  "arrow-array",
  "arrow-buffer",
  "arrow-data",
  "arrow-schema",
  "half",
  "hashbrown 0.14.5",
 ]
 
 [[package]]
 name = "arrow-schema"
-version = "48.0.1"
+version = "51.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "aaf4d737bba93da59f16129bec21e087aed0be84ff840e74146d4703879436cb"
+checksum = "02d9483aaabe910c4781153ae1b6ae0393f72d9ef757d38d09d450070cf2e528"
 dependencies = [
  "bitflags 2.5.0",
 ]
 
 [[package]]
 name = "arrow-select"
-version = "48.0.1"
+version = "51.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "374c4c3b812ecc2118727b892252a4a4308f87a8aca1dbf09f3ce4bc578e668a"
+checksum = "849524fa70e0e3c5ab58394c770cb8f514d0122d20de08475f7b472ed8075830"
 dependencies = [
  "ahash 0.8.11",
  "arrow-array",
  "arrow-buffer",
  "arrow-data",
  "arrow-schema",
  "num",
 ]
 
 [[package]]
 name = "arrow-string"
-version = "48.0.1"
+version = "51.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b15aed5624bb23da09142f58502b59c23f5bea607393298bb81dab1ce60fc769"
+checksum = "9373cb5a021aee58863498c37eb484998ef13377f69989c6c5ccfbd258236cdb"
 dependencies = [
  "arrow-array",
  "arrow-buffer",
  "arrow-data",
  "arrow-schema",
  "arrow-select",
+ "memchr",
  "num",
  "regex",
  "regex-syntax",
 ]
 
 [[package]]
 name = "async-native-tls"
@@ -329,14 +332,23 @@
  "futures-sink",
  "futures-util",
  "memchr",
  "pin-project-lite",
 ]
 
 [[package]]
+name = "atoi"
+version = "2.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f28d99ec8bfea296261ca1af174f24225171fea9664ba9003cbebee704810528"
+dependencies = [
+ "num-traits",
+]
+
+[[package]]
 name = "autocfg"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
 
 [[package]]
 name = "backtrace"
@@ -356,14 +368,20 @@
 [[package]]
 name = "base64"
 version = "0.21.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9d297deb1925b89f2ccc13d7635fa0714f12c87adce1c75356b39ca9b7178567"
 
 [[package]]
+name = "base64"
+version = "0.22.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "72b3254f16251a8381aa12e40e3c4d2f0199f8c6508fbecb9d91f575e0fbb8c6"
+
+[[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bitflags"
@@ -381,27 +399,27 @@
  "radium",
  "tap",
  "wyz",
 ]
 
 [[package]]
 name = "borsh"
-version = "1.4.0"
+version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0901fc8eb0aca4c83be0106d6f2db17d86a08dfc2c25f0e84464bf381158add6"
+checksum = "dbe5b10e214954177fb1dc9fbd20a1a2608fe99e6c832033bdc7cea287a20d77"
 dependencies = [
  "borsh-derive",
  "cfg_aliases",
 ]
 
 [[package]]
 name = "borsh-derive"
-version = "1.4.0"
+version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "51670c3aa053938b0ee3bd67c3817e471e626151131b934038e83c5bf8de48f5"
+checksum = "d7a8646f94ab393e43e8b35a2558b1624bed28b97ee09c5d15456e3c9463f46d"
 dependencies = [
  "once_cell",
  "proc-macro-crate",
  "proc-macro2",
  "quote",
  "syn 2.0.60",
  "syn_derive",
@@ -445,17 +463,17 @@
 name = "bytes"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "514de17de45fdb8dc022b1a7975556c53c86f9f0aa5f534b98977b171857c2c9"
 
 [[package]]
 name = "cc"
-version = "1.0.95"
+version = "1.0.96"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d32a725bc159af97c3e629873bb9f88fb8cf8a4867175f76dc987815ea07c83b"
+checksum = "065a29261d53ba54260972629f9ca6bffa69bac13cd1fed61420f7fa68b9f8bd"
 dependencies = [
  "jobserver",
  "libc",
  "once_cell",
 ]
 
 [[package]]
@@ -1003,14 +1021,15 @@
  "futures",
  "log",
  "pyo3",
  "pyo3-asyncio",
  "pyo3-log",
  "reqwest",
  "rust_decimal",
+ "thiserror",
  "tiberius",
  "time",
  "tokio",
  "tokio-util",
 ]
 
 [[package]]
@@ -1081,17 +1100,17 @@
 dependencies = [
  "lexical-util",
  "static_assertions",
 ]
 
 [[package]]
 name = "libc"
-version = "0.2.153"
+version = "0.2.154"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
+checksum = "ae743338b92ff9146ce83992f766a31066a91a8c84a45e0e9f21e7cf6de6d346"
 
 [[package]]
 name = "libm"
 version = "0.2.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4ec2a862134d2a7d32d7983ddcdd1c4923530833c9f2ea1a44fc5fa473989058"
 
@@ -1708,15 +1727,15 @@
 
 [[package]]
 name = "reqwest"
 version = "0.11.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dd67538700a17451e7cba03ac727fb961abb7607553461627b97de0b89cf4a62"
 dependencies = [
- "base64",
+ "base64 0.21.7",
  "bytes",
  "encoding_rs",
  "futures-core",
  "futures-util",
  "h2",
  "http",
  "http-body",
@@ -1866,15 +1885,15 @@
 
 [[package]]
 name = "rustls-pemfile"
 version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1c74cae0a4cf6ccbbf5f359f08efdf8ee7e1dc532573bf0db71968cb56b1448c"
 dependencies = [
- "base64",
+ "base64 0.21.7",
 ]
 
 [[package]]
 name = "rustls-webpki"
 version = "0.101.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b6275d1ee7a1cd780b64aca7726599a1dbc893b1e64144529e55c3c2f745765"
@@ -2011,17 +2030,17 @@
 name = "smallvec"
 version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "socket2"
-version = "0.5.6"
+version = "0.5.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "05ffd9c0a93b7543e062e759284fcf5f5e3b098501104bfbdde4d404db792871"
+checksum = "ce305eb0b4296696835b71df73eb912e0f1ffd2556a501fcede6e0c50349191c"
 dependencies = [
  "libc",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "spin"
@@ -2139,15 +2158,15 @@
  "quote",
  "syn 2.0.60",
 ]
 
 [[package]]
 name = "tiberius"
 version = "0.12.2"
-source = "git+https://github.com/aersam/tiberius.git?branch=bulk#8cee1fe5d765358ca568c96423766ae3b582b9e8"
+source = "git+https://github.com/aersam/tiberius.git?branch=expose_ado_net#be864ace05511a3682c1e1293c1356d2d1b5eff0"
 dependencies = [
  "async-native-tls",
  "async-trait",
  "asynchronous-codec",
  "bitflags 2.5.0",
  "byteorder",
  "bytes",
```

### Comparing `lakeapi2sql-0.8.3/pyproject.toml` & `lakeapi2sql-0.8.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["maturin>=1.1,<2.0"]
 build-backend = "maturin"
 
 [project]
 name = "lakeapi2sql"
 requires-python = ">=3.10"
-version = "0.8.3"
+version = "0.8.4"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 
 dependencies = ["pyarrow >= 8.0.0"]
```

### Comparing `lakeapi2sql-0.8.3/PKG-INFO` & `lakeapi2sql-0.8.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: lakeapi2sql
-Version: 0.8.3
+Version: 0.8.4
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: pyarrow >=8.0.0
 Requires-Dist: azure-identity >=1.12.0 ; extra == 'azure'
 Provides-Extra: azure
 License-File: LICENSE
```

