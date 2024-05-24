# Comparing `tmp/pidgey-0.2.4.tar.gz` & `tmp/pidgey-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pidgey-0.2.4.tar", last modified: Mon Jan 22 04:31:53 2024, max compression
+gzip compressed data, was "pidgey-1.0.0.tar", last modified: Fri May 24 19:52:51 2024, max compression
```

## Comparing `pidgey-0.2.4.tar` & `pidgey-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1073 2024-01-22 04:31:41.887827 pidgey-0.2.4/LICENSE
--rw-r--r--   0        0        0     1951 2024-01-22 04:31:41.887827 pidgey-0.2.4/README.md
--rw-r--r--   0        0        0     1069 2024-01-22 04:31:53.267809 pidgey-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      634 2024-01-22 04:31:41.887827 pidgey-0.2.4/src/pidgey/__init__.py
--rw-r--r--   0        0        0     1296 2024-01-22 04:31:41.887827 pidgey-0.2.4/src/pidgey/agama_backend.py
--rw-r--r--   0        0        0     1907 2024-01-22 04:31:41.891827 pidgey-0.2.4/src/pidgey/base.py
--rw-r--r--   0        0        0      857 2024-01-22 04:31:41.891827 pidgey-0.2.4/src/pidgey/gala_backend.py
--rw-r--r--   0        0        0     1111 2024-01-22 04:31:41.891827 pidgey-0.2.4/src/pidgey/galpy_backend.py
--rw-r--r--   0        0        0        0 2024-01-22 04:31:41.891827 pidgey-0.2.4/tests/__init__.py
--rw-r--r--   0        0        0     1699 2024-01-22 04:31:41.891827 pidgey-0.2.4/tests/gala_env.yml
--rw-r--r--   0        0        0     2771 2024-01-22 04:31:41.891827 pidgey-0.2.4/tests/galpy_env.yml
--rw-r--r--   0        0        0     2056 2024-01-22 04:31:41.891827 pidgey-0.2.4/tests/test_agama.py
--rw-r--r--   0        0        0     1935 2024-01-22 04:31:41.891827 pidgey-0.2.4/tests/test_gala.py
--rw-r--r--   0        0        0     1820 2024-01-22 04:31:41.891827 pidgey-0.2.4/tests/test_galpy.py
--rw-r--r--   0        0        0     2850 1970-01-01 00:00:00.000000 pidgey-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-24 19:52:38.373597 pidgey-1.0.0/LICENSE
+-rw-r--r--   0        0        0     4444 2024-05-24 19:52:38.373597 pidgey-1.0.0/README.md
+-rw-r--r--   0        0        0     1064 2024-05-24 19:52:51.313699 pidgey-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      634 2024-05-24 19:52:38.373597 pidgey-1.0.0/src/pidgey/__init__.py
+-rw-r--r--   0        0        0     1449 2024-05-24 19:52:38.373597 pidgey-1.0.0/src/pidgey/agama_backend.py
+-rw-r--r--   0        0        0     1916 2024-05-24 19:52:38.373597 pidgey-1.0.0/src/pidgey/base.py
+-rw-r--r--   0        0        0     1024 2024-05-24 19:52:38.373597 pidgey-1.0.0/src/pidgey/gala_backend.py
+-rw-r--r--   0        0        0     1111 2024-05-24 19:52:38.373597 pidgey-1.0.0/src/pidgey/galpy_backend.py
+-rw-r--r--   0        0        0        0 2024-05-24 19:52:38.373597 pidgey-1.0.0/tests/__init__.py
+-rw-r--r--   0        0        0     1699 2024-05-24 19:52:38.373597 pidgey-1.0.0/tests/gala_env.yml
+-rw-r--r--   0        0        0     2771 2024-05-24 19:52:38.373597 pidgey-1.0.0/tests/galpy_env.yml
+-rw-r--r--   0        0        0     2056 2024-05-24 19:52:38.373597 pidgey-1.0.0/tests/test_agama.py
+-rw-r--r--   0        0        0     1935 2024-05-24 19:52:38.373597 pidgey-1.0.0/tests/test_gala.py
+-rw-r--r--   0        0        0     1820 2024-05-24 19:52:38.373597 pidgey-1.0.0/tests/test_galpy.py
+-rw-r--r--   0        0        0     5343 1970-01-01 00:00:00.000000 pidgey-1.0.0/PKG-INFO
```

### Comparing `pidgey-0.2.4/LICENSE` & `pidgey-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pidgey-0.2.4/pyproject.toml` & `pidgey-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pidgey"
-version = "0.2.4"
+version = "1.0.0"
 description = "Python interface for the dynamics of galaxies. Uses agama, gala, and galpy as backends."
 authors = [
     { name = "ilikecubesnstuff", email = "25328250+ilikecubesnstuff@users.noreply.github.com" },
 ]
 dependencies = [
     "iext>=1",
     "numpy>=1.22",
@@ -31,13 +31,13 @@
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [tool.pdm]
-package-type = "library"
+distribution = true
 
 [tool.pdm.dev-dependencies]
 dev = [
     "pytest>=7.4.4",
 ]
```

### Comparing `pidgey-0.2.4/src/pidgey/__init__.py` & `pidgey-1.0.0/src/pidgey/__init__.py`

 * *Files identical despite different names*

### Comparing `pidgey-0.2.4/src/pidgey/agama_backend.py` & `pidgey-1.0.0/src/pidgey/galpy_backend.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,39 @@
 import astropy.coordinates as coord
 import astropy.units as u
 import numpy as np
 
 from .base import Backend
 
 
-class AgamaBackend(Backend):
+class GalpyBackend(Backend):
     def __imports__():
-        import agama
+        from galpy import orbit
+        from galpy.util import conversion
 
     def ORBIT_TYPE(self):
-        return tuple
+        return self.orbit.Orbit
 
     def _compute_orbit(
         self, skycoord, pot, dt, steps, pattern_speed=0 * u.km / u.s / u.kpc
     ):
-        pos = [getattr(skycoord, attr).to(u.kpc).value for attr in ("x", "y", "z")]
-        vel = [
-            getattr(skycoord, attr).to(u.km / u.s).value
-            for attr in ("v_x", "v_y", "v_z")
-        ]
-        posvel = np.array([*pos, *vel]).T
-        orbit = self.agama.orbit(
-            potential=pot, ic=posvel, time=(dt * steps).to(u.Gyr).value, trajsize=steps
-        )
+        # unit consistency issues... look into this later
+        pot_units = self.conversion.get_physical(pot)
+        orbit = self.orbit.Orbit(skycoord, **pot_units)
+
+        t = np.arange(steps) * dt
+        orbit.integrate(t, pot)
         return orbit
 
     def _extract_points(self, orbit, pattern_speed=0 * u.km / u.s / u.kpc):
         skycoord, pot, dt, steps = self._args
-        if not skycoord.shape:
-            orbit = [orbit]
-        xs = []
-        ys = []
-        zs = []
-        for times, posvel in orbit:
-            x, y, z, *_ = posvel.T
-            xs.append(x)
-            ys.append(y)
-            zs.append(z)
-        if not skycoord.shape:
-            (xs,) = xs
-            (ys,) = ys
-            (zs,) = zs
-        return coord.representation.CartesianRepresentation(xs, ys, zs)
+        t = np.arange(steps) * dt
+        phi_offset = t * pattern_speed
+
+        R = orbit.R(t)
+        phi = orbit.phi(t) + phi_offset.to(u.dimensionless_unscaled)
+
+        x = R * np.cos(phi.value)
+        y = R * np.sin(phi.value)
+        z = orbit.z(t)
+
+        return coord.representation.CartesianRepresentation(x, y, z)
```

### Comparing `pidgey-0.2.4/src/pidgey/base.py` & `pidgey-1.0.0/src/pidgey/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-from abc import abstractmethod, abstractproperty
+from abc import abstractmethod
 
 import astropy.coordinates as coord
 import astropy.units as u
 from iext import ExtendImports
 
 
 class Backend(ExtendImports):
     def __imports__():
         ...
 
     def __init__(self):
         self._args = None
         self._result = None
 
-    @abstractproperty
+    @property
+    @abstractmethod
     def ORBIT_TYPE(self):
         pass
 
     @abstractmethod
     def _compute_orbit(
         self, skycoord, pot, dt, steps, pattern_speed=0 * u.km / u.s / u.kpc
     ):
@@ -42,15 +43,15 @@
             )
         if not isinstance(dt, u.Quantity):
             raise TypeError(
                 "dt must be passed in as a astropy.units.Quantity object."
                 f"{dt} is not a astropy.coordinates.SkyCoord object."
             )
         self._args = skycoord, pot, dt, steps
-        self._result = self._compute_orbit(skycoord, pot, dt, steps)
+        self._result = self._compute_orbit(skycoord, pot, dt, steps, pattern_speed)
         return self._extract_points(self._result, pattern_speed)
 
     @abstractmethod
     def _extract_points(self, orbit, pattern_speed=0 * u.km / u.s / u.kpc):
         pass
 
     def get_points(self):
```

### Comparing `pidgey-0.2.4/src/pidgey/gala_backend.py` & `pidgey-1.0.0/src/pidgey/gala_backend.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 import astropy.units as u
 
 from .base import Backend
 
 
 class GalaBackend(Backend):
     def __imports__():
-        from gala import dynamics, potential
+        from gala import dynamics, potential, units
 
     def ORBIT_TYPE(self):
         return self.dynamics.orbit.Orbit
 
     def _compute_orbit(
         self, skycoord, pot, dt, steps, pattern_speed=0 * u.km / u.s / u.kpc
     ):
         pos = [skycoord.x.value, skycoord.y.value, skycoord.z.value] * skycoord.x.unit
         vel = [
             skycoord.v_x.value,
             skycoord.v_y.value,
             skycoord.v_z.value,
         ] * skycoord.v_x.unit
         ics = self.dynamics.PhaseSpacePosition(pos, vel)
-        orbit = self.potential.Hamiltonian(pot).integrate_orbit(
-            ics, dt=dt, n_steps=steps - 1
-        )
+
+        orbit = pot.integrate_orbit(ics, dt=dt, n_steps=steps - 1)
         return orbit
 
     def _extract_points(self, orbit, pattern_speed=0 * u.km / u.s / u.kpc):
+        frame = self.potential.ConstantRotatingFrame(
+            Omega=[0, 0, pattern_speed.value] * pattern_speed.unit,
+            units=self.units.galactic,
+        )
+        orbit = orbit.to_frame(frame)
         return orbit.data.T
```

### Comparing `pidgey-0.2.4/tests/gala_env.yml` & `pidgey-1.0.0/tests/gala_env.yml`

 * *Files identical despite different names*

### Comparing `pidgey-0.2.4/tests/galpy_env.yml` & `pidgey-1.0.0/tests/galpy_env.yml`

 * *Files identical despite different names*

### Comparing `pidgey-0.2.4/tests/test_agama.py` & `pidgey-1.0.0/tests/test_agama.py`

 * *Files identical despite different names*

### Comparing `pidgey-0.2.4/tests/test_gala.py` & `pidgey-1.0.0/tests/test_gala.py`

 * *Files identical despite different names*

### Comparing `pidgey-0.2.4/tests/test_galpy.py` & `pidgey-1.0.0/tests/test_galpy.py`

 * *Files identical despite different names*

