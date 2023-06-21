# Comparing `tmp/atomcalc-0.1.1.tar.gz` & `tmp/atomcalc-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atomcalc-0.1.1.tar", max compression
+gzip compressed data, was "atomcalc-0.1.2.tar", max compression
```

## Comparing `atomcalc-0.1.1.tar` & `atomcalc-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,9 @@
--rw-r--r--   0        0        0      279 2023-06-03 16:12:35.652726 atomcalc-0.1.1/atomcalc/__init__.py
--rw-r--r--   0        0        0    27600 2023-06-12 18:09:46.970110 atomcalc-0.1.1/atomcalc/fidelity.py
--rw-r--r--   0        0        0      526 2023-06-12 18:14:20.133388 atomcalc-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-06 11:10:34.022007 atomcalc-0.1.1/README.md
--rw-r--r--   0        0        0      476 1970-01-01 00:00:00.000000 atomcalc-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-21 19:10:51.546476 atomcalc-0.1.2/atomcalc/__init__.py
+-rw-r--r--   0        0        0     1206 2023-06-21 19:20:53.765656 atomcalc-0.1.2/atomcalc/Decay.py
+-rw-r--r--   0        0        0     1531 2023-06-21 19:20:53.766656 atomcalc-0.1.2/atomcalc/Laser.py
+-rw-r--r--   0        0        0      457 2023-06-21 19:20:53.762652 atomcalc-0.1.2/atomcalc/Level.py
+-rw-r--r--   0        0        0      876 2023-06-21 19:20:53.792679 atomcalc-0.1.2/atomcalc/plot_pulse.py
+-rw-r--r--   0        0        0    24121 2023-06-21 19:20:54.536355 atomcalc-0.1.2/atomcalc/System.py
+-rw-r--r--   0        0        0      562 2023-06-21 19:43:03.779088 atomcalc-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1142 2023-06-21 18:51:17.200721 atomcalc-0.1.2/README.md
+-rw-r--r--   0        0        0     1636 1970-01-01 00:00:00.000000 atomcalc-0.1.2/PKG-INFO
```

### Comparing `atomcalc-0.1.1/atomcalc/fidelity.py` & `atomcalc-0.1.2/atomcalc/System.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,100 +1,12 @@
-# %%
-# Imports
 import numpy as np
 import qutip
-
-# import matplotlib
 import matplotlib.pylab as plt
 import scipy
 
-# import time
-
-
-class Level:
-    """
-    An object that describes an energy level.
-
-    Args:
-        energy (number): value for :attr:`energy`
-
-
-    Attributes:
-        energy (number): The energy of the level.
-
-    Example:
-
-        >>> Level(5)
-        This is a Level object with an energy of 5.
-    """
-
-    def __init__(self, energy):
-        self.energy = energy
-
-
-class Decay:
-    """An object that describes the decay of the system with the decay rates and the respective transitions.
-
-    Args:
-        rates (list): value for :attr:`rates`
-        final_states (list): value for :attr:`final_states`
-
-
-    Attributes:
-        rates (list): A list of decay rates.
-        final_states (list): A list of tupels of :class:`Level` objects that assign the decay rates to a corresponding transition.
-
-    Example:
-
-        >>> Decay([0, 1], [[Level([20]), Level([0])], [Level([5]), Level([0])]])
-        The transition between Level([20]) and Level([0]) is assigned a decay rate of 0. The transition between Level([5]) and Level([0]) is assigned a decay rate of 1.
-    """
-
-    def __init__(
-        self, rates, final_states
-    ):  # final_states is a Level-list with two-level-couples in each entry. rates is the respective decay-rate-list to each couple
-        if type(rates) != list or type(final_states) != list:
-            raise TypeError("rates and final_states need to be a list")
-        self.rates = np.array(rates)
-        self.final_states = np.array(final_states)
-
-
-class Laser:
-    """
-    An object that describes values for a laser: Rabi frequency, frequency, and coupled states.
-
-    Args:
-        rabifreq (number): value for :attr:`rabifreq`
-        frequency (number): value for :attr:`frequency`
-        couple (list): value for :attr:`couple`
-        pulse (None or function or list): value for :attr:`pulse`
-
-
-    Attributes:
-        rabifreq (number): Rabi frequency of the laser.
-        frequency (number): The to the frequency of the laser corresponding energy.
-        couple (list): A tupel of :class:`Level` objects that assigns the laser to this transition.
-        pulse (None or function or list): A time dependent function of the Rabi frequency of the laser OR a list of numbers describing a Rabi frequency pulse.
-
-    Example:
-
-        >>> Laser(1, 100, [Level([0]),Level([20])])
-        The transition between Level([20]) and Level([0]) is assigned a laser with Rabi frequency of 1 and a frequency of 100.
-
-    Note:
-        Sort Level couples from low to high.
-    """
-
-    def __init__(self, rabifreq, frequency, couple, polarization=None, pulse=None):
-        self.rabi = rabifreq
-        self.couple = couple
-        self.frequency = frequency
-        self.polarization = polarization  # Not yet included. A list of a normalized E-field vector in the laser coordinate system, a theta_k and a theta_p (in degrees) and a pair [m_i,m_f].
-        self.pulse = pulse
-
 
 class System:
     """An object that inherits all parameters used for simulation of the system.
 
     Args:
         levels (list): value for :attr:`levels`
         lasers (list): value for :attr:`lasers`
@@ -104,17 +16,17 @@
     Attributes:
         levels (list): A list of :class:`Level` objects.
         lasers (list): A list of :class:`Laser` objects.
         decay (class object): A :class:`Decay` object.
         dim (number): Number of levels.
 
     Example:
-        >>> level1 = Level([0])
-        >>> level2 = Level([20])
-        >>> level3 = Level([100])
+        >>> level1 = Level(0)
+        >>> level2 = Level(20)
+        >>> level3 = Level(100)
         >>> laser1 = Laser(1, 120, [level1,level3])
         >>> laser2 = Laser(1, 100, [level2,level3])
         >>> decay = Decay([0],[[level3,level1]])
         >>> system = System([level1, level2, level3], [laser1,laser2], decay)
 
     Note:
         Sort levels by energy in ascending order.
@@ -172,27 +84,27 @@
             i2 = self.levels.index(self.lasers[i].couple[1])
             x = [0.1 + 0.2 * i1, 0.1 + 0.2 * i2]
             y = [min_couple, max_couple + detuning[i]]
             plt.plot(x, y, linestyle="-", label="Laser {}".format(i + 1))
         plt.legend(loc="center left", bbox_to_anchor=(1, 0.5))
         plt.show()
 
-    def fidelity(
+    def simulate(
         self,
         initial_state_index_list,
         read_out_level,
         maxtime,
         delta_stark_shift=0,
         Diagonalization=True,
         plot_pop=True,
         Trotterintervals=500,
         resolution=250,
     ):
         """
-        A function to calculate the maximum population of the read_out_level
+        A function to simulate the time evolution of the population of every level. It also returns the maximum population of specifically the read_out_level.
 
         Args:
             initial_state_index_list (list): value for :attr:`initial_state_index_list`
             read_out_level (number): value for :attr:`read_out_level`
             maxtime (integer): value for :attr:`maxtime`
             delta_stark_shift (number): value for :attr:`delta_stark_shift`
             Diagonalization (bool): value for :attr:`Diagonalization`
@@ -357,15 +269,15 @@
                         lasermitpuls_index, n
                     )  # All laser indices from the lasers that have a pulse are in here
                     lasermitpuls_index = lasermitpuls_index.astype(int)
                     Trotter = True
                 else:
                     H = H + (1 / 2 * rabifreqs[n]) * (H_couple1[n] + H_couple2[n])
         print(
-            "Transformed Hamiltonian: {}".format(H)
+            "Hamiltonian in the rotating frame: {}".format(H)
         )  # Only the Rabi frequency entries are missing if the pulse is time dependent.
 
         # The Hamiltonian is created, now we solve it.
         # collapse operators are defined
         c_ops = [[]] * len(self.decay.rates)
         for i in range(len(self.decay.rates)):
             c_ops[i] = qutip.Qobj(np.sqrt(self.decay.rates[i]) * sigma[i])
@@ -412,16 +324,14 @@
                 )
             result[0] = np.array(expect_value_0)
 
             H_list = [H] * len(td)
             L = [[]] * len(td)
             # For t > 0:
             for n in range(len(td) - 1):  # loop over all trotter intervals
-                if n % 100 == 0:
-                    print(n)
                 # add the Rabi frequency entries for the Trotter interval we want to simulate here
                 for i in range(len(lasermitpuls_index)):
                     if hasattr(
                         self.lasers[0].pulse, "__len__"
                     ):  # If the pulse is given as a list
                         H_list[n] = H_list[n] + (
                             1 / 2 * self.lasers[lasermitpuls_index[i]].pulse[n]
@@ -551,29 +461,14 @@
             result = qutip.mesolve(H, initial_state_dm, tlist, c_ops, proj)
             # end = time.time()
             # print(f"{end-start:5.3f}s")
             plot_population(result, self.dim)
             print(result.expect[1][-1])
 
 
-# Plotting functions
-def plot_pulse(pulse, tlist):
-    fig, ax = plt.subplots()
-    pulse = np.array([pulse(t) for t in tlist])
-    tlist = np.array(tlist)
-    ax.set_yticks([0, 1], labels=[r"0", r"$\Omega$"])
-    ax.set_ylim([-0.1, 1.1])
-    ax.plot(tlist, pulse / max(pulse), label=r"$\Omega(t)$")
-    ax.legend()
-    ax.set_xlabel(r"Time")
-    ax.set_ylabel(r"Pulse amplitude")
-    plt.grid(linestyle=(0, (5, 10)), axis="both")
-    plt.show(fig)
-
-
 def plot_population(result, dim):
     fig, ax = plt.subplots()
     for i in range(dim):
         if i != 12:
             ax.plot(
                 result.times, result.expect[i], linewidth=1, label="{}".format(i + 1)
             )
```

### Comparing `atomcalc-0.1.1/pyproject.toml` & `atomcalc-0.1.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 [tool.poetry]
 name = "atomcalc"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["Moritz Wilke"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8.5,<3.12"
 numpy = "^1.24.3"
 matplotlib = "^3.7.1"
 qutip = "^4.7.1"
-
+scipy = "1.10.1"
 
 [tool.poetry.group.dev.dependencies]
 sphinx = "^6.2.1"
 sphinx-autobuild = "^2021.3.14"
 sphinx-rtd-theme = "^1.2.0"
 nbsphinx = "^0.9.2"
 pandoc = "^2.3"
 pypandoc = "^1.11"
 pytest = "^7.3.1"
+ipython = "^7.1.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

