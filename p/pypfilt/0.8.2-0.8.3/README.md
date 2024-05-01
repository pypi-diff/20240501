# Comparing `tmp/pypfilt-0.8.2-py3-none-any.whl.zip` & `tmp/pypfilt-0.8.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 105883 bytes, number of entries: 35
+Zip file size: 106168 bytes, number of entries: 35
 -rw-r--r--  2.0 unx    19221 b- defN 20-Feb-02 00:00 pypfilt/__init__.py
 -rw-r--r--  2.0 unx     8742 b- defN 20-Feb-02 00:00 pypfilt/adaptive.py
 -rw-r--r--  2.0 unx    39166 b- defN 20-Feb-02 00:00 pypfilt/build.py
 -rw-r--r--  2.0 unx    18881 b- defN 20-Feb-02 00:00 pypfilt/cache.py
 -rw-r--r--  2.0 unx     4813 b- defN 20-Feb-02 00:00 pypfilt/crps.py
 -rw-r--r--  2.0 unx     2775 b- defN 20-Feb-02 00:00 pypfilt/event.py
 -rw-r--r--  2.0 unx    28010 b- defN 20-Feb-02 00:00 pypfilt/io.py
@@ -26,12 +26,12 @@
 -rw-r--r--  2.0 unx      182 b- defN 20-Feb-02 00:00 pypfilt/examples/predation-counts-y.ssv
 -rw-r--r--  2.0 unx     1656 b- defN 20-Feb-02 00:00 pypfilt/examples/predation-datetime.toml
 -rw-r--r--  2.0 unx    14306 b- defN 20-Feb-02 00:00 pypfilt/examples/predation.py
 -rw-r--r--  2.0 unx     1635 b- defN 20-Feb-02 00:00 pypfilt/examples/predation.toml
 -rw-r--r--  2.0 unx     1966 b- defN 20-Feb-02 00:00 pypfilt/examples/simple.py
 -rw-r--r--  2.0 unx    14328 b- defN 20-Feb-02 00:00 pypfilt/examples/sir.py
 -rw-r--r--  2.0 unx     1545 b- defN 20-Feb-02 00:00 pypfilt/examples/sir.toml
-?rw-r--r--  2.0 unx     4713 b- defN 20-Feb-02 00:00 pypfilt-0.8.2.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 pypfilt-0.8.2.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1499 b- defN 20-Feb-02 00:00 pypfilt-0.8.2.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx     2813 b- defN 20-Feb-02 00:00 pypfilt-0.8.2.dist-info/RECORD
-35 files, 407407 bytes uncompressed, 101469 bytes compressed:  75.1%
+?rw-r--r--  2.0 unx     5450 b- defN 20-Feb-02 00:00 pypfilt-0.8.3.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 pypfilt-0.8.3.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1499 b- defN 20-Feb-02 00:00 pypfilt-0.8.3.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx     2813 b- defN 20-Feb-02 00:00 pypfilt-0.8.3.dist-info/RECORD
+35 files, 408144 bytes uncompressed, 101754 bytes compressed:  75.1%
```

## zipnote {}

```diff
@@ -87,20 +87,20 @@
 
 Filename: pypfilt/examples/sir.py
 Comment: 
 
 Filename: pypfilt/examples/sir.toml
 Comment: 
 
-Filename: pypfilt-0.8.2.dist-info/METADATA
+Filename: pypfilt-0.8.3.dist-info/METADATA
 Comment: 
 
-Filename: pypfilt-0.8.2.dist-info/WHEEL
+Filename: pypfilt-0.8.3.dist-info/WHEEL
 Comment: 
 
-Filename: pypfilt-0.8.2.dist-info/licenses/LICENSE
+Filename: pypfilt-0.8.3.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: pypfilt-0.8.2.dist-info/RECORD
+Filename: pypfilt-0.8.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `pypfilt-0.8.2.dist-info/METADATA` & `pypfilt-0.8.3.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypfilt
-Version: 0.8.2
+Version: 0.8.3
 Summary: Bootstrap particle filter for epidemic forecasting
 Project-URL: homepage, https://bitbucket.org/robmoss/particle-filter-for-python/
 Project-URL: repository, https://bitbucket.org/robmoss/particle-filter-for-python/
 Project-URL: documentation, https://pypfilt.readthedocs.io/en/latest/
 Project-URL: changelog, https://pypfilt.readthedocs.io/en/latest/changelog.html
 Author-email: Rob Moss <rgmoss@unimelb.edu.au>
 Maintainer-email: Rob Moss <rgmoss@unimelb.edu.au>
@@ -42,30 +42,30 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Requires-Python: >=3.8
 Requires-Dist: h5py~=3.0
 Requires-Dist: lhs~=0.4
-Requires-Dist: numpy~=1.17
+Requires-Dist: numpy>=1.17
 Requires-Dist: packaging~=21.3
 Requires-Dist: scipy~=1.4
 Requires-Dist: tomli-w~=1.0
 Requires-Dist: tomli~=2.0
 Provides-Extra: plot
 Requires-Dist: matplotlib~=3.4; extra == 'plot'
 Provides-Extra: tests
 Requires-Dist: pytest; extra == 'tests'
 Requires-Dist: pytest-cov~=4.0; extra == 'tests'
 Description-Content-Type: text/x-rst
 
 Bootstrap particle filter for epidemic forecasting
 ==================================================
 
-|version| |docs| |tests| |coverage|
+|version| |joss| |docs| |tests| |coverage|
 
 Description
 -----------
 
 A bootstrap particle filter that can be used for recursive Bayesian estimation and forecasting.
 See the `online documentation <https://pypfilt.readthedocs.io/>`_ for tutorials, how-to guides, and API documentation.
 
@@ -88,18 +88,41 @@
 
     pip install pypfilt[plot]
 
 To install the latest development version, clone this repository and run::
 
     pip install .
 
+Citation
+--------
+
+If you use ``pypfilt``, please cite our `JOSS article <https://doi.org/10.21105/joss.06276>`_ and an archived release of the software (see ``CITATION.cff``).
+
+.. code-block:: bibtex
+
+   @article{pypfilt,
+     author = {Moss, Robert},
+     title = {pypfilt: a particle filter for {Python}},
+     journal = {Journal of Open Source Software},
+     volume = {9},
+     issue = {96},
+     pages = {6276},
+     year = {2024},
+     doi = {10.21105/joss.06276},
+     note = {Please cite this article and an archived release (see CITATION.cff)},
+   }
+
 .. |version| image:: https://badge.fury.io/py/pypfilt.svg
    :alt: Latest version
    :target: https://pypi.org/project/pypfilt/
 
+.. |joss| image:: https://joss.theoj.org/papers/10.21105/joss.06276/status.svg
+   :alt: Journal of Open Source Software
+   :target: https://doi.org/10.21105/joss.06276
+
 .. |docs| image::  https://readthedocs.org/projects/pypfilt/badge/
    :alt: Documentation
    :target: https://pypfilt.readthedocs.io/
 
 .. |tests| image:: https://gitlab.unimelb.edu.au/rgmoss/particle-filter-for-python/badges/master/pipeline.svg
    :alt: Test cases
    :target: https://gitlab.unimelb.edu.au/rgmoss/particle-filter-for-python
```

## Comparing `pypfilt-0.8.2.dist-info/licenses/LICENSE` & `pypfilt-0.8.3.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `pypfilt-0.8.2.dist-info/RECORD` & `pypfilt-0.8.3.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -25,11 +25,11 @@
 pypfilt/examples/predation-counts-y.ssv,sha256=JWv7v3JnrsuS59WNrd3D9hRAUeHWAgFU3KVeY6ptgKw,182
 pypfilt/examples/predation-datetime.toml,sha256=pggfXLNXMUBVdQjEFdi1m_0YwQtxfJigig8XdXdxp0k,1656
 pypfilt/examples/predation.py,sha256=yHJHIOCLhD6H1b65-D5_mh_K430kiqftUG0jLlVAxBw,14306
 pypfilt/examples/predation.toml,sha256=j603IYyp0YnfoiJW5lY7BALjhinHAvTuEwPqbGZB7X8,1635
 pypfilt/examples/simple.py,sha256=_RgywpuxSr_nj32JaOVIR4ZrYGqOe22u270OWGCoQA0,1966
 pypfilt/examples/sir.py,sha256=paPFZ2LTzTQWqTlDFzTFupFsjKNUCq6qKZQNOcsGdOo,14328
 pypfilt/examples/sir.toml,sha256=Qb1Ljbb194JPXkrqZQzGYE0VSWefzugljlSwKlVfLiQ,1545
-pypfilt-0.8.2.dist-info/METADATA,sha256=vMVJ3jf13TVECtUCq2FJltFyJQ2iZOzouiSiAcx--Vs,4713
-pypfilt-0.8.2.dist-info/WHEEL,sha256=uNdcs2TADwSd5pVaP0Z_kcjcvvTUklh2S7bxZMF8Uj0,87
-pypfilt-0.8.2.dist-info/licenses/LICENSE,sha256=n6NHAuK5rNxjBjRwh8NEWP6Vyd3qH7dZMnynVd3fg1Y,1499
-pypfilt-0.8.2.dist-info/RECORD,,
+pypfilt-0.8.3.dist-info/METADATA,sha256=_T2GWzPlSs0hpvv3Rr1rEx1K8uP981Lul9ZUbnrJDE8,5450
+pypfilt-0.8.3.dist-info/WHEEL,sha256=zEMcRr9Kr03x1ozGwg5v9NQBKn3kndp6LSoSlVg-jhU,87
+pypfilt-0.8.3.dist-info/licenses/LICENSE,sha256=n6NHAuK5rNxjBjRwh8NEWP6Vyd3qH7dZMnynVd3fg1Y,1499
+pypfilt-0.8.3.dist-info/RECORD,,
```

