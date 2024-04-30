# Comparing `tmp/bany-1.4.3.tar.gz` & `tmp/bany-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bany-1.4.3.tar", max compression
+gzip compressed data, was "bany-1.4.4.tar", max compression
```

## Comparing `bany-1.4.3.tar` & `bany-1.4.4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0    10118 2023-11-15 21:03:19.115145 bany-1.4.3/README.md
--rw-r--r--   0        0        0        0 2022-10-02 15:09:36.217615 bany-1.4.3/bany/__init__.py
--rw-r--r--   0        0        0     4292 2023-11-18 23:05:09.907810 bany-1.4.3/bany/__main__.py
--rw-r--r--   0        0        0        0 2022-11-03 00:40:20.325732 bany-1.4.3/bany/cmd/__init__.py
--rw-r--r--   0        0        0        0 2023-11-15 21:03:19.115345 bany-1.4.3/bany/cmd/extract/__init__.py
--rw-r--r--   0        0        0     1853 2023-11-15 20:50:59.755388 bany-1.4.3/bany/cmd/extract/app.py
--rw-r--r--   0        0        0      115 2023-01-02 22:11:13.071746 bany-1.4.3/bany/cmd/extract/extractors/__init__.py
--rw-r--r--   0        0        0      528 2023-01-02 22:29:16.298716 bany-1.4.3/bany/cmd/extract/extractors/base.py
--rw-r--r--   0        0        0     8925 2023-11-14 20:24:28.250057 bany-1.4.3/bany/cmd/extract/extractors/pdf.py
--rw-r--r--   0        0        0     3432 2023-11-14 20:41:46.783479 bany-1.4.3/bany/cmd/extract/rules.py
--rw-r--r--   0        0        0        0 2023-11-15 20:50:59.755526 bany-1.4.3/bany/cmd/solve/__init__.py
--rw-r--r--   0        0        0     2136 2023-11-17 16:26:28.922422 bany-1.4.3/bany/cmd/solve/app.py
--rw-r--r--   0        0        0        0 2023-01-04 02:52:24.554271 bany-1.4.3/bany/cmd/solve/network/__init__.py
--rw-r--r--   0        0        0     8344 2023-01-04 02:52:24.554650 bany-1.4.3/bany/cmd/solve/network/algo.py
--rw-r--r--   0        0        0     5163 2023-11-18 23:05:09.908173 bany-1.4.3/bany/cmd/solve/network/attrs.py
--rw-r--r--   0        0        0     3266 2023-11-18 23:05:09.908470 bany-1.4.3/bany/cmd/solve/network/loader.py
--rw-r--r--   0        0        0     4017 2023-01-04 02:52:24.555422 bany-1.4.3/bany/cmd/solve/network/validate.py
--rw-r--r--   0        0        0     4225 2023-11-18 23:05:09.908758 bany-1.4.3/bany/cmd/solve/network/visualize.py
--rw-r--r--   0        0        0      479 2023-01-04 02:52:24.555930 bany-1.4.3/bany/cmd/solve/solvers/__init__.py
--rw-r--r--   0        0        0     1495 2023-01-04 02:52:24.556171 bany-1.4.3/bany/cmd/solve/solvers/basesolver.py
--rw-r--r--   0        0        0     3804 2023-01-04 02:52:24.556400 bany-1.4.3/bany/cmd/solve/solvers/bucketdata.py
--rw-r--r--   0        0        0     2863 2023-11-18 23:05:09.909067 bany-1.4.3/bany/cmd/solve/solvers/constrained.py
--rw-r--r--   0        0        0     6045 2023-11-15 20:50:59.756452 bany-1.4.3/bany/cmd/solve/solvers/graphsolver.py
--rw-r--r--   0        0        0     3158 2023-01-04 02:52:24.557117 bany-1.4.3/bany/cmd/solve/solvers/montecarlo.py
--rw-r--r--   0        0        0     1877 2023-01-04 02:52:24.557334 bany-1.4.3/bany/cmd/solve/solvers/unconstrained.py
--rw-r--r--   0        0        0        0 2023-11-15 20:50:59.756584 bany-1.4.3/bany/cmd/split/__init__.py
--rw-r--r--   0        0        0    12650 2023-11-15 21:03:19.116596 bany-1.4.3/bany/cmd/split/app.py
--rw-r--r--   0        0        0    12731 2023-11-14 20:41:46.783826 bany-1.4.3/bany/cmd/split/splitter.py
--rw-r--r--   0        0        0        0 2022-11-03 00:47:00.532709 bany-1.4.3/bany/core/__init__.py
--rw-r--r--   0        0        0     1573 2022-10-19 01:24:39.858651 bany-1.4.3/bany/core/cache.py
--rw-r--r--   0        0        0      323 2023-01-04 02:52:24.557561 bany-1.4.3/bany/core/config.py
--rw-r--r--   0        0        0      130 2023-11-18 23:05:09.909346 bany-1.4.3/bany/core/logger.py
--rw-r--r--   0        0        0     1146 2023-02-11 03:40:57.081932 bany-1.4.3/bany/core/money.py
--rw-r--r--   0        0        0      376 2023-11-14 20:41:46.784103 bany-1.4.3/bany/core/settings.py
--rw-r--r--   0        0        0        0 2022-10-19 01:37:38.770632 bany-1.4.3/bany/ynab/__init__.py
--rw-r--r--   0        0        0     4351 2023-11-15 20:50:59.757429 bany-1.4.3/bany/ynab/api.py
--rw-r--r--   0        0        0     1843 2023-11-14 20:41:46.784683 bany-1.4.3/bany/ynab/mock.py
--rw-r--r--   0        0        0     1537 2023-11-14 20:41:46.784945 bany-1.4.3/bany/ynab/transaction.py
--rw-r--r--   0        0        0     1277 2023-11-18 23:06:27.446946 bany-1.4.3/pyproject.toml
--rw-r--r--   0        0        0    11475 1970-01-01 00:00:00.000000 bany-1.4.3/PKG-INFO
+-rw-r--r--   0        0        0    10118 2023-11-15 21:03:19.115145 bany-1.4.4/README.md
+-rw-r--r--   0        0        0        0 2022-10-02 15:09:36.217615 bany-1.4.4/bany/__init__.py
+-rw-r--r--   0        0        0     4294 2024-04-30 23:26:47.920509 bany-1.4.4/bany/__main__.py
+-rw-r--r--   0        0        0        0 2022-11-03 00:40:20.325732 bany-1.4.4/bany/cmd/__init__.py
+-rw-r--r--   0        0        0        0 2023-11-15 21:03:19.115345 bany-1.4.4/bany/cmd/extract/__init__.py
+-rw-r--r--   0        0        0     1853 2023-11-15 20:50:59.755388 bany-1.4.4/bany/cmd/extract/app.py
+-rw-r--r--   0        0        0      115 2023-01-02 22:11:13.071746 bany-1.4.4/bany/cmd/extract/extractors/__init__.py
+-rw-r--r--   0        0        0      528 2023-01-02 22:29:16.298716 bany-1.4.4/bany/cmd/extract/extractors/base.py
+-rw-r--r--   0        0        0     9005 2024-04-30 23:26:47.931277 bany-1.4.4/bany/cmd/extract/extractors/pdf.py
+-rw-r--r--   0        0        0     3452 2024-04-30 23:26:47.951010 bany-1.4.4/bany/cmd/extract/rules.py
+-rw-r--r--   0        0        0        0 2023-11-15 20:50:59.755526 bany-1.4.4/bany/cmd/solve/__init__.py
+-rw-r--r--   0        0        0     2136 2023-11-17 16:26:28.922422 bany-1.4.4/bany/cmd/solve/app.py
+-rw-r--r--   0        0        0        0 2023-01-04 02:52:24.554271 bany-1.4.4/bany/cmd/solve/network/__init__.py
+-rw-r--r--   0        0        0     8344 2023-01-04 02:52:24.554650 bany-1.4.4/bany/cmd/solve/network/algo.py
+-rw-r--r--   0        0        0     5163 2023-11-18 23:05:09.908173 bany-1.4.4/bany/cmd/solve/network/attrs.py
+-rw-r--r--   0        0        0     3266 2023-11-18 23:05:09.908470 bany-1.4.4/bany/cmd/solve/network/loader.py
+-rw-r--r--   0        0        0     4017 2023-01-04 02:52:24.555422 bany-1.4.4/bany/cmd/solve/network/validate.py
+-rw-r--r--   0        0        0     4225 2023-11-18 23:05:09.908758 bany-1.4.4/bany/cmd/solve/network/visualize.py
+-rw-r--r--   0        0        0      479 2023-01-04 02:52:24.555930 bany-1.4.4/bany/cmd/solve/solvers/__init__.py
+-rw-r--r--   0        0        0     1495 2023-01-04 02:52:24.556171 bany-1.4.4/bany/cmd/solve/solvers/basesolver.py
+-rw-r--r--   0        0        0     3804 2023-01-04 02:52:24.556400 bany-1.4.4/bany/cmd/solve/solvers/bucketdata.py
+-rw-r--r--   0        0        0     2863 2023-11-18 23:05:09.909067 bany-1.4.4/bany/cmd/solve/solvers/constrained.py
+-rw-r--r--   0        0        0     6045 2023-11-15 20:50:59.756452 bany-1.4.4/bany/cmd/solve/solvers/graphsolver.py
+-rw-r--r--   0        0        0     3158 2023-01-04 02:52:24.557117 bany-1.4.4/bany/cmd/solve/solvers/montecarlo.py
+-rw-r--r--   0        0        0     1877 2023-01-04 02:52:24.557334 bany-1.4.4/bany/cmd/solve/solvers/unconstrained.py
+-rw-r--r--   0        0        0        0 2023-11-15 20:50:59.756584 bany-1.4.4/bany/cmd/split/__init__.py
+-rw-r--r--   0        0        0    12650 2023-11-15 21:03:19.116596 bany-1.4.4/bany/cmd/split/app.py
+-rw-r--r--   0        0        0    12731 2023-11-14 20:41:46.783826 bany-1.4.4/bany/cmd/split/splitter.py
+-rw-r--r--   0        0        0        0 2022-11-03 00:47:00.532709 bany-1.4.4/bany/core/__init__.py
+-rw-r--r--   0        0        0     1573 2022-10-19 01:24:39.858651 bany-1.4.4/bany/core/cache.py
+-rw-r--r--   0        0        0      323 2023-01-04 02:52:24.557561 bany-1.4.4/bany/core/config.py
+-rw-r--r--   0        0        0      130 2023-11-18 23:05:09.909346 bany-1.4.4/bany/core/logger.py
+-rw-r--r--   0        0        0     1146 2023-02-11 03:40:57.081932 bany-1.4.4/bany/core/money.py
+-rw-r--r--   0        0        0      376 2023-11-14 20:41:46.784103 bany-1.4.4/bany/core/settings.py
+-rw-r--r--   0        0        0        0 2022-10-19 01:37:38.770632 bany-1.4.4/bany/ynab/__init__.py
+-rw-r--r--   0        0        0     4351 2023-11-15 20:50:59.757429 bany-1.4.4/bany/ynab/api.py
+-rw-r--r--   0        0        0     1843 2023-11-14 20:41:46.784683 bany-1.4.4/bany/ynab/mock.py
+-rw-r--r--   0        0        0     1537 2023-11-14 20:41:46.784945 bany-1.4.4/bany/ynab/transaction.py
+-rw-r--r--   0        0        0     1282 2024-04-30 23:30:17.412184 bany-1.4.4/pyproject.toml
+-rw-r--r--   0        0        0    11471 1970-01-01 00:00:00.000000 bany-1.4.4/PKG-INFO
```

### Comparing `bany-1.4.3/README.md` & `bany-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `bany-1.4.3/bany/__main__.py` & `bany-1.4.4/bany/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,29 +11,30 @@
 import pandas as pd
 from rich.console import Console
 from rich.logging import RichHandler
 from rich.theme import Theme
 from typer import Option
 from typer import Typer
 
+
 app = Typer(add_completion=False, help=__doc__, rich_markup_mode="rich")
 
 
 @app.callback()
 def setup(
     verbose: Annotated[bool, Option()] = False,
 ) -> None:
     logging.basicConfig(
         level=logging.DEBUG,
         format="%(message)s",
         datefmt="[%X]",
         handlers=[
             RichHandler(
                 show_path=False,
-                rich_tracebacks=True,
+                rich_tracebacks=False,
                 tracebacks_suppress=(pandas,),
                 console=Console(theme=Theme({"repr.number": ""})),
             )
         ],
     )
     logging.getLogger("pdfminer").setLevel(logging.WARNING)
 
@@ -50,17 +51,17 @@
     config: Annotated[Path, Option(help="The config file to use.")] = Path.cwd().joinpath("config.yml"),
     step_size: Annotated[float, Option(help="The Monte Carlo step size to use.")] = 0.01,
     sheet_name: Annotated[str, Option(help="The sheet name or # when loading xlsx")] = "Sheet1",
 ) -> None:
     """
     Solve the partitioning problem using Monte Carlo techniques.
     """
-    from bany.cmd.solve.solvers.montecarlo import BucketSolverConstrainedMonteCarlo
-    from bany.cmd.solve.solvers.basesolver import BucketSolver
     from bany.cmd.solve.app import main
+    from bany.cmd.solve.solvers.basesolver import BucketSolver
+    from bany.cmd.solve.solvers.montecarlo import BucketSolverConstrainedMonteCarlo
 
     main(
         config=config,
         solver=cast(
             type[BucketSolver],
             partial(
                 BucketSolverConstrainedMonteCarlo.solve,
@@ -75,17 +76,17 @@
 def constrained(
     config: Annotated[Path, Option(help="The config file to use.")] = Path.cwd().joinpath("config.yml"),
     sheet_name: Annotated[str, Option(help="The sheet name or # when loading xlsx")] = "Sheet1",
 ) -> None:
     """
     Solve the partitioning problem using constrained optimization.
     """
-    from bany.cmd.solve.solvers.constrained import BucketSolverConstrained
-    from bany.cmd.solve.solvers.basesolver import BucketSolver
     from bany.cmd.solve.app import main
+    from bany.cmd.solve.solvers.basesolver import BucketSolver
+    from bany.cmd.solve.solvers.constrained import BucketSolverConstrained
 
     main(
         config=config,
         solver=cast(
             type[BucketSolver],
             partial(
                 BucketSolverConstrained.solve,
@@ -99,17 +100,17 @@
 def unconstrained(
     config: Annotated[Path, Option(help="The config file to use.")] = Path.cwd().joinpath("config.yml"),
     sheet_name: Annotated[str, Option(help="The sheet name or # when loading xlsx")] = "Sheet1",
 ) -> None:
     """
     Solve the partitioning problem using unconstrained optimization.
     """
-    from bany.cmd.solve.solvers.unconstrained import BucketSolverSimple
-    from bany.cmd.solve.solvers.basesolver import BucketSolver
     from bany.cmd.solve.app import main
+    from bany.cmd.solve.solvers.basesolver import BucketSolver
+    from bany.cmd.solve.solvers.unconstrained import BucketSolverSimple
 
     main(
         config=config,
         solver=cast(
             type[BucketSolver],
             partial(
                 BucketSolverSimple.solve,
```

### Comparing `bany-1.4.3/bany/cmd/extract/app.py` & `bany-1.4.4/bany/cmd/extract/app.py`

 * *Files identical despite different names*

### Comparing `bany-1.4.3/bany/cmd/extract/extractors/base.py` & `bany-1.4.4/bany/cmd/extract/extractors/base.py`

 * *Files identical despite different names*

### Comparing `bany-1.4.3/bany/cmd/extract/extractors/pdf.py` & `bany-1.4.4/bany/cmd/extract/extractors/pdf.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,15 +124,15 @@
         if rule.inflow:
             return money
         else:
             return -1 * money
 
     def _get_transactions_for_matches(self, dates: pd.DataFrame, amounts: pd.DataFrame) -> Iterator[Transaction]:
         for rule in self.rules.transactions:
-            if (amount := self._lookup_amount(rule.amount, amounts)) is not None:
+            if (amount := self._lookup_amount(rule.amount, amounts, rule.factor)) is not None:
                 budget_id = self.ynab.budget_id(rule.budget)
                 transaction = Transaction(
                     ####################################################################################################
                     # budget
                     ####################################################################################################
                     budget_id=budget_id,
                     budget_name=rule.budget,
@@ -176,22 +176,23 @@
                 return dates.loc[key, "value"]
             except KeyError:
                 self._log_block("_lookup_date", "[%11s] KeyError: %s", "dates".center(11, "-"), key)
                 return date(1970, 1, 1)
         else:
             raise NotImplementedError(type(key))
 
-    def _lookup_amount(self, key: int | tuple[int, int, str], amounts: pd.DataFrame) -> Money | None:
+    def _lookup_amount(self, key: int | tuple[int, int, str], amounts: pd.DataFrame, factor: int = 1) -> Money | None:
         if isinstance(key, Money):
-            return key
+            return factor * key
         elif isinstance(key, tuple):
             try:
-                return amounts.loc[key, "value"]
+                amount = amounts.loc[key, "value"]
+                return factor * amount
             except KeyError:
-                self._log_block("_lookup_date", "[%11s] KeyError: %s", "amounts".center(11, "-"), key)
+                self._log_block("_lookup_$$$$", "[%11s] KeyError: %s", "amounts".center(11, "-"), key)
                 return
         else:
             raise NotImplementedError(type(key))
 
     def _log_block(self, key: str, msg: str, *args, line: int = logging.INFO, level: int = logging.ERROR):
         if not self.state.get(key, False):
             logline(level=line)
```

### Comparing `bany-1.4.3/bany/cmd/extract/rules.py` & `bany-1.4.4/bany/cmd/extract/rules.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,14 +72,15 @@
     account: str
     payee: str | None = None
     category: str | None = None
     memo: str | None = None
     color: str | None = None
     amount: int | str | tuple[int, int, str]
     date: date | str | tuple[int, int, str]
+    factor: int = 1
 
     @field_validator("budget", mode="before")
     def _validate_budget(cls, value: str):
         return str(value)
 
     @field_validator("account", mode="before")
     def _validate_account(cls, value: str):
```

### Comparing `bany-1.4.3/bany/cmd/solve/app.py` & `bany-1.4.4/bany/cmd/solve/app.py`

 * *Files identical despite different names*

### Comparing `bany-1.4.3/bany/cmd/solve/network/algo.py` & `bany-1.4.4/bany/cmd/solve/network/algo.py`

 * *Files identical despite different names*

### Comparing `bany-1.4.3/bany/cmd/solve/network/attrs.py` & `bany-1.4.4/bany/cmd/solve/network/attrs.py`

 * *Files identical despite different names*

### Comparing `bany-1.4.3/bany/cmd/solve/network/loader.py` & `bany-1.4.4/bany/cmd/solve/network/loader.py`

 * *Files identical despite different names*

### Comparing `bany-1.4.3/bany/cmd/solve/network/validate.py` & `bany-1.4.4/bany/cmd/solve/network/validate.py`

 * *Files identical despite different names*

### Comparing `bany-1.4.3/bany/cmd/solve/network/visualize.py` & `bany-1.4.4/bany/cmd/solve/network/visualize.py`

 * *Files identical despite different names*

### Comparing `bany-1.4.3/bany/cmd/solve/solvers/basesolver.py` & `bany-1.4.4/bany/cmd/solve/solvers/basesolver.py`

 * *Files identical despite different names*

### Comparing `bany-1.4.3/bany/cmd/solve/solvers/bucketdata.py` & `bany-1.4.4/bany/cmd/solve/solvers/bucketdata.py`

 * *Files identical despite different names*

### Comparing `bany-1.4.3/bany/cmd/solve/solvers/constrained.py` & `bany-1.4.4/bany/cmd/solve/solvers/constrained.py`

 * *Files identical despite different names*

### Comparing `bany-1.4.3/bany/cmd/solve/solvers/graphsolver.py` & `bany-1.4.4/bany/cmd/solve/solvers/graphsolver.py`

 * *Files identical despite different names*

### Comparing `bany-1.4.3/bany/cmd/solve/solvers/montecarlo.py` & `bany-1.4.4/bany/cmd/solve/solvers/montecarlo.py`

 * *Files identical despite different names*

### Comparing `bany-1.4.3/bany/cmd/solve/solvers/unconstrained.py` & `bany-1.4.4/bany/cmd/solve/solvers/unconstrained.py`

 * *Files identical despite different names*

### Comparing `bany-1.4.3/bany/cmd/split/app.py` & `bany-1.4.4/bany/cmd/split/app.py`

 * *Files identical despite different names*

### Comparing `bany-1.4.3/bany/cmd/split/splitter.py` & `bany-1.4.4/bany/cmd/split/splitter.py`

 * *Files identical despite different names*

### Comparing `bany-1.4.3/bany/core/cache.py` & `bany-1.4.4/bany/core/cache.py`

 * *Files identical despite different names*

### Comparing `bany-1.4.3/bany/core/money.py` & `bany-1.4.4/bany/core/money.py`

 * *Files identical despite different names*

### Comparing `bany-1.4.3/bany/ynab/api.py` & `bany-1.4.4/bany/ynab/api.py`

 * *Files identical despite different names*

### Comparing `bany-1.4.3/bany/ynab/mock.py` & `bany-1.4.4/bany/ynab/mock.py`

 * *Files identical despite different names*

### Comparing `bany-1.4.3/bany/ynab/transaction.py` & `bany-1.4.4/bany/ynab/transaction.py`

 * *Files identical despite different names*

### Comparing `bany-1.4.3/pyproject.toml` & `bany-1.4.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 [tool.isort]
 profile = "black"
 line_length = 120
 lines_after_imports = 2
 
 [tool.poetry]
 name = "bany"
-version = "1.4.3"
+version = "1.4.4"
 description = "A collection of scripts for personal finance"
 authors = ["Adam Gagorik <adam.gagorik@gmail.com>"]
 readme = "README.md"
 license = "WTFPL"
 repository = "https://github.com/AdamGagorik/bany"
 keywords = ["YNAB", "finance", "budgeting"]
 
@@ -27,15 +27,15 @@
 python-dateutil = "^2.8.2"
 oauthlib = "^3.2.2"
 pydantic = "^2.5.1"
 python-dotenv = ">=1.0.0"
 requests = "^2.31.0"
 rich = "^13.7.0"
 diskcache = "^5.6.3"
-responses = "^0.22.0"
+responses = ">=0.22,<0.25"
 pandas = "^2.1.3"
 py-moneyed = "^3.0"
 PyYAML = "^6.0.1"
 networkx = "^3.2.1"
 scipy = "^1.11.3"
 cmd2 = "^2.4.3"
 textualize = "^0.1"
```

### Comparing `bany-1.4.3/PKG-INFO` & `bany-1.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bany
-Version: 1.4.3
+Version: 1.4.4
 Summary: A collection of scripts for personal finance
 Home-page: https://github.com/AdamGagorik/bany
 License: WTFPL
 Keywords: YNAB,finance,budgeting
 Author: Adam Gagorik
 Author-email: adam.gagorik@gmail.com
 Requires-Python: >=3.11,<3.12
@@ -21,15 +21,15 @@
 Requires-Dist: pdfplumber (>=0.10.3)
 Requires-Dist: py-moneyed (>=3.0,<4.0)
 Requires-Dist: pydantic (>=2.5.1,<3.0.0)
 Requires-Dist: pydantic-settings (>=2.1.0,<3.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
-Requires-Dist: responses (>=0.22.0,<0.23.0)
+Requires-Dist: responses (>=0.22,<0.25)
 Requires-Dist: rich (>=13.7.0,<14.0.0)
 Requires-Dist: scipy (>=1.11.3,<2.0.0)
 Requires-Dist: setuptools (>=68.2.2,<69.0.0)
 Requires-Dist: textualize (>=0.1,<0.2)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
 Project-URL: Repository, https://github.com/AdamGagorik/bany
 Description-Content-Type: text/markdown
```

