# Comparing `tmp/lielab-0.1.1-cp39-none-win_amd64.whl.zip` & `tmp/lielab-0.1.2-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 504543 bytes, number of entries: 18
--rw-rw-rw-  2.0 fat      321 b- defN 24-Feb-25 17:19 lielab/__init__.py
--rw-rw-rw-  2.0 fat  1337856 b- defN 24-Feb-25 17:54 lielab/cppLielab.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat       69 b- defN 24-Feb-24 20:26 lielab/domain/__init__.py
--rw-rw-rw-  2.0 fat        6 b- defN 23-Mar-08 21:02 lielab/domain/domain.py
--rw-rw-rw-  2.0 fat       36 b- defN 24-Feb-24 20:26 lielab/dynamics/__init__.py
--rw-rw-rw-  2.0 fat       37 b- defN 24-Feb-24 20:26 lielab/functions/__init__.py
--rw-rw-rw-  2.0 fat       53 b- defN 24-Feb-24 20:26 lielab/kinematics/__init__.py
--rw-rw-rw-  2.0 fat       40 b- defN 23-Mar-08 21:02 lielab/optim/__init__.py
--rw-rw-rw-  2.0 fat     1493 b- defN 24-Feb-24 20:26 lielab/optim/optim.py
--rw-rw-rw-  2.0 fat       26 b- defN 23-Mar-08 21:02 lielab/testing/__init__.py
--rw-rw-rw-  2.0 fat     1121 b- defN 23-Mar-08 21:02 lielab/testing/test_main.py
--rw-rw-rw-  2.0 fat      299 b- defN 24-Feb-24 20:26 lielab/topos/__init__.py
--rw-rw-rw-  2.0 fat     7139 b- defN 24-Feb-24 20:26 lielab/topos/topos.py
--rw-rw-rw-  2.0 fat       52 b- defN 24-Feb-24 20:26 lielab/transform/__init__.py
--rw-rw-rw-  2.0 fat      426 b- defN 24-Feb-25 18:14 lielab-0.1.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       99 b- defN 24-Feb-25 18:14 lielab-0.1.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 24-Feb-25 18:14 lielab-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     2003 b- defN 24-Feb-25 18:14 lielab-0.1.1.dist-info/RECORD
-18 files, 1351083 bytes uncompressed, 502193 bytes compressed:  62.8%
+Zip file size: 549922 bytes, number of entries: 18
+-rw-r--r--  2.0 unx      298 b- defN 24-Apr-30 20:05 lielab/__init__.py
+-rwxr-xr-x  2.0 unx  1507264 b- defN 24-Apr-30 20:36 lielab/cppLielab.cpython-310-x86_64-linux-gnu.so
+-rw-r--r--  2.0 unx       65 b- defN 24-Apr-30 17:04 lielab/domain/__init__.py
+-rw-r--r--  2.0 unx        5 b- defN 24-Apr-30 17:04 lielab/domain/domain.py
+-rw-r--r--  2.0 unx       35 b- defN 24-Apr-30 17:04 lielab/dynamics/__init__.py
+-rw-r--r--  2.0 unx       36 b- defN 24-Apr-30 17:04 lielab/functions/__init__.py
+-rw-r--r--  2.0 unx       51 b- defN 24-Apr-30 17:04 lielab/kinematics/__init__.py
+-rw-r--r--  2.0 unx       39 b- defN 24-Apr-30 17:04 lielab/optim/__init__.py
+-rw-r--r--  2.0 unx     1438 b- defN 24-Apr-30 17:04 lielab/optim/optim.py
+-rw-r--r--  2.0 unx       25 b- defN 24-Apr-30 17:04 lielab/testing/__init__.py
+-rw-r--r--  2.0 unx     1075 b- defN 24-Apr-30 17:04 lielab/testing/test_main.py
+-rw-r--r--  2.0 unx      290 b- defN 24-Apr-30 17:04 lielab/topos/__init__.py
+-rw-r--r--  2.0 unx     6921 b- defN 24-Apr-30 20:05 lielab/topos/topos.py
+-rw-r--r--  2.0 unx       50 b- defN 24-Apr-30 17:04 lielab/transform/__init__.py
+-rw-r--r--  2.0 unx      412 b- defN 24-Apr-30 20:36 lielab-0.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 24-Apr-30 20:36 lielab-0.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 24-Apr-30 20:36 lielab-0.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1444 b- defN 24-Apr-30 20:36 lielab-0.1.2.dist-info/RECORD
+18 files, 1519563 bytes uncompressed, 547546 bytes compressed:  64.0%
```

## zipnote {}

```diff
@@ -1,11 +1,11 @@
 Filename: lielab/__init__.py
 Comment: 
 
-Filename: lielab/cppLielab.cp39-win_amd64.pyd
+Filename: lielab/cppLielab.cpython-310-x86_64-linux-gnu.so
 Comment: 
 
 Filename: lielab/domain/__init__.py
 Comment: 
 
 Filename: lielab/domain/domain.py
 Comment: 
@@ -36,20 +36,20 @@
 
 Filename: lielab/topos/topos.py
 Comment: 
 
 Filename: lielab/transform/__init__.py
 Comment: 
 
-Filename: lielab-0.1.1.dist-info/METADATA
+Filename: lielab-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: lielab-0.1.1.dist-info/WHEEL
+Filename: lielab-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: lielab-0.1.1.dist-info/top_level.txt
+Filename: lielab-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: lielab-0.1.1.dist-info/RECORD
+Filename: lielab-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## lielab/__init__.py

```diff
@@ -1,12 +1,13 @@
-from lielab.cppLielab import ALGO_STATUS
-from lielab.cppLielab import __author__, __contact__, __location__, __version__
-
-from . import testing
-
-from .domain import *
-from .dynamics import *
-from .functions import *
-from .kinematics import *
-from .optim import *
-from .topos import *
-from .transform import *
+from .cppLielab import ALGO_STATUS
+
+from .cppLielab import __author__, __contact__, __location__, __version__
+
+from . import testing
+
+from .domain import *
+from .dynamics import *
+from .functions import *
+from .kinematics import *
+from .optim import *
+from .topos import *
+from .transform import *
```

## lielab/domain/__init__.py

 * *Ordering differences only*

```diff
@@ -1,4 +1,4 @@
-# C++ imports
-from ..cppLielab.domain import *
-
-# Python imports
+# C++ imports
+from ..cppLielab.domain import *
+
+# Python imports
```

## lielab/domain/domain.py

 * *Ordering differences only*

```diff
@@ -1 +1 @@
-pass
+pass
```

## lielab/dynamics/__init__.py

 * *Ordering differences only*

```diff
@@ -1 +1 @@
-from ..cppLielab.dynamics import *
+from ..cppLielab.dynamics import *
```

## lielab/functions/__init__.py

 * *Ordering differences only*

```diff
@@ -1 +1 @@
-from ..cppLielab.functions import *
+from ..cppLielab.functions import *
```

## lielab/kinematics/__init__.py

 * *Ordering differences only*

```diff
@@ -1,2 +1,2 @@
-# C++ imports
-from ..cppLielab.kinematics import *
+# C++ imports
+from ..cppLielab.kinematics import *
```

## lielab/optim/__init__.py

 * *Ordering differences only*

```diff
@@ -1 +1 @@
-from .optim import opt_golden, hnewton
+from .optim import opt_golden, hnewton
```

## lielab/optim/optim.py

 * *Ordering differences only*

```diff
@@ -1,55 +1,55 @@
-from ..cppLielab.optim import opt_golden as _opt_golden
-from ..cppLielab.optim import hnewton as _hnewton
-from lielab import ALGO_STATUS
-import numpy as np
-
-class opt_golden(_opt_golden):
-    def __call__(self, function):
-        self.init()
-
-        while (self.algo_status == ALGO_STATUS.OK):
-            self._f1 = function(self._X1)
-            self.num_objective_evals += 1
-
-            self._f2 = function(self._X2)
-            self.num_objective_evals += 1
-            self.step()
-        
-        self._f1 = function(self._X1)
-        self.num_objective_evals += 1
-
-        self._f2 = function(self._X2)
-        self.num_objective_evals += 1
-
-        if (self._f1 < self._f2):
-            self.val_objective = self._f1
-            self._X = self._X1
-        else:
-            self.val_objective = self._f2
-            self._X = self._X2
-
-        return self._X
-
-class hnewton(_hnewton):
-    def __call__(self, fun, m0):
-        self.init(m0, fun(m0))
-
-        while (self.algo_status == ALGO_STATUS.OK):
-            self.step0()
-            self.fnext = fun(self.mnext)
-            self.step1()
-            self.fnext = fun(self.mnext)
-
-        self.m = self.mnext
-
-        return self.m
-
-# class search_linearx(_search_linearx):
-#     def __call__(self, function, x0):
-#         self.init(x0)
-#         x = x0
-
-#         while (self.algo_status == ALGO_STATUS.OK):
-#             x = self.step(x, function(x))
-
-#         return x
+from ..cppLielab.optim import opt_golden as _opt_golden
+from ..cppLielab.optim import hnewton as _hnewton
+from lielab import ALGO_STATUS
+import numpy as np
+
+class opt_golden(_opt_golden):
+    def __call__(self, function):
+        self.init()
+
+        while (self.algo_status == ALGO_STATUS.OK):
+            self._f1 = function(self._X1)
+            self.num_objective_evals += 1
+
+            self._f2 = function(self._X2)
+            self.num_objective_evals += 1
+            self.step()
+        
+        self._f1 = function(self._X1)
+        self.num_objective_evals += 1
+
+        self._f2 = function(self._X2)
+        self.num_objective_evals += 1
+
+        if (self._f1 < self._f2):
+            self.val_objective = self._f1
+            self._X = self._X1
+        else:
+            self.val_objective = self._f2
+            self._X = self._X2
+
+        return self._X
+
+class hnewton(_hnewton):
+    def __call__(self, fun, m0):
+        self.init(m0, fun(m0))
+
+        while (self.algo_status == ALGO_STATUS.OK):
+            self.step0()
+            self.fnext = fun(self.mnext)
+            self.step1()
+            self.fnext = fun(self.mnext)
+
+        self.m = self.mnext
+
+        return self.m
+
+# class search_linearx(_search_linearx):
+#     def __call__(self, function, x0):
+#         self.init(x0)
+#         x = x0
+
+#         while (self.algo_status == ALGO_STATUS.OK):
+#             x = self.step(x, function(x))
+
+#         return x
```

## lielab/testing/__init__.py

 * *Ordering differences only*

```diff
@@ -1 +1 @@
-from .test_main import *
+from .test_main import *
```

## lielab/testing/test_main.py

 * *Ordering differences only*

```diff
@@ -1,46 +1,46 @@
-import numpy as np
-
-TOL_FINE = 1e-6
-TOL_COARSE = 1e-3
-
-an_int = int(2)
-a_double = float(2)
-an_imag_int = 2j # TODO: I think this is actually just a double
-an_imag_double = 2.0j
-
-def assert_matrix(mat1: np.ndarray, mat2: np.ndarray) -> None:
-    if isinstance(mat1, np.ndarray):
-        pass
-    else:
-        mat1 = mat1.get_ados_representation()
-
-    r1 = mat1.shape[0]
-    if len(mat1.shape) == 1:
-        c1 = 0
-    else:
-        c1 = mat1.shape[1]
-    
-    if isinstance(mat2, np.ndarray):
-        pass
-    else:
-        mat2 = mat2.get_ados_representation()
-    
-    r2 = mat2.shape[0]
-    if len(mat2.shape) == 1:
-        c2 = 0
-    else:
-        c2 = mat2.shape[1]
-    
-    assert r1 == r2
-    assert c1 == c2
-
-    if (c1 != 0 and c2 != 0):
-        for ii in range(r1):
-            for jj in range(c1):
-                assert abs(mat1[ii,jj] - mat2[ii,jj]) < TOL_FINE
-    else:
-        for ii in range(r1):
-            assert abs(mat1[ii] - mat2[ii]) < TOL_FINE
-
-def assert_domain(d1, d2):
-    assert_matrix(d1.get_ados_representation(), d2.get_ados_representation())
+import numpy as np
+
+TOL_FINE = 1e-6
+TOL_COARSE = 1e-3
+
+an_int = int(2)
+a_double = float(2)
+an_imag_int = 2j # TODO: I think this is actually just a double
+an_imag_double = 2.0j
+
+def assert_matrix(mat1: np.ndarray, mat2: np.ndarray) -> None:
+    if isinstance(mat1, np.ndarray):
+        pass
+    else:
+        mat1 = mat1.get_ados_representation()
+
+    r1 = mat1.shape[0]
+    if len(mat1.shape) == 1:
+        c1 = 0
+    else:
+        c1 = mat1.shape[1]
+    
+    if isinstance(mat2, np.ndarray):
+        pass
+    else:
+        mat2 = mat2.get_ados_representation()
+    
+    r2 = mat2.shape[0]
+    if len(mat2.shape) == 1:
+        c2 = 0
+    else:
+        c2 = mat2.shape[1]
+    
+    assert r1 == r2
+    assert c1 == c2
+
+    if (c1 != 0 and c2 != 0):
+        for ii in range(r1):
+            for jj in range(c1):
+                assert abs(mat1[ii,jj] - mat2[ii,jj]) < TOL_FINE
+    else:
+        for ii in range(r1):
+            assert abs(mat1[ii] - mat2[ii]) < TOL_FINE
+
+def assert_domain(d1, d2):
+    assert_matrix(d1.get_ados_representation(), d2.get_ados_representation())
```

## lielab/topos/__init__.py

 * *Ordering differences only*

```diff
@@ -1,9 +1,9 @@
-# Need to list every function and class to prevent collisions
-# C++ Imports
-from ..cppLielab.topos import Ad, dexp, dexpinv, exp, log
-from ..cppLielab.topos import RKMETHOD
-from ..cppLielab.topos import IntegralCurve
-
-# Python imports
-from .topos import MuntheKaas, Flow, CustomMuntheKaas
-
+# Need to list every function and class to prevent collisions
+# C++ Imports
+from ..cppLielab.topos import Ad, dexp, dexpinv, exp, log
+from ..cppLielab.topos import RKMETHOD
+from ..cppLielab.topos import IntegralCurve
+
+# Python imports
+from .topos import MuntheKaas, Flow, CustomMuntheKaas
+
```

## lielab/topos/topos.py

 * *Ordering differences only*

```diff
@@ -1,218 +1,218 @@
-from lielab import ALGO_STATUS
-from lielab.domain import halie, hmlie
-from lielab.topos import IntegralCurve
-from lielab.cppLielab.topos import Flow as _Flow
-from lielab.cppLielab.topos import MuntheKaas as _MuntheKaas
-from lielab.cppLielab.topos import TimeStepper as _TimeStepper
-from lielab.cppLielab.topos import TSOutput
-import numpy as np
-
-# Import hnewton as a python object
-from lielab.optim import hnewton
-
-class MuntheKaas(_MuntheKaas):
-    """
-    MuntheKaas integrator that maximizes time spent in C++
-    for performance.
-    """
-    
-    def __call__(self, vectorfield, y0, t0, dt):
-        self.init(t0, y0, dt, vectorfield(t0, y0))
-
-        while (self.algo_status == ALGO_STATUS.OK):
-            self.step_0()
-            self.set_dy(vectorfield(self.next_t, self.next_y))
-            self.step_1()
-
-        return self.postprocess()
-
-
-class CustomMuntheKaas(_TimeStepper):
-    """
-    MuntheKaas integrator with customizable actions.
-    """
-
-    def __init__(self, *args, **kwargs):
-        """
-        Instantiates a new MuntheKaas object.
-        """
-
-        super(CustomMuntheKaas, self).__init__(*args, **kwargs)
-
-        from lielab.functions import left_exp_default
-        from lielab.topos import dexpinv
-        # self.RKT = RKTYPE::RKTYPE_EXPLICIT; # TODO:
-
-        self.left = left_exp_default
-        self.dphiinv = dexpinv
-
-        self._t0 = None
-        self._y0 = None
-        self._dt = None
-
-        self.next_t = None
-        self.next_y = None
-
-        self._dy = None
-        self._U = None
-        self._KK = None
-
-    def init(self, t0, y0, dt, dy0):
-        """
-        Initializes the MuntheKaas process.
-        """
-        
-        super(CustomMuntheKaas, self).init()
-
-        self._t0 = t0
-        self._y0 = y0
-        self._dt = dt
-        self._KK = [halie()]*self.n
-        self._KK[0] = dy0
-        self._dy = dy0
-        self._U = 0*dy0
-
-        if (self.iterations >= self.n - 1):
-            self.algo_status = ALGO_STATUS.FINISHED
-        
-    def step_0(self):
-        """
-        Advances the solution to current iteration and returns pair
-        (next_t, next_y) to be evaluated by the vectorfield.
-        """
-
-        self._U *= 0
-
-        for jj in range(self.iterations + 1):
-            self._U += self._dt*self.A[self.iterations+1, jj]*self._KK[jj]
-        
-        self.next_y = self.left(self._U, self._y0)
-        self.next_t = self._t0 + self._dt*self.C[self.iterations + 1]
-    
-    def set_dy(self, dy):
-        """
-        Sets the current vectorfield value. Do this after step_0()
-        and before step_1().
-        """
-
-        self._dy = dy
-
-    def step_1(self):
-        """
-        Evaluates the $ d phi^{-1} u ( xi(s,y)) $ map.
-        """
-
-        self._KK[self.iterations + 1] = self.dphiinv(self._U, self._dy, self.n - 1)
-
-        super(CustomMuntheKaas, self).step()
-
-        if (self.iterations == self.n - 1):
-            self.algo_status = ALGO_STATUS.FINISHED
-    
-    def postprocess(self):
-        Ulow = 0*self._KK[0]
-        Uhigh = 0*self._KK[0]
-
-        for ii in range(self.n):
-            Ulow += self._dt*self.B[ii]*self._KK[ii]
-
-        low = self.left(Ulow, self._y0)
-
-        if self.variable_step:
-            for ii in range(self.n):
-                Uhigh += self._dt*self.Bhat[ii]*self._KK[ii]
-            
-            high = self.left(Uhigh, self._y0)
-            error = np.linalg.norm(Uhigh.get_vector() - Ulow.get_vector())
-            return TSOutput(low, high, error)
-        
-        return TSOutput(low)
-    
-    def __call__(self, vectorfield, y0, t0, dt):
-        self.init(t0, y0, dt, vectorfield(t0, y0))
-
-        while (self.algo_status == ALGO_STATUS.OK):
-            self.step_0()
-            self.set_dy(vectorfield(self.next_t, self.next_y))
-            self.step_1()
-        
-        return self.postprocess()
-
-
-class Flow(_Flow):
-    search = hnewton()
-    stepper = MuntheKaas()
-
-    def __call__(self, vectorfield, tspan, y0, *args):
-        from lielab.domain import rn, RN, halie, hmlie
-
-        # Check if the solution we're running has an event
-        has_event = False
-        if len(args) > 0:
-            has_event = True
-            event = args[0]
-        
-        # Check the type of inputs
-        dy0 = vectorfield(tspan[0], y0)
-
-        if isinstance(dy0, np.ndarray) or isinstance(dy0, list):
-            # NumPy and list type inputs, we need to wrap these in
-            # sophus objects
-            _y0 = hmlie([RN(y0)])
-            def _vectorfield(_t, M):
-                _RN = M.space[0]
-                _states = _RN.serialize()
-                gradient = vectorfield(_t, _states)
-                dx = rn(gradient)
-                return halie([dx])
-            
-            if has_event:
-                def _event(_t, M):
-                    _RN = M.space[0]
-                    _states = _RN.serialize()
-                    return event(_t, _states)
-        else:
-            # Assume these are sophus type inputs and
-            # don't need to be wrapped
-            _y0 = y0
-            _vectorfield = vectorfield
-            if has_event:
-                _event = event
-        
-        # Initialize the Flow object
-        self.init(tspan, _y0)
-
-        # Main loop. Run until algorithm says it's done
-        while (self.algo_status == ALGO_STATUS.OK):
-            accepted = False
-
-            # This is the RK loop. It's the error control loop that will
-            # change step size until we have an acceptable step
-            while (not accepted):
-                next = self.stepper(_vectorfield, self._ynext, self._out.t[self.iterations], self._dt)
-                if has_event:
-                    if _event(self._out.t[self.iterations], self._ynext) > 0 and _event(self._out.t[self.iterations] + self._dt, next.high) <= 0:
-                        self.search.lower = halie([rn([self.tol])])
-                        self.search.upper = halie([rn([self._dt])])
-
-                        def sfun(sdt):
-                            _sdt = sdt.space[0](0)
-                            return _event(self._out.t[self.iterations] + _sdt, self.stepper(_vectorfield, self._ynext, self._out.t[self.iterations], _sdt).high)
-
-                        temp_dt = self.search(sfun, halie([rn([self._dt/2])]))
-                        self._dt = temp_dt.space[0](0)
-                        next = self.stepper(_vectorfield, self._ynext, self._out.t[self.iterations], self._dt)
-
-                accepted = self.step0(next)
-            
-            # We have an acceptable step at this point. Step the solution forward by one
-            self.step()
-
-            # If there's an event, check to see if conditions are met
-            # This will stop integration if an event returns <= 0
-            if has_event:
-                self.stepE(_event(self._out.t[self.iterations], self._ynext))
-        
-        self.postprocess()
-        
-        return IntegralCurve(self._out)
+from lielab import ALGO_STATUS
+from lielab.domain import halie, hmlie
+from lielab.topos import IntegralCurve
+from lielab.cppLielab.topos import Flow as _Flow
+from lielab.cppLielab.topos import MuntheKaas as _MuntheKaas
+from lielab.cppLielab.topos import TimeStepper as _TimeStepper
+from lielab.cppLielab.topos import TSOutput
+import numpy as np
+
+# Import hnewton as a python object
+from lielab.optim import hnewton
+
+class MuntheKaas(_MuntheKaas):
+    """
+    MuntheKaas integrator that maximizes time spent in C++
+    for performance.
+    """
+    
+    def __call__(self, vectorfield, y0, t0, dt):
+        self.init(t0, y0, dt, vectorfield(t0, y0))
+
+        while (self.algo_status == ALGO_STATUS.OK):
+            self.step_0()
+            self.set_dy(vectorfield(self.next_t, self.next_y))
+            self.step_1()
+
+        return self.postprocess()
+
+
+class CustomMuntheKaas(_TimeStepper):
+    """
+    MuntheKaas integrator with customizable actions.
+    """
+
+    def __init__(self, *args, **kwargs):
+        """
+        Instantiates a new MuntheKaas object.
+        """
+
+        super(CustomMuntheKaas, self).__init__(*args, **kwargs)
+
+        from lielab.functions import left_exp_default
+        from lielab.topos import dexpinv
+        # self.RKT = RKTYPE::RKTYPE_EXPLICIT; # TODO:
+
+        self.left = left_exp_default
+        self.dphiinv = dexpinv
+
+        self._t0 = None
+        self._y0 = None
+        self._dt = None
+
+        self.next_t = None
+        self.next_y = None
+
+        self._dy = None
+        self._U = None
+        self._KK = None
+
+    def init(self, t0, y0, dt, dy0):
+        """
+        Initializes the MuntheKaas process.
+        """
+        
+        super(CustomMuntheKaas, self).init()
+
+        self._t0 = t0
+        self._y0 = y0
+        self._dt = dt
+        self._KK = [halie()]*self.n
+        self._KK[0] = dy0
+        self._dy = dy0
+        self._U = 0*dy0
+
+        if (self.iterations >= self.n - 1):
+            self.algo_status = ALGO_STATUS.FINISHED
+        
+    def step_0(self):
+        """
+        Advances the solution to current iteration and returns pair
+        (next_t, next_y) to be evaluated by the vectorfield.
+        """
+
+        self._U *= 0
+
+        for jj in range(self.iterations + 1):
+            self._U += self._dt*self.A[self.iterations+1, jj]*self._KK[jj]
+        
+        self.next_y = self.left(self._U, self._y0)
+        self.next_t = self._t0 + self._dt*self.C[self.iterations + 1]
+    
+    def set_dy(self, dy):
+        """
+        Sets the current vectorfield value. Do this after step_0()
+        and before step_1().
+        """
+
+        self._dy = dy
+
+    def step_1(self):
+        """
+        Evaluates the $ d phi^{-1} u ( xi(s,y)) $ map.
+        """
+
+        self._KK[self.iterations + 1] = self.dphiinv(self._U, self._dy, self.n - 1)
+
+        super(CustomMuntheKaas, self).step()
+
+        if (self.iterations == self.n - 1):
+            self.algo_status = ALGO_STATUS.FINISHED
+    
+    def postprocess(self):
+        Ulow = 0*self._KK[0]
+        Uhigh = 0*self._KK[0]
+
+        for ii in range(self.n):
+            Ulow += self._dt*self.B[ii]*self._KK[ii]
+
+        low = self.left(Ulow, self._y0)
+
+        if self.variable_step:
+            for ii in range(self.n):
+                Uhigh += self._dt*self.Bhat[ii]*self._KK[ii]
+            
+            high = self.left(Uhigh, self._y0)
+            error = np.linalg.norm(Uhigh.get_vector() - Ulow.get_vector())
+            return TSOutput(low, high, error)
+        
+        return TSOutput(low)
+    
+    def __call__(self, vectorfield, y0, t0, dt):
+        self.init(t0, y0, dt, vectorfield(t0, y0))
+
+        while (self.algo_status == ALGO_STATUS.OK):
+            self.step_0()
+            self.set_dy(vectorfield(self.next_t, self.next_y))
+            self.step_1()
+        
+        return self.postprocess()
+
+
+class Flow(_Flow):
+    search = hnewton()
+    stepper = MuntheKaas()
+
+    def __call__(self, vectorfield, tspan, y0, *args):
+        from lielab.domain import rn, RN, halie, hmlie
+
+        # Check if the solution we're running has an event
+        has_event = False
+        if len(args) > 0:
+            has_event = True
+            event = args[0]
+        
+        # Check the type of inputs
+        dy0 = vectorfield(tspan[0], y0)
+
+        if isinstance(dy0, np.ndarray) or isinstance(dy0, list):
+            # NumPy and list type inputs, we need to wrap these in
+            # sophus objects
+            _y0 = hmlie([RN(y0)])
+            def _vectorfield(_t, M):
+                _RN = M.space[0]
+                _states = _RN.serialize()
+                gradient = vectorfield(_t, _states)
+                dx = rn(gradient)
+                return halie([dx])
+            
+            if has_event:
+                def _event(_t, M):
+                    _RN = M.space[0]
+                    _states = _RN.serialize()
+                    return event(_t, _states)
+        else:
+            # Assume these are sophus type inputs and
+            # don't need to be wrapped
+            _y0 = y0
+            _vectorfield = vectorfield
+            if has_event:
+                _event = event
+        
+        # Initialize the Flow object
+        self.init(tspan, _y0)
+
+        # Main loop. Run until algorithm says it's done
+        while (self.algo_status == ALGO_STATUS.OK):
+            accepted = False
+
+            # This is the RK loop. It's the error control loop that will
+            # change step size until we have an acceptable step
+            while (not accepted):
+                next = self.stepper(_vectorfield, self._ynext, self._out.t[self.iterations], self._dt)
+                if has_event:
+                    if _event(self._out.t[self.iterations], self._ynext) > 0 and _event(self._out.t[self.iterations] + self._dt, next.high) <= 0:
+                        self.search.lower = halie([rn([self.tol])])
+                        self.search.upper = halie([rn([self._dt])])
+
+                        def sfun(sdt):
+                            _sdt = sdt.space[0](0)
+                            return _event(self._out.t[self.iterations] + _sdt, self.stepper(_vectorfield, self._ynext, self._out.t[self.iterations], _sdt).high)
+
+                        temp_dt = self.search(sfun, halie([rn([self._dt/2])]))
+                        self._dt = temp_dt.space[0](0)
+                        next = self.stepper(_vectorfield, self._ynext, self._out.t[self.iterations], self._dt)
+
+                accepted = self.step0(next)
+            
+            # We have an acceptable step at this point. Step the solution forward by one
+            self.step()
+
+            # If there's an event, check to see if conditions are met
+            # This will stop integration if an event returns <= 0
+            if has_event:
+                self.stepE(_event(self._out.t[self.iterations], self._ynext))
+        
+        self.postprocess()
+        
+        return IntegralCurve(self._out)
```

## lielab/transform/__init__.py

 * *Ordering differences only*

```diff
@@ -1,2 +1,2 @@
-# C++ imports
-from ..cppLielab.transform import *
+# C++ imports
+from ..cppLielab.transform import *
```

