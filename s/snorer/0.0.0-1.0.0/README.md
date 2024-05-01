# Comparing `tmp/snorer-0.0.0.tar.gz` & `tmp/snorer-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snorer-0.0.0.tar", last modified: Fri Mar 29 01:52:44 2024, max compression
+gzip compressed data, was "snorer-1.0.0.tar", last modified: Wed May  1 05:49:51 2024, max compression
```

## Comparing `snorer-0.0.0.tar` & `snorer-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,23 @@
-drwxrwxr-x   0 yenhsun   (1000) yenhsun   (1000)        0 2024-03-29 01:52:44.680707 snorer-0.0.0/
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)    35129 2024-03-29 01:27:08.000000 snorer-0.0.0/LICENSE
--rw-r--r--   0 yenhsun   (1000) yenhsun   (1000)    42017 2024-03-29 01:52:44.680707 snorer-0.0.0/PKG-INFO
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)     1082 2024-03-29 01:33:46.000000 snorer-0.0.0/README.md
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)     1005 2024-03-29 01:40:26.000000 snorer-0.0.0/pyproject.toml
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)       38 2024-03-29 01:52:44.680707 snorer-0.0.0/setup.cfg
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)       49 2024-03-28 13:38:04.000000 snorer-0.0.0/setup.py
-drwxrwxr-x   0 yenhsun   (1000) yenhsun   (1000)        0 2024-03-29 01:52:44.680707 snorer-0.0.0/src/
-drwxrwxr-x   0 yenhsun   (1000) yenhsun   (1000)        0 2024-03-29 01:52:44.680707 snorer-0.0.0/src/snorer/
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)      909 2024-03-29 01:39:13.000000 snorer-0.0.0/src/snorer/__init__.py
-drwxrwxr-x   0 yenhsun   (1000) yenhsun   (1000)        0 2024-03-29 01:52:44.680707 snorer-0.0.0/src/snorer.egg-info/
--rw-r--r--   0 yenhsun   (1000) yenhsun   (1000)    42017 2024-03-29 01:52:44.000000 snorer-0.0.0/src/snorer.egg-info/PKG-INFO
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)      233 2024-03-29 01:52:44.000000 snorer-0.0.0/src/snorer.egg-info/SOURCES.txt
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)        1 2024-03-29 01:52:44.000000 snorer-0.0.0/src/snorer.egg-info/dependency_links.txt
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)       41 2024-03-29 01:52:44.000000 snorer-0.0.0/src/snorer.egg-info/requires.txt
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)        7 2024-03-29 01:52:44.000000 snorer-0.0.0/src/snorer.egg-info/top_level.txt
+drwxrwxr-x   0 yenhsun   (1000) yenhsun   (1000)        0 2024-05-01 05:49:51.632844 snorer-1.0.0/
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)    35129 2024-03-29 01:27:08.000000 snorer-1.0.0/LICENSE
+-rw-r--r--   0 yenhsun   (1000) yenhsun   (1000)    49151 2024-05-01 05:49:51.632844 snorer-1.0.0/PKG-INFO
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)     8123 2024-05-01 05:46:42.000000 snorer-1.0.0/README.md
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)     1094 2024-05-01 05:49:34.000000 snorer-1.0.0/pyproject.toml
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)       38 2024-05-01 05:49:51.632844 snorer-1.0.0/setup.cfg
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)       49 2024-03-28 13:38:04.000000 snorer-1.0.0/setup.py
+drwxrwxr-x   0 yenhsun   (1000) yenhsun   (1000)        0 2024-05-01 05:49:51.628844 snorer-1.0.0/src/
+drwxrwxr-x   0 yenhsun   (1000) yenhsun   (1000)        0 2024-05-01 05:49:51.632844 snorer-1.0.0/src/snorer/
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)     1983 2024-05-01 05:49:34.000000 snorer-1.0.0/src/snorer/__init__.py
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)     4299 2024-04-29 15:04:44.000000 snorer-1.0.0/src/snorer/constants.py
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)     9088 2024-04-27 15:23:37.000000 snorer-1.0.0/src/snorer/geometry.py
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)    18337 2024-04-30 11:09:15.000000 snorer-1.0.0/src/snorer/halo.py
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)    14000 2024-05-01 02:58:10.000000 snorer-1.0.0/src/snorer/kinematics.py
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)    13472 2024-04-30 11:21:06.000000 snorer-1.0.0/src/snorer/snorerMain.py
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)     1230 2024-04-28 14:34:31.000000 snorer-1.0.0/src/snorer/sysmsg.py
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)    17991 2024-05-01 02:58:17.000000 snorer-1.0.0/src/snorer/utils.py
+drwxrwxr-x   0 yenhsun   (1000) yenhsun   (1000)        0 2024-05-01 05:49:51.632844 snorer-1.0.0/src/snorer.egg-info/
+-rw-r--r--   0 yenhsun   (1000) yenhsun   (1000)    49151 2024-05-01 05:49:51.000000 snorer-1.0.0/src/snorer.egg-info/PKG-INFO
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)      390 2024-05-01 05:49:51.000000 snorer-1.0.0/src/snorer.egg-info/SOURCES.txt
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)        1 2024-05-01 05:49:51.000000 snorer-1.0.0/src/snorer.egg-info/dependency_links.txt
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)       56 2024-05-01 05:49:51.000000 snorer-1.0.0/src/snorer.egg-info/requires.txt
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)        7 2024-05-01 05:49:51.000000 snorer-1.0.0/src/snorer.egg-info/top_level.txt
```

### Comparing `snorer-0.0.0/LICENSE` & `snorer-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `snorer-0.0.0/PKG-INFO` & `snorer-1.0.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: snorer
-Version: 0.0.0
-Summary: Supernova-neutrino-boosted dark matter from our Milky Way
+Version: 1.0.0
+Summary: This package evaluates the time-of-flight signatures of boosted dark matter due to supernova neutrinos from our Milky Way
 Author-email: Yen-Hsun Lin <yenhsun@phys.ncku.edu.tw>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -675,45 +675,178 @@
         into proprietary programs.  If your program is a subroutine library, you
         may consider it more useful to permit linking proprietary applications with
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
 Project-URL: Homepage, https://github.com/yenhsunlin/snorer
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.20.0
 Requires-Dist: scipy>=1.10.0
 Requires-Dist: vegas>=6.0.1
+Requires-Dist: astropy>=6.0.0
 
-# snorer
+<a href = "https://python.org" target = "_blank">![Python](https://img.shields.io/badge/python-3.8-blue.svg)</a>
+<a href = "https://choosealicense.com/licenses/gpl-3.0/"  target = "_blank">![License](https://img.shields.io/badge/License-GPL_3.0-blue.svg)</a>
+<a href = "https://arxiv.org/abs/2206.06864"  target = "_blank">![ArXiv](https://img.shields.io/badge/arXiv-2206.06864-yellowgreen.svg)</a>
+<a href = "https://arxiv.org/abs/2307.03522"  target = "_blank">![ArXiv](https://img.shields.io/badge/arXiv-2307.03522-yellowgreen.svg)</a>
 
+# snorer: *S*upernova-*N*eutrino-b*O*osted da*R*k matt*ER*
 
-`snorer` is a package for evaluating the signatures of **S**upernova-**N**eutrino-b**O**osted da**R**k matt**ER** from our Milky Way based on *Phys. Rev. Lett.* **130**, 111002 (2023) and *Phys. Rev. D* **108**, 083013 (2023).
+
+`snorer` is a package for evaluating time-of-flight signatures of supernova-neutrino-boosted dark matter (SN*ν* BDM) from our Milky Way (MW) and SN1987a in Large Magellanic Cloud (LMC) based on
+<a href = "https://doi.org/10.1103/PhysRevLett.130.111002" target = "_blank">*Phys. Rev. Lett.* **130**, 111002 (2023)</a> [<a href = "https://arxiv.org/abs/2206.06864" target = "_blank">arXiv:2206.06864</a>]
+and
+<a href = "https://doi.org/10.1103/PhysRevD.108.083013" target = "_blank">*Phys. Rev. D* **108**, 083013 (2023)</a>
+[<a href = "https://arxiv.org/abs/2307.03522" target = "_blank">arXiv:2307.03522</a>].
 
 ## Installation
 
 To install, excute the following command on the prompt
 
     $ pip install snorer
 
 and everything should be processed on-the-fly.
 
 ### Dependency
 
-`dukes` requires these external packages
+`snorer` requires python >= 3.8 and the following packages these external packages
 
 - `numpy` >= 1.20.0
 - `scipy` >= 1.10.0
 - `vegas` >= 6.0.1
+- `astropy` >= 6.0.0
+
+where `vegas` is a the backend engine for evaluating multidimensional integrals based on adaptive Monte Carlo vegas algorithm, see its homepage: <a heref = "https://pypi.org/project/vegas/" target = "_blank">https://pypi.org/project/vegas/</a>.
+
+Other packages maybe required by these dependencies during the installation, see `requirements.txt` for details.
+The versions of these dependencies are not strict, but are recommended to update to the latest ones to avoid incompatibility.
+
+## Usage
+
+We briefly summarize the usage in this section and a comprehensive tutorial can be found in the jupyter notebook in `examples/tutorial.ipynb`.
+
+To import, do
+
+    >>> import snorer
+
+in python terminal and is similar in the jupyter notebook.
+All functions and classes can be accessed by typing `snorer.foo()` where `foo` is the name.
+
+
+
+
+### Useful Constants
+
+We document various useful physical constants and conversion factors...etc as the *attributes* of an instance `snorer.constant`.
+For example, we can retrieve
+
+    >>> snorer.constant.me      # electron mas, MeV
+    0.511
+    >>> snorer.constant.kpc2cm  # kpc to cm
+    3.085e+21
+
+We did this instead of naming them as constant variables in some module to prevent them from being edited.
+
+### BDM Velocity
+
+A boosted dark matter (BDM) with mass $m_\chi$ and kinetic energy $T_\chi$ has the velocity $v_\chi$,
+
+$$
+\frac{v_\chi}{c} = \frac{\sqrt{T_\chi(2m_\chi+T_\chi)}}{m_\chi+T_\chi}.
+$$
+
+Let $(T_\chi,m_\chi)=(15,0.075)$ MeV, we can use
+`snorer.get_vx()` to evaluate
+
+    >>> Tx,mx = 15,0.075
+    >>> snorer.get_vx(Tx,mx)
+    0.9999876239921284
+
+
+### SN*ν* BDM Flux 
+
+The BDM flux, or *afterglow* to the ${\rm SN}\nu$, due to SN that is $R_\star$ distant away from us can be evaluated by 
+
+$$
+\frac{d\Phi_{\chi}(T_\chi, t^\prime)}{dT_{\chi}dt} =
+\tau\int_0^{2\pi} d\phi\int_{0}^{\pi/2}\sin\theta d\theta~ \mathcal{J} j_{\chi}(r(\phi),D,T_{\chi},\psi)
+$$
+
+where $t$ is the BDM ToF with time-zero at the discovery of SN*ν* on Earth and $t^\prime$ is the total time. We focus on $t$ instead of $t^\prime$.
+Zenith angle $\theta$ and azimuthal angle $\phi$ are relative to the SN-Earth line-of-sight. The default DM-*ν* cross section is $\sigma_{\chi\nu}=10^{-45}$ cm<sup>2</sup>.
+
+The function to evaluate this flux is `snorer.flux()` with $(t,T_\chi,m_\chi,R_\star,\beta)$ are the necessary inputs. 
+Suppose SN's location is at GC, we have $R_\star=8.5$ kpc and $\beta=0$, and examine the flux with turning on DM spike feature
+
+    >>> t,Tx,mx,Rstar,beta = 100,15,1e-2,8.5,0
+    >>> snorer.flux(t,Tx,mx,Rstar,beta,neval=15000)
+    4.572295175982701e-16
+
+Users can turn off the spike feature by inserting `is_spike=False` and will find both numerical results are similar. It implies the contribution to the BDM flux is due to the place outside the spike's influencial region.
+
+### SN*ν* BDM Event
+
+The BDM event number in a detector after exposing to the flux for a period of time, $(t_{\rm min},t_{\rm max})$, can be evaluated by
+
+$$
+N_{\rm BDM} = \int_{t_{\rm min}}^{\rm t_{\rm max}} dt \int_{T_{\chi,{\rm min}}}^{T_{\chi,{\rm max}}}
+\frac{d\Phi_{\chi}(T_\chi, t^\prime)}{dT_{\chi}dt} \times N_e \sigma_{\chi e}
+$$
+
+where $N_e$ is the total electron number in the detector and $\sigma_{\chi e}$ the DM-*e* cross section.
+This can be accomplished by `snorer.event()` with $(m_\chi,R_\star,\beta)$ the necessary inputs.
+The default $(t_{\rm min},t_{\rm max})=(10~{\rm s},35~{\rm yrs})$ and $(T_{\chi,{\rm min}},T_{\chi,{\rm max}})=(5,30)$ MeV.
+
+Note that this function is normalized to $N_e=1$ and $\sigma_{\chi e}=1$ cm<sup>2</sup>.
+To have the correct $N_{\rm BDM}$ in a specific detector, users have to mutiply the corresponding $N_e$ and $\sigma_{\chi e}$.
+
+Now let $m_\chi=0.015$ MeV,
+
+    >>> mx,Rstar,beta = 0.015,8,0
+    >>> N_BDM = snorer.event(mx,Rstar,beta,is_spike=False,neval=50000)
+    >>> N_BDM
+    1.662174035857532e-06
+
+Suppose it happened in Super-Kamiokande with $N_e\approx 7\times 10^{33}$ and assume $\sigma_{\chi e}=10^{-30}$ cm<sup>2</sup>. The correct $N_{\rm BDM}$ would be
+
+    >>> Ne,sigma_xe = 7e33,1e-35
+    >>> N_BDM*Ne*sigma_xe
+    1.1635218251002724e-07
+
+### *Experimental* :: Implementation of Particle Physics Model and SN in Arbitrary Distant Galaxy
+
+The aforementioned functions for evaluating BDM signatures are based on model-agnostic picture. It means the cross sections between dark and visble sectors are generally independent of any physical quantities, eg. energy, mass and coupling constants.
+
+The most important feature of `snorer` is that it offers a general interface for users to implement their favorite particle models.
+Furthermore, SN is not necessary residing in MW or LMC. As long as users can provide these celetial objects' coordinates expressed in *ICRS J2000.0* system, `snorer` can do the calculation.
+`snorer` also allows users to customize the halo shape, by manipulating $\rho_s$, $r_s$ and $n$...etc, and including or excluding spike feature, of such distant galaxy.
+
+This will be done by introducing a *class* `snorer.GeneralInterface`.
+All these user-specified features will compose an instance of `snorer.GeneralInterface`.
+The BDM signatures can be evaluated by calling the associated *methods* within it.
+We have an example in `examples/tutorial.ipynb`, also see the in-class docstring for more information.
+
+
+### Other Useful Functions Classes
+
+We also provide many useful functions and classes at users' disposal. See `examples/tutorial.ipynb` for details.
+
+## Known Issue
+
+To evaluate BDM event, `snorer` uses `vegas` to handle the multidimensional integration.
+The sampling method of `vegas` cannot manipulate`snorer.event()` as well as the method in the instance of `snorer.GeneralInterface` properly, when SN is exactly at GC with spike feature turning on and no DM self-annihilation.
 
-where `vegas` is a the backend engine for evaluating multidimensional integrals based on adaptive Monte Carlo vegas algorithm, see its homepage: [https://pypi.org/project/vegas/](https://pypi.org/project/vegas/).
+Since the spike is a highly singular behavior, the sampling method may miss the substantial DM contribution from the inner galactic region and causes underestimate of $N_{\rm BDM}$ plus unstable results. 
+To avoid this, users may try to displace the SN from GC when evaluating $N_{\rm BDM}$ whith DM sipke turning on and no DM annihilation.
+For BDM flux evaluation, there is no such issue.
 
-Other packages, e.g. `gvar`, maybe required by these dependencies during the installation.
-The versions of these dependencies are not strict, but are recommended to update to the latest ones to avoid incompatibility. 
+To be fair, the probability of a very cuspy DM spike surving the gravitational disturbance without annihilating away and SN happening exactly at the GC might be very rare.
 
+This issue is scheduled to fix in the next version of `snorer`.
 
+## Bugs and troubleshooting
 
-## Misc
+Please report to the author, Yen-Hsun Lin, via [yenhsun@phys.ncku.edu.tw](mailto:yenhsun@phys.ncku.edu.tw).
 
-Bug report and troubleshooting please contact the author Yen-Hsun Lin via [yenhsun@phys.ncku.edu.tw](mailto:yenhsun@phys.ncku.edu.tw).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `snorer-0.0.0/pyproject.toml` & `snorer-1.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "snorer"
-version = "0.0.0"
-description = "Supernova-neutrino-boosted dark matter from our Milky Way"
+version = "1.0.0"
+description = "This package evaluates the time-of-flight signatures of boosted dark matter due to supernova neutrinos from our Milky Way"
 readme = "README.md"
 authors = [{ name = "Yen-Hsun Lin", email = "yenhsun@phys.ncku.edu.tw" }]
 license = { file = "LICENSE" }
 dependencies = [
     "numpy >= 1.20.0",
     "scipy >= 1.10.0",
-    "vegas >= 6.0.1",]
-requires-python = ">=3.6"
+    "vegas >= 6.0.1",
+    "astropy >= 6.0.0",]
+requires-python = ">=3.8"
 
 [project.urls]
 Homepage = "https://github.com/yenhsunlin/snorer"
 
 [tool.bumpver]
-current_version = "0.0.0"
+current_version = "1.0.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 tag_message = "{new_version}"
 tag_scope = "default"
 pre_commit_hook = ""
 post_commit_hook = ""
 commit = true
 tag = true
-push = true
+push = false
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = [
     'current_version = "{version}"',
 ]
 
 #"README.md" = [
```

### Comparing `snorer-0.0.0/src/snorer.egg-info/PKG-INFO` & `snorer-1.0.0/src/snorer.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: snorer
-Version: 0.0.0
-Summary: Supernova-neutrino-boosted dark matter from our Milky Way
+Version: 1.0.0
+Summary: This package evaluates the time-of-flight signatures of boosted dark matter due to supernova neutrinos from our Milky Way
 Author-email: Yen-Hsun Lin <yenhsun@phys.ncku.edu.tw>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -675,45 +675,178 @@
         into proprietary programs.  If your program is a subroutine library, you
         may consider it more useful to permit linking proprietary applications with
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
 Project-URL: Homepage, https://github.com/yenhsunlin/snorer
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.20.0
 Requires-Dist: scipy>=1.10.0
 Requires-Dist: vegas>=6.0.1
+Requires-Dist: astropy>=6.0.0
 
-# snorer
+<a href = "https://python.org" target = "_blank">![Python](https://img.shields.io/badge/python-3.8-blue.svg)</a>
+<a href = "https://choosealicense.com/licenses/gpl-3.0/"  target = "_blank">![License](https://img.shields.io/badge/License-GPL_3.0-blue.svg)</a>
+<a href = "https://arxiv.org/abs/2206.06864"  target = "_blank">![ArXiv](https://img.shields.io/badge/arXiv-2206.06864-yellowgreen.svg)</a>
+<a href = "https://arxiv.org/abs/2307.03522"  target = "_blank">![ArXiv](https://img.shields.io/badge/arXiv-2307.03522-yellowgreen.svg)</a>
 
+# snorer: *S*upernova-*N*eutrino-b*O*osted da*R*k matt*ER*
 
-`snorer` is a package for evaluating the signatures of **S**upernova-**N**eutrino-b**O**osted da**R**k matt**ER** from our Milky Way based on *Phys. Rev. Lett.* **130**, 111002 (2023) and *Phys. Rev. D* **108**, 083013 (2023).
+
+`snorer` is a package for evaluating time-of-flight signatures of supernova-neutrino-boosted dark matter (SN*ν* BDM) from our Milky Way (MW) and SN1987a in Large Magellanic Cloud (LMC) based on
+<a href = "https://doi.org/10.1103/PhysRevLett.130.111002" target = "_blank">*Phys. Rev. Lett.* **130**, 111002 (2023)</a> [<a href = "https://arxiv.org/abs/2206.06864" target = "_blank">arXiv:2206.06864</a>]
+and
+<a href = "https://doi.org/10.1103/PhysRevD.108.083013" target = "_blank">*Phys. Rev. D* **108**, 083013 (2023)</a>
+[<a href = "https://arxiv.org/abs/2307.03522" target = "_blank">arXiv:2307.03522</a>].
 
 ## Installation
 
 To install, excute the following command on the prompt
 
     $ pip install snorer
 
 and everything should be processed on-the-fly.
 
 ### Dependency
 
-`dukes` requires these external packages
+`snorer` requires python >= 3.8 and the following packages these external packages
 
 - `numpy` >= 1.20.0
 - `scipy` >= 1.10.0
 - `vegas` >= 6.0.1
+- `astropy` >= 6.0.0
+
+where `vegas` is a the backend engine for evaluating multidimensional integrals based on adaptive Monte Carlo vegas algorithm, see its homepage: <a heref = "https://pypi.org/project/vegas/" target = "_blank">https://pypi.org/project/vegas/</a>.
+
+Other packages maybe required by these dependencies during the installation, see `requirements.txt` for details.
+The versions of these dependencies are not strict, but are recommended to update to the latest ones to avoid incompatibility.
+
+## Usage
+
+We briefly summarize the usage in this section and a comprehensive tutorial can be found in the jupyter notebook in `examples/tutorial.ipynb`.
+
+To import, do
+
+    >>> import snorer
+
+in python terminal and is similar in the jupyter notebook.
+All functions and classes can be accessed by typing `snorer.foo()` where `foo` is the name.
+
+
+
+
+### Useful Constants
+
+We document various useful physical constants and conversion factors...etc as the *attributes* of an instance `snorer.constant`.
+For example, we can retrieve
+
+    >>> snorer.constant.me      # electron mas, MeV
+    0.511
+    >>> snorer.constant.kpc2cm  # kpc to cm
+    3.085e+21
+
+We did this instead of naming them as constant variables in some module to prevent them from being edited.
+
+### BDM Velocity
+
+A boosted dark matter (BDM) with mass $m_\chi$ and kinetic energy $T_\chi$ has the velocity $v_\chi$,
+
+$$
+\frac{v_\chi}{c} = \frac{\sqrt{T_\chi(2m_\chi+T_\chi)}}{m_\chi+T_\chi}.
+$$
+
+Let $(T_\chi,m_\chi)=(15,0.075)$ MeV, we can use
+`snorer.get_vx()` to evaluate
+
+    >>> Tx,mx = 15,0.075
+    >>> snorer.get_vx(Tx,mx)
+    0.9999876239921284
+
+
+### SN*ν* BDM Flux 
+
+The BDM flux, or *afterglow* to the ${\rm SN}\nu$, due to SN that is $R_\star$ distant away from us can be evaluated by 
+
+$$
+\frac{d\Phi_{\chi}(T_\chi, t^\prime)}{dT_{\chi}dt} =
+\tau\int_0^{2\pi} d\phi\int_{0}^{\pi/2}\sin\theta d\theta~ \mathcal{J} j_{\chi}(r(\phi),D,T_{\chi},\psi)
+$$
+
+where $t$ is the BDM ToF with time-zero at the discovery of SN*ν* on Earth and $t^\prime$ is the total time. We focus on $t$ instead of $t^\prime$.
+Zenith angle $\theta$ and azimuthal angle $\phi$ are relative to the SN-Earth line-of-sight. The default DM-*ν* cross section is $\sigma_{\chi\nu}=10^{-45}$ cm<sup>2</sup>.
+
+The function to evaluate this flux is `snorer.flux()` with $(t,T_\chi,m_\chi,R_\star,\beta)$ are the necessary inputs. 
+Suppose SN's location is at GC, we have $R_\star=8.5$ kpc and $\beta=0$, and examine the flux with turning on DM spike feature
+
+    >>> t,Tx,mx,Rstar,beta = 100,15,1e-2,8.5,0
+    >>> snorer.flux(t,Tx,mx,Rstar,beta,neval=15000)
+    4.572295175982701e-16
+
+Users can turn off the spike feature by inserting `is_spike=False` and will find both numerical results are similar. It implies the contribution to the BDM flux is due to the place outside the spike's influencial region.
+
+### SN*ν* BDM Event
+
+The BDM event number in a detector after exposing to the flux for a period of time, $(t_{\rm min},t_{\rm max})$, can be evaluated by
+
+$$
+N_{\rm BDM} = \int_{t_{\rm min}}^{\rm t_{\rm max}} dt \int_{T_{\chi,{\rm min}}}^{T_{\chi,{\rm max}}}
+\frac{d\Phi_{\chi}(T_\chi, t^\prime)}{dT_{\chi}dt} \times N_e \sigma_{\chi e}
+$$
+
+where $N_e$ is the total electron number in the detector and $\sigma_{\chi e}$ the DM-*e* cross section.
+This can be accomplished by `snorer.event()` with $(m_\chi,R_\star,\beta)$ the necessary inputs.
+The default $(t_{\rm min},t_{\rm max})=(10~{\rm s},35~{\rm yrs})$ and $(T_{\chi,{\rm min}},T_{\chi,{\rm max}})=(5,30)$ MeV.
+
+Note that this function is normalized to $N_e=1$ and $\sigma_{\chi e}=1$ cm<sup>2</sup>.
+To have the correct $N_{\rm BDM}$ in a specific detector, users have to mutiply the corresponding $N_e$ and $\sigma_{\chi e}$.
+
+Now let $m_\chi=0.015$ MeV,
+
+    >>> mx,Rstar,beta = 0.015,8,0
+    >>> N_BDM = snorer.event(mx,Rstar,beta,is_spike=False,neval=50000)
+    >>> N_BDM
+    1.662174035857532e-06
+
+Suppose it happened in Super-Kamiokande with $N_e\approx 7\times 10^{33}$ and assume $\sigma_{\chi e}=10^{-30}$ cm<sup>2</sup>. The correct $N_{\rm BDM}$ would be
+
+    >>> Ne,sigma_xe = 7e33,1e-35
+    >>> N_BDM*Ne*sigma_xe
+    1.1635218251002724e-07
+
+### *Experimental* :: Implementation of Particle Physics Model and SN in Arbitrary Distant Galaxy
+
+The aforementioned functions for evaluating BDM signatures are based on model-agnostic picture. It means the cross sections between dark and visble sectors are generally independent of any physical quantities, eg. energy, mass and coupling constants.
+
+The most important feature of `snorer` is that it offers a general interface for users to implement their favorite particle models.
+Furthermore, SN is not necessary residing in MW or LMC. As long as users can provide these celetial objects' coordinates expressed in *ICRS J2000.0* system, `snorer` can do the calculation.
+`snorer` also allows users to customize the halo shape, by manipulating $\rho_s$, $r_s$ and $n$...etc, and including or excluding spike feature, of such distant galaxy.
+
+This will be done by introducing a *class* `snorer.GeneralInterface`.
+All these user-specified features will compose an instance of `snorer.GeneralInterface`.
+The BDM signatures can be evaluated by calling the associated *methods* within it.
+We have an example in `examples/tutorial.ipynb`, also see the in-class docstring for more information.
+
+
+### Other Useful Functions Classes
+
+We also provide many useful functions and classes at users' disposal. See `examples/tutorial.ipynb` for details.
+
+## Known Issue
+
+To evaluate BDM event, `snorer` uses `vegas` to handle the multidimensional integration.
+The sampling method of `vegas` cannot manipulate`snorer.event()` as well as the method in the instance of `snorer.GeneralInterface` properly, when SN is exactly at GC with spike feature turning on and no DM self-annihilation.
 
-where `vegas` is a the backend engine for evaluating multidimensional integrals based on adaptive Monte Carlo vegas algorithm, see its homepage: [https://pypi.org/project/vegas/](https://pypi.org/project/vegas/).
+Since the spike is a highly singular behavior, the sampling method may miss the substantial DM contribution from the inner galactic region and causes underestimate of $N_{\rm BDM}$ plus unstable results. 
+To avoid this, users may try to displace the SN from GC when evaluating $N_{\rm BDM}$ whith DM sipke turning on and no DM annihilation.
+For BDM flux evaluation, there is no such issue.
 
-Other packages, e.g. `gvar`, maybe required by these dependencies during the installation.
-The versions of these dependencies are not strict, but are recommended to update to the latest ones to avoid incompatibility. 
+To be fair, the probability of a very cuspy DM spike surving the gravitational disturbance without annihilating away and SN happening exactly at the GC might be very rare.
 
+This issue is scheduled to fix in the next version of `snorer`.
 
+## Bugs and troubleshooting
 
-## Misc
+Please report to the author, Yen-Hsun Lin, via [yenhsun@phys.ncku.edu.tw](mailto:yenhsun@phys.ncku.edu.tw).
 
-Bug report and troubleshooting please contact the author Yen-Hsun Lin via [yenhsun@phys.ncku.edu.tw](mailto:yenhsun@phys.ncku.edu.tw).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

