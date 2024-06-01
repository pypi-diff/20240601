# Comparing `tmp/mechanism-1.1.7.tar.gz` & `tmp/mechanism-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mechanism-1.1.7.tar", last modified: Sun Oct 22 18:52:08 2023, max compression
+gzip compressed data, was "mechanism-1.1.8.tar", last modified: Sat Jun  1 00:43:23 2024, max compression
```

## Comparing `mechanism-1.1.7.tar` & `mechanism-1.1.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-10-22 18:52:08.132269 mechanism-1.1.7/
--rw-rw-rw-   0        0        0       26 2021-12-25 06:04:05.000000 mechanism-1.1.7/MANIFEST.in
--rw-rw-rw-   0        0        0    20467 2023-10-22 18:52:08.132269 mechanism-1.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     1063 2021-12-25 03:35:22.000000 mechanism-1.1.7/license.txt
-drwxrwxrwx   0        0        0        0 2023-10-22 18:52:08.115536 mechanism-1.1.7/mechanism/
--rw-rw-rw-   0        0        0      779 2022-01-05 05:07:15.000000 mechanism-1.1.7/mechanism/__init__.py
--rw-rw-rw-   0        0        0     2110 2023-10-22 18:42:49.000000 mechanism-1.1.7/mechanism/_player.py
--rw-rw-rw-   0        0        0     1980 2022-07-30 00:19:18.000000 mechanism-1.1.7/mechanism/appearance.json
--rw-rw-rw-   0        0        0    34067 2022-06-29 00:33:58.000000 mechanism-1.1.7/mechanism/cams.py
--rw-rw-rw-   0        0        0     7559 2021-09-30 00:43:13.000000 mechanism-1.1.7/mechanism/dataframe.py
--rw-rw-rw-   0        0        0    15503 2023-01-23 14:43:13.000000 mechanism-1.1.7/mechanism/gears.py
--rw-rw-rw-   0        0        0    42129 2023-10-22 18:44:41.000000 mechanism-1.1.7/mechanism/mechanism.py
--rw-rw-rw-   0        0        0    12646 2022-06-29 00:01:19.000000 mechanism-1.1.7/mechanism/vectors.py
-drwxrwxrwx   0        0        0        0 2023-10-22 18:52:08.132269 mechanism-1.1.7/mechanism.egg-info/
--rw-rw-rw-   0        0        0    20467 2023-10-22 18:52:08.000000 mechanism-1.1.7/mechanism.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      369 2023-10-22 18:52:08.000000 mechanism-1.1.7/mechanism.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-22 18:52:08.000000 mechanism-1.1.7/mechanism.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-10-22 18:52:08.000000 mechanism-1.1.7/mechanism.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-10-22 18:52:08.000000 mechanism-1.1.7/mechanism.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-10-22 18:52:08.132269 mechanism-1.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1343 2023-09-19 22:39:36.000000 mechanism-1.1.7/setup.py
+drwxr-xr-x   0 gabemorris   (501) staff       (20)        0 2024-06-01 00:43:23.813687 mechanism-1.1.8/
+-rw-r--r--   0 gabemorris   (501) staff       (20)       43 2024-06-01 00:42:18.000000 mechanism-1.1.8/MANIFEST.in
+-rw-r--r--   0 gabemorris   (501) staff       (20)    20277 2024-06-01 00:43:23.813299 mechanism-1.1.8/PKG-INFO
+drwxr-xr-x   0 gabemorris   (501) staff       (20)        0 2024-06-01 00:43:23.812196 mechanism-1.1.8/mechanism/
+-rw-r--r--   0 gabemorris   (501) staff       (20)      757 2024-05-31 23:45:16.000000 mechanism-1.1.8/mechanism/__init__.py
+-rw-r--r--   0 gabemorris   (501) staff       (20)     1908 2024-06-01 00:26:41.000000 mechanism-1.1.8/mechanism/_player.py
+-rw-r--r--   0 gabemorris   (501) staff       (20)     1874 2024-05-31 23:45:16.000000 mechanism-1.1.8/mechanism/appearance.json
+-rw-r--r--   0 gabemorris   (501) staff       (20)    33317 2024-05-31 23:45:16.000000 mechanism-1.1.8/mechanism/cams.py
+-rw-r--r--   0 gabemorris   (501) staff       (20)     7364 2024-05-31 23:45:16.000000 mechanism-1.1.8/mechanism/dataframe.py
+-rw-r--r--   0 gabemorris   (501) staff       (20)    15205 2024-05-31 23:45:16.000000 mechanism-1.1.8/mechanism/gears.py
+-rw-r--r--   0 gabemorris   (501) staff       (20)    41172 2024-06-01 00:26:41.000000 mechanism-1.1.8/mechanism/mechanism.py
+-rw-r--r--   0 gabemorris   (501) staff       (20)    12320 2024-05-31 23:45:16.000000 mechanism-1.1.8/mechanism/vectors.py
+drwxr-xr-x   0 gabemorris   (501) staff       (20)        0 2024-06-01 00:43:23.813106 mechanism-1.1.8/mechanism.egg-info/
+-rw-r--r--   0 gabemorris   (501) staff       (20)    20277 2024-06-01 00:43:23.000000 mechanism-1.1.8/mechanism.egg-info/PKG-INFO
+-rw-r--r--   0 gabemorris   (501) staff       (20)      367 2024-06-01 00:43:23.000000 mechanism-1.1.8/mechanism.egg-info/SOURCES.txt
+-rw-r--r--   0 gabemorris   (501) staff       (20)        1 2024-06-01 00:43:23.000000 mechanism-1.1.8/mechanism.egg-info/dependency_links.txt
+-rw-r--r--   0 gabemorris   (501) staff       (20)       17 2024-06-01 00:43:23.000000 mechanism-1.1.8/mechanism.egg-info/requires.txt
+-rw-r--r--   0 gabemorris   (501) staff       (20)       10 2024-06-01 00:43:23.000000 mechanism-1.1.8/mechanism.egg-info/top_level.txt
+-rw-r--r--   0 gabemorris   (501) staff       (20)    19618 2024-05-31 23:45:16.000000 mechanism-1.1.8/readme.md
+-rw-r--r--   0 gabemorris   (501) staff       (20)       38 2024-06-01 00:43:23.813721 mechanism-1.1.8/setup.cfg
+-rw-r--r--   0 gabemorris   (501) staff       (20)     1292 2024-06-01 00:29:08.000000 mechanism-1.1.8/setup.py
```

### Comparing `mechanism-1.1.7/PKG-INFO` & `mechanism-1.1.8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,447 +1,449 @@
-Metadata-Version: 2.1
-Name: mechanism
-Version: 1.1.7
-Summary: A package that provides a kinematic analysis of mechanisms and cams and custom tooth profile for spur gears.
-Home-page: https://github.com/gabemorris12/mechanism
-Author: Gabe Morris
-Author-email: gabemorris1231@gmail.com
-License: MIT
-Keywords: mechanism,kinematic,cams,linkages,analysis,animations
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
-License-File: license.txt
-Requires-Dist: matplotlib
-Requires-Dist: scipy
-
-# Purpose
-
-This package was created to aid with the designing process of mechanisms involving linkages, cams, and gears. In regard
-to linkages, it is capable of implementing a kinematic analysis with the knowledge of the degrees of freedom for the
-vectors that make up the mechanism. With the aid of numerical solving and iteration, the position, velocity, and
-acceleration of these vectors and points may be acquired.
-
-In regard to cams, this package is capable of supplying coordinates of a cam profile, plotting SVAJ diagrams, and
-getting a cam and follower animation for roller and flat faced followers. In turn, the coordinates may be supplied to a
-machinist or imported into SolidWorks. All that is needed to know is the motion description (i.e. rise 2 inches in 1
-second, dwell for 1.5 seconds, fall 2 inches in 3 seconds). As of right now, the kinds of motion supported are
-naive/uniform motion (how the cam shouldn't be designed), harmonic motion, and cycloidal motion. It is possible that
-this gets updated in the future with better options such as modified sinusoidal motion.
-
-For gears, this package is capable of providing the coordinates of a spur gear tooth profile given a set of properties.
-The analysis is based on the diametral pitch, number of teeth, and pitch diameter if desired over the number of teeth.
-An argument for AGMA standards may be set to `True` if desired.
-
-Install this package via pip: `pip install mechanism`.
-
-# Results/Examples
-
-`fourbarlinkage.py`
-
-![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/fourbarlinkage.gif)
-
-`fivebarlinkage.py`
-
-![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/fivebarlinkage.gif)
-
-`crunode_coupler.py`
-
-![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/crunode_coupler.gif)
-
-`crankslider.py`
-
-![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/crankslider.gif)
-
-`engine.py`
-
-![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/engine.gif)
-
-`non_grashof.py`
-
-![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/non_grashof.gif)
-
-`offset_crankslider.py`
-
-![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/offset_crankslider.gif)
-
-`cam2_example.py`
-
-![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/cam2.gif)
-
-# Linkages, Cranks, Couplers, and Rockers
-
-In order to use the contents of `mechanism.py`, a basic knowledge of vector loops must be known. The structure of the
-vector loops function is shown in several files under the `examples` folder. To gain a greater understanding of this
-package's usage, this walk through is provided.
-
-## Four Bar Linkage Example
-
-![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/fourbarlinkage.PNG)
-
-A four bar linkage is the basic building block of all mechanisms. This is similar to how the triangle is the basic
-building block of all structures. What defines a mechanism or structure is the system's overall number of degrees of
-freedom, and the number of degrees of freedom is determined via Kutzbachâ€™s equation.
-
-![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/fourbarlinkage_dof.PNG)
-
-Kutzbach's equation is: *total degrees of freedom = 3(#links - 1) - 2(J1) - J2* where J1 is the number of full joints
-(also known as a revolute joint) and J2 is the number of half joints. For this four bar linkage, there are 4 full
-joints.
-
-The number of degrees of freedom is: 3(4 - 1) - 2(4) = 1
-
-This means that we need one known input to find the unknowns of the system. This can be explained further with a diagram
-of the vectors that make up the four bar linkage.
-
-![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/fourbarlinkage_loop.PNG)
-
-From the above image, the vector "a" is the crank. The speed at which it rotates will be considered as the input to the
-system, and thus, it is the defining parameter to the system.
-
-The lengths of all the vectors are known. The only two unknowns are the angle that corresponds to vector "b" and "d". It
-is important to note that the objects that make up this package are vectors, and the polar form of the vectors is the
-main interest.
-
-There is only one loop equation which provides two equations when breaking down the vectors into its components. With
-two equations and two unknowns, this system becomes solvable.
-
-### Problem Statement
-
-Consider the four bar linkage shown above. The lengths of a, b, c, and d are 5", 8", 8" and 9". The crank (a) rotates at
-a constant 500 RPM. Use `mechanism` to get an animation of this linkage system and plot the angles, angular velocity,
-and angular acceleration of vector d as a function of time.
-
-### Solution
-
-The four bar linkage is a grashof linkage because it satisfies the grashof condition (9 + 5 < 8 + 8). This means that
-the crank is able to fully rotate. The input can be deduced by integrating and differentiating the constant value of the
-constant angular velocity of the crank.
-
-Always begin with defining the joints and vectors.
-
-```python
-from mechanism import *
-import numpy as np
-import matplotlib.pyplot as plt
-
-# Declare the joints that make up the system.
-O, A, B, C = get_joints('O A B C')
-
-# Declare the vectors and keep in mind that angles are in radians and start from the positive x-axis.
-a = Vector((O, A), r=5)
-b = Vector((A, B), r=8)
-c = Vector((O, C), r=8, theta=0, style='ground')
-d = Vector((C, B), r=9)
-```
-
-Always define the vectors in the polar form. The first argument is the joints, and the first joint is the tail of the
-vector, and the second is the head. Additionally, extra keyword arguments will be passed to plt.plot() for styling.
-
-By not defining the angles for a vector (like `a`, `b`, and `c`) you are saying that this vector will have a varying
-angle and the same is true for the length argument (`r`). If both the length and the angle are defined, as with `c`,
-then the vector is stationary and will remain at this length and angle. If niether `r` or `theta` is specified, then you
-are saying that the vector changes in length and angle, so you should expect two degrees of freedom for the input of
-this vector in the vector loop equations. There should be half as many loop equations as there are unknown. The input
-vector "a" does not need to have its known values at its declaration. Instead, it's values will be accounted for in the
-loop equation. The next thing to do is to define the known input and guesses for the first iteration of the unknown
-values.
-
-```python
-# Define the known input to the system.
-# For a 500 RMP crank, the time it takes to rotate one rev is 0.12s
-time = np.linspace(0, 0.12, 300)
-angular_velocity = 50*np.pi/3  # This is 500 RPM in rad/s
-
-theta = angular_velocity*time  # Integrate to find the theta
-omega = np.full((time.size,), angular_velocity)  # Just an array of the same angular velocity
-alpha = np.zeros(time.size)
-
-# Guess the unknowns
-pos_guess = np.deg2rad([45, 90])
-vel_guess = np.array([1000, 1000])
-acc_guess = np.array([1000, 1000])
-```
-
-The guess values need to be arrays of the same length as the number of unknowns. These arrays will be passed as the
-first iteration. The next thing to do is to define the loop function and create the mechanism object.
-
-```python
-# Define the loop equation(s)
-def loop(x, i):
-    return a(i) + b(x[0]) - c() - d(x[1])
-
-
-# Create the mechanism object
-mechanism = Mechanism(vectors=(a, b, c, d), origin=O, loops=loop, pos=theta, vel=omega, acc=alpha,
-                      guess=(pos_guess, vel_guess, acc_guess))
-```
-
-This example is simpler than most others because there is only one loop equation. For multiple loop equations, it is
-important that the function returns a flattened array of the same length as there are unknown, and the indexing of the
-first array argument to the loop corresponds to the input guess values. The second argument is the input. It is strongly
-encouraged to view the examples for the more rigorous structure of the loop function. The last thing to do is to
-call `mechanism.iterate()`, which is necessary if the input from `pos`, `vel`, and `acc` are arrays. If they are not
-arrays, then it is assumed that the mechanism at an instant is desired. If this is the case, then
-call `mechanism.calculate()` then call `mechanism.plot()` (see `plot_at_instant.py`).
-
-```python
-# Call mechanism.iterate() then get and show the animation
-mechanism.iterate()
-ani, fig_, ax_ = mechanism.get_animation()
-
-# Plot the angles, angular velocity, and angular acceleration of vector d
-fig, ax = plt.subplots(nrows=3, ncols=1)
-ax[0].plot(time, d.pos.thetas, color='maroon')
-ax[1].plot(time, d.vel.omegas, color='maroon')
-ax[2].plot(time, d.acc.alphas, color='maroon')
-
-ax[0].set_ylabel(r'$\theta$')
-ax[1].set_ylabel(r'$\omega$')
-ax[2].set_ylabel(r'$\alpha$')
-
-ax[2].set_xlabel(r'Time (s)')
-ax[0].set_title(r'Analysis of $\vec{d}$')
-
-for a in (ax[0], ax[1], ax[2]):
-    a.minorticks_on()
-    a.grid(which='both')
-
-fig.set_size_inches(7, 7)
-# fig.savefig('../images/analysis_d.png')
-
-plt.show()
-```
-
-This will produce the following output:
-
-![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/fourbar_animation.gif)
-![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/analysis_d.png)
-
-# Cams
-
-There are several kinds of motion types for a cam, but there is an important corollary when designing cams: *The jerk
-function must be finite across the entire interval (360 degrees)* (Robert Norton's *Design of Machinery*). Usually, the
-cycloidal motion type achieves this corollary, but it comes at a cost. It produces an acceleration and velocity that is
-typically higher than the other motion types. More motion types are to come later (hopefully).
-
-## Problem Statement
-
-Design a cam using cycloidal motion that has the following motion description:
-
-* Dwell at zero displacement for 90 degrees
-* Rise 1 inch in 90 degrees
-* Dwell for 90 degrees
-* Fall 1 inch in 90 degrees
-
-The cam's angular velocity is 2*pi radians per second. Show the SVAJ diagram as well as the cam's profile. Size the cam
-for a roller follower with a radius of 1/2" with a maximum pressure angle of 30 degrees. Also size the cam for a flat
-faced follower. Get an animation for both a roller/flat faced follower. Finally, save the coordinates of the profile to
-a text file and show the steps for creating a part in SolidWorks.
-
-## Solution
-
-Begin by creating a cam object with the correct motion description.
-
-```python
-import numpy as np
-from mechanism import Cam
-import matplotlib.pyplot as plt
-
-cam = Cam(motion=[
-    ('Dwell', 90),
-    ('Rise', 1, 90),
-    ('Dwell', 90),
-    ('Fall', 1, 90)
-], degrees=True, omega=2*np.pi)
-```
-
-The motion description is a list of tuples. Each tuple must contain 3 items for rising and falling and two items for
-dwelling. The first item of the tuple is a string equal to "Rise", "Fall", or "Dwell" (not case-sensitive). For rise and
-fall motion, the second item in the tuple is the distance at which the follower falls or rises. For dwelling, the second
-item in the tuple is either the time (in seconds) or angle (in degrees) for which the displacement remains constant. The
-third item in the tuple for rising and falling is equivalent to the second item for dwelling. If degrees is set to true,
-then the last item in each tuple is interpreted as the angle for which the action occurs. A manual input for the angular
-velocity is then required if conducting further analysis via SVAJ.
-
-This is all that's required to call the following methods.
-
-```python
-fig1, ax1 = cam.plot(kind='all')
-fig2, ax2 = cam.svaj(kind='cycloidal')
-plt.show()
-```
-
-This produces the following:
-
-![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/displacement_plot.png)
-![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/svaj.png)
-
-Looking at the acceleration plot, there are no vertical lines. This means that there is no infinite derivative at any
-instant along the cam's profile; the jerk function is finite across each instant, making this an acceptable motion type.
-
-If a roller follower with a 1/2" radius is desired, an analysis depending on the cam's radius of curvature and pressure
-angle can be conducted to determine the base circle of the cam.
-
-```python
-roller_analysis = cam.get_base_circle(kind='cycloidal', follower='roller', roller_radius=1/2, max_pressure_angle=30,
-                                      plot=True)
-fig3, ax3 = cam.profile(kind='cycloidal', base=roller_analysis['Rb'], show_base=True, roller_radius=1/2,
-                        show_pitch=True)
-plt.show()
-```
-
-Output:
-
-![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/pressure_angle.png)
-![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/roller_profile.png)
-
-For a flat faced follower, the radius of curvature at the point of contact should be positive (or greater than 0.25")
-for all theta. There is an option to return the base radius such that the radius of curvature of the cam's profile is
-positive for all values of theta (this is the conservative approach).
-
-```python
-flat_analysis = cam.get_base_circle(kind='cycloidal', follower='flat', desired_min_rho=0.25)
-print(flat_analysis['Rb'])
-print(flat_analysis['Min Face Width'])
-fig4, ax4 = cam.profile(kind='cycloidal', base=flat_analysis['Rb'], show_base=True)
-plt.show()
-```
-
-Output:
-
-![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/flat_profile.png)
-
-The base circle radius was found to be 1.893" and the minimum face width for the follower was found to be 2.55".
-
-To get the roller animation, call this:
-
-```python
-ani, fig5, ax5, follower = cam.get_animation(kind='cycloidal', base=roller_analysis['Rb'], roller_radius=1/2, length=2,
-                                             width=3/8, inc=5)
-fig6, ax6 = follower.plot()
-plt.show()
-```
-
-Output:
-
-![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/cam_roller.gif)
-![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/roller_follower_displacement.png)
-
-The graph above shows the actual follower displacement due to the circle having to always be tangent to the surface of
-the cam. Note that as a result of this physical limitation, the follower will have higher magnitudes of velocity and
-acceleration.
-
-For the flat faced follower,
-
-```python
-ani_flat, fig7, ax7, follower = cam.get_animation(kind='cycloidal', base=flat_analysis['Rb'], face_width=2.75, length=2,
-                                                  width=3/8, inc=5)
-fig8, ax8 = follower.plot()
-plt.show()
-```
-
-Output:
-
-![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/cam_flat.gif)
-![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/flat_follower_displacement.png)
-
-### Getting Coordinates into SolidWorks
-
-Save the coordinates to a text file.
-
-```python
-cam.save_coordinates('cam_coordinates.txt', kind='cycloidal', base=1.3, solidworks=True)
-```
-
-Select `Curve Through XYZ Points`
-
-![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/curve_xyz.png)
-
-The cam profile will always be extended to the front plane due to the manner in which SolidWorks defines the global
-coordinates. Next, select browse and choose the saved coordinate file, making sure that text files are able to be seen.
-
-![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/select_file.PNG)
-
-Create a sketch on the front plane. Select the curve and then convert entities. The sketch is now projected to the front
-plane.
-
-![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/front_plane.PNG)
-
-Notice that the sketch is not closed. Add a line to close the sketch, then extrude the sketch.
-
-![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/solidworks_cam.PNG)
-
-# Gears
-
-To use this feature, a knowledge of gear nomenclature must be known. Here is a figure from Robert Norton's *Design of
-Machinery*:
-
-![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/gear_nomenclature.PNG)
-
-For gears, a general rule of thumb is that the base circle must fall below the dedendum circle because the curve below
-base circle cannot be an involute curve. This package will send a warning if this occurs, and if it is desired to
-continue, the curve below the circle is just a straight line, and undercutting will occur.
-
-For a reference, here are the AGMA (American Gear Manufacturers Association) standards from *Design of Machinery*:
-
-![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/agma.PNG)
-
-## Problem Statement
-
-Design a gear that has a diametral pitch of 32 and has 60 teeth using `mechanism`. The gear follows the AGMA standards.
-Compare the gear to SolidWorks' gear from the tool library.
-
-## Solution
-
-Define a gear object with the known information and save the coordinates to a file.
-
-```python
-from mechanism import SpurGear
-import matplotlib.pyplot as plt
-
-gear = SpurGear(N=60, pd=32, agma=True, size=500)
-fig, ax = gear.plot()
-fig.savefig('../images/gear60.PNG', dpi=240)
-plt.show()
-gear.save_coordinates(file='gear_tooth_coordinates.txt', solidworks=True)
-gear.rundown()
-```
-
-output:
-
-![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/gear60.PNG)
-
-| Property                 | Value    |
-|--------------------------|----------|
-| Number of Teeth (N)      | 60       |
-| Diametral Pitch (pd)     | 32.00000 |
-| Pitch Diameter (d)       | 1.87500  |
-| Pitch Radius (r)         | 0.93750  |
-| Pressure Angle (phi)     | 20.00000 |
-| Base Radius              | 0.88096  |
-| Addendum (a)             | 0.03125  |
-| Dedendum (b)             | 0.03906  |
-| Circular Tooth Thickness | 0.04846  |
-| Circular Space Width     | 0.04971  |
-| Circular Backlash        | 0.00125  |
-
-Keep in mind that the `size` argument refers to the size of the coordinates that make up the involute curve. The more
-points, the sharper it is, but SolidWorks sometimes struggles with points being too close together. To fix this issue,
-make the size smaller. The default value is 1000.
-
-### SolidWorks Results
-
-Follow the same steps to get the curve into SolidWorks from the cam example. Make sure that the units in SolidWorks
-matches the units of the analysis.
-
-![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/gear60_compare.PNG)
-
-The results are a near identical match, and the addendum and dedendum fit perfectly. If analyzed closely, the only
-difference is the tooth thickness. The gray gear (the resulting gear from this package) has a slightly larger tooth
-thickness compared to SolidWorks' gear. This is due to the fact that SolidWorks doesn't use an involute gear tooth
-profile, as gears from the SolidWorks toolbox are for visuals only. Instead, the tooth profile is circular. Their gears
-should not be used for manufacturing as this is not accurate at all. The purpose of the involute tooth profile is that
-the meshing of gears will always produce a constant angular velocity, even when the gears aren't perfectly placed
-tangent to the pitch circles.
+Metadata-Version: 2.1
+Name: mechanism
+Version: 1.1.8
+Summary: A package that provides a kinematic analysis of mechanisms and cams and custom tooth profile for spur gears.
+Home-page: https://github.com/gabemorris12/mechanism
+Author: Gabe Morris
+Author-email: gabemorris1231@gmail.com
+License: MIT
+Keywords: mechanism,kinematic,cams,linkages,analysis,animations
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Programming Language :: Python :: 3.10
+Description-Content-Type: text/markdown
+Requires-Dist: matplotlib
+Requires-Dist: scipy
+
+# Purpose
+[![PyPI version](https://badge.fury.io/py/mechanism.svg)](https://badge.fury.io/py/mechanism)
+[![Downloads](https://static.pepy.tech/badge/mechanism)](https://pepy.tech/project/mechanism)
+[![Downloads](https://static.pepy.tech/badge/mechanism/month)](https://pepy.tech/project/mechanism)
+
+This package was created to aid with the designing process of mechanisms involving linkages, cams, and gears. In regard
+to linkages, it is capable of implementing a kinematic analysis with the knowledge of the degrees of freedom for the
+vectors that make up the mechanism. With the aid of numerical solving and iteration, the position, velocity, and
+acceleration of these vectors and points may be acquired.
+
+In regard to cams, this package is capable of supplying coordinates of a cam profile, plotting SVAJ diagrams, and
+getting a cam and follower animation for roller and flat faced followers. In turn, the coordinates may be supplied to a
+machinist or imported into SolidWorks. All that is needed to know is the motion description (i.e. rise 2 inches in 1
+second, dwell for 1.5 seconds, fall 2 inches in 3 seconds). As of right now, the kinds of motion supported are
+naive/uniform motion (how the cam shouldn't be designed), harmonic motion, and cycloidal motion. It is possible that
+this gets updated in the future with better options such as modified sinusoidal motion.
+
+For gears, this package is capable of providing the coordinates of a spur gear tooth profile given a set of properties.
+The analysis is based on the diametral pitch, number of teeth, and pitch diameter if desired over the number of teeth.
+An argument for AGMA standards may be set to `True` if desired.
+
+Install this package via pip: `pip install mechanism`.
+
+# Results/Examples
+
+`fourbarlinkage.py`
+
+![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/fourbarlinkage.gif)
+
+`fivebarlinkage.py`
+
+![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/fivebarlinkage.gif)
+
+`crunode_coupler.py`
+
+![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/crunode_coupler.gif)
+
+`crankslider.py`
+
+![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/crankslider.gif)
+
+`engine.py`
+
+![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/engine.gif)
+
+`non_grashof.py`
+
+![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/non_grashof.gif)
+
+`offset_crankslider.py`
+
+![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/offset_crankslider.gif)
+
+`cam2_example.py`
+
+![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/cam2.gif)
+
+# Linkages, Cranks, Couplers, and Rockers
+
+In order to use the contents of `mechanism.py`, a basic knowledge of vector loops must be known. The structure of the
+vector loops function is shown in several files under the `examples` folder. To gain a greater understanding of this
+package's usage, this walk through is provided.
+
+## Four Bar Linkage Example
+
+![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/fourbarlinkage.PNG)
+
+A four bar linkage is the basic building block of all mechanisms. This is similar to how the triangle is the basic
+building block of all structures. What defines a mechanism or structure is the system's overall number of degrees of
+freedom, and the number of degrees of freedom is determined via Kutzbach’s equation.
+
+![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/fourbarlinkage_dof.PNG)
+
+Kutzbach's equation is: *total degrees of freedom = 3(#links - 1) - 2(J1) - J2* where J1 is the number of full joints
+(also known as a revolute joint) and J2 is the number of half joints. For this four bar linkage, there are 4 full
+joints.
+
+The number of degrees of freedom is: 3(4 - 1) - 2(4) = 1
+
+This means that we need one known input to find the unknowns of the system. This can be explained further with a diagram
+of the vectors that make up the four bar linkage.
+
+![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/fourbarlinkage_loop.PNG)
+
+From the above image, the vector "a" is the crank. The speed at which it rotates will be considered as the input to the
+system, and thus, it is the defining parameter to the system.
+
+The lengths of all the vectors are known. The only two unknowns are the angle that corresponds to vector "b" and "d". It
+is important to note that the objects that make up this package are vectors, and the polar form of the vectors is the
+main interest.
+
+There is only one loop equation which provides two equations when breaking down the vectors into its components. With
+two equations and two unknowns, this system becomes solvable.
+
+### Problem Statement
+
+Consider the four bar linkage shown above. The lengths of a, b, c, and d are 5", 8", 8" and 9". The crank (a) rotates at
+a constant 500 RPM. Use `mechanism` to get an animation of this linkage system and plot the angles, angular velocity,
+and angular acceleration of vector d as a function of time.
+
+### Solution
+
+The four bar linkage is a grashof linkage because it satisfies the grashof condition (9 + 5 < 8 + 8). This means that
+the crank is able to fully rotate. The input can be deduced by integrating and differentiating the constant value of the
+constant angular velocity of the crank.
+
+Always begin with defining the joints and vectors.
+
+```python
+from mechanism import *
+import numpy as np
+import matplotlib.pyplot as plt
+
+# Declare the joints that make up the system.
+O, A, B, C = get_joints('O A B C')
+
+# Declare the vectors and keep in mind that angles are in radians and start from the positive x-axis.
+a = Vector((O, A), r=5)
+b = Vector((A, B), r=8)
+c = Vector((O, C), r=8, theta=0, style='ground')
+d = Vector((C, B), r=9)
+```
+
+Always define the vectors in the polar form. The first argument is the joints, and the first joint is the tail of the
+vector, and the second is the head. Additionally, extra keyword arguments will be passed to plt.plot() for styling.
+
+By not defining the angles for a vector (like `a`, `b`, and `c`) you are saying that this vector will have a varying
+angle and the same is true for the length argument (`r`). If both the length and the angle are defined, as with `c`,
+then the vector is stationary and will remain at this length and angle. If niether `r` or `theta` is specified, then you
+are saying that the vector changes in length and angle, so you should expect two degrees of freedom for the input of
+this vector in the vector loop equations. There should be half as many loop equations as there are unknown. The input
+vector "a" does not need to have its known values at its declaration. Instead, it's values will be accounted for in the
+loop equation. The next thing to do is to define the known input and guesses for the first iteration of the unknown
+values.
+
+```python
+# Define the known input to the system.
+# For a 500 RMP crank, the time it takes to rotate one rev is 0.12s
+time = np.linspace(0, 0.12, 300)
+angular_velocity = 50*np.pi/3  # This is 500 RPM in rad/s
+
+theta = angular_velocity*time  # Integrate to find the theta
+omega = np.full((time.size,), angular_velocity)  # Just an array of the same angular velocity
+alpha = np.zeros(time.size)
+
+# Guess the unknowns
+pos_guess = np.deg2rad([45, 90])
+vel_guess = np.array([1000, 1000])
+acc_guess = np.array([1000, 1000])
+```
+
+The guess values need to be arrays of the same length as the number of unknowns. These arrays will be passed as the
+first iteration. The next thing to do is to define the loop function and create the mechanism object.
+
+```python
+# Define the loop equation(s)
+def loop(x, i):
+    return a(i) + b(x[0]) - c() - d(x[1])
+
+
+# Create the mechanism object
+mechanism = Mechanism(vectors=(a, b, c, d), origin=O, loops=loop, pos=theta, vel=omega, acc=alpha,
+                      guess=(pos_guess, vel_guess, acc_guess))
+```
+
+This example is simpler than most others because there is only one loop equation. For multiple loop equations, it is
+important that the function returns a flattened array of the same length as there are unknown, and the indexing of the
+first array argument to the loop corresponds to the input guess values. The second argument is the input. It is strongly
+encouraged to view the examples for the more rigorous structure of the loop function. The last thing to do is to
+call `mechanism.iterate()`, which is necessary if the input from `pos`, `vel`, and `acc` are arrays. If they are not
+arrays, then it is assumed that the mechanism at an instant is desired. If this is the case, then
+call `mechanism.calculate()` then call `mechanism.plot()` (see `plot_at_instant.py`).
+
+```python
+# Call mechanism.iterate() then get and show the animation
+mechanism.iterate()
+ani, fig_, ax_ = mechanism.get_animation()
+
+# Plot the angles, angular velocity, and angular acceleration of vector d
+fig, ax = plt.subplots(nrows=3, ncols=1)
+ax[0].plot(time, d.pos.thetas, color='maroon')
+ax[1].plot(time, d.vel.omegas, color='maroon')
+ax[2].plot(time, d.acc.alphas, color='maroon')
+
+ax[0].set_ylabel(r'$\theta$')
+ax[1].set_ylabel(r'$\omega$')
+ax[2].set_ylabel(r'$\alpha$')
+
+ax[2].set_xlabel(r'Time (s)')
+ax[0].set_title(r'Analysis of $\vec{d}$')
+
+for a in (ax[0], ax[1], ax[2]):
+    a.minorticks_on()
+    a.grid(which='both')
+
+fig.set_size_inches(7, 7)
+# fig.savefig('../images/analysis_d.png')
+
+plt.show()
+```
+
+This will produce the following output:
+
+![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/fourbar_animation.gif)
+![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/analysis_d.png)
+
+# Cams
+
+There are several kinds of motion types for a cam, but there is an important corollary when designing cams: *The jerk
+function must be finite across the entire interval (360 degrees)* (Robert Norton's *Design of Machinery*). Usually, the
+cycloidal motion type achieves this corollary, but it comes at a cost. It produces an acceleration and velocity that is
+typically higher than the other motion types. More motion types are to come later (hopefully).
+
+## Problem Statement
+
+Design a cam using cycloidal motion that has the following motion description:
+
+* Dwell at zero displacement for 90 degrees
+* Rise 1 inch in 90 degrees
+* Dwell for 90 degrees
+* Fall 1 inch in 90 degrees
+
+The cam's angular velocity is 2*pi radians per second. Show the SVAJ diagram as well as the cam's profile. Size the cam
+for a roller follower with a radius of 1/2" with a maximum pressure angle of 30 degrees. Also size the cam for a flat
+faced follower. Get an animation for both a roller/flat faced follower. Finally, save the coordinates of the profile to
+a text file and show the steps for creating a part in SolidWorks.
+
+## Solution
+
+Begin by creating a cam object with the correct motion description.
+
+```python
+import numpy as np
+from mechanism import Cam
+import matplotlib.pyplot as plt
+
+cam = Cam(motion=[
+    ('Dwell', 90),
+    ('Rise', 1, 90),
+    ('Dwell', 90),
+    ('Fall', 1, 90)
+], degrees=True, omega=2*np.pi)
+```
+
+The motion description is a list of tuples. Each tuple must contain 3 items for rising and falling and two items for
+dwelling. The first item of the tuple is a string equal to "Rise", "Fall", or "Dwell" (not case-sensitive). For rise and
+fall motion, the second item in the tuple is the distance at which the follower falls or rises. For dwelling, the second
+item in the tuple is either the time (in seconds) or angle (in degrees) for which the displacement remains constant. The
+third item in the tuple for rising and falling is equivalent to the second item for dwelling. If degrees is set to true,
+then the last item in each tuple is interpreted as the angle for which the action occurs. A manual input for the angular
+velocity is then required if conducting further analysis via SVAJ.
+
+This is all that's required to call the following methods.
+
+```python
+fig1, ax1 = cam.plot(kind='all')
+fig2, ax2 = cam.svaj(kind='cycloidal')
+plt.show()
+```
+
+This produces the following:
+
+![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/displacement_plot.png)
+![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/svaj.png)
+
+Looking at the acceleration plot, there are no vertical lines. This means that there is no infinite derivative at any
+instant along the cam's profile; the jerk function is finite across each instant, making this an acceptable motion type.
+
+If a roller follower with a 1/2" radius is desired, an analysis depending on the cam's radius of curvature and pressure
+angle can be conducted to determine the base circle of the cam.
+
+```python
+roller_analysis = cam.get_base_circle(kind='cycloidal', follower='roller', roller_radius=1/2, max_pressure_angle=30,
+                                      plot=True)
+fig3, ax3 = cam.profile(kind='cycloidal', base=roller_analysis['Rb'], show_base=True, roller_radius=1/2,
+                        show_pitch=True)
+plt.show()
+```
+
+Output:
+
+![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/pressure_angle.png)
+![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/roller_profile.png)
+
+For a flat faced follower, the radius of curvature at the point of contact should be positive (or greater than 0.25")
+for all theta. There is an option to return the base radius such that the radius of curvature of the cam's profile is
+positive for all values of theta (this is the conservative approach).
+
+```python
+flat_analysis = cam.get_base_circle(kind='cycloidal', follower='flat', desired_min_rho=0.25)
+print(flat_analysis['Rb'])
+print(flat_analysis['Min Face Width'])
+fig4, ax4 = cam.profile(kind='cycloidal', base=flat_analysis['Rb'], show_base=True)
+plt.show()
+```
+
+Output:
+
+![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/flat_profile.png)
+
+The base circle radius was found to be 1.893" and the minimum face width for the follower was found to be 2.55".
+
+To get the roller animation, call this:
+
+```python
+ani, fig5, ax5, follower = cam.get_animation(kind='cycloidal', base=roller_analysis['Rb'], roller_radius=1/2, length=2,
+                                             width=3/8, inc=5)
+fig6, ax6 = follower.plot()
+plt.show()
+```
+
+Output:
+
+![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/cam_roller.gif)
+![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/roller_follower_displacement.png)
+
+The graph above shows the actual follower displacement due to the circle having to always be tangent to the surface of
+the cam. Note that as a result of this physical limitation, the follower will have higher magnitudes of velocity and
+acceleration.
+
+For the flat faced follower,
+
+```python
+ani_flat, fig7, ax7, follower = cam.get_animation(kind='cycloidal', base=flat_analysis['Rb'], face_width=2.75, length=2,
+                                                  width=3/8, inc=5)
+fig8, ax8 = follower.plot()
+plt.show()
+```
+
+Output:
+
+![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/cam_flat.gif)
+![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/flat_follower_displacement.png)
+
+### Getting Coordinates into SolidWorks
+
+Save the coordinates to a text file.
+
+```python
+cam.save_coordinates('cam_coordinates.txt', kind='cycloidal', base=1.3, solidworks=True)
+```
+
+Select `Curve Through XYZ Points`
+
+![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/curve_xyz.png)
+
+The cam profile will always be extended to the front plane due to the manner in which SolidWorks defines the global
+coordinates. Next, select browse and choose the saved coordinate file, making sure that text files are able to be seen.
+
+![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/select_file.PNG)
+
+Create a sketch on the front plane. Select the curve and then convert entities. The sketch is now projected to the front
+plane.
+
+![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/front_plane.PNG)
+
+Notice that the sketch is not closed. Add a line to close the sketch, then extrude the sketch.
+
+![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/solidworks_cam.PNG)
+
+# Gears
+
+To use this feature, a knowledge of gear nomenclature must be known. Here is a figure from Robert Norton's *Design of
+Machinery*:
+
+![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/gear_nomenclature.PNG)
+
+For gears, a general rule of thumb is that the base circle must fall below the dedendum circle because the curve below
+base circle cannot be an involute curve. This package will send a warning if this occurs, and if it is desired to
+continue, the curve below the circle is just a straight line, and undercutting will occur.
+
+For a reference, here are the AGMA (American Gear Manufacturers Association) standards from *Design of Machinery*:
+
+![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/agma.PNG)
+
+## Problem Statement
+
+Design a gear that has a diametral pitch of 32 and has 60 teeth using `mechanism`. The gear follows the AGMA standards.
+Compare the gear to SolidWorks' gear from the tool library.
+
+## Solution
+
+Define a gear object with the known information and save the coordinates to a file.
+
+```python
+from mechanism import SpurGear
+import matplotlib.pyplot as plt
+
+gear = SpurGear(N=60, pd=32, agma=True, size=500)
+fig, ax = gear.plot()
+fig.savefig('../images/gear60.PNG', dpi=240)
+plt.show()
+gear.save_coordinates(file='gear_tooth_coordinates.txt', solidworks=True)
+gear.rundown()
+```
+
+output:
+
+![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/gear60.PNG)
+
+| Property                 | Value    |
+|--------------------------|----------|
+| Number of Teeth (N)      | 60       |
+| Diametral Pitch (pd)     | 32.00000 |
+| Pitch Diameter (d)       | 1.87500  |
+| Pitch Radius (r)         | 0.93750  |
+| Pressure Angle (phi)     | 20.00000 |
+| Base Radius              | 0.88096  |
+| Addendum (a)             | 0.03125  |
+| Dedendum (b)             | 0.03906  |
+| Circular Tooth Thickness | 0.04846  |
+| Circular Space Width     | 0.04971  |
+| Circular Backlash        | 0.00125  |
+
+Keep in mind that the `size` argument refers to the size of the coordinates that make up the involute curve. The more
+points, the sharper it is, but SolidWorks sometimes struggles with points being too close together. To fix this issue,
+make the size smaller. The default value is 1000.
+
+### SolidWorks Results
+
+Follow the same steps to get the curve into SolidWorks from the cam example. Make sure that the units in SolidWorks
+matches the units of the analysis.
+
+![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/gear60_compare.PNG)
+
+The results are a near identical match, and the addendum and dedendum fit perfectly. If analyzed closely, the only
+difference is the tooth thickness. The gray gear (the resulting gear from this package) has a slightly larger tooth
+thickness compared to SolidWorks' gear. This is due to the fact that SolidWorks doesn't use an involute gear tooth
+profile, as gears from the SolidWorks toolbox are for visuals only. Instead, the tooth profile is circular. Their gears
+should not be used for manufacturing as this is not accurate at all. The purpose of the involute tooth profile is that
+the meshing of gears will always produce a constant angular velocity, even when the gears aren't perfectly placed
+tangent to the pitch circles.
```

### Comparing `mechanism-1.1.7/mechanism/__init__.py` & `mechanism-1.1.8/mechanism/__init__.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-import os
-import sys
-import warnings
-
-# Warning that arise due to using quiver:
-warnings.filterwarnings('ignore', 'divide by zero encountered in double_scalars')
-warnings.filterwarnings('ignore', 'invalid value encountered in multiply')
-
-# Warning that arises due to the 'move circle' function:
-warnings.filterwarnings('ignore', 'invalid value encountered in sqrt')
-
-from .mechanism import Joint, Mechanism, get_joints, get_sum
-from .dataframe import Data, read_csv, print_matrix
-from .vectors import Vector
-from .cams import Cam
-from .gears import SpurGear
-
-THIS_DIR = os.path.dirname(__file__)
-sys.path.append(THIS_DIR)
-
-__all__ = ['Data', 'read_csv', 'print_matrix', 'Joint', 'Vector', 'Mechanism', 'get_joints', 'get_sum', 'Cam',
-           'SpurGear']
+import os
+import sys
+import warnings
+
+# Warning that arise due to using quiver:
+warnings.filterwarnings('ignore', 'divide by zero encountered in double_scalars')
+warnings.filterwarnings('ignore', 'invalid value encountered in multiply')
+
+# Warning that arises due to the 'move circle' function:
+warnings.filterwarnings('ignore', 'invalid value encountered in sqrt')
+
+from .mechanism import Joint, Mechanism, get_joints, get_sum
+from .dataframe import Data, read_csv, print_matrix
+from .vectors import Vector
+from .cams import Cam
+from .gears import SpurGear
+
+THIS_DIR = os.path.dirname(__file__)
+sys.path.append(THIS_DIR)
+
+__all__ = ['Data', 'read_csv', 'print_matrix', 'Joint', 'Vector', 'Mechanism', 'get_joints', 'get_sum', 'Cam',
+           'SpurGear']
```

### Comparing `mechanism-1.1.7/mechanism/cams.py` & `mechanism-1.1.8/mechanism/cams.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,750 +1,750 @@
-import csv
-import json
-
-import matplotlib.pyplot as plt
-import numpy as np
-from matplotlib.animation import FuncAnimation
-from scipy.optimize import fsolve
-
-from .vectors import APPEARANCE
-
-
-class Cam:
-    def __init__(self, motion=None, degrees=False, omega=0., rotation='ccw', h=0.0062):
-        """
-        :param motion: Description of motion as a list of tuples. Each tuple must contain 3 items for rising and falling
-                       and two items for dwelling. The first item of the tuple is a string equal to "Rise", "Fall", or
-                       "Dwell" (not case-sensitive). For rise and fall motion, the second item in the tuple is the
-                       distance at which the follower falls or rises. For dwelling, the second item in the tuple is
-                       either the time (in seconds) or angle (in degrees) for which the displacement remains constant.
-                       The third item in the tuple for rising and falling is equivalent to the second item for dwelling.
-        :param degrees: If true, the last item in each tuple of 'motion' will be considered as degree inputs. If false,
-                        they will be considered as the time at which the rising, falling, or dwelling occurs. This will
-                        be enough to calculate the angular velocity, omega. The angular velocity will have to be given
-                        if 'degrees' is set to true.
-        :param omega: The angular velocity of the cam. This is always assumed to be constant and should only be given if
-                      'degrees' is set to true.
-        :param rotation: The direction of the cam rotation. Use 'ccw' for counterclockwise and 'cw' for clockwise. This
-                         will affect the animation and profile plots.
-        :param h: The step at which the data set gets initialized from 0 to 2*pi radians.
-
-        Instance Attributes
-        -------------------
-        motion: A list of tuples that describe the desired motion of the cam and follower
-        thetas: An np.ndarray from 0 to 2*pi at given step interval
-        thetas_d: An np.ndarray of thetas in degrees
-        thetas_r: An np.ndarray of thetas going in either the counterclockwise direction (negative values) or clockwise
-                  direction (positive values). This is only used to display the profile and retrieve the animation.
-        omega: The angular velocity of the cam in radians per second
-        rotation: The cam direction as a string ('ccw' or 'cw')
-        times: A list of time intervals of the motion. Only exists if 'degrees' is false.
-        intervals: A list of angle intervals (in radians) of the motion.
-        shifts: A list of the shifts that would occur when implementing the piecewise functions.
-        conditions: A list of np.ndarray's of booleans for each interval, corresponding to thetas. All sizes are equal.
-        default: A dictionary that gets past to **kwargs when specifying a default appearance in a plot.
-
-        Supported motion types are as follows:
-        naive: Naive object (how not to design a cam)
-        harmonic: Harmonic object
-        cycloidal: Cycloidal object
-
-        More motion types may be created in the future for overall better cam designs.
-
-        Useful Methods to Mention
-        -------------------------
-        plot: Plots the displacement of a specified motion type
-        svaj: Plots the svaj diagram of a specified motion type
-        profile: Plots the cam profile of a specified motion type
-        get_base_circle: Performs an analysis to appropriately size a cam
-        save_coordinates: Saves the coordinates of the cam profile to a file (can be used to create solidworks part)
-        get_animation: Retrieves and animation and follower object.
-        """
-        self.motion = motion
-        self.thetas = np.arange(0, 2*np.pi, h)
-        self.thetas_d = np.rad2deg(self.thetas)
-        self.omega = omega
-        self.rotation = rotation
-
-        # I am also assuming that the input will bring the follower back to zero in one full rotation...
-        # I am also assuming that the follower height is 0 when theta is 0
-        if not degrees:
-            self.times = np.array([t[-1] for t in motion], dtype=np.float64)
-            self.omega = 2*np.pi/np.sum(self.times)
-            self.intervals = self.omega*self.times
-        else:
-            self.intervals = np.deg2rad([t[-1] for t in motion])
-            if omega:
-                self.times = self.intervals/omega
-            assert np.abs(
-                np.sum(self.intervals) - 2*np.pi) < 1e-8, "Given degree increments don't add up to full rotation."
-
-        self.shifts = np.zeros(self.intervals.size)
-        self.shifts[0] = self.intervals[0]
-        for i in range(1, self.intervals.size):
-            self.shifts[i] = self.shifts[i - 1] + self.intervals[i]
-
-        assert all([m[0].lower() in ('dwell', 'rise', 'fall') for m in
-                    self.motion]), 'Only "rise", "fall", and "dwell" are acceptable descriptions.'
-
-        self.conditions = self._get_conditions(self.thetas)
-
-        if not self.omega:
-            self.naive = Naive(self.motion, self.shifts, self.intervals, self.conditions, self.thetas)
-            self.harmonic = Harmonic(self.motion, self.shifts, self.intervals, self.conditions, self.thetas)
-            self.cycloidal = Cycloidal(self.motion, self.shifts, self.intervals, self.conditions, self.thetas)
-        else:
-            self.naive = Naive(self.motion, self.shifts, self.intervals, self.conditions, self.thetas, omega=self.omega)
-            self.harmonic = Harmonic(self.motion, self.shifts, self.intervals, self.conditions, self.thetas,
-                                     omega=self.omega)
-            self.cycloidal = Cycloidal(self.motion, self.shifts, self.intervals, self.conditions, self.thetas,
-                                       omega=self.omega)
-
-        with open(APPEARANCE, 'r') as f:
-            appearance = json.load(f)
-
-        self.default = appearance['cam_plot']['default']
-
-        assert self.rotation == 'ccw' or self.rotation == 'cw', "Only 'ccw' or 'cw' must be specified for rotation."
-
-        if self.rotation == 'ccw':
-            self.thetas_r = self.thetas*-1
-        else:
-            self.thetas_r = self.thetas
-
-    def _get_conditions(self, t):
-        """ Returns a list of conditional arrays"""
-        # t is short for theta
-        conditions = [np.logical_and(t >= 0, t < self.shifts[0])]
-        for i in range(1, self.shifts.size):
-            conditions.append(np.logical_and(t >= self.shifts[i - 1], t < self.shifts[i]))
-        return conditions
-
-    def plot(self, kind='', grid=True):
-        """
-        :param kind: The type of motion desired as a string (i.e. 'cycloidal')
-        :param grid: If true, the grid will be added to the axes object
-        :return: figure and axes objects
-        """
-        fig, ax = plt.subplots()
-
-        if grid:
-            ax.grid(zorder=1)
-
-        if kind == 'all':
-            for obj in (self.naive, self.harmonic, self.cycloidal):
-                ax.plot(self.thetas_d, obj.S, **obj.appearance)
-            ax.legend()
-            ax.set_title('All Motion Types')
-        else:
-            motion_type = self._get_motion_type(kind)
-            ax.plot(self.thetas_d, motion_type.S, **self.default)
-            ax.set_title(f'{motion_type} Motion')
-
-        ax.set_xlabel(r'$\theta$ (degrees)')
-        ax.set_ylabel(r'$Displacement$')
-
-        return fig, ax
-
-    def svaj(self, kind=''):
-        """
-        :param kind: The type of motion desired as a string
-        :return: figure and axes objects
-        """
-        fig, ax = plt.subplots(nrows=4, ncols=1)
-        assert self.omega is not None, Exception(
-            'You must include omega input in order to know velocity, acceleration, and jerk.')
-
-        motion_type = self._get_motion_type(kind)
-        ax[0].set_title(f'{motion_type} Motion')
-        ax[0].plot(self.thetas_d, motion_type.S, **self.default)
-        ax[1].plot(self.thetas_d, motion_type.V, **self.default)
-        ax[2].plot(self.thetas_d, motion_type.A, **self.default)
-        ax[3].plot(self.thetas_d, motion_type.J, **self.default)
-
-        ax[0].set_ylabel(r'$Displacement$')
-        ax[1].set_ylabel(r'$Velocity$')
-        ax[2].set_ylabel(r'$Acceleration$')
-        ax[3].set_ylabel(r'$Jerk$')
-
-        fig.set_size_inches(7, 7.75)
-        ax[3].set_xlabel(r'$\theta$ (degrees)')
-
-        return fig, ax
-
-    def profile(self, kind='', base=0, show_base=False, roller_radius=0, show_pitch=False, grid=True):
-        """
-        This will not call ax.legend() because that is not always desired.
-
-        :param kind: The type of motion desired
-        :param base: The base circle radius of the cam
-        :param show_base: If true, the base circle will be present in the plot
-        :param roller_radius: To be used if the pitch curve is desired
-        :param show_pitch: If true, the pitch curve will be present in the plot (roller_radius must be given)
-        :param grid: If true, the grid will be added to the axes object
-        :return: figure and axes object
-        """
-        fig, ax = plt.subplots()
-        if grid:
-            ax.grid(zorder=1)
-
-        pitch_line = self.naive.cam_plot['pitch_line']
-
-        if kind == 'all':
-            ax.set_title('All Profiles')
-            for obj in (self.naive, self.harmonic, self.cycloidal):
-                x, y = obj.get_profile(base, self.thetas_r)
-                ax.plot(x, y, **obj.appearance)
-        else:
-            motion_type = self._get_motion_type(kind)
-            ax.set_title(f'{motion_type} Motion Profile')
-            x, y = motion_type.get_profile(base, self.thetas_r)
-            ax.fill(x, y, **motion_type.cam_plot['fill'])
-            if show_pitch:
-                assert roller_radius, 'Must include the roller radius to show the pitch.'
-                x, y = motion_type.get_profile(base + roller_radius, self.thetas_r)
-                ax.plot(x, y, **pitch_line)
-
-        if show_base:
-            c_nums = base*np.exp(1j*self.thetas)
-            ax.plot(np.real(c_nums), np.imag(c_nums), **self.naive.cam_plot['base_circle'])
-
-        ax.set_aspect('equal')
-
-        return fig, ax
-
-    def get_base_circle(self, kind='', follower='', roller_radius=0, eccentricity=0, max_pressure_angle=0,
-                        desired_min_rho=0, conservative_flat=False, plot=False):
-        """
-        :param kind: Type of motion desired for the analysis (i.e. 'harmonic', 'cycloidal').
-        :param follower: The type of follower. Either 'roller' or 'flat' are acceptable arguments.
-        :param roller_radius: The radius of the roller follower.
-        :param eccentricity: The offset of the follower from the center (used for roller followers).
-        :param max_pressure_angle: The desired maximum pressure angle (used for roller followers).
-        :param desired_min_rho: The desired minimum radius of curvature. Used for flat follower.
-        :param conservative_flat: If the follower is a flat follower and this is set to true, then a cam profile with
-                                  a positive radius of curvature for the entire profile will be returned. This implies
-                                  that the surface of the cam is concave down from 0 to 180 degrees and concave up from
-                                  180 to 360 degrees.
-        :param plot: Choose whether to include a plot of the pressure angles at the calculated base circle. Only used
-                     with roller followers.
-        :return: A dictionary of the suggested base circle, minimum radius of curvature at that base circle, and the
-                 calculated rho values. Minimum face width is added for a flat-faced follower. The values of phi are
-                 also added to the dictionary if "plot" is set to true.
-        """
-        assert self.omega is not None, Exception(
-            'The angular velocity of the cam must be known to conduct this analysis')
-
-        motion_type = self._get_motion_type(kind)
-        y = motion_type.S
-        y_ = motion_type.V/self.omega
-        y__ = motion_type.A/self.omega**2
-
-        if follower == 'roller':
-            assert roller_radius is not None and max_pressure_angle is not None, Exception(
-                'Roller radius (Rf) and max pressure angle must be included in order to complete analysis.')
-
-            phi = np.deg2rad(max_pressure_angle)
-            Rf = roller_radius
-
-            phi_max = lambda Rb: phi - np.max(
-                np.abs(np.arctan((y_ - eccentricity)/(y + np.sqrt((Rb + Rf)**2 + eccentricity**2)))))
-            base_radius = fsolve(phi_max, np.array([.1]))[0]
-
-            # Checking the minimum radius of curvature
-            Rp = base_radius + roller_radius
-            rhos = ((Rp + y)**2 + y_**2)**1.5/(
-                    (Rp + y)**2 + 2*y_**2 - y__*(Rp + y))
-            min_rho = np.min(np.abs(rhos))
-
-            assert min_rho > roller_radius, 'Calculated base radius results in a minimum radius of curvature that is ' \
-                                            'less than or equal to the roller radius.'
-
-            if plot:
-                fig, ax = plt.subplots()
-                phis = np.abs(np.arctan((y_ - eccentricity)/(y + np.sqrt((base_radius + Rf)**2 + eccentricity**2))))
-                ax.plot(self.thetas_d, np.rad2deg(phis), label=r'$|\phi(\theta)|$', **self.default)
-                ax.plot(self.thetas_d, max_pressure_angle*np.ones(self.thetas.size), color='black', ls='--',
-                        label=fr'$\phi={max_pressure_angle}^\circ$')
-                ax.set_title(f'Pressure Angles with $R_b={base_radius:.5f}$')
-                ax.set_xlabel(r'$\theta$ (deg)')
-                ax.set_ylabel(r'$|\phi|$ (deg)')
-                ax.grid()
-                ax.legend()
-                plt.show()
-                return {'Rb': base_radius, 'Min Rho': min_rho, 'phis': np.rad2deg(phis), 'rhos': rhos}
-            return {'Rb': base_radius, 'Min Rho': min_rho, 'rhos': rhos}
-        elif follower == 'flat':
-            assert desired_min_rho is not None, 'Minimum rho must be specified.'
-
-            min_face_width = np.max(y_) - np.min(y_)
-
-            if not conservative_flat:
-                base_circle = desired_min_rho - np.min(y + y__)
-                rhos = base_circle + y + y__
-
-                return {'Rb': base_circle, 'Min Rho': desired_min_rho, 'Min Face Width': min_face_width, 'rhos': rhos}
-
-            Rb_, min_rho, step = 1/2, -1, 0.001
-            rhos = None
-
-            while min_rho < desired_min_rho:
-                rhos = ((Rb_ + y)**2 + y_**2)**1.5/(
-                        (Rb_ + y)**2 + 2*y_**2 - y__*(Rb_ + y))
-                min_rho = np.min(rhos)
-                Rb_ += step
-
-            return {'Rb': Rb_, 'Min Rho': min_rho, 'Min Face Width': min_face_width, 'rhos': rhos}
-
-        else:
-            raise Exception('Only acceptable arguments for follower are "flat" and "roller".')
-
-    def save_coordinates(self, file='', kind='', base=0, solidworks=False):
-        """
-        :param file: The filepath to save the file too
-        :param kind: The desired motion type
-        :param base: The base circle radius of the cam
-        :param solidworks: If true, the file structure will be acceptable by solidworks standards. Use a .txt file
-                           extension for solidworks to be able to select the file.
-        """
-        motion_type = self._get_motion_type(kind)
-
-        x_coords, y_coords = motion_type.get_profile(base, self.thetas_r)
-
-        with open(file, 'w', newline='') as f:
-            if solidworks:
-                writer = csv.writer(f, delimiter='\t')
-                for x, y in zip(x_coords, y_coords):
-                    writer.writerow([f'{x:.8f}', f'{y:.8f}', 0])
-            else:
-                writer = csv.writer(f, delimiter=',')
-                writer.writerow(['x', 'y'])
-                for x, y in zip(x_coords, y_coords):
-                    writer.writerow([x, y])
-
-    def _get_motion_type(self, kind):
-        """Returns the motion object specified by 'kind'"""
-        if kind == 'naive':
-            return self.naive
-        elif kind == 'harmonic':
-            return self.harmonic
-        elif kind == 'cycloidal':
-            return self.cycloidal
-        else:
-            raise Exception('Unknown kind specified.')
-
-    def get_animation(self, kind=None, base=0, inc=10, cushion=0.5, roller_radius=0, face_width=0, length=0, width=0,
-                      eccentricity=0, grid=True):
-        """
-        :param kind: The motion type to base the animation off of
-        :param base: The base radius of the cam
-        :param inc: Adjusts the speed of the animation by incrementing across the values of thetas.
-        :param cushion: The cushion of the window around the objects
-        :param roller_radius: The radius of the roller follower. If specified, the animation returns a roller animation.
-        :param face_width: The face_width of the follower. If specified, the animation returns a flat faced follower
-                           animation
-        :param length: The length of the follower (optional)
-        :param width: The width of the follower (optional)
-        :param eccentricity: The offset of the follower
-        :param grid: If true, the grid will be added to the axes object
-        :return: animation, figure, axes, and follower object
-        """
-        motion_type = self._get_motion_type(kind)
-
-        fig, ax = plt.subplots()
-        ax.set_aspect('equal')
-        ax.set_title(f'{motion_type} Animation')
-        if grid:
-            ax.grid(zorder=1)
-
-        if roller_radius:
-            follower = RollerFollower(motion_type, base, self.thetas_r, inc, roller_radius=roller_radius, length=length,
-                                      width=width, eccentricity=eccentricity)
-            items = [ax.fill([], [], **motion_type.cam_plot['fill'])[0],
-                     ax.fill([], [], **motion_type.cam_plot['follower_fill'])[0],
-                     ax.fill([], [], **motion_type.cam_plot['follower_fill'])[0]]
-        elif face_width:
-            follower = FlatFollower(motion_type, base, self.thetas_r, inc, face_width=face_width, length=length,
-                                    width=width, eccentricity=eccentricity)
-            items = [ax.fill([], [], **motion_type.cam_plot['fill'])[0],
-                     ax.fill([], [], **motion_type.cam_plot['follower_fill'])[0]]
-        else:
-            raise Exception('A roller radius or face width must be specified.')
-
-        (x_min, x_max), (y_min, y_max) = follower.get_bounds()
-
-        ax.set_xlim(x_min - cushion, x_max + cushion)
-        ax.set_ylim(y_min - cushion, y_max + cushion)
-
-        def init():
-            return items
-
-        def animate_roller(index):
-            items[0].set_xy(np.stack((follower.cam_x[index], follower.cam_y[index]), axis=1))
-            items[1].set_xy(np.stack((follower.roller_x[index], follower.roller_y[index]), axis=1))
-            items[2].set_xy(follower.vertices[index])
-            return items
-
-        def animate_flat(index):
-            items[0].set_xy(np.stack((follower.cam_x[index], follower.cam_y[index]), axis=1))
-            items[1].set_xy(follower.vertices[index])
-            return items
-
-        if roller_radius:
-            animate = animate_roller
-        else:
-            animate = animate_flat
-
-        # noinspection PyTypeChecker
-        return FuncAnimation(fig, animate, frames=range(follower.motion_length), interval=20, blit=True,
-                             init_func=init), fig, ax, follower
-
-
-class Motion:
-    def __init__(self, motion, shifts, intervals, conditions, thetas, omega=None):
-        """
-        :param motion: The same list of tuples described in the Cam class documentation
-        :param shifts: The shifts from class Cam
-        :param intervals: The intervals from class Cam
-        :param conditions: The conditions from class Cam
-        :param thetas: The np.ndarray from class Cam
-        :param omega: The angular velocity of the cam
-
-        Instance Attributes
-        -------------------
-        motion, shifts, intervals, thetas, and omega are all the same as described in Cam documentation
-        S: The displacements of the cam corresponding to each value of theta
-        V: The velocity of the cam corresponding to each value of theta
-        A: The acceleration of the cam corresponding to each value of theta
-        J: The jerk of the cam corresponding to each value of theta
-
-        Methods used are primarily used for internal use to aid the useful methods within the Cam class.
-        """
-        self.motion = motion
-        self.shifts, self.intervals = shifts, intervals
-        self.conditions = conditions
-        self.thetas = thetas
-        self.omega = omega
-
-        self.S = np.piecewise(self.thetas, condlist=self.conditions, funclist=self._get_functions(self.f))
-        self.V, self.A, self.J = None, None, None
-        if self.omega is not None:
-            self._get_rates()
-
-        with open(APPEARANCE, 'r') as f:
-            appearance = json.load(f)
-
-        self.cam_plot = appearance['cam_plot']
-
-    def _get_functions(self, func_maker, rate=False):
-        """
-        :param func_maker: A function that returns a lambda expression
-        :param rate: If true, then dwells will be zero
-        :return: A list of lambda expressions corresponding to each interval of rotation. Used to create the piecewise
-                 function.
-        """
-        start = self.motion[0]
-        if start[0].lower() == 'dwell':
-            h1, h2 = 0, 0
-            functions = [_dwell_maker(h1)]
-        else:
-            h1, h2 = 0, start[1]
-            functions = [func_maker(h1, h2, self.intervals[0], 0)]
-            h1 += h2
-            assert start[0].lower() != 'fall', "Displacement must be positive for all rotation; therefore, it can't " \
-                                               "with a fall."
-
-        for i in range(1, self.shifts.size):
-            motion = self.motion[i]
-            if motion[0].lower() == 'dwell' and not rate:
-                functions.append(_dwell_maker(h1))
-            elif motion[0].lower() == 'dwell' and rate:
-                functions.append(_dwell_maker(0))
-            else:
-                h2 = motion[1] if motion[0].lower() == 'rise' else -motion[1]
-                functions.append(func_maker(h1, h2, self.intervals[i], self.shifts[i - 1]))
-                h1 += h2
-        return functions
-
-    def _get_rates(self):
-        """Gets the rates of velocity, acceleration, and jerk of the cam"""
-        self.V = np.piecewise(self.thetas, condlist=self.conditions,
-                              funclist=self._get_functions(self.f_, rate=True))*self.omega
-        self.A = np.piecewise(self.thetas, condlist=self.conditions,
-                              funclist=self._get_functions(self.f__, rate=True))*self.omega**2
-        self.J = np.piecewise(self.thetas, condlist=self.conditions,
-                              funclist=self._get_functions(self.f___, rate=True))*self.omega**3
-
-    def get_profile(self, base, thetas):
-        """
-        :param base: The base radius of the cam
-        :param thetas: This is thetas_r for the Cam class
-        :return: The coordinates of the cam
-        """
-        c_nums = (base + self.S)*np.exp(1j*thetas)
-        return np.real(c_nums), np.imag(c_nums)
-
-    @staticmethod
-    def f(*args):
-        pass
-
-    @staticmethod
-    def f_(*args):
-        pass
-
-    @staticmethod
-    def f__(*args):
-        pass
-
-    @staticmethod
-    def f___(*args):
-        pass
-
-
-class Naive(Motion):
-    def __init__(self, motion, shifts, intervals, conditions, thetas, omega=None):
-        Motion.__init__(self, motion, shifts, intervals, conditions, thetas, omega=omega)
-        self.appearance = self.cam_plot['naive_line']
-
-    @staticmethod
-    def f(h1, h2, B, s):
-        return lambda theta: h2/B*(theta - s) + h1
-
-    @staticmethod
-    def f_(_, h2, B, __):
-        return lambda theta: h2/B
-
-    @staticmethod
-    def f__(*_):
-        return lambda theta: 0
-
-    @staticmethod
-    def f___(*_):
-        return lambda theta: 0
-
-    def __str__(self):
-        return 'Naive'
-
-
-class Harmonic(Motion):
-    def __init__(self, motion, shifts, intervals, conditions, thetas, omega=None):
-        Motion.__init__(self, motion, shifts, intervals, conditions, thetas, omega=omega)
-        self.appearance = self.cam_plot['harmonic_line']
-
-    @staticmethod
-    def f(h1, h2, B, s):
-        return lambda theta: h1 + h2*(1 - np.cos(np.pi*(theta - s)/B))/2
-
-    @staticmethod
-    def f_(_, h2, B, s):
-        return lambda theta: np.pi*h2*np.sin(np.pi*(theta - s)/B)/(2*B)
-
-    @staticmethod
-    def f__(_, h2, B, s):
-        return lambda theta: np.pi**2*h2*np.cos(np.pi*(theta - s)/B)/(2*B**2)
-
-    @staticmethod
-    def f___(_, h2, B, s):
-        return lambda theta: -np.pi**3*h2*np.sin(np.pi*(theta - s)/B)/(2*B**3)
-
-    def __str__(self):
-        return 'Harmonic'
-
-
-class Cycloidal(Motion):
-    def __init__(self, motion, shifts, intervals, conditions, thetas, omega=None):
-        Motion.__init__(self, motion, shifts, intervals, conditions, thetas, omega=omega)
-        self.appearance = self.cam_plot['cycloidal_line']
-
-    @staticmethod
-    def f(h1, h2, B, s):
-        return lambda theta: h1 + h2*((theta - s)/B - 1/(2*np.pi)*np.sin(2*np.pi*(theta - s)/B))
-
-    @staticmethod
-    def f_(_, h2, B, s):
-        return lambda theta: h2*(-np.cos(2*np.pi*(theta - s)/B)/B + 1/B)
-
-    @staticmethod
-    def f__(_, h2, B, s):
-        return lambda theta: 2*np.pi*h2*np.sin(2*np.pi*(theta - s)/B)/B**2
-
-    @staticmethod
-    def f___(_, h2, B, s):
-        return lambda theta: 4*np.pi**2*h2*np.cos(2*np.pi*(theta - s)/B)/B**3
-
-    def __str__(self):
-        return 'Cycloidal'
-
-
-class RollerFollower:
-    def __init__(self, motion, base, thetas, inc, roller_radius, length=0, width=0, eccentricity=0):
-        """
-        :param motion: Motion object
-        :param base: Base radius of the cam
-        :param thetas: thetas_r associated with the cam
-        :param inc: The increment across the data set to be used
-        :param roller_radius: The radius of the follower
-        :param length: The length of the follower
-        :param width: The width of the follower
-        :param eccentricity: The offset of the follower
-
-        Useful Instance Attributes
-        --------------------------
-        S: The displacement of the follower (np.gradient to get the velocity and acceleration)
-
-        Useful Methods to Mention
-        -------------------------
-        plot: Plots the displacement alongside the cam displacement to show the difference between the two
-        """
-        self.indexes = range(0, thetas.size, inc)
-        self.motion_length = len(self.indexes)
-        self.motion = motion
-
-        h = thetas[0] - thetas[inc]
-        start_point = (base, eccentricity)
-        width = roller_radius if not width else width
-        length = 1.25*base if not length else length
-
-        circle = roller_radius*np.exp(1j*motion.thetas)
-        circle_x, circle_y = np.real(circle), np.imag(circle)
-
-        self.cam_x, self.cam_y = [], []  # A list of x and y coordinates of the cam profile for each rotation
-        self.roller_centers = []  # A list of x coordinates of the roller center
-        self.roller_x, self.roller_y = [], []  # A list of x and y coordinates for the circle of the roller
-        self.vertices = []  # Vertices of the follower
-
-        for i in range(self.motion_length):
-            cam_profile = motion.get_profile(base, thetas + i*h)
-            self.cam_x.append(cam_profile[0])
-            self.cam_y.append(cam_profile[1])
-            roller_center = _move_circle(cam_profile, roller_radius, start_point)
-            self.roller_centers.append(roller_center)
-            self.roller_x.append(circle_x + roller_center)
-            self.roller_y.append(circle_y + eccentricity)
-            start_point = (roller_center, eccentricity)
-            self.vertices.append([
-                np.array([roller_center, eccentricity + width/2]),
-                np.array([roller_center, eccentricity - width/2]),
-                np.array([roller_center + length - 0.25, eccentricity - width/2]),
-                np.array([roller_center + length, eccentricity]),
-                np.array([roller_center + length - 0.25, eccentricity + width/2])
-            ])
-
-        self.S = np.array(self.roller_centers) - np.min(self.roller_centers)
-
-    def get_bounds(self):
-        """
-        :return: The bounds of the animation
-        """
-        x_max = np.amax(self.vertices)
-        x_min = np.amin(self.cam_x)
-        y_min, y_max = np.amin(self.cam_y), np.amax(self.cam_y)
-        return (x_min, x_max), (y_min, y_max)
-
-    def plot(self, grid=True):
-        """
-        Plots the displacement of the follower alongside the cam displacement
-
-        :param grid: If true, the grid will be added to the axes object
-        :return: figure and axes object"""
-        fig, ax = plt.subplots()
-        if grid:
-            ax.grid(zorder=1)
-        ax.plot(np.rad2deg(self.motion.thetas[self.indexes]), self.S, label='Follower Displacement',
-                **self.motion.cam_plot['default'])
-        ax.plot(np.rad2deg(self.motion.thetas), self.motion.S, **self.motion.appearance)
-        ax.set_title('Follower Displacement')
-        ax.set_xlabel(r'$\theta$ (degrees)')
-        ax.set_ylabel(r'$Displacement$')
-        ax.legend()
-        return fig, ax
-
-
-class FlatFollower:
-    """
-    See the documentation for RollerFollower
-    """
-
-    def __init__(self, motion, base, thetas, inc, face_width=0, length=0, width=0, eccentricity=0):
-        self.indexes = range(0, thetas.size, inc)
-        self.motion_length = len(self.indexes)
-        self.motion = motion
-
-        h = thetas[0] - thetas[inc]
-        width = 1/8*face_width if not width else width
-        length = 2*face_width if not length else length
-
-        self.cam_x, self.cam_y = [], []
-        self.x_positions = []
-        self.vertices = []
-
-        for i in range(self.motion_length):
-            x, y = motion.get_profile(base, thetas + i*h)
-            self.cam_x.append(x)
-            self.cam_y.append(y)
-            possible = np.logical_and(y >= -(face_width/2 - eccentricity), y <= face_width/2 + eccentricity)
-            x_position = np.max(x[possible])
-            self.x_positions.append(x_position)
-            self.vertices.append([
-                np.array([x_position, face_width/2 + eccentricity]),
-                np.array([x_position, -(face_width/2 - eccentricity)]),
-                np.array([x_position + width, -(face_width/2 - eccentricity)]),
-                np.array([x_position + width, -(face_width/2 - eccentricity) + face_width/2 - width/2]),
-                np.array([x_position + length, -(face_width/2 - eccentricity) + face_width/2 - width/2]),
-                np.array([x_position + length, -(face_width/2 - eccentricity) + face_width/2 + width/2]),
-                np.array([x_position + width, -(face_width/2 - eccentricity) + face_width/2 + width/2]),
-                np.array([x_position + width, face_width/2 + eccentricity])
-            ])
-
-        self.S = np.array(self.x_positions) - np.min(self.x_positions)
-
-    def get_bounds(self):
-        x_max = np.amax(self.vertices)
-        x_min = np.amin(self.cam_x)
-        y_min, y_max = np.amin(self.cam_y), np.amax(self.cam_y)
-        return (x_min, x_max), (y_min, y_max)
-
-    def plot(self, grid=True):
-        fig, ax = plt.subplots()
-        if grid:
-            ax.grid(zorder=1)
-        ax.plot(np.rad2deg(self.motion.thetas[self.indexes]), self.S, label='Follower Displacement',
-                **self.motion.cam_plot['default'])
-        ax.plot(np.rad2deg(self.motion.thetas), self.motion.S, **self.motion.appearance)
-        ax.set_title('Follower Displacement')
-        ax.set_xlabel(r'$\theta$ (degrees)')
-        ax.set_ylabel(r'$Displacement$')
-        ax.legend()
-
-        return fig, ax
-
-
-def _dwell_maker(h):
-    return lambda theta: h
-
-
-def _move_circle(cam_profile, r, start_point):
-    """
-    This function is responsible for keeping the roller tangent to the surface of the cam within a 1/1000th unit
-    tolerance.
-
-    :param cam_profile: The coordinates of the cam in a (2, N) format.
-    :param r: The roller radius
-    :param start_point: The point to start the circle at
-    :return: The center of the circle in the x direction to where the circle is tangent to the surface of the cam
-    """
-    cam_x, cam_y = cam_profile
-    a, b = start_point
-    inside = np.logical_and(cam_y < np.sqrt(r**2 - (cam_x - a)**2) + b, cam_y > -np.sqrt(r**2 - (cam_x - a)**2) + b)
-
-    while True:
-        if np.any(inside):
-            a += 0.001
-            np.logical_and(cam_y < np.sqrt(r**2 - (cam_x - a)**2) + b, cam_y > -np.sqrt(r**2 - (cam_x - a)**2) + b,
-                           out=inside)
-        else:
-            a -= 0.001
-            np.logical_and(cam_y < np.sqrt(r**2 - (cam_x - a)**2) + b, cam_y > -np.sqrt(r**2 - (cam_x - a)**2) + b,
-                           out=inside)
-            if np.any(inside):
-                a += 0.001
-                return a
+import csv
+import json
+
+import matplotlib.pyplot as plt
+import numpy as np
+from matplotlib.animation import FuncAnimation
+from scipy.optimize import fsolve
+
+from .vectors import APPEARANCE
+
+
+class Cam:
+    def __init__(self, motion=None, degrees=False, omega=0., rotation='ccw', h=0.0062):
+        """
+        :param motion: Description of motion as a list of tuples. Each tuple must contain 3 items for rising and falling
+                       and two items for dwelling. The first item of the tuple is a string equal to "Rise", "Fall", or
+                       "Dwell" (not case-sensitive). For rise and fall motion, the second item in the tuple is the
+                       distance at which the follower falls or rises. For dwelling, the second item in the tuple is
+                       either the time (in seconds) or angle (in degrees) for which the displacement remains constant.
+                       The third item in the tuple for rising and falling is equivalent to the second item for dwelling.
+        :param degrees: If true, the last item in each tuple of 'motion' will be considered as degree inputs. If false,
+                        they will be considered as the time at which the rising, falling, or dwelling occurs. This will
+                        be enough to calculate the angular velocity, omega. The angular velocity will have to be given
+                        if 'degrees' is set to true.
+        :param omega: The angular velocity of the cam. This is always assumed to be constant and should only be given if
+                      'degrees' is set to true.
+        :param rotation: The direction of the cam rotation. Use 'ccw' for counterclockwise and 'cw' for clockwise. This
+                         will affect the animation and profile plots.
+        :param h: The step at which the data set gets initialized from 0 to 2*pi radians.
+
+        Instance Attributes
+        -------------------
+        motion: A list of tuples that describe the desired motion of the cam and follower
+        thetas: An np.ndarray from 0 to 2*pi at given step interval
+        thetas_d: An np.ndarray of thetas in degrees
+        thetas_r: An np.ndarray of thetas going in either the counterclockwise direction (negative values) or clockwise
+                  direction (positive values). This is only used to display the profile and retrieve the animation.
+        omega: The angular velocity of the cam in radians per second
+        rotation: The cam direction as a string ('ccw' or 'cw')
+        times: A list of time intervals of the motion. Only exists if 'degrees' is false.
+        intervals: A list of angle intervals (in radians) of the motion.
+        shifts: A list of the shifts that would occur when implementing the piecewise functions.
+        conditions: A list of np.ndarray's of booleans for each interval, corresponding to thetas. All sizes are equal.
+        default: A dictionary that gets past to **kwargs when specifying a default appearance in a plot.
+
+        Supported motion types are as follows:
+        naive: Naive object (how not to design a cam)
+        harmonic: Harmonic object
+        cycloidal: Cycloidal object
+
+        More motion types may be created in the future for overall better cam designs.
+
+        Useful Methods to Mention
+        -------------------------
+        plot: Plots the displacement of a specified motion type
+        svaj: Plots the svaj diagram of a specified motion type
+        profile: Plots the cam profile of a specified motion type
+        get_base_circle: Performs an analysis to appropriately size a cam
+        save_coordinates: Saves the coordinates of the cam profile to a file (can be used to create solidworks part)
+        get_animation: Retrieves and animation and follower object.
+        """
+        self.motion = motion
+        self.thetas = np.arange(0, 2*np.pi, h)
+        self.thetas_d = np.rad2deg(self.thetas)
+        self.omega = omega
+        self.rotation = rotation
+
+        # I am also assuming that the input will bring the follower back to zero in one full rotation...
+        # I am also assuming that the follower height is 0 when theta is 0
+        if not degrees:
+            self.times = np.array([t[-1] for t in motion], dtype=np.float64)
+            self.omega = 2*np.pi/np.sum(self.times)
+            self.intervals = self.omega*self.times
+        else:
+            self.intervals = np.deg2rad([t[-1] for t in motion])
+            if omega:
+                self.times = self.intervals/omega
+            assert np.abs(
+                np.sum(self.intervals) - 2*np.pi) < 1e-8, "Given degree increments don't add up to full rotation."
+
+        self.shifts = np.zeros(self.intervals.size)
+        self.shifts[0] = self.intervals[0]
+        for i in range(1, self.intervals.size):
+            self.shifts[i] = self.shifts[i - 1] + self.intervals[i]
+
+        assert all([m[0].lower() in ('dwell', 'rise', 'fall') for m in
+                    self.motion]), 'Only "rise", "fall", and "dwell" are acceptable descriptions.'
+
+        self.conditions = self._get_conditions(self.thetas)
+
+        if not self.omega:
+            self.naive = Naive(self.motion, self.shifts, self.intervals, self.conditions, self.thetas)
+            self.harmonic = Harmonic(self.motion, self.shifts, self.intervals, self.conditions, self.thetas)
+            self.cycloidal = Cycloidal(self.motion, self.shifts, self.intervals, self.conditions, self.thetas)
+        else:
+            self.naive = Naive(self.motion, self.shifts, self.intervals, self.conditions, self.thetas, omega=self.omega)
+            self.harmonic = Harmonic(self.motion, self.shifts, self.intervals, self.conditions, self.thetas,
+                                     omega=self.omega)
+            self.cycloidal = Cycloidal(self.motion, self.shifts, self.intervals, self.conditions, self.thetas,
+                                       omega=self.omega)
+
+        with open(APPEARANCE, 'r') as f:
+            appearance = json.load(f)
+
+        self.default = appearance['cam_plot']['default']
+
+        assert self.rotation == 'ccw' or self.rotation == 'cw', "Only 'ccw' or 'cw' must be specified for rotation."
+
+        if self.rotation == 'ccw':
+            self.thetas_r = self.thetas*-1
+        else:
+            self.thetas_r = self.thetas
+
+    def _get_conditions(self, t):
+        """ Returns a list of conditional arrays"""
+        # t is short for theta
+        conditions = [np.logical_and(t >= 0, t < self.shifts[0])]
+        for i in range(1, self.shifts.size):
+            conditions.append(np.logical_and(t >= self.shifts[i - 1], t < self.shifts[i]))
+        return conditions
+
+    def plot(self, kind='', grid=True):
+        """
+        :param kind: The type of motion desired as a string (i.e. 'cycloidal')
+        :param grid: If true, the grid will be added to the axes object
+        :return: figure and axes objects
+        """
+        fig, ax = plt.subplots()
+
+        if grid:
+            ax.grid(zorder=1)
+
+        if kind == 'all':
+            for obj in (self.naive, self.harmonic, self.cycloidal):
+                ax.plot(self.thetas_d, obj.S, **obj.appearance)
+            ax.legend()
+            ax.set_title('All Motion Types')
+        else:
+            motion_type = self._get_motion_type(kind)
+            ax.plot(self.thetas_d, motion_type.S, **self.default)
+            ax.set_title(f'{motion_type} Motion')
+
+        ax.set_xlabel(r'$\theta$ (degrees)')
+        ax.set_ylabel(r'$Displacement$')
+
+        return fig, ax
+
+    def svaj(self, kind=''):
+        """
+        :param kind: The type of motion desired as a string
+        :return: figure and axes objects
+        """
+        fig, ax = plt.subplots(nrows=4, ncols=1)
+        assert self.omega is not None, Exception(
+            'You must include omega input in order to know velocity, acceleration, and jerk.')
+
+        motion_type = self._get_motion_type(kind)
+        ax[0].set_title(f'{motion_type} Motion')
+        ax[0].plot(self.thetas_d, motion_type.S, **self.default)
+        ax[1].plot(self.thetas_d, motion_type.V, **self.default)
+        ax[2].plot(self.thetas_d, motion_type.A, **self.default)
+        ax[3].plot(self.thetas_d, motion_type.J, **self.default)
+
+        ax[0].set_ylabel(r'$Displacement$')
+        ax[1].set_ylabel(r'$Velocity$')
+        ax[2].set_ylabel(r'$Acceleration$')
+        ax[3].set_ylabel(r'$Jerk$')
+
+        fig.set_size_inches(7, 7.75)
+        ax[3].set_xlabel(r'$\theta$ (degrees)')
+
+        return fig, ax
+
+    def profile(self, kind='', base=0, show_base=False, roller_radius=0, show_pitch=False, grid=True):
+        """
+        This will not call ax.legend() because that is not always desired.
+
+        :param kind: The type of motion desired
+        :param base: The base circle radius of the cam
+        :param show_base: If true, the base circle will be present in the plot
+        :param roller_radius: To be used if the pitch curve is desired
+        :param show_pitch: If true, the pitch curve will be present in the plot (roller_radius must be given)
+        :param grid: If true, the grid will be added to the axes object
+        :return: figure and axes object
+        """
+        fig, ax = plt.subplots()
+        if grid:
+            ax.grid(zorder=1)
+
+        pitch_line = self.naive.cam_plot['pitch_line']
+
+        if kind == 'all':
+            ax.set_title('All Profiles')
+            for obj in (self.naive, self.harmonic, self.cycloidal):
+                x, y = obj.get_profile(base, self.thetas_r)
+                ax.plot(x, y, **obj.appearance)
+        else:
+            motion_type = self._get_motion_type(kind)
+            ax.set_title(f'{motion_type} Motion Profile')
+            x, y = motion_type.get_profile(base, self.thetas_r)
+            ax.fill(x, y, **motion_type.cam_plot['fill'])
+            if show_pitch:
+                assert roller_radius, 'Must include the roller radius to show the pitch.'
+                x, y = motion_type.get_profile(base + roller_radius, self.thetas_r)
+                ax.plot(x, y, **pitch_line)
+
+        if show_base:
+            c_nums = base*np.exp(1j*self.thetas)
+            ax.plot(np.real(c_nums), np.imag(c_nums), **self.naive.cam_plot['base_circle'])
+
+        ax.set_aspect('equal')
+
+        return fig, ax
+
+    def get_base_circle(self, kind='', follower='', roller_radius=0, eccentricity=0, max_pressure_angle=0,
+                        desired_min_rho=0, conservative_flat=False, plot=False):
+        """
+        :param kind: Type of motion desired for the analysis (i.e. 'harmonic', 'cycloidal').
+        :param follower: The type of follower. Either 'roller' or 'flat' are acceptable arguments.
+        :param roller_radius: The radius of the roller follower.
+        :param eccentricity: The offset of the follower from the center (used for roller followers).
+        :param max_pressure_angle: The desired maximum pressure angle (used for roller followers).
+        :param desired_min_rho: The desired minimum radius of curvature. Used for flat follower.
+        :param conservative_flat: If the follower is a flat follower and this is set to true, then a cam profile with
+                                  a positive radius of curvature for the entire profile will be returned. This implies
+                                  that the surface of the cam is concave down from 0 to 180 degrees and concave up from
+                                  180 to 360 degrees.
+        :param plot: Choose whether to include a plot of the pressure angles at the calculated base circle. Only used
+                     with roller followers.
+        :return: A dictionary of the suggested base circle, minimum radius of curvature at that base circle, and the
+                 calculated rho values. Minimum face width is added for a flat-faced follower. The values of phi are
+                 also added to the dictionary if "plot" is set to true.
+        """
+        assert self.omega is not None, Exception(
+            'The angular velocity of the cam must be known to conduct this analysis')
+
+        motion_type = self._get_motion_type(kind)
+        y = motion_type.S
+        y_ = motion_type.V/self.omega
+        y__ = motion_type.A/self.omega**2
+
+        if follower == 'roller':
+            assert roller_radius is not None and max_pressure_angle is not None, Exception(
+                'Roller radius (Rf) and max pressure angle must be included in order to complete analysis.')
+
+            phi = np.deg2rad(max_pressure_angle)
+            Rf = roller_radius
+
+            phi_max = lambda Rb: phi - np.max(
+                np.abs(np.arctan((y_ - eccentricity)/(y + np.sqrt((Rb + Rf)**2 + eccentricity**2)))))
+            base_radius = fsolve(phi_max, np.array([.1]))[0]
+
+            # Checking the minimum radius of curvature
+            Rp = base_radius + roller_radius
+            rhos = ((Rp + y)**2 + y_**2)**1.5/(
+                    (Rp + y)**2 + 2*y_**2 - y__*(Rp + y))
+            min_rho = np.min(np.abs(rhos))
+
+            assert min_rho > roller_radius, 'Calculated base radius results in a minimum radius of curvature that is ' \
+                                            'less than or equal to the roller radius.'
+
+            if plot:
+                fig, ax = plt.subplots()
+                phis = np.abs(np.arctan((y_ - eccentricity)/(y + np.sqrt((base_radius + Rf)**2 + eccentricity**2))))
+                ax.plot(self.thetas_d, np.rad2deg(phis), label=r'$|\phi(\theta)|$', **self.default)
+                ax.plot(self.thetas_d, max_pressure_angle*np.ones(self.thetas.size), color='black', ls='--',
+                        label=fr'$\phi={max_pressure_angle}^\circ$')
+                ax.set_title(f'Pressure Angles with $R_b={base_radius:.5f}$')
+                ax.set_xlabel(r'$\theta$ (deg)')
+                ax.set_ylabel(r'$|\phi|$ (deg)')
+                ax.grid()
+                ax.legend()
+                plt.show()
+                return {'Rb': base_radius, 'Min Rho': min_rho, 'phis': np.rad2deg(phis), 'rhos': rhos}
+            return {'Rb': base_radius, 'Min Rho': min_rho, 'rhos': rhos}
+        elif follower == 'flat':
+            assert desired_min_rho is not None, 'Minimum rho must be specified.'
+
+            min_face_width = np.max(y_) - np.min(y_)
+
+            if not conservative_flat:
+                base_circle = desired_min_rho - np.min(y + y__)
+                rhos = base_circle + y + y__
+
+                return {'Rb': base_circle, 'Min Rho': desired_min_rho, 'Min Face Width': min_face_width, 'rhos': rhos}
+
+            Rb_, min_rho, step = 1/2, -1, 0.001
+            rhos = None
+
+            while min_rho < desired_min_rho:
+                rhos = ((Rb_ + y)**2 + y_**2)**1.5/(
+                        (Rb_ + y)**2 + 2*y_**2 - y__*(Rb_ + y))
+                min_rho = np.min(rhos)
+                Rb_ += step
+
+            return {'Rb': Rb_, 'Min Rho': min_rho, 'Min Face Width': min_face_width, 'rhos': rhos}
+
+        else:
+            raise Exception('Only acceptable arguments for follower are "flat" and "roller".')
+
+    def save_coordinates(self, file='', kind='', base=0, solidworks=False):
+        """
+        :param file: The filepath to save the file too
+        :param kind: The desired motion type
+        :param base: The base circle radius of the cam
+        :param solidworks: If true, the file structure will be acceptable by solidworks standards. Use a .txt file
+                           extension for solidworks to be able to select the file.
+        """
+        motion_type = self._get_motion_type(kind)
+
+        x_coords, y_coords = motion_type.get_profile(base, self.thetas_r)
+
+        with open(file, 'w', newline='') as f:
+            if solidworks:
+                writer = csv.writer(f, delimiter='\t')
+                for x, y in zip(x_coords, y_coords):
+                    writer.writerow([f'{x:.8f}', f'{y:.8f}', 0])
+            else:
+                writer = csv.writer(f, delimiter=',')
+                writer.writerow(['x', 'y'])
+                for x, y in zip(x_coords, y_coords):
+                    writer.writerow([x, y])
+
+    def _get_motion_type(self, kind):
+        """Returns the motion object specified by 'kind'"""
+        if kind == 'naive':
+            return self.naive
+        elif kind == 'harmonic':
+            return self.harmonic
+        elif kind == 'cycloidal':
+            return self.cycloidal
+        else:
+            raise Exception('Unknown kind specified.')
+
+    def get_animation(self, kind=None, base=0, inc=10, cushion=0.5, roller_radius=0, face_width=0, length=0, width=0,
+                      eccentricity=0, grid=True):
+        """
+        :param kind: The motion type to base the animation off of
+        :param base: The base radius of the cam
+        :param inc: Adjusts the speed of the animation by incrementing across the values of thetas.
+        :param cushion: The cushion of the window around the objects
+        :param roller_radius: The radius of the roller follower. If specified, the animation returns a roller animation.
+        :param face_width: The face_width of the follower. If specified, the animation returns a flat faced follower
+                           animation
+        :param length: The length of the follower (optional)
+        :param width: The width of the follower (optional)
+        :param eccentricity: The offset of the follower
+        :param grid: If true, the grid will be added to the axes object
+        :return: animation, figure, axes, and follower object
+        """
+        motion_type = self._get_motion_type(kind)
+
+        fig, ax = plt.subplots()
+        ax.set_aspect('equal')
+        ax.set_title(f'{motion_type} Animation')
+        if grid:
+            ax.grid(zorder=1)
+
+        if roller_radius:
+            follower = RollerFollower(motion_type, base, self.thetas_r, inc, roller_radius=roller_radius, length=length,
+                                      width=width, eccentricity=eccentricity)
+            items = [ax.fill([], [], **motion_type.cam_plot['fill'])[0],
+                     ax.fill([], [], **motion_type.cam_plot['follower_fill'])[0],
+                     ax.fill([], [], **motion_type.cam_plot['follower_fill'])[0]]
+        elif face_width:
+            follower = FlatFollower(motion_type, base, self.thetas_r, inc, face_width=face_width, length=length,
+                                    width=width, eccentricity=eccentricity)
+            items = [ax.fill([], [], **motion_type.cam_plot['fill'])[0],
+                     ax.fill([], [], **motion_type.cam_plot['follower_fill'])[0]]
+        else:
+            raise Exception('A roller radius or face width must be specified.')
+
+        (x_min, x_max), (y_min, y_max) = follower.get_bounds()
+
+        ax.set_xlim(x_min - cushion, x_max + cushion)
+        ax.set_ylim(y_min - cushion, y_max + cushion)
+
+        def init():
+            return items
+
+        def animate_roller(index):
+            items[0].set_xy(np.stack((follower.cam_x[index], follower.cam_y[index]), axis=1))
+            items[1].set_xy(np.stack((follower.roller_x[index], follower.roller_y[index]), axis=1))
+            items[2].set_xy(follower.vertices[index])
+            return items
+
+        def animate_flat(index):
+            items[0].set_xy(np.stack((follower.cam_x[index], follower.cam_y[index]), axis=1))
+            items[1].set_xy(follower.vertices[index])
+            return items
+
+        if roller_radius:
+            animate = animate_roller
+        else:
+            animate = animate_flat
+
+        # noinspection PyTypeChecker
+        return FuncAnimation(fig, animate, frames=range(follower.motion_length), interval=20, blit=True,
+                             init_func=init), fig, ax, follower
+
+
+class Motion:
+    def __init__(self, motion, shifts, intervals, conditions, thetas, omega=None):
+        """
+        :param motion: The same list of tuples described in the Cam class documentation
+        :param shifts: The shifts from class Cam
+        :param intervals: The intervals from class Cam
+        :param conditions: The conditions from class Cam
+        :param thetas: The np.ndarray from class Cam
+        :param omega: The angular velocity of the cam
+
+        Instance Attributes
+        -------------------
+        motion, shifts, intervals, thetas, and omega are all the same as described in Cam documentation
+        S: The displacements of the cam corresponding to each value of theta
+        V: The velocity of the cam corresponding to each value of theta
+        A: The acceleration of the cam corresponding to each value of theta
+        J: The jerk of the cam corresponding to each value of theta
+
+        Methods used are primarily used for internal use to aid the useful methods within the Cam class.
+        """
+        self.motion = motion
+        self.shifts, self.intervals = shifts, intervals
+        self.conditions = conditions
+        self.thetas = thetas
+        self.omega = omega
+
+        self.S = np.piecewise(self.thetas, condlist=self.conditions, funclist=self._get_functions(self.f))
+        self.V, self.A, self.J = None, None, None
+        if self.omega is not None:
+            self._get_rates()
+
+        with open(APPEARANCE, 'r') as f:
+            appearance = json.load(f)
+
+        self.cam_plot = appearance['cam_plot']
+
+    def _get_functions(self, func_maker, rate=False):
+        """
+        :param func_maker: A function that returns a lambda expression
+        :param rate: If true, then dwells will be zero
+        :return: A list of lambda expressions corresponding to each interval of rotation. Used to create the piecewise
+                 function.
+        """
+        start = self.motion[0]
+        if start[0].lower() == 'dwell':
+            h1, h2 = 0, 0
+            functions = [_dwell_maker(h1)]
+        else:
+            h1, h2 = 0, start[1]
+            functions = [func_maker(h1, h2, self.intervals[0], 0)]
+            h1 += h2
+            assert start[0].lower() != 'fall', "Displacement must be positive for all rotation; therefore, it can't " \
+                                               "with a fall."
+
+        for i in range(1, self.shifts.size):
+            motion = self.motion[i]
+            if motion[0].lower() == 'dwell' and not rate:
+                functions.append(_dwell_maker(h1))
+            elif motion[0].lower() == 'dwell' and rate:
+                functions.append(_dwell_maker(0))
+            else:
+                h2 = motion[1] if motion[0].lower() == 'rise' else -motion[1]
+                functions.append(func_maker(h1, h2, self.intervals[i], self.shifts[i - 1]))
+                h1 += h2
+        return functions
+
+    def _get_rates(self):
+        """Gets the rates of velocity, acceleration, and jerk of the cam"""
+        self.V = np.piecewise(self.thetas, condlist=self.conditions,
+                              funclist=self._get_functions(self.f_, rate=True))*self.omega
+        self.A = np.piecewise(self.thetas, condlist=self.conditions,
+                              funclist=self._get_functions(self.f__, rate=True))*self.omega**2
+        self.J = np.piecewise(self.thetas, condlist=self.conditions,
+                              funclist=self._get_functions(self.f___, rate=True))*self.omega**3
+
+    def get_profile(self, base, thetas):
+        """
+        :param base: The base radius of the cam
+        :param thetas: This is thetas_r for the Cam class
+        :return: The coordinates of the cam
+        """
+        c_nums = (base + self.S)*np.exp(1j*thetas)
+        return np.real(c_nums), np.imag(c_nums)
+
+    @staticmethod
+    def f(*args):
+        pass
+
+    @staticmethod
+    def f_(*args):
+        pass
+
+    @staticmethod
+    def f__(*args):
+        pass
+
+    @staticmethod
+    def f___(*args):
+        pass
+
+
+class Naive(Motion):
+    def __init__(self, motion, shifts, intervals, conditions, thetas, omega=None):
+        Motion.__init__(self, motion, shifts, intervals, conditions, thetas, omega=omega)
+        self.appearance = self.cam_plot['naive_line']
+
+    @staticmethod
+    def f(h1, h2, B, s):
+        return lambda theta: h2/B*(theta - s) + h1
+
+    @staticmethod
+    def f_(_, h2, B, __):
+        return lambda theta: h2/B
+
+    @staticmethod
+    def f__(*_):
+        return lambda theta: 0
+
+    @staticmethod
+    def f___(*_):
+        return lambda theta: 0
+
+    def __str__(self):
+        return 'Naive'
+
+
+class Harmonic(Motion):
+    def __init__(self, motion, shifts, intervals, conditions, thetas, omega=None):
+        Motion.__init__(self, motion, shifts, intervals, conditions, thetas, omega=omega)
+        self.appearance = self.cam_plot['harmonic_line']
+
+    @staticmethod
+    def f(h1, h2, B, s):
+        return lambda theta: h1 + h2*(1 - np.cos(np.pi*(theta - s)/B))/2
+
+    @staticmethod
+    def f_(_, h2, B, s):
+        return lambda theta: np.pi*h2*np.sin(np.pi*(theta - s)/B)/(2*B)
+
+    @staticmethod
+    def f__(_, h2, B, s):
+        return lambda theta: np.pi**2*h2*np.cos(np.pi*(theta - s)/B)/(2*B**2)
+
+    @staticmethod
+    def f___(_, h2, B, s):
+        return lambda theta: -np.pi**3*h2*np.sin(np.pi*(theta - s)/B)/(2*B**3)
+
+    def __str__(self):
+        return 'Harmonic'
+
+
+class Cycloidal(Motion):
+    def __init__(self, motion, shifts, intervals, conditions, thetas, omega=None):
+        Motion.__init__(self, motion, shifts, intervals, conditions, thetas, omega=omega)
+        self.appearance = self.cam_plot['cycloidal_line']
+
+    @staticmethod
+    def f(h1, h2, B, s):
+        return lambda theta: h1 + h2*((theta - s)/B - 1/(2*np.pi)*np.sin(2*np.pi*(theta - s)/B))
+
+    @staticmethod
+    def f_(_, h2, B, s):
+        return lambda theta: h2*(-np.cos(2*np.pi*(theta - s)/B)/B + 1/B)
+
+    @staticmethod
+    def f__(_, h2, B, s):
+        return lambda theta: 2*np.pi*h2*np.sin(2*np.pi*(theta - s)/B)/B**2
+
+    @staticmethod
+    def f___(_, h2, B, s):
+        return lambda theta: 4*np.pi**2*h2*np.cos(2*np.pi*(theta - s)/B)/B**3
+
+    def __str__(self):
+        return 'Cycloidal'
+
+
+class RollerFollower:
+    def __init__(self, motion, base, thetas, inc, roller_radius, length=0, width=0, eccentricity=0):
+        """
+        :param motion: Motion object
+        :param base: Base radius of the cam
+        :param thetas: thetas_r associated with the cam
+        :param inc: The increment across the data set to be used
+        :param roller_radius: The radius of the follower
+        :param length: The length of the follower
+        :param width: The width of the follower
+        :param eccentricity: The offset of the follower
+
+        Useful Instance Attributes
+        --------------------------
+        S: The displacement of the follower (np.gradient to get the velocity and acceleration)
+
+        Useful Methods to Mention
+        -------------------------
+        plot: Plots the displacement alongside the cam displacement to show the difference between the two
+        """
+        self.indexes = range(0, thetas.size, inc)
+        self.motion_length = len(self.indexes)
+        self.motion = motion
+
+        h = thetas[0] - thetas[inc]
+        start_point = (base, eccentricity)
+        width = roller_radius if not width else width
+        length = 1.25*base if not length else length
+
+        circle = roller_radius*np.exp(1j*motion.thetas)
+        circle_x, circle_y = np.real(circle), np.imag(circle)
+
+        self.cam_x, self.cam_y = [], []  # A list of x and y coordinates of the cam profile for each rotation
+        self.roller_centers = []  # A list of x coordinates of the roller center
+        self.roller_x, self.roller_y = [], []  # A list of x and y coordinates for the circle of the roller
+        self.vertices = []  # Vertices of the follower
+
+        for i in range(self.motion_length):
+            cam_profile = motion.get_profile(base, thetas + i*h)
+            self.cam_x.append(cam_profile[0])
+            self.cam_y.append(cam_profile[1])
+            roller_center = _move_circle(cam_profile, roller_radius, start_point)
+            self.roller_centers.append(roller_center)
+            self.roller_x.append(circle_x + roller_center)
+            self.roller_y.append(circle_y + eccentricity)
+            start_point = (roller_center, eccentricity)
+            self.vertices.append([
+                np.array([roller_center, eccentricity + width/2]),
+                np.array([roller_center, eccentricity - width/2]),
+                np.array([roller_center + length - 0.25, eccentricity - width/2]),
+                np.array([roller_center + length, eccentricity]),
+                np.array([roller_center + length - 0.25, eccentricity + width/2])
+            ])
+
+        self.S = np.array(self.roller_centers) - np.min(self.roller_centers)
+
+    def get_bounds(self):
+        """
+        :return: The bounds of the animation
+        """
+        x_max = np.amax(self.vertices)
+        x_min = np.amin(self.cam_x)
+        y_min, y_max = np.amin(self.cam_y), np.amax(self.cam_y)
+        return (x_min, x_max), (y_min, y_max)
+
+    def plot(self, grid=True):
+        """
+        Plots the displacement of the follower alongside the cam displacement
+
+        :param grid: If true, the grid will be added to the axes object
+        :return: figure and axes object"""
+        fig, ax = plt.subplots()
+        if grid:
+            ax.grid(zorder=1)
+        ax.plot(np.rad2deg(self.motion.thetas[self.indexes]), self.S, label='Follower Displacement',
+                **self.motion.cam_plot['default'])
+        ax.plot(np.rad2deg(self.motion.thetas), self.motion.S, **self.motion.appearance)
+        ax.set_title('Follower Displacement')
+        ax.set_xlabel(r'$\theta$ (degrees)')
+        ax.set_ylabel(r'$Displacement$')
+        ax.legend()
+        return fig, ax
+
+
+class FlatFollower:
+    """
+    See the documentation for RollerFollower
+    """
+
+    def __init__(self, motion, base, thetas, inc, face_width=0, length=0, width=0, eccentricity=0):
+        self.indexes = range(0, thetas.size, inc)
+        self.motion_length = len(self.indexes)
+        self.motion = motion
+
+        h = thetas[0] - thetas[inc]
+        width = 1/8*face_width if not width else width
+        length = 2*face_width if not length else length
+
+        self.cam_x, self.cam_y = [], []
+        self.x_positions = []
+        self.vertices = []
+
+        for i in range(self.motion_length):
+            x, y = motion.get_profile(base, thetas + i*h)
+            self.cam_x.append(x)
+            self.cam_y.append(y)
+            possible = np.logical_and(y >= -(face_width/2 - eccentricity), y <= face_width/2 + eccentricity)
+            x_position = np.max(x[possible])
+            self.x_positions.append(x_position)
+            self.vertices.append([
+                np.array([x_position, face_width/2 + eccentricity]),
+                np.array([x_position, -(face_width/2 - eccentricity)]),
+                np.array([x_position + width, -(face_width/2 - eccentricity)]),
+                np.array([x_position + width, -(face_width/2 - eccentricity) + face_width/2 - width/2]),
+                np.array([x_position + length, -(face_width/2 - eccentricity) + face_width/2 - width/2]),
+                np.array([x_position + length, -(face_width/2 - eccentricity) + face_width/2 + width/2]),
+                np.array([x_position + width, -(face_width/2 - eccentricity) + face_width/2 + width/2]),
+                np.array([x_position + width, face_width/2 + eccentricity])
+            ])
+
+        self.S = np.array(self.x_positions) - np.min(self.x_positions)
+
+    def get_bounds(self):
+        x_max = np.amax(self.vertices)
+        x_min = np.amin(self.cam_x)
+        y_min, y_max = np.amin(self.cam_y), np.amax(self.cam_y)
+        return (x_min, x_max), (y_min, y_max)
+
+    def plot(self, grid=True):
+        fig, ax = plt.subplots()
+        if grid:
+            ax.grid(zorder=1)
+        ax.plot(np.rad2deg(self.motion.thetas[self.indexes]), self.S, label='Follower Displacement',
+                **self.motion.cam_plot['default'])
+        ax.plot(np.rad2deg(self.motion.thetas), self.motion.S, **self.motion.appearance)
+        ax.set_title('Follower Displacement')
+        ax.set_xlabel(r'$\theta$ (degrees)')
+        ax.set_ylabel(r'$Displacement$')
+        ax.legend()
+
+        return fig, ax
+
+
+def _dwell_maker(h):
+    return lambda theta: h
+
+
+def _move_circle(cam_profile, r, start_point):
+    """
+    This function is responsible for keeping the roller tangent to the surface of the cam within a 1/1000th unit
+    tolerance.
+
+    :param cam_profile: The coordinates of the cam in a (2, N) format.
+    :param r: The roller radius
+    :param start_point: The point to start the circle at
+    :return: The center of the circle in the x direction to where the circle is tangent to the surface of the cam
+    """
+    cam_x, cam_y = cam_profile
+    a, b = start_point
+    inside = np.logical_and(cam_y < np.sqrt(r**2 - (cam_x - a)**2) + b, cam_y > -np.sqrt(r**2 - (cam_x - a)**2) + b)
+
+    while True:
+        if np.any(inside):
+            a += 0.001
+            np.logical_and(cam_y < np.sqrt(r**2 - (cam_x - a)**2) + b, cam_y > -np.sqrt(r**2 - (cam_x - a)**2) + b,
+                           out=inside)
+        else:
+            a -= 0.001
+            np.logical_and(cam_y < np.sqrt(r**2 - (cam_x - a)**2) + b, cam_y > -np.sqrt(r**2 - (cam_x - a)**2) + b,
+                           out=inside)
+            if np.any(inside):
+                a += 0.001
+                return a
```

### Comparing `mechanism-1.1.7/mechanism/dataframe.py` & `mechanism-1.1.8/mechanism/dataframe.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,195 +1,195 @@
-import sys
-import csv
-
-
-class Data:
-    # todo: add documentation once the class is more complete
-    def __init__(self, matrix, find_headers=False, headers=None):
-        if not isinstance(matrix, Data):
-            self.original = matrix
-            self.find_headers = find_headers
-            self.headers = headers
-            self.matrix = self._check_shape()
-            self.m, self.n = len(self.matrix), len(self.matrix[0])
-            self.shape = (self.m, self.n)
-
-            if self.headers:
-                self.data_dict = {self.headers[c]: self._construct_column(self.headers[c]) for c in range(self.n)}
-            else:
-                self.data_dict = {c: self._construct_column(c) for c in range(self.n)}
-        else:
-            self.original = matrix.original
-            self.matrix = matrix.matrix
-            self.m, self.n = matrix.m, matrix.n
-            self.shape = (self.m, self.n)
-            self.headers = matrix.headers
-            self.data_dict = matrix.data_dict
-
-    def _check_shape(self):
-        """
-        This checks the shape of a matrix. If the matrix is a 1-D list, it converts it to a 2-D matrix in which there is
-        one column. It also adjusts the shape of the matrix. If there are rows with unequal lengths, it finds the row
-        with the largest length and extends all other rows to the same length. WARNING: The added values are empty
-        strings. Attempts of performing calculations may be hinder the process if row lengths are not the same.
-
-        :return: A 2-D matrix
-        """
-        row_lengths, matrix = [], []
-        for r in self.original:
-            try:
-                if not isinstance(r, list):
-                    r = list(r)
-                row_lengths.append(len(r))
-                matrix.append(r)
-            except Exception:
-                r = [r]
-                row_lengths.append(1)
-                matrix.append(r)
-        n = max(row_lengths)
-        for r in matrix:
-            for _ in range(n - len(r)):
-                r.append('')
-
-        if self.find_headers and not self.headers:
-            self.headers = [str(matrix[0][c]) for c in range(n)]
-            if '' in self.headers:
-                raise Exception('There cannot be an empty string in a header.')
-            return matrix[1:]
-
-        if self.headers:
-            if '' in self.headers:
-                raise Exception('There cannot be an empty string in a header.')
-        return matrix
-
-    def _construct_column(self, item):
-        """
-        Creates a generator for specified column. Used for the __getitem__ special method.
-
-        :param item: The column header or the column index if there are no headers.
-        :return: A generator for the column of data
-        """
-        if self.headers:
-            c = self.headers.index(item)
-            for r in range(self.m):
-                yield self.matrix[r][c]
-        else:
-            for r in range(self.m):
-                yield self.matrix[r][item]
-
-    def print(self, table=False, underline=False, columns=None):
-        """
-        Prints out the dataframe in a presentable manner. If there are headers, then they will automatically be printed.
-        If there are headers, but a columns argument is specified, then the headers will be overwritten. These actions
-        do not change the original matrix.
-
-        :param table: Prints a table style.
-        :param underline: Underlines the first row. Doesn't change the original matrix.
-        :param columns: This is a list. Inserts a header if desired. Doesn't change the original matrix.
-        """
-        m, n = self.m, self.n
-        string_matrix = [[str(self.matrix[r][c]).replace('\n', ' ').replace('\t', '    ') for c in range(n)] for r in range(m)]
-
-        if columns:
-            for _ in range(n - len(columns)):
-                columns.append('')
-            string_matrix.insert(0, columns)
-            m += 1
-
-        if self.headers and not columns:
-            string_matrix.insert(0, self.headers)
-            m += 1
-
-        if table and not self.headers and not columns:
-            string_matrix.insert(0, ['' for _ in range(n)])
-            m += 1
-
-        if underline or table:
-            underlines = ['-'*len(string_matrix[0][c]) for c in range(len(string_matrix[0]))]
-            string_matrix.insert(1, underlines)
-            m += 1
-
-        column_widths = [max([len(string_matrix[r][c]) for r in range(m)]) for c in range(n)]  # Column widths in characters
-
-        for r in range(m):
-            for c in range(n):
-                value = string_matrix[r][c]
-                space = column_widths[c] - len(value)
-                if c == n - 1:
-                    if table:
-                        if r != 1:
-                            sys.stdout.write(value)
-                        else:
-                            sys.stdout.write(value + '-'*space)
-                    else:
-                        sys.stdout.write(value)
-                else:
-                    if table:
-                        if r != 1:
-                            sys.stdout.write(value + ' '*space + ' | ')
-                        else:
-                            sys.stdout.write(value + '-'*space + '-+-')
-                    else:
-                        sys.stdout.write(value + ' '*(space + 3))
-            sys.stdout.write('\n')
-
-    def write_to_csv(self, csv_file):
-        """
-        Created a csv file for the matrix. Does include the headers if they exist.
-
-        :param csv_file: The path to desired csv file
-        :return:
-        """
-        with open(csv_file, 'w', newline='') as f:
-            writer = csv.writer(f)
-            if self.headers:
-                matrix = self.matrix[:]
-                matrix.insert(0, self.headers)
-            else:
-                matrix = self.matrix[:]
-            writer.writerows(matrix)
-
-    def __repr__(self):
-        return f'Data(m={self.m}, n={self.n}, headers={self.headers})'
-
-    def __getitem__(self, item):
-        return list(self.data_dict[item])
-
-
-def print_matrix(mat, **kwargs):
-    """
-    Prints out a matrix in a presentable manner. If the matrix is being printed multiple times, consider printing from
-    a declared object.
-
-    :param mat: Matrix to print
-    :param kwargs: See Data.print() method.
-    """
-    Data(mat).print(**kwargs)
-
-
-def read_csv(csv_file, delimiter=',', find_headers=True, floats=True):
-    """
-    Reads and returns a Data object.
-
-    :param csv_file: Path to the csv file
-    :param delimiter: The delimiter
-    :param find_headers: Specifies whether or not the first row should be taken to be the header.
-    :param floats: choose weather or not to try to convert numerical values into floats
-    :return: A Data object
-    """
-    with open(csv_file, 'r') as f:
-        if not floats:
-            return Data(list(csv.reader(f, delimiter=delimiter)), find_headers=find_headers)
-        else:
-            lines = list(csv.reader(f, delimiter=delimiter))
-            for r in range(len(lines)):
-                for c in range(len(lines[0])):
-                    try:
-                        lines[r][c] = float(lines[r][c])
-                    except Exception:
-                        pass
-            return Data(lines, find_headers=find_headers)
-
-
-def augment():
-    # todo: this is something useful that could be added later
-    pass
+import sys
+import csv
+
+
+class Data:
+    # todo: add documentation once the class is more complete
+    def __init__(self, matrix, find_headers=False, headers=None):
+        if not isinstance(matrix, Data):
+            self.original = matrix
+            self.find_headers = find_headers
+            self.headers = headers
+            self.matrix = self._check_shape()
+            self.m, self.n = len(self.matrix), len(self.matrix[0])
+            self.shape = (self.m, self.n)
+
+            if self.headers:
+                self.data_dict = {self.headers[c]: self._construct_column(self.headers[c]) for c in range(self.n)}
+            else:
+                self.data_dict = {c: self._construct_column(c) for c in range(self.n)}
+        else:
+            self.original = matrix.original
+            self.matrix = matrix.matrix
+            self.m, self.n = matrix.m, matrix.n
+            self.shape = (self.m, self.n)
+            self.headers = matrix.headers
+            self.data_dict = matrix.data_dict
+
+    def _check_shape(self):
+        """
+        This checks the shape of a matrix. If the matrix is a 1-D list, it converts it to a 2-D matrix in which there is
+        one column. It also adjusts the shape of the matrix. If there are rows with unequal lengths, it finds the row
+        with the largest length and extends all other rows to the same length. WARNING: The added values are empty
+        strings. Attempts of performing calculations may be hinder the process if row lengths are not the same.
+
+        :return: A 2-D matrix
+        """
+        row_lengths, matrix = [], []
+        for r in self.original:
+            try:
+                if not isinstance(r, list):
+                    r = list(r)
+                row_lengths.append(len(r))
+                matrix.append(r)
+            except Exception:
+                r = [r]
+                row_lengths.append(1)
+                matrix.append(r)
+        n = max(row_lengths)
+        for r in matrix:
+            for _ in range(n - len(r)):
+                r.append('')
+
+        if self.find_headers and not self.headers:
+            self.headers = [str(matrix[0][c]) for c in range(n)]
+            if '' in self.headers:
+                raise Exception('There cannot be an empty string in a header.')
+            return matrix[1:]
+
+        if self.headers:
+            if '' in self.headers:
+                raise Exception('There cannot be an empty string in a header.')
+        return matrix
+
+    def _construct_column(self, item):
+        """
+        Creates a generator for specified column. Used for the __getitem__ special method.
+
+        :param item: The column header or the column index if there are no headers.
+        :return: A generator for the column of data
+        """
+        if self.headers:
+            c = self.headers.index(item)
+            for r in range(self.m):
+                yield self.matrix[r][c]
+        else:
+            for r in range(self.m):
+                yield self.matrix[r][item]
+
+    def print(self, table=False, underline=False, columns=None):
+        """
+        Prints out the dataframe in a presentable manner. If there are headers, then they will automatically be printed.
+        If there are headers, but a columns argument is specified, then the headers will be overwritten. These actions
+        do not change the original matrix.
+
+        :param table: Prints a table style.
+        :param underline: Underlines the first row. Doesn't change the original matrix.
+        :param columns: This is a list. Inserts a header if desired. Doesn't change the original matrix.
+        """
+        m, n = self.m, self.n
+        string_matrix = [[str(self.matrix[r][c]).replace('\n', ' ').replace('\t', '    ') for c in range(n)] for r in range(m)]
+
+        if columns:
+            for _ in range(n - len(columns)):
+                columns.append('')
+            string_matrix.insert(0, columns)
+            m += 1
+
+        if self.headers and not columns:
+            string_matrix.insert(0, self.headers)
+            m += 1
+
+        if table and not self.headers and not columns:
+            string_matrix.insert(0, ['' for _ in range(n)])
+            m += 1
+
+        if underline or table:
+            underlines = ['-'*len(string_matrix[0][c]) for c in range(len(string_matrix[0]))]
+            string_matrix.insert(1, underlines)
+            m += 1
+
+        column_widths = [max([len(string_matrix[r][c]) for r in range(m)]) for c in range(n)]  # Column widths in characters
+
+        for r in range(m):
+            for c in range(n):
+                value = string_matrix[r][c]
+                space = column_widths[c] - len(value)
+                if c == n - 1:
+                    if table:
+                        if r != 1:
+                            sys.stdout.write(value)
+                        else:
+                            sys.stdout.write(value + '-'*space)
+                    else:
+                        sys.stdout.write(value)
+                else:
+                    if table:
+                        if r != 1:
+                            sys.stdout.write(value + ' '*space + ' | ')
+                        else:
+                            sys.stdout.write(value + '-'*space + '-+-')
+                    else:
+                        sys.stdout.write(value + ' '*(space + 3))
+            sys.stdout.write('\n')
+
+    def write_to_csv(self, csv_file):
+        """
+        Created a csv file for the matrix. Does include the headers if they exist.
+
+        :param csv_file: The path to desired csv file
+        :return:
+        """
+        with open(csv_file, 'w', newline='') as f:
+            writer = csv.writer(f)
+            if self.headers:
+                matrix = self.matrix[:]
+                matrix.insert(0, self.headers)
+            else:
+                matrix = self.matrix[:]
+            writer.writerows(matrix)
+
+    def __repr__(self):
+        return f'Data(m={self.m}, n={self.n}, headers={self.headers})'
+
+    def __getitem__(self, item):
+        return list(self.data_dict[item])
+
+
+def print_matrix(mat, **kwargs):
+    """
+    Prints out a matrix in a presentable manner. If the matrix is being printed multiple times, consider printing from
+    a declared object.
+
+    :param mat: Matrix to print
+    :param kwargs: See Data.print() method.
+    """
+    Data(mat).print(**kwargs)
+
+
+def read_csv(csv_file, delimiter=',', find_headers=True, floats=True):
+    """
+    Reads and returns a Data object.
+
+    :param csv_file: Path to the csv file
+    :param delimiter: The delimiter
+    :param find_headers: Specifies whether or not the first row should be taken to be the header.
+    :param floats: choose weather or not to try to convert numerical values into floats
+    :return: A Data object
+    """
+    with open(csv_file, 'r') as f:
+        if not floats:
+            return Data(list(csv.reader(f, delimiter=delimiter)), find_headers=find_headers)
+        else:
+            lines = list(csv.reader(f, delimiter=delimiter))
+            for r in range(len(lines)):
+                for c in range(len(lines[0])):
+                    try:
+                        lines[r][c] = float(lines[r][c])
+                    except Exception:
+                        pass
+            return Data(lines, find_headers=find_headers)
+
+
+def augment():
+    # todo: this is something useful that could be added later
+    pass
```

### Comparing `mechanism-1.1.7/mechanism/gears.py` & `mechanism-1.1.8/mechanism/gears.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,298 +1,298 @@
-import csv
-import json
-import warnings
-
-import matplotlib.pyplot as plt
-import numpy as np
-from scipy.optimize import fsolve
-
-from .dataframe import Data
-from .vectors import APPEARANCE
-
-
-class SpurGear:
-    with open(APPEARANCE, 'r') as f:
-        appearance = json.load(f)
-
-    gear_appearance = appearance['gear_plot']
-
-    def __init__(self, N=0, pd=0, d=0, pressure_angle=20, agma=False, a=0, b=0, backlash=0, internal=False,
-                 ignore_undercut=False, size=300):
-        """
-        In order to fully define the gear,
-        - at least two of the following should be defined: N, pd, and d
-        - pressure angle needs to be declared (default value is 20)
-        - addendum and dedendum needs to be defined (declaring agma to be true will automatically do this)
-
-        If backlash is set to zero, and agma is set to True, a non-conservative approximation of the backlash will be
-        calculated. If it is desired to override the calculated value of the backlash when agma is set to true, then
-        provide a value of the backlash that is not equal to zero.
-
-        :param N: The number of teeth of the gear
-        :param pd: The diametral pitch of the gear
-        :param d: The pitch diameter of the gear
-        :param pressure_angle: The angle at which the line of action propagates in the gear mesh
-        :param agma: If true, then the addendum, dedendum, and tooth thickness will be calculated according to their
-                     standards
-        :param a: The addendum of the tooth; the radial distance above the pitch radius
-        :param b: The dedendum of the tooth; the radial distance below the pitch radius; the difference between the
-                  dedendum and the addendum are the clearance
-        :param backlash: This is the difference between the space width and the tooth thickness. Both the space width
-                         and the tooth thickness are arc length measurements along the pitch circle. If backlash is not
-                         specified and agma is set to true, the backlash will give a non-conservative estimate for the
-                         backlash. Backlash, however, can be specified and agma set to true.
-        :param internal: If true, the involute will be based off an internal gear, in which the teeth are holes and
-                         everything around it gets filled. Internal gears are the inverse of external gears. When this
-                         happens, backlash needs to make the tooth profile wider instead of smaller. Also, the dedendum
-                         and addendum circles are switched. See Shigley's Machine Design 11th Edition page 688.
-        :param ignore_undercut: If true, the undercut warning will be ignored. This occurs when the dedendum is large
-                                enough to extend passed the base circle.
-        :param size: The size of one involute curve; make this smaller in some cases if SolidWorks says that the points
-                     are too close. Default value is 300.
-
-        Instance Attributes
-        -------------------
-        r_base: The base radius of the tooth
-        ra: The addendum radius of the tooth
-        rb: The dedendum radius of the tooth
-        tooth_thickness: The arc length of the tooth about the pitch circle
-        space_width: The arc length between two teeth about the pitch circle
-
-        The following are np.ndarrays of complex numbers; use np.real() and np.imag() to get x and y components:
-        involute_points: The involute curve in the vertical position
-        involute_reflection: The involute curve points reflected about the y-axis
-        tooth_profile: All the coordinates of the tooth starting on the right side
-
-        Useful Methods to Mention
-        -------------------------
-        plot: Shows a plot of the tooth profile
-        save_coordinates: Saves the coordinates to a file
-        rundown: Prints out a table of the key properties of the tooth
-        """
-        self.pressure_angle = np.deg2rad(pressure_angle)
-        assert isinstance(N, int), 'Number of teeth must be an integer.'
-
-        if N and pd:
-            self.N, self.pd = N, pd
-            self.d = N/pd
-        elif N and d:
-            self.N, self.d = N, d
-            self.pd = N/d
-        elif d and pd:
-            self.d, self.pd = d, pd
-            self.N = pd*d
-            if isinstance(self.N, float):
-                assert self.N.is_integer(), 'The calculated number of teeth is not registering as an integer. ' \
-                                            'Try inputting the number of teeth instead in the case of floating point ' \
-                                            'error.'
-                self.N = int(self.N)
-        else:
-            raise Exception('Not enough information given between N, pd, and d.')
-
-        self.r = self.d/2
-        self.r_base = self.r*np.cos(self.pressure_angle)
-
-        self.internal = internal
-
-        if agma:
-            assert pressure_angle == 20 or pressure_angle == 25, 'AGMA standards only apply to 20 or 25 degree ' \
-                                                                 'pressure angles.'
-            if self.pd >= 20:
-                assert pressure_angle == 20, 'For diametral pitches greater than or equal to 20, the pressure angles ' \
-                                             'must be 20 degrees.'
-            self.a, self.b = 1/self.pd, 1.25/self.pd
-            # Using this from the text sometimes results in negative backlashes, which doesn't make sense with external
-            # gears. This comes from Design of Machinery, but I'm not convinced that this should be used. More research
-            # is required.
-            # self.tooth_thickness = 1.571/self.pd
-            # self.space_width = 2*np.pi*self.r/self.N - self.tooth_thickness
-            # self.backlash = self.space_width - self.tooth_thickness
-
-            if not internal:
-                self.backlash = 0.04/self.pd
-                self.tooth_thickness = np.pi*self.r/self.N - 1/2*self.backlash
-                self.space_width = self.backlash + self.tooth_thickness
-            else:
-                self.backlash = 0.04/self.pd
-                self.tooth_thickness = np.pi*self.r/self.N + 1/2*self.backlash
-                self.space_width = -self.backlash + self.tooth_thickness
-
-            if backlash:
-                self.backlash = backlash
-                # A negative backlash would imply that the user wants an internal/ring gear. If this is the case, then
-                # widening the profile is desired, since the space for a normal gear is now void.
-                assert backlash >= 0, 'Use a positive value for backlash.'
-                backlash = backlash if not internal else -backlash
-                self.tooth_thickness = np.pi*self.r/self.N - 1/2*backlash
-                self.space_width = backlash + self.tooth_thickness
-        else:
-            self.a, self.b = a, b
-            assert a > 0 and b > 0, 'Addendum and dedendum need to be defined if the agma argument is not present.'
-            self.backlash = backlash
-            assert backlash >= 0, 'Use a positive value for backlash.'
-            backlash = backlash if not internal else -backlash
-            self.tooth_thickness = np.pi*self.r/self.N - 1/2*backlash
-            self.space_width = backlash + self.tooth_thickness
-
-        if not internal:
-            ra, rb = self.r + self.a, self.r - self.b
-            self.ra, self.rb = self.r + self.a, self.r - self.b
-        else:
-            # rb and ra are not the actual values of the addendum and dedendum circles, but are presented here to make
-            # the math work out without adding a considerable amount of conditional statements.
-            ra, rb = self.r + self.b, self.r - self.a
-            self.ra, self.rb = self.r - self.a, self.r + self.b
-
-        if rb < self.r_base and not ignore_undercut:
-            warnings.warn('The dedendum circle radius is less than the base circle radius. Undercutting will occur. To '
-                          'fix this, make the gear bigger by increasing the pitch diameter or number of teeth. To '
-                          'ignore this warning, pass "ignore_undercut=True" at the declaration of the gear object.',
-                          RuntimeWarning)
-
-        # Get the involute curve coming out of the positive x-axis, then rotate the points.
-        # Getting the angle for the point at the pitch circle
-        theta_pitch = np.sqrt((self.r/self.r_base)**2 - 1)
-        x_pitch = self._x_inv(theta_pitch)
-        y_pitch = self._y_inv(theta_pitch)
-        theta_pitch = np.angle((x_pitch + 1j*y_pitch))
-
-        # Get the angle corresponding to the circular tooth thickness and the amount needed to rotate the tooth
-        pitch_angle = self.tooth_thickness/self.r
-        rotation = np.pi/2 - theta_pitch - pitch_angle/2
-
-        # Get the involute curve. Create just a linear relationship if the dedendum radius is less than the base radius.
-        # See the planetary gear branch in the gear bearing repository as this is quite complex to pick up again.
-        if rb >= self.r_base:
-            theta_min = np.sqrt((rb/self.r_base)**2 - 1)  # Relationship is a result of converting to polar form
-            theta_max = np.sqrt((ra/self.r_base)**2 - 1)
-            thetas = np.linspace(theta_min, theta_max, size)
-            x = self._x_inv(thetas)
-            y = self._y_inv(thetas)
-        else:
-            theta_max = np.sqrt((ra/self.r_base)**2 - 1)
-            # Using the absolute value because this does some funky stuff sometimes, but only when there is a greater
-            # portion of the gear under the base circle.
-            theta_min = np.abs(fsolve(self._solve_theta_min, np.array([theta_max, ]), args=(rb, )))[0]
-            theta1 = np.flip(np.linspace(0, theta_min, int(size/2)))
-            x1 = 2*self.r_base - self._x_inv(theta1)
-            y1 = self._y_inv(theta1)
-            theta2 = np.linspace(theta1[0] - theta1[1], theta_max, int(size/2))
-            x2 = self._x_inv(theta2)
-            y2 = self._y_inv(theta2)
-            x = np.concatenate((x1, x2))
-            y = np.concatenate((y1, y2))
-
-        involute_points = x + 1j*y
-
-        # Rotate the involute curve and get the reflection/addendum circle
-        self.involute_points = _rotate(involute_points, rotation)
-        self.involute_reflection = -1*np.real(self.involute_points) + 1j*np.imag(self.involute_points)
-        addendum_start = np.angle(self.involute_points[-1])
-        addendum_end = np.angle(self.involute_reflection[-1])
-        addendum_circle = ra*np.exp(1j*np.linspace(addendum_start, addendum_end, size))
-
-        # Construct the tooth profile
-        self.tooth_profile = np.concatenate((self.involute_points, addendum_circle[1:-1],
-                                             np.flip(self.involute_reflection)))
-
-    def plot(self, grid=True):
-        """
-        Shows a plot of the gear tooth.
-        :param grid: If true, the grid will be added to the axes object
-        :return: figure and axes objects
-        """
-        between_teeth = 2*np.pi/self.N
-        dedendum_angle = np.angle(self.involute_reflection[0]) - np.angle(self.involute_points[0])
-        cushion_angle = (between_teeth - dedendum_angle)/2
-
-        angle_start = np.angle(self.involute_points[0]) - cushion_angle
-        angle_end = np.angle(self.involute_reflection[0]) + cushion_angle
-        dedendum_draw = np.linspace(angle_start, np.angle(self.involute_points[0]), 1000)
-        thetas = np.linspace(angle_start, angle_end, 1000)
-
-        base = self.r_base*np.exp(1j*thetas)
-        pitch = self.r*np.exp(1j*thetas)
-        rb = self.r - self.b if not self.internal else self.r - self.a  # Not technically true
-        dedendum = rb*np.exp(1j*dedendum_draw)
-
-        fig, ax = plt.subplots()
-        if grid:
-            ax.grid(zorder=1)
-        ax.plot(np.real(base), np.imag(base), **SpurGear.gear_appearance['base'])
-        ax.plot(np.real(pitch), np.imag(pitch), **SpurGear.gear_appearance['pitch'])
-        ax.plot(np.real(self.tooth_profile), np.imag(self.tooth_profile), **SpurGear.gear_appearance['tooth'])
-        ax.plot(np.real(dedendum), np.imag(dedendum), **SpurGear.gear_appearance['tooth'])
-        ax.plot(-1*np.real(dedendum), np.imag(dedendum), **SpurGear.gear_appearance['tooth'])
-
-        ax.set_title('Spur Gear Tooth Profile')
-        ax.set_aspect('equal')
-        ax.legend()
-
-        return fig, ax
-
-    def save_coordinates(self, file='', solidworks=False):
-        """
-        Saves the coordinates to a file.
-
-        :param file: The filepath to save the coordinates to
-        :param solidworks: It true, the coordinates will be saved in a format acceptable to SolidWorks
-        """
-        with open(file, 'w', newline='') as f:
-            if solidworks:
-                writer = csv.writer(f, delimiter='\t')
-                for c_num in self.tooth_profile:
-                    writer.writerow([f'{np.real(c_num):.8f}', f'{np.imag(c_num):.8f}', 0])
-            else:
-                writer = csv.writer(f, delimiter=',')
-                writer.writerow(['x', 'y'])
-                for c_num in self.tooth_profile:
-                    writer.writerow([np.real(c_num), np.imag(c_num)])
-
-    def rundown(self):
-        """
-        Prints a table of the properties of the gear tooth.
-        """
-        info = [['Number of Teeth (N)', self.N],
-                ['Diametral Pitch (pd)', f'{self.pd:.5f}'],
-                ['Pitch Diameter (d)', f'{self.d:.5f}'],
-                ['Pitch Radius (r)', f'{self.r:.5f}'],
-                ['Pressure Angle (phi)', f'{np.rad2deg(self.pressure_angle):.5f}'],
-                ['Base Radius', f'{self.r_base:.5f}'],
-                ['Addendum (a)', f'{self.a:.5f}'],
-                ['Dedendum (b)', f'{self.b:.5f}'],
-                ['Circular Tooth Thickness', f'{self.tooth_thickness:.5f}'],
-                ['Circular Space Width', f'{self.space_width:.5f}'],
-                ['Circular Backlash', f'{self.backlash:.5f}']]
-
-        Data(info, headers=['Property', 'Value']).print(table=True)
-
-    def _x_inv(self, thetas_):
-        """
-        Calculates the x values of an involute curve.
-        """
-        return self.r_base*np.cos(thetas_) + self.r_base*thetas_*np.sin(thetas_)
-
-    def _y_inv(self, thetas_):
-        """
-        Calculates the y values of an involute curve.
-        """
-        return self.r_base*np.sin(thetas_) - self.r_base*thetas_*np.cos(thetas_)
-
-    def _solve_theta_min(self, theta_, rb_):
-        """
-        Solves for the value of theta min when the base circle is larger than the dedendum circle.
-        """
-        x_prime_ = 2*self.r_base - self._x_inv(theta_)
-        y_ = self._y_inv(theta_)
-        return np.abs(x_prime_ + 1j*y_) - rb_
-
-
-def _rotate(coords, rotation):
-    """
-    Rotates a set of complex coordinates.
-
-    :param coords: An np.ndarray of complex numbers
-    :param rotation: The angle of rotation of the coordinates in radians
-    :return: An np.ndarray of complex numbers that is rotated the amount of 'rotation'
-    """
-    return np.abs(coords)*np.exp(1j*(np.angle(coords) + rotation))
+import csv
+import json
+import warnings
+
+import matplotlib.pyplot as plt
+import numpy as np
+from scipy.optimize import fsolve
+
+from .dataframe import Data
+from .vectors import APPEARANCE
+
+
+class SpurGear:
+    with open(APPEARANCE, 'r') as f:
+        appearance = json.load(f)
+
+    gear_appearance = appearance['gear_plot']
+
+    def __init__(self, N=0, pd=0, d=0, pressure_angle=20, agma=False, a=0, b=0, backlash=0, internal=False,
+                 ignore_undercut=False, size=300):
+        """
+        In order to fully define the gear,
+        - at least two of the following should be defined: N, pd, and d
+        - pressure angle needs to be declared (default value is 20)
+        - addendum and dedendum needs to be defined (declaring agma to be true will automatically do this)
+
+        If backlash is set to zero, and agma is set to True, a non-conservative approximation of the backlash will be
+        calculated. If it is desired to override the calculated value of the backlash when agma is set to true, then
+        provide a value of the backlash that is not equal to zero.
+
+        :param N: The number of teeth of the gear
+        :param pd: The diametral pitch of the gear
+        :param d: The pitch diameter of the gear
+        :param pressure_angle: The angle at which the line of action propagates in the gear mesh
+        :param agma: If true, then the addendum, dedendum, and tooth thickness will be calculated according to their
+                     standards
+        :param a: The addendum of the tooth; the radial distance above the pitch radius
+        :param b: The dedendum of the tooth; the radial distance below the pitch radius; the difference between the
+                  dedendum and the addendum are the clearance
+        :param backlash: This is the difference between the space width and the tooth thickness. Both the space width
+                         and the tooth thickness are arc length measurements along the pitch circle. If backlash is not
+                         specified and agma is set to true, the backlash will give a non-conservative estimate for the
+                         backlash. Backlash, however, can be specified and agma set to true.
+        :param internal: If true, the involute will be based off an internal gear, in which the teeth are holes and
+                         everything around it gets filled. Internal gears are the inverse of external gears. When this
+                         happens, backlash needs to make the tooth profile wider instead of smaller. Also, the dedendum
+                         and addendum circles are switched. See Shigley's Machine Design 11th Edition page 688.
+        :param ignore_undercut: If true, the undercut warning will be ignored. This occurs when the dedendum is large
+                                enough to extend passed the base circle.
+        :param size: The size of one involute curve; make this smaller in some cases if SolidWorks says that the points
+                     are too close. Default value is 300.
+
+        Instance Attributes
+        -------------------
+        r_base: The base radius of the tooth
+        ra: The addendum radius of the tooth
+        rb: The dedendum radius of the tooth
+        tooth_thickness: The arc length of the tooth about the pitch circle
+        space_width: The arc length between two teeth about the pitch circle
+
+        The following are np.ndarrays of complex numbers; use np.real() and np.imag() to get x and y components:
+        involute_points: The involute curve in the vertical position
+        involute_reflection: The involute curve points reflected about the y-axis
+        tooth_profile: All the coordinates of the tooth starting on the right side
+
+        Useful Methods to Mention
+        -------------------------
+        plot: Shows a plot of the tooth profile
+        save_coordinates: Saves the coordinates to a file
+        rundown: Prints out a table of the key properties of the tooth
+        """
+        self.pressure_angle = np.deg2rad(pressure_angle)
+        assert isinstance(N, int), 'Number of teeth must be an integer.'
+
+        if N and pd:
+            self.N, self.pd = N, pd
+            self.d = N/pd
+        elif N and d:
+            self.N, self.d = N, d
+            self.pd = N/d
+        elif d and pd:
+            self.d, self.pd = d, pd
+            self.N = pd*d
+            if isinstance(self.N, float):
+                assert self.N.is_integer(), 'The calculated number of teeth is not registering as an integer. ' \
+                                            'Try inputting the number of teeth instead in the case of floating point ' \
+                                            'error.'
+                self.N = int(self.N)
+        else:
+            raise Exception('Not enough information given between N, pd, and d.')
+
+        self.r = self.d/2
+        self.r_base = self.r*np.cos(self.pressure_angle)
+
+        self.internal = internal
+
+        if agma:
+            assert pressure_angle == 20 or pressure_angle == 25, 'AGMA standards only apply to 20 or 25 degree ' \
+                                                                 'pressure angles.'
+            if self.pd >= 20:
+                assert pressure_angle == 20, 'For diametral pitches greater than or equal to 20, the pressure angles ' \
+                                             'must be 20 degrees.'
+            self.a, self.b = 1/self.pd, 1.25/self.pd
+            # Using this from the text sometimes results in negative backlashes, which doesn't make sense with external
+            # gears. This comes from Design of Machinery, but I'm not convinced that this should be used. More research
+            # is required.
+            # self.tooth_thickness = 1.571/self.pd
+            # self.space_width = 2*np.pi*self.r/self.N - self.tooth_thickness
+            # self.backlash = self.space_width - self.tooth_thickness
+
+            if not internal:
+                self.backlash = 0.04/self.pd
+                self.tooth_thickness = np.pi*self.r/self.N - 1/2*self.backlash
+                self.space_width = self.backlash + self.tooth_thickness
+            else:
+                self.backlash = 0.04/self.pd
+                self.tooth_thickness = np.pi*self.r/self.N + 1/2*self.backlash
+                self.space_width = -self.backlash + self.tooth_thickness
+
+            if backlash:
+                self.backlash = backlash
+                # A negative backlash would imply that the user wants an internal/ring gear. If this is the case, then
+                # widening the profile is desired, since the space for a normal gear is now void.
+                assert backlash >= 0, 'Use a positive value for backlash.'
+                backlash = backlash if not internal else -backlash
+                self.tooth_thickness = np.pi*self.r/self.N - 1/2*backlash
+                self.space_width = backlash + self.tooth_thickness
+        else:
+            self.a, self.b = a, b
+            assert a > 0 and b > 0, 'Addendum and dedendum need to be defined if the agma argument is not present.'
+            self.backlash = backlash
+            assert backlash >= 0, 'Use a positive value for backlash.'
+            backlash = backlash if not internal else -backlash
+            self.tooth_thickness = np.pi*self.r/self.N - 1/2*backlash
+            self.space_width = backlash + self.tooth_thickness
+
+        if not internal:
+            ra, rb = self.r + self.a, self.r - self.b
+            self.ra, self.rb = self.r + self.a, self.r - self.b
+        else:
+            # rb and ra are not the actual values of the addendum and dedendum circles, but are presented here to make
+            # the math work out without adding a considerable amount of conditional statements.
+            ra, rb = self.r + self.b, self.r - self.a
+            self.ra, self.rb = self.r - self.a, self.r + self.b
+
+        if rb < self.r_base and not ignore_undercut:
+            warnings.warn('The dedendum circle radius is less than the base circle radius. Undercutting will occur. To '
+                          'fix this, make the gear bigger by increasing the pitch diameter or number of teeth. To '
+                          'ignore this warning, pass "ignore_undercut=True" at the declaration of the gear object.',
+                          RuntimeWarning)
+
+        # Get the involute curve coming out of the positive x-axis, then rotate the points.
+        # Getting the angle for the point at the pitch circle
+        theta_pitch = np.sqrt((self.r/self.r_base)**2 - 1)
+        x_pitch = self._x_inv(theta_pitch)
+        y_pitch = self._y_inv(theta_pitch)
+        theta_pitch = np.angle((x_pitch + 1j*y_pitch))
+
+        # Get the angle corresponding to the circular tooth thickness and the amount needed to rotate the tooth
+        pitch_angle = self.tooth_thickness/self.r
+        rotation = np.pi/2 - theta_pitch - pitch_angle/2
+
+        # Get the involute curve. Create just a linear relationship if the dedendum radius is less than the base radius.
+        # See the planetary gear branch in the gear bearing repository as this is quite complex to pick up again.
+        if rb >= self.r_base:
+            theta_min = np.sqrt((rb/self.r_base)**2 - 1)  # Relationship is a result of converting to polar form
+            theta_max = np.sqrt((ra/self.r_base)**2 - 1)
+            thetas = np.linspace(theta_min, theta_max, size)
+            x = self._x_inv(thetas)
+            y = self._y_inv(thetas)
+        else:
+            theta_max = np.sqrt((ra/self.r_base)**2 - 1)
+            # Using the absolute value because this does some funky stuff sometimes, but only when there is a greater
+            # portion of the gear under the base circle.
+            theta_min = np.abs(fsolve(self._solve_theta_min, np.array([theta_max, ]), args=(rb, )))[0]
+            theta1 = np.flip(np.linspace(0, theta_min, int(size/2)))
+            x1 = 2*self.r_base - self._x_inv(theta1)
+            y1 = self._y_inv(theta1)
+            theta2 = np.linspace(theta1[0] - theta1[1], theta_max, int(size/2))
+            x2 = self._x_inv(theta2)
+            y2 = self._y_inv(theta2)
+            x = np.concatenate((x1, x2))
+            y = np.concatenate((y1, y2))
+
+        involute_points = x + 1j*y
+
+        # Rotate the involute curve and get the reflection/addendum circle
+        self.involute_points = _rotate(involute_points, rotation)
+        self.involute_reflection = -1*np.real(self.involute_points) + 1j*np.imag(self.involute_points)
+        addendum_start = np.angle(self.involute_points[-1])
+        addendum_end = np.angle(self.involute_reflection[-1])
+        addendum_circle = ra*np.exp(1j*np.linspace(addendum_start, addendum_end, size))
+
+        # Construct the tooth profile
+        self.tooth_profile = np.concatenate((self.involute_points, addendum_circle[1:-1],
+                                             np.flip(self.involute_reflection)))
+
+    def plot(self, grid=True):
+        """
+        Shows a plot of the gear tooth.
+        :param grid: If true, the grid will be added to the axes object
+        :return: figure and axes objects
+        """
+        between_teeth = 2*np.pi/self.N
+        dedendum_angle = np.angle(self.involute_reflection[0]) - np.angle(self.involute_points[0])
+        cushion_angle = (between_teeth - dedendum_angle)/2
+
+        angle_start = np.angle(self.involute_points[0]) - cushion_angle
+        angle_end = np.angle(self.involute_reflection[0]) + cushion_angle
+        dedendum_draw = np.linspace(angle_start, np.angle(self.involute_points[0]), 1000)
+        thetas = np.linspace(angle_start, angle_end, 1000)
+
+        base = self.r_base*np.exp(1j*thetas)
+        pitch = self.r*np.exp(1j*thetas)
+        rb = self.r - self.b if not self.internal else self.r - self.a  # Not technically true
+        dedendum = rb*np.exp(1j*dedendum_draw)
+
+        fig, ax = plt.subplots()
+        if grid:
+            ax.grid(zorder=1)
+        ax.plot(np.real(base), np.imag(base), **SpurGear.gear_appearance['base'])
+        ax.plot(np.real(pitch), np.imag(pitch), **SpurGear.gear_appearance['pitch'])
+        ax.plot(np.real(self.tooth_profile), np.imag(self.tooth_profile), **SpurGear.gear_appearance['tooth'])
+        ax.plot(np.real(dedendum), np.imag(dedendum), **SpurGear.gear_appearance['tooth'])
+        ax.plot(-1*np.real(dedendum), np.imag(dedendum), **SpurGear.gear_appearance['tooth'])
+
+        ax.set_title('Spur Gear Tooth Profile')
+        ax.set_aspect('equal')
+        ax.legend()
+
+        return fig, ax
+
+    def save_coordinates(self, file='', solidworks=False):
+        """
+        Saves the coordinates to a file.
+
+        :param file: The filepath to save the coordinates to
+        :param solidworks: It true, the coordinates will be saved in a format acceptable to SolidWorks
+        """
+        with open(file, 'w', newline='') as f:
+            if solidworks:
+                writer = csv.writer(f, delimiter='\t')
+                for c_num in self.tooth_profile:
+                    writer.writerow([f'{np.real(c_num):.8f}', f'{np.imag(c_num):.8f}', 0])
+            else:
+                writer = csv.writer(f, delimiter=',')
+                writer.writerow(['x', 'y'])
+                for c_num in self.tooth_profile:
+                    writer.writerow([np.real(c_num), np.imag(c_num)])
+
+    def rundown(self):
+        """
+        Prints a table of the properties of the gear tooth.
+        """
+        info = [['Number of Teeth (N)', self.N],
+                ['Diametral Pitch (pd)', f'{self.pd:.5f}'],
+                ['Pitch Diameter (d)', f'{self.d:.5f}'],
+                ['Pitch Radius (r)', f'{self.r:.5f}'],
+                ['Pressure Angle (phi)', f'{np.rad2deg(self.pressure_angle):.5f}'],
+                ['Base Radius', f'{self.r_base:.5f}'],
+                ['Addendum (a)', f'{self.a:.5f}'],
+                ['Dedendum (b)', f'{self.b:.5f}'],
+                ['Circular Tooth Thickness', f'{self.tooth_thickness:.5f}'],
+                ['Circular Space Width', f'{self.space_width:.5f}'],
+                ['Circular Backlash', f'{self.backlash:.5f}']]
+
+        Data(info, headers=['Property', 'Value']).print(table=True)
+
+    def _x_inv(self, thetas_):
+        """
+        Calculates the x values of an involute curve.
+        """
+        return self.r_base*np.cos(thetas_) + self.r_base*thetas_*np.sin(thetas_)
+
+    def _y_inv(self, thetas_):
+        """
+        Calculates the y values of an involute curve.
+        """
+        return self.r_base*np.sin(thetas_) - self.r_base*thetas_*np.cos(thetas_)
+
+    def _solve_theta_min(self, theta_, rb_):
+        """
+        Solves for the value of theta min when the base circle is larger than the dedendum circle.
+        """
+        x_prime_ = 2*self.r_base - self._x_inv(theta_)
+        y_ = self._y_inv(theta_)
+        return np.abs(x_prime_ + 1j*y_) - rb_
+
+
+def _rotate(coords, rotation):
+    """
+    Rotates a set of complex coordinates.
+
+    :param coords: An np.ndarray of complex numbers
+    :param rotation: The angle of rotation of the coordinates in radians
+    :return: An np.ndarray of complex numbers that is rotated the amount of 'rotation'
+    """
+    return np.abs(coords)*np.exp(1j*(np.angle(coords) + rotation))
```

### Comparing `mechanism-1.1.7/mechanism/mechanism.py` & `mechanism-1.1.8/mechanism/mechanism.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,954 +1,959 @@
-import json
-
-import matplotlib.pyplot as plt
-from matplotlib.patches import FancyArrowPatch
-import numpy as np
-from scipy.optimize import fsolve
-
-from .dataframe import Data
-from .vectors import VectorBase, APPEARANCE
-from ._player import Player
-
-
-# going = True
-
-
-class Joint:
-    follow_all = False
-
-    def __init__(self, name='', follow=None, style=None, exclude=None, vel_arrow_kwargs=None, acc_arrow_kwargs=None,
-                 **kwargs):
-        """
-        :param: name: str; The name of the joint. Typically, a capital letter.
-        :param: follow: bool; If true, the path of the joint will be drawn in the animation.
-        :param: style: str; A named style located in the appearance json and under the 'joint_path' option.
-        :param: exclude: bool; If true, the velocity and acceleration arrows will not be displayed in plots.
-        :param: vel_arrow_kwargs: dict; kwargs to be passed into the FancyArrowPatch that makes up the velocity arrows.
-        :param: acc_arrow_kwargs: dict; kwargs to be passed into the FancyArrowPatch that makes up the acceleration
-                arrows.
-        :param: kwargs: Extra arguments that get past to plt.plot(). Useful only if follow is set to true.
-
-        Instance Variables
-        ------------------
-        x_pos, y_pos: The global x and y position of the joint
-        x_vel, y_vel: The global x and y velocity components of the joint.
-        x_acc, y_acc: The global x and y acceleration components of the joint.
-
-        x_positions, y_positions: An ndarray consisting of the x and y positions. Values get populated only when
-            the iterate() method gets called.
-        x_velocities, y_velocities: An ndarray consisting of the x and y velocities. Values get populated only when
-            the iterate() method gets called.
-        x_accelerations, y_accelerations: An ndarray consisting of the x and y accelerations. Values get populated only
-            when the iterate() method gets called.
-        vel_mags, vel_angles: An ndarray consisting of the velocity magnitudes and angles. Values get populated only
-            when the iterate() method gets called.
-        acc_mags, acc_angles: An ndarray consisting of the acceleration magnitudes and angles. Values get populated only
-            when the iterate() method gets called.
-        """
-        self.name = name
-        self.x_pos, self.y_pos = None, None
-        self.x_vel, self.y_vel = None, None
-        self.x_acc, self.y_acc = None, None
-
-        self.x_positions, self.y_positions = None, None
-        self.x_velocities, self.y_velocities = None, None
-        self.x_accelerations, self.y_accelerations = None, None
-
-        self.vel_mags, self.vel_angles = None, None
-        self.acc_mags, self.acc_angles = None, None
-
-        self._x_vel_scaled, self._y_vel_scaled = None, None
-        self._x_acc_scaled, self._y_acc_scaled = None, None
-        self._x_vel_scales, self._y_vel_scales = None, None
-        self._x_acc_scales, self._y_acc_scales = None, None
-        self._vel_heads, self._acc_heads = None, None  # array of complex numbers
-
-        if follow is None:
-            self.follow = self.follow_all
-        else:
-            self.follow = follow
-
-        with open(APPEARANCE, 'r') as f:
-            appearance = json.load(f)
-
-        if style:
-            self.kwargs = appearance['joint_path'][style]
-        elif kwargs:
-            self.kwargs = kwargs
-        else:
-            self.kwargs = appearance['joint_path']['default']
-
-        if vel_arrow_kwargs:
-            self.vel_arrow_kwargs = vel_arrow_kwargs
-        elif exclude:
-            self.vel_arrow_kwargs = dict(lw=0, mutation_scale=0)
-        else:
-            self.vel_arrow_kwargs = appearance['vel_arrow']
-
-        if acc_arrow_kwargs:
-            self.acc_arrow_kwargs = acc_arrow_kwargs
-        elif exclude:
-            self.acc_arrow_kwargs = dict(lw=0, mutation_scale=0)
-        else:
-            self.acc_arrow_kwargs = appearance['acc_arrow']
-
-    def _position_is_fixed(self):
-        """
-        :return: True if the position is globally defined.
-        """
-        return False if self.x_pos is None or self.y_pos is None else True
-
-    def _velocity_is_fixed(self):
-        """
-        :return: True if the velocity is globally defined.
-        """
-        return False if self.x_vel is None or self.y_vel is None else True
-
-    def _acceleration_is_fixed(self):
-        """
-        :return: True if the acceleration is globally defined.
-        """
-        return False if self.x_acc is None or self.y_acc is None else True
-
-    def _fix_position(self, x_pos, y_pos):
-        """
-        Sets self.x_pos and self.y_pos
-        """
-        self.x_pos, self.y_pos = x_pos, y_pos
-
-    def _fix_velocity(self, x_vel, y_vel):
-        """
-        Sets self.x_vel and self.y_vel
-        """
-        self.x_vel, self.y_vel = x_vel, y_vel
-        if abs(self.x_vel) < 1e-10:
-            self.x_vel = 0
-        if abs(self.y_vel) < 1e-10:
-            self.y_vel = 0
-
-    def _fix_acceleration(self, x_acc, y_acc):
-        """
-        Sets self.x_acc and self.y_acc
-        """
-        self.x_acc, self.y_acc = x_acc, y_acc
-        if abs(self.x_acc) < 1e-10:
-            self.x_acc = 0
-        if abs(self.y_acc) < 1e-10:
-            self.y_acc = 0
-
-    def _clear(self):
-        """
-        Clears the non-iterable instance variables. This must be called between two different calls of calculate() from
-        the mechanism instance.
-        """
-        self.x_pos, self.y_pos = None, None
-        self.x_vel, self.y_vel = None, None
-        self.x_acc, self.y_acc = None, None
-
-    def _vel_mag(self):
-        """
-        :return: A tuple of the magnitude and angle of the velocity of the joint.
-        """
-        return VectorBase(x=self.x_vel, y=self.y_vel)._get_mag()
-
-    def _acc_mag(self):
-        """
-        :return: A tuple of the magnitude and angle of the acceleration of the joint.
-        """
-        return VectorBase(x=self.x_acc, y=self.y_acc)._get_mag()
-
-    def _zero(self, s):
-        """
-        Zeros the iterable instances of the joint object.
-
-        :param s: The size of the iterable instances
-        """
-        self.x_positions, self.y_positions = np.zeros(s), np.zeros(s)
-        self.x_velocities, self.y_velocities = np.zeros(s), np.zeros(s)
-        self.x_accelerations, self.y_accelerations = np.zeros(s), np.zeros(s)
-
-        self.vel_mags, self.vel_angles = np.zeros(s), np.zeros(s)
-        self.acc_mags, self.acc_angles = np.zeros(s), np.zeros(s)
-
-    def _set_position_data(self, i):
-        """
-        Sets the position data at the index i.
-
-        :param i: Index
-        """
-        self.x_positions[i] = self.x_pos
-        self.y_positions[i] = self.y_pos
-
-    def _set_velocity_data(self, i):
-        """
-        Sets the velocity, vel_mag, and vel_angle data at the index i.
-
-        :param i: Index
-        """
-
-        self.x_velocities[i] = self.x_vel
-        self.y_velocities[i] = self.y_vel
-
-        mag, angle = self._vel_mag()
-        self.vel_mags[i] = mag
-        self.vel_angles[i] = angle
-
-    def _set_acceleration_data(self, i):
-        """
-        Sets the acceleration, acc_mag, and acc_angle data at the index i.
-
-        :param i: Index
-        """
-
-        self.x_accelerations[i] = self.x_acc
-        self.y_accelerations[i] = self.y_acc
-
-        mag, angle = self._acc_mag()
-        self.acc_mags[i] = mag
-        self.acc_angles[i] = angle
-
-    def _scale_xy(self, scale, velocity=False, acceleration=False):
-        """
-        Sets the x and y components of a length scaled by the amount 'scale'.
-        """
-        if velocity:
-            c_num = self.x_vel + 1j*self.y_vel
-            c_num = scale*np.abs(c_num)*np.exp(1j*np.angle(c_num))
-            self._x_vel_scaled, self._y_vel_scaled = np.real(c_num), np.imag(c_num)
-        elif acceleration:
-            c_num = self.x_acc + 1j*self.y_acc
-            c_num = scale*np.abs(c_num)*np.exp(1j*np.angle(c_num))
-            self._x_acc_scaled, self._y_acc_scaled = np.real(c_num), np.imag(c_num)
-
-    def _get_head_point(self, velocity=False, acceleration=False):
-        """
-        :return: returns a complex number of a global position of the scaled arrow heads
-        """
-        Rp = self.x_pos + 1j*self.y_pos
-        if velocity:
-            R_prime_p = self._x_vel_scaled + 1j*self._y_vel_scaled  # A point relative to the position of the joint
-            c_num = Rp + R_prime_p
-            return c_num
-        elif acceleration:
-            R_prime_p = self._x_acc_scaled + 1j*self._y_acc_scaled  # A point relative to the position of the joint
-            c_num = Rp + R_prime_p
-            return c_num
-
-    def _scale_xys(self, scale, velocity=False, acceleration=False):
-        """
-        Sets the x and y components of a length scaled by the amount 'scale' for all positions. Used in the animation.
-        """
-        if velocity:
-            c_nums = self.x_velocities + 1j*self.y_velocities
-            c_nums = scale*np.abs(c_nums)*np.exp(1j*np.angle(c_nums))
-            self._x_vel_scales, self._y_vel_scales = np.real(c_nums), np.imag(c_nums)
-        elif acceleration:
-            c_nums = self.x_accelerations + 1j*self.y_accelerations
-            c_nums = scale*np.abs(c_nums)*np.exp(1j*np.angle(c_nums))
-            self._x_acc_scales, self._y_acc_scales = np.real(c_nums), np.imag(c_nums)
-
-    def _get_head_points(self, velocity=False, acceleration=False):
-        """
-        Populates the head points.
-        """
-        Rp = self.x_positions + 1j*self.y_positions
-        if velocity:
-            R_prime_p = self._x_vel_scales + 1j*self._y_vel_scales  # A point relative to the position of the joint
-            self._vel_heads = Rp + R_prime_p
-        elif acceleration:
-            R_prime_p = self._x_acc_scales + 1j*self._y_acc_scales  # A point relative to the position of the joint
-            self._acc_heads = Rp + R_prime_p
-
-    def __repr__(self):
-        return f'Joint(name={self.name})'
-
-    def __str__(self):
-        return self.name
-
-
-class Mechanism:
-    def __init__(self, vectors=None, origin=None, loops=None, pos=None, vel=None, acc=None, guess=None):
-        """
-        :param vectors: tup, list; A list or tuple of vector objects.
-        :param origin: Joint; The joint object to be taken as the origin. This will be assumed to be fixed and forces
-                       a fixed frame of reference.
-        :param loops: func; This is a function of loop equations of that returns a flattened ndarray. This function is
-            used in fsolve. Essentially, a loop is defined as a set of vectors whose sum returns to the original point
-            or joint. The set of loop equations will determine how the system moves, and it is the user's responsibility
-            to provide an independent/solvable system. This means that the number of unknowns needs to match the number
-            of equations, and each loop returns two equations (one for the x direction and one for the y
-            direction). Consider an example that contains vectors 'a', 'b', 'c', etc. and has 6 unknowns. If 'x' is an
-            array that acts as a means to store the unknowns, and 'i' is the known input to the system,
-            the loop equation could look like this:
-
-            def loops(x, i):
-                temp = np.zeros((3, 2))  # Three by two matrix of zeros to act as a placeholder.
-                temp[0] = a(i) + b(i) - c(x[1]) + d(x[0])
-                temp[1] = e(x[2]) + f(x[3]) + d(x[0])
-                temp[2] = g(x[4]) - h(x[5]) + i()
-                return temp.flatten()
-
-            'a', 'b', 'c', etc. are Vector objects. The index of 'x' corresponds to a system's unknowns, which may be an
-            unknown length or angle of a vector. If a vector has an unknown length and angle, then the call signature
-            of the vector object would be 'a(r, theta)'. It takes practice to get this right, so it is best to look to
-            other examples provided.
-
-        :param pos: int, float, ndarray; Value(s) of pos for the input vector. This gets past as a second argument
-            in the loop equation. Could be an angle input or a length input. 
-        :param vel: int, float, ndarray; Value(s) of velocity for the input vector. This gets past as a second argument
-            in the loop equation when fixing the velocities of the vector objects.
-        :param acc: int, float, ndarray; Value(s) of acc for the input vector. This gets past as a second argument
-            in the loop equation when fixing the accelerations of the vector objects.
-        :param guess: list, tup; List or tuple of ndarrays. The first ndarray is the guess values for position; the
-            second is for velocity; the third is for acceleration. Only the position guess is required. If pos, vel,
-            and acc are ndarrays, then the guess value corresponds to the first value in the ndarrays.
-
-        Instance Variables
-        ------------------
-        joints: A list of Joint objects.
-        positions: A list of Position objects.
-        velocities: A list of Velocity objects.
-        accelerations: A list of Acceleration objects.
-        """
-        self.vectors, self.origin = vectors, origin
-        joints = set()
-        for v in vectors:
-            joints.update(v.joints)
-        self.joints = list(joints)
-
-        self.positions, self.velocities, self.accelerations = [], [], []
-        for v in self.vectors:
-            self.positions.append(v.pos)
-            self.velocities.append(v.vel)
-            self.accelerations.append(v.acc)
-
-        self.loops = loops
-        self.pos = pos  # Angle of the input vector
-        self.vel = vel  # Angular velocity of the input vector
-        self.acc = acc  # Angular acceleration of the input vector
-
-        self.guess = guess
-        self.dic = {v: v for v in self.vectors}
-
-        assert self.vectors, 'Vector argument not defined.'
-        assert self.origin, 'Input vector argument not defined.'
-        assert self.loops, 'Loops argument not defined.'
-        assert self.pos is not None, "pos argument must be defined."
-
-        if isinstance(self.pos, np.ndarray):
-            for v in self.vectors:
-                v._zero(self.pos.shape[0])
-
-            for j in self.joints:
-                j._zero(self.pos.shape[0])
-
-            if isinstance(self.vel, np.ndarray):
-                assert self.pos.size == self.vel.size, "vel input size does not match pos input size."
-
-            if isinstance(self.acc, np.ndarray):
-                assert self.pos.size == self.acc.size, "acc input size does not match pos input size."
-
-    def _fix_position(self):
-        """
-        Fixes the positions of all the joints assuming that all vectors are defined locally, meaning that each vector's
-        length, angle, r_dot, omega, r_ddot, and alpha are known.
-        """
-        origin = self.origin
-        origin._fix_position(0, 0)
-
-        attached_to_origin = []
-        vectors = self.positions[:]
-
-        for v in vectors:
-            if v.joints[0] == origin:
-                v._fix_global_position()
-                attached_to_origin.append(v)
-            elif v.joints[1] == origin:
-                v_rev = v._reverse()
-                v_rev._fix_global_position()
-                attached_to_origin.append(v)
-
-        for v in attached_to_origin:
-            vectors.remove(v)
-
-        counter = 0
-        while not self._position_is_fixed():
-            for v in vectors:
-                if self._position_is_fixed():
-                    break
-                for r in attached_to_origin:
-                    sum_ = get_sum(r, v)
-                    if sum_:
-                        attached_to_origin.append(sum_)
-                        sum_._fix_global_position()
-                        break
-            counter += 1
-            if counter > 10:
-                raise Exception('Not all position vectors are able to be fixed to origin. Are the all joints linked?')
-
-    def _fix_velocity(self):
-        """
-        Fixes the velocity of all the joints assuming that all vectors are defined locally, meaning that each vector's
-        length, angle, r_dot, omega, r_ddot, and alpha are known.
-        """
-        origin = self.origin
-        origin._fix_velocity(0, 0)
-
-        attached_to_origin = []
-        vectors = self.velocities[:]
-
-        for v in vectors:
-            if v.joints[0] == origin:
-                v._fix_global_velocity()
-                attached_to_origin.append(v)
-            elif v.joints[1] == origin:
-                v_rev = v._reverse()
-                v_rev._fix_global_velocity()
-                attached_to_origin.append(v)
-
-        for v in attached_to_origin:
-            vectors.remove(v)
-
-        counter = 0
-        while not self._velocity_is_fixed():
-            for v in vectors:
-                if self._velocity_is_fixed():
-                    break
-                for r in attached_to_origin:
-                    sum_ = get_sum(r, v)
-                    if sum_:
-                        attached_to_origin.append(sum_)
-                        sum_._fix_global_velocity()
-                        break
-            counter += 1
-            if counter > 10:
-                raise Exception('Not all velocity vectors are able to be fixed to origin. Are the all joints linked?')
-
-    def _fix_acceleration(self):
-        """
-        Fixes the accelerations of all the joints assuming that all vectors are defined locally, meaning that the
-        vector's length, angle, r_dot, omega, r_ddot, and alpha are known.
-        """
-        origin = self.origin
-        origin._fix_acceleration(0, 0)
-
-        attached_to_origin = []
-        vectors = self.accelerations[:]
-
-        for v in vectors:
-            if v.joints[0] == origin:
-                v._fix_global_acceleration()
-                attached_to_origin.append(v)
-            elif v.joints[1] == origin:
-                v_rev = v._reverse()
-                v_rev._fix_global_acceleration()
-                attached_to_origin.append(v)
-
-        for v in attached_to_origin:
-            vectors.remove(v)
-
-        counter = 0
-        while not self._acceleration_is_fixed():
-            for v in vectors:
-                if self._acceleration_is_fixed():
-                    break
-                for r in attached_to_origin:
-                    sum_ = get_sum(r, v)
-                    if sum_:
-                        attached_to_origin.append(sum_)
-                        sum_._fix_global_acceleration()
-                        break
-            counter += 1
-            if counter > 10:
-                raise Exception('Not all velocity vectors are able to be fixed to origin. Are the all joints linked?')
-
-    def _position_is_fixed(self):
-        """
-        :return: True if all the positions of the joints are fixed.
-        """
-        for joint in self.joints:
-            if not joint._position_is_fixed():
-                return False
-        return True
-
-    def _velocity_is_fixed(self):
-        """
-        :return: True if all the velocities of the joints are fixed.
-        """
-        for joint in self.joints:
-            if not joint._velocity_is_fixed():
-                return False
-        return True
-
-    def _acceleration_is_fixed(self):
-        """
-        :return: True if all the accelerations of the joints are fixed.
-        """
-        for joint in self.joints:
-            if not joint._acceleration_is_fixed():
-                return False
-        return True
-
-    def tables(self, position=False, velocity=False, acceleration=False, to_five=False):
-        """
-        Prints a specified data table.
-
-        :param position: bool; Print position data if set to True
-        :param velocity: bool; Print velocity data if set to True
-        :param acceleration: bool; Print acceleration data if set to True
-        :param to_five: bool; Print all data to five decimal places if set to True.
-        """
-        if position:
-            print('POSITION')
-            print('--------\n')
-            if not to_five:
-                mechanism_data = [[v, v.r, np.rad2deg(v.theta), v.x, v.y] for v in self.positions]
-                joint_data = [[j, j.x_pos, j.y_pos] for j in sorted(self.joints, key=lambda x: x.name)]
-            else:
-                mechanism_data = [[v, f'{v.r:.5f}', f'{np.rad2deg(v.theta):.5f}', f'{v.x:.5f}', f'{v.y:.5f}'] for v
-                                  in self.positions]
-                joint_data = [[j, f'{j.x_pos:.5f}', f'{j.y_pos:.5f}'] for j in
-                              sorted(self.joints, key=lambda x: x.name)]
-            Data(mechanism_data, headers=['Vector', 'R', 'Theta', 'x', 'y']).print(table=True)
-            print('')
-            Data(joint_data, headers=['Joint', 'x', 'y']).print(table=True)
-            print('')
-
-        if velocity:
-            print('VELOCITY')
-            print('--------\n')
-            if not to_five:
-                mechanism_data = [[v, v._get_mag()[0], np.rad2deg(v._get_mag()[1]), v.x, v.y] for v in
-                                  self.velocities]
-                omega_slip_data = [[v, v.omega, v.r_dot] for v in self.velocities]
-                joint_data = [[j, j._vel_mag()[0], np.rad2deg(j._vel_mag()[1]), j.x_vel, j.y_vel] for j in
-                              sorted(self.joints, key=lambda x: x.name)]
-            else:
-                mechanism_data = [[v, f'{v._get_mag()[0]:.5f}', f'{np.rad2deg(v._get_mag()[1]):.5f}', f'{v.x:.5f}',
-                                   f'{v.y:.5f}'] for v in self.velocities]
-                omega_slip_data = [[v, f'{v.omega:.5f}', f'{v.r_dot:.5f}'] for v in self.velocities]
-                joint_data = [[j, f'{j._vel_mag()[0]:.5f}', f'{np.rad2deg(j._vel_mag()[1]):.5f}', f'{j.x_vel:.5f}',
-                               f'{j.y_vel:.5f}'] for j in sorted(self.joints, key=lambda x: x.name)]
-
-            Data(mechanism_data, headers=['Vector', 'Mag', 'Angle', 'x', 'y']).print(table=True)
-            print('')
-            Data(omega_slip_data, headers=['Vector', 'Omega', 'R_dot']).print(table=True)
-            print('')
-            Data(joint_data, headers=['Joint', 'Mag', 'Angle', 'x', 'y']).print(table=True)
-            print('')
-
-        if acceleration:
-            print('ACCELERATION')
-            print('------------\n')
-            if not to_five:
-                mechanism_data = [[v, v._get_mag()[0], np.rad2deg(v._get_mag()[1]), v.x, v.y] for v in
-                                  self.accelerations]
-                alpha_slip_data = [[v, v.alpha, v.r_ddot] for v in self.accelerations]
-                joint_data = [[j, j._acc_mag()[0], np.rad2deg(j._acc_mag()[1]), j.x_acc, j.y_acc] for j in
-                              sorted(self.joints, key=lambda x: x.name)]
-
-            else:
-                mechanism_data = [
-                    [v, f'{v._get_mag()[0]:.5f}', f'{np.rad2deg(v._get_mag()[1]):.5f}', f'{v.x:.5f}', f'{v.y:.5f}'] for v
-                    in self.accelerations]
-                alpha_slip_data = [[v, f'{v.alpha:.5f}', f'{v.r_ddot:.5f}'] for v in self.accelerations]
-                joint_data = [[j, f'{j._acc_mag()[0]:.5f}', f'{np.rad2deg(j._acc_mag()[1]):.5f}', f'{j.x_acc:.5f}',
-                               f'{j.y_acc:.5f}'] for j in sorted(self.joints, key=lambda x: x.name)]
-
-            Data(mechanism_data, headers=['Vector', 'Mag', 'Angle', 'x', 'y']).print(table=True)
-            print('')
-            Data(alpha_slip_data, headers=['Vector', 'Alpha', 'R_ddot']).print(table=True)
-            print('')
-            Data(joint_data, headers=['Joint', 'Mag', 'Angle', 'x', 'y']).print(table=True)
-
-    def _find_scale(self, x_min, x_max, y_min, y_max, scale_length=0.1, kind='plot', velocity=False,
-                    acceleration=False):
-        """
-        x_min, x_max, y_min, y_max are data points that define the bounding box of the system. The 'kind' parameter
-        determine whether to find the scale for an instant "plot" or an "animation" (those are the only two possible
-        kinds). The 'velocity' and 'acceleration' parameters determines whether to find the scale for velocity or
-        acceleration. The 'scale_length' is the fraction for which the velocity/acceleration vector is to the
-        diagonal length of the bounding box.
-
-        Finds the maximum magnitude of velocity/acceleration for all joints, then returns a scale value for which to
-        scale up/down
-        the velocity arrows when plotting.
-        """
-        if kind == 'plot':
-            if velocity:
-                max_mag = max([np.sqrt(j.x_vel**2 + j.y_vel**2) for j in self.joints])
-            elif acceleration:
-                max_mag = max([np.sqrt(j.x_acc**2 + j.y_acc**2) for j in self.joints])
-            else:
-                raise Exception('Neither velocity or acceleration specified.')
-            # Diagonal of bounding box
-            max_length = np.sqrt((x_max - x_min)**2 + (y_max - y_min)**2)
-            return scale_length*max_length/max_mag
-        elif kind == 'animation':
-            if velocity:
-                vel_mags = [j.vel_mags for j in self.joints]
-                max_mag = np.amax(vel_mags)
-            elif acceleration:
-                acc_mags = [j.acc_mags for j in self.joints]
-                max_mag = np.amax(acc_mags)
-            else:
-                raise Exception('Neither velocity or acceleration specified.')
-            # Diagonal of bounding box
-            max_length = np.sqrt((x_max - x_min)**2 + (y_max - y_min)**2)
-            return scale_length*max_length/max_mag
-
-    def plot(self, velocity=False, acceleration=False, scale=0.1, show_joints=True, grid=True, cushion=1):
-        """
-        Plots the instance of the mechanism; calculate() method must be called before calling this method.
-
-        :param velocity: bool; Plots velocity vectors if True
-        :param acceleration: bool; Plots acceleration vectors if True
-        :param scale: float; If velocity or acceleration is specified, the scale will define the relative length of the
-                      maximum magnitude to the diagonal of the bounding box. A scale of 0.1 (default) would indicate
-                      that the maximum magnitude of the velocity/acceleration is 1/10 the diagonal of the bounding box.
-        :param show_joints: bool; Adds joint labels to the plot (only if velocity=False and acceleration=False)
-        :param grid: bool; Add the grid if true.
-        :param cushion: int, float; The thickness of the cushion around the plot.
-        """
-        fig, ax = plt.subplots()
-        ax.set_aspect('equal')
-
-        if grid:
-            ax.grid(zorder=1)
-
-        y_values = [j.y_pos for j in self.joints]
-        x_values = [j.x_pos for j in self.joints]
-        min_y, max_y = min(y_values), max(y_values)
-        min_x, max_x = min(x_values), max(x_values)
-
-        if velocity:
-            assert self.vel is not None, 'There is no input for velocity.'
-            sf = self._find_scale(min_x, max_x, min_y, max_y, scale_length=scale, kind='plot', velocity=True)
-            for j in self.joints:
-                j._scale_xy(sf, velocity=True)
-                c_num = j._get_head_point(velocity=True)
-                x_values.append(np.real(c_num))
-                y_values.append(np.imag(c_num))
-        if acceleration:
-            assert self.acc is not None, 'There is no input for acceleration.'
-            sf = self._find_scale(min_x, max_x, min_y, max_y, scale_length=scale, kind='plot', acceleration=True)
-            for j in self.joints:
-                j._scale_xy(sf, acceleration=True)
-                c_num = j._get_head_point(acceleration=True)
-                x_values.append(np.real(c_num))
-                y_values.append(np.imag(c_num))
-
-        min_y, max_y = min(y_values), max(y_values)
-        min_x, max_x = min(x_values), max(x_values)
-
-        ax.set_xlim(min_x - cushion, max_x + cushion)
-        ax.set_ylim(min_y - cushion, max_y + cushion)
-
-        for v in self.positions:
-            if not v.show:
-                continue
-            j1, j2 = v.joints
-            v_x = (j1.x_pos, j2.x_pos)
-            v_y = (j1.y_pos, j2.y_pos)
-            ax.plot(v_x, v_y, **v.kwargs)
-
-        for j in self.joints:
-            if velocity:
-                c_num = j._get_head_point(velocity=True)
-                arrow = FancyArrowPatch(posA=(j.x_pos, j.y_pos), posB=(np.real(c_num), np.imag(c_num)),
-                                        **j.vel_arrow_kwargs)
-                ax.add_patch(arrow)
-
-            if acceleration:
-                c_num = j._get_head_point(acceleration=True)
-                arrow = FancyArrowPatch(posA=(j.x_pos, j.y_pos), posB=(np.real(c_num), np.imag(c_num)),
-                                        **j.acc_arrow_kwargs)
-                ax.add_patch(arrow)
-            if not velocity and not acceleration and show_joints:
-                ax.annotate(j.name, (j.x_pos, j.y_pos), size='large', zorder=5)
-
-        return fig, ax
-
-    def test(self):
-        """
-        Checks the distances between joints.
-        """
-        print('Distances:')
-        for v in self.vectors:
-            j1, j2 = v.joints
-            print(f'- {j1} to {j2}: {np.sqrt((j1.x_pos - j2.x_pos)**2 + (j1.y_pos - j2.y_pos)**2)}')
-
-    def calculate(self):
-        """
-        Fixes the position of all the joints and vectors. Also fixes the velocity and acceleration data for all the
-        vectors and joints if vel and acc for the mechanism is given.
-        """
-        fsolve(self.loops, self.guess[0], args=(self.pos,))
-        self._fix_position()
-
-        if self.vel is not None:
-            for v in self.vectors:
-                v.get = v.vel.get
-                v._update_velocity()
-
-            fsolve(self.loops, self.guess[1], args=(self.vel,))
-            self._fix_velocity()
-
-        if self.acc is not None:
-            assert self.vel is not None, "vel input not defined, but necessary to solve for accelerations."
-            for v in self.vectors:
-                v.get = v.acc.get
-                v._update_acceleration()
-
-            fsolve(self.loops, self.guess[2], args=(self.acc,))
-            self._fix_acceleration()
-
-    def iterate(self):
-        """
-        Iterates over each pos, vel, and acc input, solving at each instance. Must be called before creating
-        an animation. This method must also only be used if pos, vel, and acc are ndarrays. pos argument is a
-        minimum requirement.
-        """
-        assert isinstance(self.pos, np.ndarray), "pos input is not an ndarray."
-
-        guess1 = self.guess[0]
-        guess2, guess3 = None, None
-
-        if self.vel is not None:
-            guess2 = self.guess[1]
-
-        if self.vel is not None and self.acc is not None:
-            guess3 = self.guess[2]
-
-        for i in range(self.pos.shape[0]):
-            for v in self.vectors:
-                v.get = v.pos.get
-
-            pos = fsolve(self.loops, guess1, args=(self.pos[i],))
-            guess1 = pos
-            self._fix_position()
-            for v in self.vectors:
-                v._set_position_data(i)
-
-            for j in self.joints:
-                j._set_position_data(i)
-
-            if self.vel is not None:
-                for v in self.vectors:
-                    v.get = v.vel.get
-                    v._update_velocity()
-
-                vel = fsolve(self.loops, guess2, args=(self.vel[i],))
-                guess2 = vel
-                self._fix_velocity()
-
-                for v in self.vectors:
-                    v._set_velocity_data(i)
-
-                for j in self.joints:
-                    j._set_velocity_data(i)
-
-            if self.acc is not None:
-                assert self.vel is not None, "vel input not defined, but necessary to solve for accelerations."
-                for v in self.vectors:
-                    v.get = v.acc.get
-                    v._update_acceleration()
-
-                acc = fsolve(self.loops, guess3, args=(self.acc[i],))
-                guess3 = acc
-                self._fix_acceleration()
-
-                for v in self.vectors:
-                    v._set_acceleration_data(i)
-
-                for j in self.joints:
-                    j._set_acceleration_data(i)
-
-            self.clear_joints()
-
-    def clear_joints(self):
-        """
-        Clears the joint data. Must be called between two different calls of calculate()
-        """
-        for joint in self.joints:
-            joint._clear()
-
-    def get_bounds(self):
-        """
-        :return: Two tuples; the first is the minimum and maximum x position of the mechanism, and the second is the
-            minimum and maximum y position of the mechanism.
-        """
-        x_positions = [j.x_positions for j in self.joints]
-        y_positions = [j.y_positions for j in self.joints]
-
-        x_min = np.amin(x_positions)
-        x_max = np.amax(x_positions)
-        y_min = np.amin(y_positions)
-        y_max = np.amax(y_positions)
-
-        return (x_min, x_max), (y_min, y_max)
-
-    def get_animation(self, velocity=False, acceleration=False, scale=0.1, stamp=None, stamp_loc=(0.05, 0.9),
-                      grid=True, cushion=1, show_joints=False, interval=50, mouse_buttons=True):
-        """
-        :param velocity: bool; Plots velocity vectors if True
-        :param acceleration: bool; Plots acceleration vectors if True
-        :param scale: float; If velocity or acceleration is specified, the scale will define the relative length of the
-                      maximum magnitude to the diagonal of the bounding box. A scale of 0.1 (default) would indicate
-                      that the maximum magnitude of the velocity/acceleration is 1/10 the diagonal of the bounding box.
-        :param stamp: np.ndarray; Shows a text stamp in the animation for displaying any kind of input. Must be the same
-                      size as the input and correspond to the input motion.
-        :param stamp_loc: tuple; Position of the stamp in axes transform units. A location of (0.5, 0.75) would place
-                          the stamp 50% along the x direction and 75% along the y direction.
-        :param grid: bool; Add the grid if true.
-        :param cushion: int, float; Add a cushion around the plot.
-        :param show_joints: bool; Show joint names if true.
-        :param interval: int; Delay in milliseconds between frames. Smaller values will speed up the animation.
-        :param mouse_buttons: bool; Choose to have the ability to go frame by frame or pause the animation with the
-                              mouse buttons. Use the right and left-click on a mouse to go frame by frame, and then use
-                              the scroll wheel to play and pause the animation. This is set true by default, so if you
-                              have a laptop that doesn't have a mouse, then you might want to toggle this to False if
-                              you are keep unintentionally clicking on the GUI window, and then can no longer continue
-                              the animation due to the absence of the scroll wheel.
-        :return: An animation, figure, and axes object.
-        """
-        fig, ax = plt.subplots()
-        ax.set_aspect('equal')
-        x_limits, y_limits = self.get_bounds()
-
-        vel_arrow_patches, acc_arrow_patches = [], []
-        x_points, y_points = [], []
-        if velocity:
-            assert self.vel is not None, 'There is no input for velocity.'
-            sf = self._find_scale(*(x_limits + y_limits), scale_length=scale, kind='animation', velocity=True)
-            for j in self.joints:
-                j._scale_xys(sf, velocity=True)
-                j._get_head_points(velocity=True)
-                arrow_obj = FancyArrowPatch(posA=(0, 0), posB=(0, 0), **j.vel_arrow_kwargs)
-                vel_arrow_patches.append(arrow_obj)
-                ax.add_patch(arrow_obj)
-                x_points.extend([j.x_positions, np.real(j._vel_heads)])
-                y_points.extend([j.y_positions, np.imag(j._vel_heads)])
-        if acceleration:
-            assert self.acc is not None, 'There is no input for acceleration.'
-            sf = self._find_scale(*(x_limits + y_limits), scale_length=scale, kind='animation', acceleration=True)
-            for j in self.joints:
-                j._scale_xys(sf, acceleration=True)
-                j._get_head_points(acceleration=True)
-                arrow_obj = FancyArrowPatch(posA=(0, 0), posB=(0, 0), **j.acc_arrow_kwargs)
-                acc_arrow_patches.append(arrow_obj)
-                ax.add_patch(arrow_obj)
-                x_points.append(np.real(j._acc_heads))
-                y_points.append(np.imag(j._acc_heads))
-
-        if grid:
-            ax.grid(zorder=1)
-
-        if velocity or acceleration:
-            x_min, x_max = np.amin(x_points), np.amax(x_points)
-            y_min, y_max = np.amin(y_points), np.amax(y_points)
-        else:
-            x_min, x_max = x_limits
-            y_min, y_max = y_limits
-        ax.set_xlim(x_min - cushion, x_max + cushion)
-        ax.set_ylim(y_min - cushion, y_max + cushion)
-
-        plot_dict = {}
-        joints = {}
-        for v in self.vectors:
-            if not v.pos.show:
-                continue
-
-            plot_dict.update({v.pos: ax.plot([], [], **v.pos.kwargs)[0]})
-            if show_joints:
-                for j in v.joints:
-                    joints.update({j: ax.text(x=0.0, y=0.0, s=j.name, visible=False, zorder=5)})
-
-        for j in self.joints:
-            if j.follow:
-                ax.plot(j.x_positions, j.y_positions, **j.kwargs)
-
-        text_list = []
-        if stamp is not None:
-            assert stamp.size == self.pos.shape[0], "Given stamp array doesn't match the input size."
-            text = ax.text(stamp_loc[0], stamp_loc[1], '', transform=ax.transAxes,
-                           bbox=dict(facecolor='white', edgecolor='white'), zorder=6)
-            text_list.append(text)
-
-        def init():
-            for line in plot_dict.values():
-                line.set_data([], [])
-            for j_ in joints.values():
-                j_.set(visible=True)
-            for arrow in vel_arrow_patches:
-                arrow.set_positions(posA=(0, 0), posB=(0, 0))
-            for arrow in acc_arrow_patches:
-                arrow.set_positions(posA=(0, 0), posB=(0, 0))
-            if text_list:
-                text.set_text('')
-            return list(plot_dict.values()) + vel_arrow_patches + acc_arrow_patches + text_list + list(joints.values())
-
-        def animate(i):
-            for vec, line in plot_dict.items():
-                j1, j2 = vec.joints
-                line.set_data((j1.x_positions[i], j2.x_positions[i]), (j1.y_positions[i], j2.y_positions[i]))
-                if show_joints:
-                    offset = 0.2
-                    joints[j1].set_position((j1.x_positions[i] + offset, j1.y_positions[i] + offset))
-                    joints[j2].set_position((j2.x_positions[i] + offset, j2.y_positions[i] + offset))
-            if velocity:
-                for joint, arrow in zip(self.joints, vel_arrow_patches):
-                    x_head, y_head = np.real(joint._vel_heads)[i], np.imag(joint._vel_heads)[i]
-                    arrow.set_positions(posA=(joint.x_positions[i], joint.y_positions[i]), posB=(x_head, y_head))
-            if acceleration:
-                for joint, arrow in zip(self.joints, acc_arrow_patches):
-                    x_head, y_head = np.real(joint._acc_heads)[i], np.imag(joint._acc_heads)[i]
-                    arrow.set_positions(posA=(joint.x_positions[i], joint.y_positions[i]), posB=(x_head, y_head))
-            if text_list:
-                text.set_text(f'{stamp[i]:.3f}')
-            return list(plot_dict.values()) + vel_arrow_patches + acc_arrow_patches + text_list + list(joints.values())
-
-        # noinspection PyTypeChecker
-        ani = Player(fig, animate, frames=self.pos.shape[0], interval=interval, blit=True, init_func=init,
-                     mouse_buttons=mouse_buttons)
-
-        return ani, fig, ax
-
-    def __getitem__(self, item):
-        return self.dic[item]
-
-
-def get_joints(names):
-    """
-    :param names: str; A string with the joint names separated by spaces.
-    :return: A list of joint objects.
-    """
-    return [Joint(ch) for ch in names.split()]
-
-
-def get_sum(v1, v2):
-    """
-    This function returns the sum of two vectors. It will reverse the vector(s) in such a way that it only sums the two
-    when the head of v1 is attached to the tail of v2.
-
-    :param v1: VectorBase; The vector that is attached to the origin (the tail does not have to be the origin of the
-        mechanism).
-    :param v2: VectorBase; A vector that has a common joint with v1.
-    :return: A VectorBase object sum of v1 and v2. If there are no common joints between the two, then it returns None.
-    """
-    j1, j2 = v1.joints
-    j3, j4 = v2.joints
-
-    if j2 == j3:
-        return v1 + v2
-    elif j1 == j3:
-        return v1._reverse() + v2
-    elif j1 == j4:
-        return v1._reverse() + v2._reverse()
-    elif j2 == j4:
-        return v1 + v2._reverse()
-    return None
-
-
-if __name__ == '__main__':
-    pass
+import json
+
+import matplotlib.pyplot as plt
+from matplotlib.patches import FancyArrowPatch
+import numpy as np
+from scipy.optimize import fsolve
+
+from .dataframe import Data
+from .vectors import VectorBase, APPEARANCE
+from ._player import Player
+
+
+class Joint:
+    follow_all = False
+
+    def __init__(self, name='', follow=None, style=None, exclude=None, vel_arrow_kwargs=None, acc_arrow_kwargs=None,
+                 **kwargs):
+        """
+        :param: name: str; The name of the joint. Typically, a capital letter.
+        :param: follow: bool; If true, the path of the joint will be drawn in the animation.
+        :param: style: str; A named style located in the appearance json and under the 'joint_path' option.
+        :param: exclude: bool; If true, the velocity and acceleration arrows will not be displayed in plots.
+        :param: vel_arrow_kwargs: dict; kwargs to be passed into the FancyArrowPatch that makes up the velocity arrows.
+        :param: acc_arrow_kwargs: dict; kwargs to be passed into the FancyArrowPatch that makes up the acceleration
+                arrows.
+        :param: kwargs: Extra arguments that get past to plt.plot(). Useful only if follow is set to true.
+
+        Instance Variables
+        ------------------
+        x_pos, y_pos: The global x and y position of the joint
+        x_vel, y_vel: The global x and y velocity components of the joint.
+        x_acc, y_acc: The global x and y acceleration components of the joint.
+
+        x_positions, y_positions: An ndarray consisting of the x and y positions. Values get populated only when
+            the iterate() method gets called.
+        x_velocities, y_velocities: An ndarray consisting of the x and y velocities. Values get populated only when
+            the iterate() method gets called.
+        x_accelerations, y_accelerations: An ndarray consisting of the x and y accelerations. Values get populated only
+            when the iterate() method gets called.
+        vel_mags, vel_angles: An ndarray consisting of the velocity magnitudes and angles. Values get populated only
+            when the iterate() method gets called.
+        acc_mags, acc_angles: An ndarray consisting of the acceleration magnitudes and angles. Values get populated only
+            when the iterate() method gets called.
+        """
+        self.name = name
+        self.x_pos, self.y_pos = None, None
+        self.x_vel, self.y_vel = None, None
+        self.x_acc, self.y_acc = None, None
+
+        self.x_positions, self.y_positions = None, None
+        self.x_velocities, self.y_velocities = None, None
+        self.x_accelerations, self.y_accelerations = None, None
+
+        self.vel_mags, self.vel_angles = None, None
+        self.acc_mags, self.acc_angles = None, None
+
+        self._x_vel_scaled, self._y_vel_scaled = None, None
+        self._x_acc_scaled, self._y_acc_scaled = None, None
+        self._x_vel_scales, self._y_vel_scales = None, None
+        self._x_acc_scales, self._y_acc_scales = None, None
+        self._vel_heads, self._acc_heads = None, None  # array of complex numbers
+
+        if follow is None:
+            self.follow = self.follow_all
+        else:
+            self.follow = follow
+
+        with open(APPEARANCE, 'r') as f:
+            appearance = json.load(f)
+
+        if style:
+            self.kwargs = appearance['joint_path'][style]
+        elif kwargs:
+            self.kwargs = kwargs
+        else:
+            self.kwargs = appearance['joint_path']['default']
+
+        if vel_arrow_kwargs:
+            self.vel_arrow_kwargs = vel_arrow_kwargs
+        elif exclude:
+            self.vel_arrow_kwargs = dict(lw=0, mutation_scale=0)
+        else:
+            self.vel_arrow_kwargs = appearance['vel_arrow']
+
+        if acc_arrow_kwargs:
+            self.acc_arrow_kwargs = acc_arrow_kwargs
+        elif exclude:
+            self.acc_arrow_kwargs = dict(lw=0, mutation_scale=0)
+        else:
+            self.acc_arrow_kwargs = appearance['acc_arrow']
+
+    def _position_is_fixed(self):
+        """
+        :return: True if the position is globally defined.
+        """
+        return False if self.x_pos is None or self.y_pos is None else True
+
+    def _velocity_is_fixed(self):
+        """
+        :return: True if the velocity is globally defined.
+        """
+        return False if self.x_vel is None or self.y_vel is None else True
+
+    def _acceleration_is_fixed(self):
+        """
+        :return: True if the acceleration is globally defined.
+        """
+        return False if self.x_acc is None or self.y_acc is None else True
+
+    def _fix_position(self, x_pos, y_pos):
+        """
+        Sets self.x_pos and self.y_pos
+        """
+        self.x_pos, self.y_pos = x_pos, y_pos
+
+    def _fix_velocity(self, x_vel, y_vel):
+        """
+        Sets self.x_vel and self.y_vel
+        """
+        self.x_vel, self.y_vel = x_vel, y_vel
+        if abs(self.x_vel) < 1e-10:
+            self.x_vel = 0
+        if abs(self.y_vel) < 1e-10:
+            self.y_vel = 0
+
+    def _fix_acceleration(self, x_acc, y_acc):
+        """
+        Sets self.x_acc and self.y_acc
+        """
+        self.x_acc, self.y_acc = x_acc, y_acc
+        if abs(self.x_acc) < 1e-10:
+            self.x_acc = 0
+        if abs(self.y_acc) < 1e-10:
+            self.y_acc = 0
+
+    def _clear(self):
+        """
+        Clears the non-iterable instance variables. This must be called between two different calls of calculate() from
+        the mechanism instance.
+        """
+        self.x_pos, self.y_pos = None, None
+        self.x_vel, self.y_vel = None, None
+        self.x_acc, self.y_acc = None, None
+
+    def _vel_mag(self):
+        """
+        :return: A tuple of the magnitude and angle of the velocity of the joint.
+        """
+        return VectorBase(x=self.x_vel, y=self.y_vel)._get_mag()
+
+    def _acc_mag(self):
+        """
+        :return: A tuple of the magnitude and angle of the acceleration of the joint.
+        """
+        return VectorBase(x=self.x_acc, y=self.y_acc)._get_mag()
+
+    def _zero(self, s):
+        """
+        Zeros the iterable instances of the joint object.
+
+        :param s: The size of the iterable instances
+        """
+        self.x_positions, self.y_positions = np.zeros(s), np.zeros(s)
+        self.x_velocities, self.y_velocities = np.zeros(s), np.zeros(s)
+        self.x_accelerations, self.y_accelerations = np.zeros(s), np.zeros(s)
+
+        self.vel_mags, self.vel_angles = np.zeros(s), np.zeros(s)
+        self.acc_mags, self.acc_angles = np.zeros(s), np.zeros(s)
+
+    def _set_position_data(self, i):
+        """
+        Sets the position data at the index i.
+
+        :param i: Index
+        """
+        self.x_positions[i] = self.x_pos
+        self.y_positions[i] = self.y_pos
+
+    def _set_velocity_data(self, i):
+        """
+        Sets the velocity, vel_mag, and vel_angle data at the index i.
+
+        :param i: Index
+        """
+
+        self.x_velocities[i] = self.x_vel
+        self.y_velocities[i] = self.y_vel
+
+        mag, angle = self._vel_mag()
+        self.vel_mags[i] = mag
+        self.vel_angles[i] = angle
+
+    def _set_acceleration_data(self, i):
+        """
+        Sets the acceleration, acc_mag, and acc_angle data at the index i.
+
+        :param i: Index
+        """
+
+        self.x_accelerations[i] = self.x_acc
+        self.y_accelerations[i] = self.y_acc
+
+        mag, angle = self._acc_mag()
+        self.acc_mags[i] = mag
+        self.acc_angles[i] = angle
+
+    def _scale_xy(self, scale, velocity=False, acceleration=False):
+        """
+        Sets the x and y components of a length scaled by the amount 'scale'.
+        """
+        if velocity:
+            c_num = self.x_vel + 1j*self.y_vel
+            c_num = scale*np.abs(c_num)*np.exp(1j*np.angle(c_num))
+            self._x_vel_scaled, self._y_vel_scaled = np.real(c_num), np.imag(c_num)
+        elif acceleration:
+            c_num = self.x_acc + 1j*self.y_acc
+            c_num = scale*np.abs(c_num)*np.exp(1j*np.angle(c_num))
+            self._x_acc_scaled, self._y_acc_scaled = np.real(c_num), np.imag(c_num)
+
+    def _get_head_point(self, velocity=False, acceleration=False):
+        """
+        :return: returns a complex number of a global position of the scaled arrow heads
+        """
+        Rp = self.x_pos + 1j*self.y_pos
+        if velocity:
+            R_prime_p = self._x_vel_scaled + 1j*self._y_vel_scaled  # A point relative to the position of the joint
+            c_num = Rp + R_prime_p
+            return c_num
+        elif acceleration:
+            R_prime_p = self._x_acc_scaled + 1j*self._y_acc_scaled  # A point relative to the position of the joint
+            c_num = Rp + R_prime_p
+            return c_num
+
+    def _scale_xys(self, scale, velocity=False, acceleration=False):
+        """
+        Sets the x and y components of a length scaled by the amount 'scale' for all positions. Used in the animation.
+        """
+        if velocity:
+            c_nums = self.x_velocities + 1j*self.y_velocities
+            c_nums = scale*np.abs(c_nums)*np.exp(1j*np.angle(c_nums))
+            self._x_vel_scales, self._y_vel_scales = np.real(c_nums), np.imag(c_nums)
+        elif acceleration:
+            c_nums = self.x_accelerations + 1j*self.y_accelerations
+            c_nums = scale*np.abs(c_nums)*np.exp(1j*np.angle(c_nums))
+            self._x_acc_scales, self._y_acc_scales = np.real(c_nums), np.imag(c_nums)
+
+    def _get_head_points(self, velocity=False, acceleration=False):
+        """
+        Populates the head points.
+        """
+        Rp = self.x_positions + 1j*self.y_positions
+        if velocity:
+            R_prime_p = self._x_vel_scales + 1j*self._y_vel_scales  # A point relative to the position of the joint
+            self._vel_heads = Rp + R_prime_p
+        elif acceleration:
+            R_prime_p = self._x_acc_scales + 1j*self._y_acc_scales  # A point relative to the position of the joint
+            self._acc_heads = Rp + R_prime_p
+
+    def __repr__(self):
+        return f'Joint(name={self.name})'
+
+    def __str__(self):
+        return self.name
+
+
+class Mechanism:
+    def __init__(self, vectors=None, origin=None, loops=None, pos=None, vel=None, acc=None, guess=None):
+        """
+        :param vectors: tup, list; A list or tuple of vector objects.
+        :param origin: Joint; The joint object to be taken as the origin. This will be assumed to be fixed and forces
+                       a fixed frame of reference.
+        :param loops: func; This is a function of loop equations of that returns a flattened ndarray. This function is
+            used in fsolve. Essentially, a loop is defined as a set of vectors whose sum returns to the original point
+            or joint. The set of loop equations will determine how the system moves, and it is the user's responsibility
+            to provide an independent/solvable system. This means that the number of unknowns needs to match the number
+            of equations, and each loop returns two equations (one for the x direction and one for the y
+            direction). Consider an example that contains vectors 'a', 'b', 'c', etc. and has 6 unknowns. If 'x' is an
+            array that acts as a means to store the unknowns, and 'i' is the known input to the system,
+            the loop equation could look like this:
+
+            def loops(x, i):
+                temp = np.zeros((3, 2))  # Three by two matrix of zeros to act as a placeholder.
+                temp[0] = a(i) + b(i) - c(x[1]) + d(x[0])
+                temp[1] = e(x[2]) + f(x[3]) + d(x[0])
+                temp[2] = g(x[4]) - h(x[5]) + i()
+                return temp.flatten()
+
+            'a', 'b', 'c', etc. are Vector objects. The index of 'x' corresponds to a system's unknowns, which may be an
+            unknown length or angle of a vector. If a vector has an unknown length and angle, then the call signature
+            of the vector object would be 'a(r, theta)'. It takes practice to get this right, so it is best to look to
+            other examples provided.
+
+        :param pos: int, float, ndarray; Value(s) of pos for the input vector. This gets past as a second argument
+            in the loop equation. Could be an angle input or a length input. 
+        :param vel: int, float, ndarray; Value(s) of velocity for the input vector. This gets past as a second argument
+            in the loop equation when fixing the velocities of the vector objects.
+        :param acc: int, float, ndarray; Value(s) of acc for the input vector. This gets past as a second argument
+            in the loop equation when fixing the accelerations of the vector objects.
+        :param guess: list, tup; List or tuple of ndarrays. The first ndarray is the guess values for position; the
+            second is for velocity; the third is for acceleration. Only the position guess is required. If pos, vel,
+            and acc are ndarrays, then the guess value corresponds to the first value in the ndarrays.
+
+        Instance Variables
+        ------------------
+        joints: A list of Joint objects.
+        positions: A list of Position objects.
+        velocities: A list of Velocity objects.
+        accelerations: A list of Acceleration objects.
+        """
+        self.vectors, self.origin = vectors, origin
+        joints = set()
+        for v in vectors:
+            joints.update(v.joints)
+        self.joints = list(joints)
+
+        self.positions, self.velocities, self.accelerations = [], [], []
+        for v in self.vectors:
+            self.positions.append(v.pos)
+            self.velocities.append(v.vel)
+            self.accelerations.append(v.acc)
+
+        self.loops = loops
+        self.pos = pos  # Angle of the input vector
+        self.vel = vel  # Angular velocity of the input vector
+        self.acc = acc  # Angular acceleration of the input vector
+
+        self.guess = guess
+        self.dic = {v: v for v in self.vectors}
+
+        assert self.vectors, 'Vector argument not defined.'
+        assert self.origin, 'Input vector argument not defined.'
+        assert self.loops, 'Loops argument not defined.'
+        assert self.pos is not None, "pos argument must be defined."
+
+        if isinstance(self.pos, np.ndarray):
+            for v in self.vectors:
+                v._zero(self.pos.shape[0])
+
+            for j in self.joints:
+                j._zero(self.pos.shape[0])
+
+            if isinstance(self.vel, np.ndarray):
+                assert self.pos.size == self.vel.size, "vel input size does not match pos input size."
+
+            if isinstance(self.acc, np.ndarray):
+                assert self.pos.size == self.acc.size, "acc input size does not match pos input size."
+
+    def _fix_position(self):
+        """
+        Fixes the positions of all the joints assuming that all vectors are defined locally, meaning that each vector's
+        length, angle, r_dot, omega, r_ddot, and alpha are known.
+        """
+        origin = self.origin
+        origin._fix_position(0, 0)
+
+        attached_to_origin = []
+        vectors = self.positions[:]
+
+        for v in vectors:
+            if v.joints[0] == origin:
+                v._fix_global_position()
+                attached_to_origin.append(v)
+            elif v.joints[1] == origin:
+                v_rev = v._reverse()
+                v_rev._fix_global_position()
+                attached_to_origin.append(v)
+
+        for v in attached_to_origin:
+            vectors.remove(v)
+
+        counter = 0
+        while not self._position_is_fixed():
+            for v in vectors:
+                if self._position_is_fixed():
+                    break
+                for r in attached_to_origin:
+                    sum_ = get_sum(r, v)
+                    if sum_:
+                        attached_to_origin.append(sum_)
+                        sum_._fix_global_position()
+                        break
+            counter += 1
+            if counter > 10:
+                raise Exception('Not all position vectors are able to be fixed to origin. Are the all joints linked?')
+
+    def _fix_velocity(self):
+        """
+        Fixes the velocity of all the joints assuming that all vectors are defined locally, meaning that each vector's
+        length, angle, r_dot, omega, r_ddot, and alpha are known.
+        """
+        origin = self.origin
+        origin._fix_velocity(0, 0)
+
+        attached_to_origin = []
+        vectors = self.velocities[:]
+
+        for v in vectors:
+            if v.joints[0] == origin:
+                v._fix_global_velocity()
+                attached_to_origin.append(v)
+            elif v.joints[1] == origin:
+                v_rev = v._reverse()
+                v_rev._fix_global_velocity()
+                attached_to_origin.append(v)
+
+        for v in attached_to_origin:
+            vectors.remove(v)
+
+        counter = 0
+        while not self._velocity_is_fixed():
+            for v in vectors:
+                if self._velocity_is_fixed():
+                    break
+                for r in attached_to_origin:
+                    sum_ = get_sum(r, v)
+                    if sum_:
+                        attached_to_origin.append(sum_)
+                        sum_._fix_global_velocity()
+                        break
+            counter += 1
+            if counter > 10:
+                raise Exception('Not all velocity vectors are able to be fixed to origin. Are the all joints linked?')
+
+    def _fix_acceleration(self):
+        """
+        Fixes the accelerations of all the joints assuming that all vectors are defined locally, meaning that the
+        vector's length, angle, r_dot, omega, r_ddot, and alpha are known.
+        """
+        origin = self.origin
+        origin._fix_acceleration(0, 0)
+
+        attached_to_origin = []
+        vectors = self.accelerations[:]
+
+        for v in vectors:
+            if v.joints[0] == origin:
+                v._fix_global_acceleration()
+                attached_to_origin.append(v)
+            elif v.joints[1] == origin:
+                v_rev = v._reverse()
+                v_rev._fix_global_acceleration()
+                attached_to_origin.append(v)
+
+        for v in attached_to_origin:
+            vectors.remove(v)
+
+        counter = 0
+        while not self._acceleration_is_fixed():
+            for v in vectors:
+                if self._acceleration_is_fixed():
+                    break
+                for r in attached_to_origin:
+                    sum_ = get_sum(r, v)
+                    if sum_:
+                        attached_to_origin.append(sum_)
+                        sum_._fix_global_acceleration()
+                        break
+            counter += 1
+            if counter > 10:
+                raise Exception('Not all velocity vectors are able to be fixed to origin. Are the all joints linked?')
+
+    def _position_is_fixed(self):
+        """
+        :return: True if all the positions of the joints are fixed.
+        """
+        for joint in self.joints:
+            if not joint._position_is_fixed():
+                return False
+        return True
+
+    def _velocity_is_fixed(self):
+        """
+        :return: True if all the velocities of the joints are fixed.
+        """
+        for joint in self.joints:
+            if not joint._velocity_is_fixed():
+                return False
+        return True
+
+    def _acceleration_is_fixed(self):
+        """
+        :return: True if all the accelerations of the joints are fixed.
+        """
+        for joint in self.joints:
+            if not joint._acceleration_is_fixed():
+                return False
+        return True
+
+    def tables(self, position=False, velocity=False, acceleration=False, to_five=False):
+        """
+        Prints a specified data table.
+
+        :param position: bool; Print position data if set to True
+        :param velocity: bool; Print velocity data if set to True
+        :param acceleration: bool; Print acceleration data if set to True
+        :param to_five: bool; Print all data to five decimal places if set to True.
+        """
+        if position:
+            print('POSITION')
+            print('--------\n')
+            if not to_five:
+                mechanism_data = [[v, v.r, np.rad2deg(v.theta), v.x, v.y] for v in self.positions]
+                joint_data = [[j, j.x_pos, j.y_pos] for j in sorted(self.joints, key=lambda x: x.name)]
+            else:
+                mechanism_data = [[v, f'{v.r:.5f}', f'{np.rad2deg(v.theta):.5f}', f'{v.x:.5f}', f'{v.y:.5f}'] for v
+                                  in self.positions]
+                joint_data = [[j, f'{j.x_pos:.5f}', f'{j.y_pos:.5f}'] for j in
+                              sorted(self.joints, key=lambda x: x.name)]
+            Data(mechanism_data, headers=['Vector', 'R', 'Theta', 'x', 'y']).print(table=True)
+            print('')
+            Data(joint_data, headers=['Joint', 'x', 'y']).print(table=True)
+            print('')
+
+        if velocity:
+            print('VELOCITY')
+            print('--------\n')
+            if not to_five:
+                mechanism_data = [[v, v._get_mag()[0], np.rad2deg(v._get_mag()[1]), v.x, v.y] for v in
+                                  self.velocities]
+                omega_slip_data = [[v, v.omega, v.r_dot] for v in self.velocities]
+                joint_data = [[j, j._vel_mag()[0], np.rad2deg(j._vel_mag()[1]), j.x_vel, j.y_vel] for j in
+                              sorted(self.joints, key=lambda x: x.name)]
+            else:
+                mechanism_data = [[v, f'{v._get_mag()[0]:.5f}', f'{np.rad2deg(v._get_mag()[1]):.5f}', f'{v.x:.5f}',
+                                   f'{v.y:.5f}'] for v in self.velocities]
+                omega_slip_data = [[v, f'{v.omega:.5f}', f'{v.r_dot:.5f}'] for v in self.velocities]
+                joint_data = [[j, f'{j._vel_mag()[0]:.5f}', f'{np.rad2deg(j._vel_mag()[1]):.5f}', f'{j.x_vel:.5f}',
+                               f'{j.y_vel:.5f}'] for j in sorted(self.joints, key=lambda x: x.name)]
+
+            Data(mechanism_data, headers=['Vector', 'Mag', 'Angle', 'x', 'y']).print(table=True)
+            print('')
+            Data(omega_slip_data, headers=['Vector', 'Omega', 'R_dot']).print(table=True)
+            print('')
+            Data(joint_data, headers=['Joint', 'Mag', 'Angle', 'x', 'y']).print(table=True)
+            print('')
+
+        if acceleration:
+            print('ACCELERATION')
+            print('------------\n')
+            if not to_five:
+                mechanism_data = [[v, v._get_mag()[0], np.rad2deg(v._get_mag()[1]), v.x, v.y] for v in
+                                  self.accelerations]
+                alpha_slip_data = [[v, v.alpha, v.r_ddot] for v in self.accelerations]
+                joint_data = [[j, j._acc_mag()[0], np.rad2deg(j._acc_mag()[1]), j.x_acc, j.y_acc] for j in
+                              sorted(self.joints, key=lambda x: x.name)]
+
+            else:
+                mechanism_data = [
+                    [v, f'{v._get_mag()[0]:.5f}', f'{np.rad2deg(v._get_mag()[1]):.5f}', f'{v.x:.5f}', f'{v.y:.5f}'] for v
+                    in self.accelerations]
+                alpha_slip_data = [[v, f'{v.alpha:.5f}', f'{v.r_ddot:.5f}'] for v in self.accelerations]
+                joint_data = [[j, f'{j._acc_mag()[0]:.5f}', f'{np.rad2deg(j._acc_mag()[1]):.5f}', f'{j.x_acc:.5f}',
+                               f'{j.y_acc:.5f}'] for j in sorted(self.joints, key=lambda x: x.name)]
+
+            Data(mechanism_data, headers=['Vector', 'Mag', 'Angle', 'x', 'y']).print(table=True)
+            print('')
+            Data(alpha_slip_data, headers=['Vector', 'Alpha', 'R_ddot']).print(table=True)
+            print('')
+            Data(joint_data, headers=['Joint', 'Mag', 'Angle', 'x', 'y']).print(table=True)
+
+    def _find_scale(self, x_min, x_max, y_min, y_max, scale_length=0.1, kind='plot', velocity=False,
+                    acceleration=False):
+        """
+        x_min, x_max, y_min, y_max are data points that define the bounding box of the system. The 'kind' parameter
+        determine whether to find the scale for an instant "plot" or an "animation" (those are the only two possible
+        kinds). The 'velocity' and 'acceleration' parameters determines whether to find the scale for velocity or
+        acceleration. The 'scale_length' is the fraction for which the velocity/acceleration vector is to the
+        diagonal length of the bounding box.
+
+        Finds the maximum magnitude of velocity/acceleration for all joints, then returns a scale value for which to
+        scale up/down
+        the velocity arrows when plotting.
+        """
+        if kind == 'plot':
+            if velocity:
+                max_mag = max([np.sqrt(j.x_vel**2 + j.y_vel**2) for j in self.joints])
+            elif acceleration:
+                max_mag = max([np.sqrt(j.x_acc**2 + j.y_acc**2) for j in self.joints])
+            else:
+                raise Exception('Neither velocity or acceleration specified.')
+            # Diagonal of bounding box
+            max_length = np.sqrt((x_max - x_min)**2 + (y_max - y_min)**2)
+            return scale_length*max_length/max_mag
+        elif kind == 'animation':
+            if velocity:
+                vel_mags = [j.vel_mags for j in self.joints]
+                max_mag = np.amax(vel_mags)
+            elif acceleration:
+                acc_mags = [j.acc_mags for j in self.joints]
+                max_mag = np.amax(acc_mags)
+            else:
+                raise Exception('Neither velocity or acceleration specified.')
+            # Diagonal of bounding box
+            max_length = np.sqrt((x_max - x_min)**2 + (y_max - y_min)**2)
+            return scale_length*max_length/max_mag
+
+    def plot(self, velocity=False, acceleration=False, scale=0.1, show_joints=True, grid=True, cushion=1):
+        """
+        Plots the instance of the mechanism; calculate() method must be called before calling this method.
+
+        :param velocity: bool; Plots velocity vectors if True
+        :param acceleration: bool; Plots acceleration vectors if True
+        :param scale: float; If velocity or acceleration is specified, the scale will define the relative length of the
+                      maximum magnitude to the diagonal of the bounding box. A scale of 0.1 (default) would indicate
+                      that the maximum magnitude of the velocity/acceleration is 1/10 the diagonal of the bounding box.
+        :param show_joints: bool; Adds joint labels to the plot (only if velocity=False and acceleration=False)
+        :param grid: bool; Add the grid if true.
+        :param cushion: int, float; The thickness of the cushion around the plot.
+        """
+        fig, ax = plt.subplots()
+        ax.set_aspect('equal')
+
+        if grid:
+            ax.grid(zorder=1)
+
+        y_values = [j.y_pos for j in self.joints]
+        x_values = [j.x_pos for j in self.joints]
+        min_y, max_y = min(y_values), max(y_values)
+        min_x, max_x = min(x_values), max(x_values)
+
+        if velocity:
+            assert self.vel is not None, 'There is no input for velocity.'
+            sf = self._find_scale(min_x, max_x, min_y, max_y, scale_length=scale, kind='plot', velocity=True)
+            for j in self.joints:
+                j._scale_xy(sf, velocity=True)
+                c_num = j._get_head_point(velocity=True)
+                x_values.append(np.real(c_num))
+                y_values.append(np.imag(c_num))
+        if acceleration:
+            assert self.acc is not None, 'There is no input for acceleration.'
+            sf = self._find_scale(min_x, max_x, min_y, max_y, scale_length=scale, kind='plot', acceleration=True)
+            for j in self.joints:
+                j._scale_xy(sf, acceleration=True)
+                c_num = j._get_head_point(acceleration=True)
+                x_values.append(np.real(c_num))
+                y_values.append(np.imag(c_num))
+
+        min_y, max_y = min(y_values), max(y_values)
+        min_x, max_x = min(x_values), max(x_values)
+
+        ax.set_xlim(min_x - cushion, max_x + cushion)
+        ax.set_ylim(min_y - cushion, max_y + cushion)
+
+        for v in self.positions:
+            if not v.show:
+                continue
+            j1, j2 = v.joints
+            v_x = (j1.x_pos, j2.x_pos)
+            v_y = (j1.y_pos, j2.y_pos)
+            ax.plot(v_x, v_y, **v.kwargs)
+
+        for j in self.joints:
+            if velocity:
+                c_num = j._get_head_point(velocity=True)
+                arrow = FancyArrowPatch(posA=(j.x_pos, j.y_pos), posB=(np.real(c_num), np.imag(c_num)),
+                                        **j.vel_arrow_kwargs)
+                ax.add_patch(arrow)
+
+            if acceleration:
+                c_num = j._get_head_point(acceleration=True)
+                arrow = FancyArrowPatch(posA=(j.x_pos, j.y_pos), posB=(np.real(c_num), np.imag(c_num)),
+                                        **j.acc_arrow_kwargs)
+                ax.add_patch(arrow)
+            if not velocity and not acceleration and show_joints:
+                ax.annotate(j.name, (j.x_pos, j.y_pos), size='large', zorder=5)
+
+        return fig, ax
+
+    def test(self):
+        """
+        Checks the distances between joints.
+        """
+        print('Distances:')
+        for v in self.vectors:
+            j1, j2 = v.joints
+            print(f'- {j1} to {j2}: {np.sqrt((j1.x_pos - j2.x_pos)**2 + (j1.y_pos - j2.y_pos)**2)}')
+
+    def calculate(self):
+        """
+        Fixes the position of all the joints and vectors. Also fixes the velocity and acceleration data for all the
+        vectors and joints if vel and acc for the mechanism is given.
+        """
+        fsolve(self.loops, self.guess[0], args=(self.pos,))
+        self._fix_position()
+
+        if self.vel is not None:
+            for v in self.vectors:
+                v.get = v.vel.get
+                v._update_velocity()
+
+            fsolve(self.loops, self.guess[1], args=(self.vel,))
+            self._fix_velocity()
+
+        if self.acc is not None:
+            assert self.vel is not None, "vel input not defined, but necessary to solve for accelerations."
+            for v in self.vectors:
+                v.get = v.acc.get
+                v._update_acceleration()
+
+            fsolve(self.loops, self.guess[2], args=(self.acc,))
+            self._fix_acceleration()
+
+    def iterate(self):
+        """
+        Iterates over each pos, vel, and acc input, solving at each instance. Must be called before creating
+        an animation. This method must also only be used if pos, vel, and acc are ndarrays. pos argument is a
+        minimum requirement.
+        """
+        assert isinstance(self.pos, np.ndarray), "pos input is not an ndarray."
+
+        guess1 = self.guess[0]
+        guess2, guess3 = None, None
+
+        if self.vel is not None:
+            guess2 = self.guess[1]
+
+        if self.vel is not None and self.acc is not None:
+            guess3 = self.guess[2]
+
+        for i in range(self.pos.shape[0]):
+            for v in self.vectors:
+                v.get = v.pos.get
+
+            pos = fsolve(self.loops, guess1, args=(self.pos[i],))
+            guess1 = pos
+            self._fix_position()
+            for v in self.vectors:
+                v._set_position_data(i)
+
+            for j in self.joints:
+                j._set_position_data(i)
+
+            if self.vel is not None:
+                for v in self.vectors:
+                    v.get = v.vel.get
+                    v._update_velocity()
+
+                vel = fsolve(self.loops, guess2, args=(self.vel[i],))
+                guess2 = vel
+                self._fix_velocity()
+
+                for v in self.vectors:
+                    v._set_velocity_data(i)
+
+                for j in self.joints:
+                    j._set_velocity_data(i)
+
+            if self.acc is not None:
+                assert self.vel is not None, "vel input not defined, but necessary to solve for accelerations."
+                for v in self.vectors:
+                    v.get = v.acc.get
+                    v._update_acceleration()
+
+                acc = fsolve(self.loops, guess3, args=(self.acc[i],))
+                guess3 = acc
+                self._fix_acceleration()
+
+                for v in self.vectors:
+                    v._set_acceleration_data(i)
+
+                for j in self.joints:
+                    j._set_acceleration_data(i)
+
+            self.clear_joints()
+
+    def clear_joints(self):
+        """
+        Clears the joint data. Must be called between two different calls of calculate()
+        """
+        for joint in self.joints:
+            joint._clear()
+
+    def get_bounds(self):
+        """
+        :return: Two tuples; the first is the minimum and maximum x position of the mechanism, and the second is the
+            minimum and maximum y position of the mechanism.
+        """
+        x_positions = [j.x_positions for j in self.joints]
+        y_positions = [j.y_positions for j in self.joints]
+
+        x_min = np.amin(x_positions)
+        x_max = np.amax(x_positions)
+        y_min = np.amin(y_positions)
+        y_max = np.amax(y_positions)
+
+        return (x_min, x_max), (y_min, y_max)
+
+    def get_animation(self, velocity=False, acceleration=False, scale=0.1, stamp=None, stamp_loc=(0.05, 0.9),
+                      grid=True, cushion=1, show_joints=False, interval=50, key_bindings=True):
+        """
+        :param velocity: bool; Plots velocity vectors if True
+        :param acceleration: bool; Plots acceleration vectors if True
+        :param scale: float; If velocity or acceleration is specified, the scale will define the relative length of the
+                      maximum magnitude to the diagonal of the bounding box. A scale of 0.1 (default) would indicate
+                      that the maximum magnitude of the velocity/acceleration is 1/10 the diagonal of the bounding box.
+        :param stamp: np.ndarray; Shows a text stamp in the animation for displaying any kind of input. Must be the same
+                      size as the input and correspond to the input motion.
+        :param stamp_loc: tuple; Position of the stamp in axes transform units. A location of (0.5, 0.75) would place
+                          the stamp 50% along the x direction and 75% along the y direction.
+        :param grid: bool; Add the grid if true.
+        :param cushion: int, float; Add a cushion around the plot.
+        :param show_joints: bool; Show joint names if true.
+        :param interval: int; Delay in milliseconds between frames. Smaller values will speed up the animation.
+        :param key_bindings: bool; Choose to have the ability to go frame by frame or pause the animation with keys. Use
+                             the right and left arrow keys to go frame by frame. Use the space bar to pause and play
+                             the animation.
+        :return: An animation, figure, and axes object.
+        """
+        fig, ax = plt.subplots()
+        ax.set_aspect('equal')
+        x_limits, y_limits = self.get_bounds()
+
+        vel_arrow_patches, acc_arrow_patches = [], []
+        x_points, y_points = [], []
+        if velocity:
+            assert self.vel is not None, 'There is no input for velocity.'
+            sf = self._find_scale(*(x_limits + y_limits), scale_length=scale, kind='animation', velocity=True)
+            for j in self.joints:
+                j._scale_xys(sf, velocity=True)
+                j._get_head_points(velocity=True)
+                arrow_obj = FancyArrowPatch(posA=(0, 0), posB=(0, 0), **j.vel_arrow_kwargs)
+                vel_arrow_patches.append(arrow_obj)
+                ax.add_patch(arrow_obj)
+                x_points.extend([j.x_positions, np.real(j._vel_heads)])
+                y_points.extend([j.y_positions, np.imag(j._vel_heads)])
+        if acceleration:
+            assert self.acc is not None, 'There is no input for acceleration.'
+            sf = self._find_scale(*(x_limits + y_limits), scale_length=scale, kind='animation', acceleration=True)
+            for j in self.joints:
+                j._scale_xys(sf, acceleration=True)
+                j._get_head_points(acceleration=True)
+                arrow_obj = FancyArrowPatch(posA=(0, 0), posB=(0, 0), **j.acc_arrow_kwargs)
+                acc_arrow_patches.append(arrow_obj)
+                ax.add_patch(arrow_obj)
+                x_points.append(np.real(j._acc_heads))
+                y_points.append(np.imag(j._acc_heads))
+
+        if grid:
+            ax.grid(zorder=1)
+
+        if velocity or acceleration:
+            x_min, x_max = np.amin(x_points), np.amax(x_points)
+            y_min, y_max = np.amin(y_points), np.amax(y_points)
+        else:
+            x_min, x_max = x_limits
+            y_min, y_max = y_limits
+        ax.set_xlim(x_min - cushion, x_max + cushion)
+        ax.set_ylim(y_min - cushion, y_max + cushion)
+
+        plot_dict = {}
+        joints = {}
+        for v in self.vectors:
+            if not v.pos.show:
+                continue
+
+            plot_dict.update({v.pos: ax.plot([], [], **v.pos.kwargs)[0]})
+            if show_joints:
+                for j in v.joints:
+                    joints.update({j: ax.text(x=0.0, y=0.0, s=j.name, visible=False, zorder=5)})
+
+        for j in self.joints:
+            if j.follow:
+                ax.plot(j.x_positions, j.y_positions, **j.kwargs)
+
+        text_list = []
+        if stamp is not None:
+            assert stamp.size == self.pos.shape[0], "Given stamp array doesn't match the input size."
+            text = ax.text(stamp_loc[0], stamp_loc[1], '', transform=ax.transAxes,
+                           bbox=dict(facecolor='white', edgecolor='white'), zorder=6)
+            text_list.append(text)
+
+        def init():
+            for line in plot_dict.values():
+                line.set_data([], [])
+            for j_ in joints.values():
+                j_.set(visible=True)
+            for arrow in vel_arrow_patches:
+                arrow.set_positions(posA=(0, 0), posB=(0, 0))
+            for arrow in acc_arrow_patches:
+                arrow.set_positions(posA=(0, 0), posB=(0, 0))
+            if text_list:
+                text.set_text('')
+            return list(plot_dict.values()) + vel_arrow_patches + acc_arrow_patches + text_list + list(joints.values())
+
+        def animate(i):
+            for vec, line in plot_dict.items():
+                j1, j2 = vec.joints
+                line.set_data((j1.x_positions[i], j2.x_positions[i]), (j1.y_positions[i], j2.y_positions[i]))
+                if show_joints:
+                    offset = 0.2
+                    joints[j1].set_position((j1.x_positions[i] + offset, j1.y_positions[i] + offset))
+                    joints[j2].set_position((j2.x_positions[i] + offset, j2.y_positions[i] + offset))
+            if velocity:
+                for joint, arrow in zip(self.joints, vel_arrow_patches):
+                    x_head, y_head = np.real(joint._vel_heads)[i], np.imag(joint._vel_heads)[i]
+                    arrow.set_positions(posA=(joint.x_positions[i], joint.y_positions[i]), posB=(x_head, y_head))
+            if acceleration:
+                for joint, arrow in zip(self.joints, acc_arrow_patches):
+                    x_head, y_head = np.real(joint._acc_heads)[i], np.imag(joint._acc_heads)[i]
+                    arrow.set_positions(posA=(joint.x_positions[i], joint.y_positions[i]), posB=(x_head, y_head))
+            if text_list:
+                text.set_text(f'{stamp[i]:.3f}')
+            return list(plot_dict.values()) + vel_arrow_patches + acc_arrow_patches + text_list + list(joints.values())
+
+        # noinspection PyTypeChecker
+        ani = Player(fig, animate, frames=self.pos.shape[0], interval=interval, blit=True, init_func=init,
+                     key_bindings=key_bindings)
+
+        return ani, fig, ax
+
+    @staticmethod
+    def exclude(joints: list[Joint]):
+        """
+        Exclude the joint velocities and accelerations from the animations.
+
+        :param joints: list[Joint]; A list of joint objects to exclude from the animations.
+        """
+        for joint in joints:
+            joint.vel_arrow_kwargs = dict(lw=0, mutation_scale=0)
+            joint.acc_arrow_kwargs = dict(lw=0, mutation_scale=0)
+
+    def __getitem__(self, item):
+        return self.dic[item]
+
+
+def get_joints(names):
+    """
+    :param names: str; A string with the joint names separated by spaces.
+    :return: A list of joint objects.
+    """
+    return [Joint(ch) for ch in names.split()]
+
+
+def get_sum(v1, v2):
+    """
+    This function returns the sum of two vectors. It will reverse the vector(s) in such a way that it only sums the two
+    when the head of v1 is attached to the tail of v2.
+
+    :param v1: VectorBase; The vector that is attached to the origin (the tail does not have to be the origin of the
+        mechanism).
+    :param v2: VectorBase; A vector that has a common joint with v1.
+    :return: A VectorBase object sum of v1 and v2. If there are no common joints between the two, then it returns None.
+    """
+    j1, j2 = v1.joints
+    j3, j4 = v2.joints
+
+    if j2 == j3:
+        return v1 + v2
+    elif j1 == j3:
+        return v1._reverse() + v2
+    elif j1 == j4:
+        return v1._reverse() + v2._reverse()
+    elif j2 == j4:
+        return v1 + v2._reverse()
+    return None
+
+
+if __name__ == '__main__':
+    pass
```

### Comparing `mechanism-1.1.7/mechanism/vectors.py` & `mechanism-1.1.8/mechanism/vectors.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,326 +1,326 @@
-import numpy as np
-import json
-import os
-
-THIS_DIR = os.path.dirname(os.path.abspath(__file__))
-APPEARANCE = os.path.join(THIS_DIR, 'appearance.json')
-
-
-class VectorBase:
-    def __init__(self, joints=None, r=None, theta=None, x=None, y=None, show=True, style=None, **kwargs):
-        """
-        :param joints: tup; A tuple of Joint objects. The first Joint is the tail, and the second is the head.
-        :param r: int, float; The length of the vector. If specified, the vector is taken to be a constant length,
-            meaning r_dot and r_ddot is zero.
-        :param theta: int, float; The angle of the vector in radians from the positive x-axis. Counterclockwise is
-            positive. If specified, the vector is directed at a constant angle, meaning omega and alpha is zero.
-        :param x: int, float; The value of the x component of the vector.
-        :param y: int, float; The value of the y component of the vector.
-        :param show: bool; If True, then the vector will be present in plots and animations.
-        :param style: str; Applies a certain style passed to plt.plot().
-            Options: 
-                ground - a dashed black line for grounded link
-                dotted - a black dotted line
-        :param kwargs: Extra arguments that are passed to plt.plot(). If not specified, the line will be maroon with a
-            marker style = 'o'
-
-        Instance Variables
-        ------------------
-        rs: An ndarray of r values.
-        thetas: An ndarray of theta values.
-        r_dots: An ndarray of r_dot values (r_dot is the rate of change of the length of the vector length with respect
-            to time).
-        omegas: An ndarray of omega values (omega is the rate of change of the angle of the vector with respect to
-            time).
-        r_ddots: An ndarray of r_ddot values (r_ddot is the rate of change of the rate of change of the vector length
-            with respect to time).
-        alphas: An ndarray of alpha values (alpha is the rate of change of the rate of change of the angle of the vector
-            with respect to time).
-        get: A function that returns the x and y component of the vector. The arguments for this function depends on
-            what is specified at the initialization of the object. For instance, if r is set to a certain value, the get
-            function will require an angle input.
-        """
-        self.joints, self.r, self.theta, self.show = joints, r, theta, show
-
-        with open(APPEARANCE, 'r') as f:
-            appearance = json.load(f)
-
-        if style:
-            self.kwargs = appearance['mechanism_plot'][style]
-        elif kwargs:
-            self.kwargs = kwargs
-        else:
-            self.kwargs = appearance['mechanism_plot']['default']
-
-        self.x, self.y = x, y
-
-        self.rs, self.thetas, self.r_dots, self.omegas, self.r_ddots, self.alphas = None, None, None, None, None, None
-
-        if self.r is not None and self.theta is not None:
-            self.r_dot, self.omega = 0, 0
-            self.r_ddot, self.alpha = 0, 0
-            self.get = self._neither
-        elif self.r is not None and self.theta is None:
-            self.r_dot, self.omega = 0, None
-            self.r_ddot, self.alpha = 0, None
-            self.get = self._tangent
-        elif self.r is None and self.theta is not None:
-            self.r_dot, self.omega = None, 0
-            self.r_ddot, self.alpha = None, 0
-            self.get = self._slip
-        else:
-            self.r_dot, self.omega = None, None
-            self.r_ddot, self.alpha = None, None
-            self.get = self._both
-
-    def _neither(self):
-        pass
-
-    def _both(self, _, __):
-        pass
-
-    def _slip(self, _):
-        pass
-
-    def _tangent(self, _):
-        pass
-
-    def _fix_global_position(self):
-        """
-        Fixes the position of the head joint by making its position the x and y components of the current instance.
-        """
-        self.joints[1]._fix_position(self.x, self.y)
-
-    def _fix_global_velocity(self):
-        """
-        Fixes the velocity of the head joint by making its velocity the x and y components of the current instance.
-        """
-        self.joints[1]._fix_velocity(self.x, self.y)
-
-    def _fix_global_acceleration(self):
-        """
-        Fixes the acceleration of the head joint by making its acceleration the x and y components of the current
-        instance.
-        """
-        self.joints[1]._fix_acceleration(self.x, self.y)
-
-    def _reverse(self):
-        """
-        :return: A VectorBase object that is reversed. The joints get reversed as well as the x and y components.
-        """
-        x, y = -self.x, -self.y
-        return VectorBase(joints=(self.joints[1], self.joints[0]), x=x, y=y)
-
-    def _get_mag(self):
-        """
-        :return: A tuple consisting of the magnitude of the current instance and the angle.
-        """
-        mag = np.sqrt(self.x ** 2 + self.y ** 2)
-
-        if self.x > 0 and self.y >= 0:
-            angle = np.arctan(self.y/self.x)
-        elif self.x < 0 and self.y >= 0:
-            angle = np.arctan(self.y/self.x) + np.pi
-        elif self.x < 0 and self.y <= 0:
-            angle = np.arctan(self.y/self.x) + np.pi
-        elif self.x > 0 and self.y <= 0:
-            angle = np.arctan(self.y/self.x) + 2*np.pi
-        elif self.x == 0 and self.y >= 0:
-            angle = np.pi/2  # when x is zero
-        else:
-            angle = 3*np.pi/2
-
-        return mag, angle
-
-    def __add__(self, other):
-        x, y = self.x + other.x, self.y + other.y
-        return VectorBase(joints=(self.joints[0], other.joints[1]), x=x, y=y)
-
-
-class Vector:
-    def __init__(self, joints=None, r=None, theta=None, x=None, y=None, show=True, style=None, **kwargs):
-        """
-        See the VectorBase class for details regarding the parameters. The purpose of this class is to group Position,
-        Velocity, and Acceleration objects.
-
-        Instance Variables
-        ------------------
-        pos: Position object which is a subclass of VectorBase. Does not include the r_dot, omega, r_ddot, and alpha
-            attributes.
-        vel: Velocity object which is a subclass of VectorBase. Does not include the r_ddot and alpha attributes.
-        acc: Acceleration object which is a subclass of VectorBase.
-        """
-        self.pos = Position(joints=joints, r=r, theta=theta, x=x, y=y, show=show, style=style, **kwargs)
-        self.vel = Velocity(joints=joints, r=r, theta=theta, x=x, y=y, show=show, style=style, **kwargs)
-        self.acc = Acceleration(joints=joints, r=r, theta=theta, x=x, y=y, show=show, style=style, **kwargs)
-
-        self.get = self.pos.get
-        self.joints = joints
-
-    def _update_velocity(self):
-        """
-        Updates the velocity object to include the length, r, and the angle ,theta.
-        """
-        self.vel.r = self.pos.r
-        self.vel.theta = self.pos.theta
-
-    def _update_acceleration(self):
-        """
-        Updates the acceleration object to include r, theta, r_dot, and omega.
-        """
-        self.acc.r = self.vel.r
-        self.acc.theta = self.vel.theta
-        self.acc.r_dot = self.vel.r_dot
-        self.acc.omega = self.vel.omega
-
-    def _zero(self, s):
-        """
-        Zeros all the ndarray attributes at a certain size, s.
-
-        :param s: int; The size of the data
-        """
-        self.pos.rs = np.zeros(s)
-        self.pos.thetas = np.zeros(s)
-        self.vel.rs = self.pos.rs
-        self.vel.thetas = self.pos.thetas
-        self.vel.r_dots = np.zeros(s)
-        self.vel.omegas = np.zeros(s)
-        self.acc.rs = self.vel.rs
-        self.acc.thetas = self.vel.thetas
-        self.acc.r_dots = self.vel.r_dots
-        self.acc.omegas = self.vel.omegas
-        self.acc.r_ddots = np.zeros(s)
-        self.acc.alphas = np.zeros(s)
-
-    def _set_position_data(self, i):
-        """
-        Sets position data at index, i.
-
-        :param i: Index
-        """
-        self.pos.rs[i] = self.pos.r
-        self.pos.thetas[i] = self.pos.theta
-
-    def _set_velocity_data(self, i):
-        """
-        Sets velocity data at index, i.
-
-        :param i: Index
-        """
-        self.vel.r_dots[i] = self.vel.r_dot
-        self.vel.omegas[i] = self.vel.omega
-
-    def _set_acceleration_data(self, i):
-        """
-        Sets acceleration data at index, i.
-
-        :param i: Index
-        """
-        self.acc.r_ddots[i] = self.acc.r_ddot
-        self.acc.alphas[i] = self.acc.alpha
-
-    def __call__(self, *args):
-        return self.get(*args)
-
-    def __repr__(self):
-        return f'{self.joints[0]}{self.joints[1]}'
-
-
-class Position(VectorBase):
-    def __init__(self, **kwargs):
-        VectorBase.__init__(self, **kwargs)
-        del self.r_dot, self.r_ddot, self.omega, self.alpha, self.r_dots, self.omegas, self.r_ddots, self.alphas
-
-    def _both(self, r, theta):
-        # When both the theta and the radius are unknown
-        self.x, self.y = r*np.cos(theta), r*np.sin(theta)
-        self.r, self.theta = r, theta
-        return np.array([self.x, self.y])
-
-    def _neither(self):
-        self.x, self.y = self.r*np.cos(self.theta), self.r*np.sin(self.theta)
-        return np.array([self.x, self.y])
-
-    def _tangent(self, theta):
-        # When the theta is unknown
-        self.x, self.y = self.r*np.cos(theta), self.r*np.sin(theta)
-        self.theta = theta
-        return np.array([self.x, self.y])
-
-    def _slip(self, r):
-        # When the radius is unknown
-        self.x, self.y = r*np.cos(self.theta), r*np.sin(self.theta)
-        self.r = r
-        return np.array([self.x, self.y])
-
-    def __repr__(self):
-        return f'Position(joints={self.joints}, r={self.r}, theta={self.theta})'
-
-    def __str__(self):
-        return f'R_{self.joints[0]}{self.joints[1]}'
-
-
-class Velocity(VectorBase):
-    def __init__(self, **kwargs):
-        VectorBase.__init__(self, **kwargs)
-        del self.r_ddot, self.alpha, self.r_ddots, self.alphas
-
-    def _neither(self):
-        self.x, self.y = 0, 0
-        return np.array([self.x, self.y])
-
-    def _both(self, r_dot, omega):
-        self.x, self.y = (r_dot*np.cos(self.theta) - self.r*omega*np.sin(self.theta),
-                          r_dot*np.sin(self.theta) + self.r*omega*np.cos(self.theta))
-        self.r_dot, self.omega = r_dot, omega
-        return np.array([self.x, self.y])
-
-    def _tangent(self, omega):
-        self.x, self.y = self.r*omega*-np.sin(self.theta), self.r*omega*np.cos(self.theta)
-        self.omega = omega
-        return np.array([self.x, self.y])
-
-    def _slip(self, r_dot):
-        self.x, self.y = r_dot*np.cos(self.theta), r_dot*np.sin(self.theta)
-        self.r_dot = r_dot
-        return np.array([self.x, self.y])
-
-    def __repr__(self):
-        return f'Velocity(joints={self.joints}, r_dot={self.r_dot}, omega={self.omega})'
-
-    def __str__(self):
-        return f'V_{self.joints[0]}{self.joints[1]}'
-
-
-class Acceleration(VectorBase):
-    def __init__(self, **kwargs):
-        VectorBase.__init__(self, **kwargs)
-
-    def _neither(self):
-        self.x, self.y = 0, 0
-        return np.array([self.x, self.y])
-
-    def _both(self, r_ddot, alpha):
-        self.x, self.y = (r_ddot*np.cos(self.theta) - 2*self.r_dot*self.omega*np.sin(self.theta) - self.r*alpha*np.sin(
-            self.theta) - self.r*self.omega ** 2*np.cos(self.theta),
-                          r_ddot*np.sin(self.theta) + 2*self.r_dot*self.omega*np.cos(self.theta) + self.r*alpha*np.cos(
-                              self.theta) - self.r*self.omega ** 2*np.sin(self.theta))
-        self.r_ddot, self.alpha = r_ddot, alpha
-        return np.array([self.x, self.y])
-
-    def _tangent(self, alpha):
-        self.x, self.y = (self.r*alpha*-np.sin(self.theta) - self.r*self.omega**2*np.cos(self.theta),
-                          self.r*alpha*np.cos(self.theta) - self.r*self.omega**2*np.sin(self.theta))
-        self.alpha = alpha
-        return np.array([self.x, self.y])
-
-    def _slip(self, r_ddot):
-        self.x, self.y = r_ddot*np.cos(self.theta), r_ddot*np.sin(self.theta)
-        self.r_ddot = r_ddot
-        return np.array([self.x, self.y])
-
-    def __repr__(self):
-        return f'Acceleration(joints={self.joints}, r_ddot={self.r_ddot}, alpha={self.alpha})'
-
-    def __str__(self):
-        return f'A_{self.joints[0]}{self.joints[1]}'
+import numpy as np
+import json
+import os
+
+THIS_DIR = os.path.dirname(os.path.abspath(__file__))
+APPEARANCE = os.path.join(THIS_DIR, 'appearance.json')
+
+
+class VectorBase:
+    def __init__(self, joints=None, r=None, theta=None, x=None, y=None, show=True, style=None, **kwargs):
+        """
+        :param joints: tup; A tuple of Joint objects. The first Joint is the tail, and the second is the head.
+        :param r: int, float; The length of the vector. If specified, the vector is taken to be a constant length,
+            meaning r_dot and r_ddot is zero.
+        :param theta: int, float; The angle of the vector in radians from the positive x-axis. Counterclockwise is
+            positive. If specified, the vector is directed at a constant angle, meaning omega and alpha is zero.
+        :param x: int, float; The value of the x component of the vector.
+        :param y: int, float; The value of the y component of the vector.
+        :param show: bool; If True, then the vector will be present in plots and animations.
+        :param style: str; Applies a certain style passed to plt.plot().
+            Options: 
+                ground - a dashed black line for grounded link
+                dotted - a black dotted line
+        :param kwargs: Extra arguments that are passed to plt.plot(). If not specified, the line will be maroon with a
+            marker style = 'o'
+
+        Instance Variables
+        ------------------
+        rs: An ndarray of r values.
+        thetas: An ndarray of theta values.
+        r_dots: An ndarray of r_dot values (r_dot is the rate of change of the length of the vector length with respect
+            to time).
+        omegas: An ndarray of omega values (omega is the rate of change of the angle of the vector with respect to
+            time).
+        r_ddots: An ndarray of r_ddot values (r_ddot is the rate of change of the rate of change of the vector length
+            with respect to time).
+        alphas: An ndarray of alpha values (alpha is the rate of change of the rate of change of the angle of the vector
+            with respect to time).
+        get: A function that returns the x and y component of the vector. The arguments for this function depends on
+            what is specified at the initialization of the object. For instance, if r is set to a certain value, the get
+            function will require an angle input.
+        """
+        self.joints, self.r, self.theta, self.show = joints, r, theta, show
+
+        with open(APPEARANCE, 'r') as f:
+            appearance = json.load(f)
+
+        if style:
+            self.kwargs = appearance['mechanism_plot'][style]
+        elif kwargs:
+            self.kwargs = kwargs
+        else:
+            self.kwargs = appearance['mechanism_plot']['default']
+
+        self.x, self.y = x, y
+
+        self.rs, self.thetas, self.r_dots, self.omegas, self.r_ddots, self.alphas = None, None, None, None, None, None
+
+        if self.r is not None and self.theta is not None:
+            self.r_dot, self.omega = 0, 0
+            self.r_ddot, self.alpha = 0, 0
+            self.get = self._neither
+        elif self.r is not None and self.theta is None:
+            self.r_dot, self.omega = 0, None
+            self.r_ddot, self.alpha = 0, None
+            self.get = self._tangent
+        elif self.r is None and self.theta is not None:
+            self.r_dot, self.omega = None, 0
+            self.r_ddot, self.alpha = None, 0
+            self.get = self._slip
+        else:
+            self.r_dot, self.omega = None, None
+            self.r_ddot, self.alpha = None, None
+            self.get = self._both
+
+    def _neither(self):
+        pass
+
+    def _both(self, _, __):
+        pass
+
+    def _slip(self, _):
+        pass
+
+    def _tangent(self, _):
+        pass
+
+    def _fix_global_position(self):
+        """
+        Fixes the position of the head joint by making its position the x and y components of the current instance.
+        """
+        self.joints[1]._fix_position(self.x, self.y)
+
+    def _fix_global_velocity(self):
+        """
+        Fixes the velocity of the head joint by making its velocity the x and y components of the current instance.
+        """
+        self.joints[1]._fix_velocity(self.x, self.y)
+
+    def _fix_global_acceleration(self):
+        """
+        Fixes the acceleration of the head joint by making its acceleration the x and y components of the current
+        instance.
+        """
+        self.joints[1]._fix_acceleration(self.x, self.y)
+
+    def _reverse(self):
+        """
+        :return: A VectorBase object that is reversed. The joints get reversed as well as the x and y components.
+        """
+        x, y = -self.x, -self.y
+        return VectorBase(joints=(self.joints[1], self.joints[0]), x=x, y=y)
+
+    def _get_mag(self):
+        """
+        :return: A tuple consisting of the magnitude of the current instance and the angle.
+        """
+        mag = np.sqrt(self.x ** 2 + self.y ** 2)
+
+        if self.x > 0 and self.y >= 0:
+            angle = np.arctan(self.y/self.x)
+        elif self.x < 0 and self.y >= 0:
+            angle = np.arctan(self.y/self.x) + np.pi
+        elif self.x < 0 and self.y <= 0:
+            angle = np.arctan(self.y/self.x) + np.pi
+        elif self.x > 0 and self.y <= 0:
+            angle = np.arctan(self.y/self.x) + 2*np.pi
+        elif self.x == 0 and self.y >= 0:
+            angle = np.pi/2  # when x is zero
+        else:
+            angle = 3*np.pi/2
+
+        return mag, angle
+
+    def __add__(self, other):
+        x, y = self.x + other.x, self.y + other.y
+        return VectorBase(joints=(self.joints[0], other.joints[1]), x=x, y=y)
+
+
+class Vector:
+    def __init__(self, joints=None, r=None, theta=None, x=None, y=None, show=True, style=None, **kwargs):
+        """
+        See the VectorBase class for details regarding the parameters. The purpose of this class is to group Position,
+        Velocity, and Acceleration objects.
+
+        Instance Variables
+        ------------------
+        pos: Position object which is a subclass of VectorBase. Does not include the r_dot, omega, r_ddot, and alpha
+            attributes.
+        vel: Velocity object which is a subclass of VectorBase. Does not include the r_ddot and alpha attributes.
+        acc: Acceleration object which is a subclass of VectorBase.
+        """
+        self.pos = Position(joints=joints, r=r, theta=theta, x=x, y=y, show=show, style=style, **kwargs)
+        self.vel = Velocity(joints=joints, r=r, theta=theta, x=x, y=y, show=show, style=style, **kwargs)
+        self.acc = Acceleration(joints=joints, r=r, theta=theta, x=x, y=y, show=show, style=style, **kwargs)
+
+        self.get = self.pos.get
+        self.joints = joints
+
+    def _update_velocity(self):
+        """
+        Updates the velocity object to include the length, r, and the angle ,theta.
+        """
+        self.vel.r = self.pos.r
+        self.vel.theta = self.pos.theta
+
+    def _update_acceleration(self):
+        """
+        Updates the acceleration object to include r, theta, r_dot, and omega.
+        """
+        self.acc.r = self.vel.r
+        self.acc.theta = self.vel.theta
+        self.acc.r_dot = self.vel.r_dot
+        self.acc.omega = self.vel.omega
+
+    def _zero(self, s):
+        """
+        Zeros all the ndarray attributes at a certain size, s.
+
+        :param s: int; The size of the data
+        """
+        self.pos.rs = np.zeros(s)
+        self.pos.thetas = np.zeros(s)
+        self.vel.rs = self.pos.rs
+        self.vel.thetas = self.pos.thetas
+        self.vel.r_dots = np.zeros(s)
+        self.vel.omegas = np.zeros(s)
+        self.acc.rs = self.vel.rs
+        self.acc.thetas = self.vel.thetas
+        self.acc.r_dots = self.vel.r_dots
+        self.acc.omegas = self.vel.omegas
+        self.acc.r_ddots = np.zeros(s)
+        self.acc.alphas = np.zeros(s)
+
+    def _set_position_data(self, i):
+        """
+        Sets position data at index, i.
+
+        :param i: Index
+        """
+        self.pos.rs[i] = self.pos.r
+        self.pos.thetas[i] = self.pos.theta
+
+    def _set_velocity_data(self, i):
+        """
+        Sets velocity data at index, i.
+
+        :param i: Index
+        """
+        self.vel.r_dots[i] = self.vel.r_dot
+        self.vel.omegas[i] = self.vel.omega
+
+    def _set_acceleration_data(self, i):
+        """
+        Sets acceleration data at index, i.
+
+        :param i: Index
+        """
+        self.acc.r_ddots[i] = self.acc.r_ddot
+        self.acc.alphas[i] = self.acc.alpha
+
+    def __call__(self, *args):
+        return self.get(*args)
+
+    def __repr__(self):
+        return f'{self.joints[0]}{self.joints[1]}'
+
+
+class Position(VectorBase):
+    def __init__(self, **kwargs):
+        VectorBase.__init__(self, **kwargs)
+        del self.r_dot, self.r_ddot, self.omega, self.alpha, self.r_dots, self.omegas, self.r_ddots, self.alphas
+
+    def _both(self, r, theta):
+        # When both the theta and the radius are unknown
+        self.x, self.y = r*np.cos(theta), r*np.sin(theta)
+        self.r, self.theta = r, theta
+        return np.array([self.x, self.y])
+
+    def _neither(self):
+        self.x, self.y = self.r*np.cos(self.theta), self.r*np.sin(self.theta)
+        return np.array([self.x, self.y])
+
+    def _tangent(self, theta):
+        # When the theta is unknown
+        self.x, self.y = self.r*np.cos(theta), self.r*np.sin(theta)
+        self.theta = theta
+        return np.array([self.x, self.y])
+
+    def _slip(self, r):
+        # When the radius is unknown
+        self.x, self.y = r*np.cos(self.theta), r*np.sin(self.theta)
+        self.r = r
+        return np.array([self.x, self.y])
+
+    def __repr__(self):
+        return f'Position(joints={self.joints}, r={self.r}, theta={self.theta})'
+
+    def __str__(self):
+        return f'R_{self.joints[0]}{self.joints[1]}'
+
+
+class Velocity(VectorBase):
+    def __init__(self, **kwargs):
+        VectorBase.__init__(self, **kwargs)
+        del self.r_ddot, self.alpha, self.r_ddots, self.alphas
+
+    def _neither(self):
+        self.x, self.y = 0, 0
+        return np.array([self.x, self.y])
+
+    def _both(self, r_dot, omega):
+        self.x, self.y = (r_dot*np.cos(self.theta) - self.r*omega*np.sin(self.theta),
+                          r_dot*np.sin(self.theta) + self.r*omega*np.cos(self.theta))
+        self.r_dot, self.omega = r_dot, omega
+        return np.array([self.x, self.y])
+
+    def _tangent(self, omega):
+        self.x, self.y = self.r*omega*-np.sin(self.theta), self.r*omega*np.cos(self.theta)
+        self.omega = omega
+        return np.array([self.x, self.y])
+
+    def _slip(self, r_dot):
+        self.x, self.y = r_dot*np.cos(self.theta), r_dot*np.sin(self.theta)
+        self.r_dot = r_dot
+        return np.array([self.x, self.y])
+
+    def __repr__(self):
+        return f'Velocity(joints={self.joints}, r_dot={self.r_dot}, omega={self.omega})'
+
+    def __str__(self):
+        return f'V_{self.joints[0]}{self.joints[1]}'
+
+
+class Acceleration(VectorBase):
+    def __init__(self, **kwargs):
+        VectorBase.__init__(self, **kwargs)
+
+    def _neither(self):
+        self.x, self.y = 0, 0
+        return np.array([self.x, self.y])
+
+    def _both(self, r_ddot, alpha):
+        self.x, self.y = (r_ddot*np.cos(self.theta) - 2*self.r_dot*self.omega*np.sin(self.theta) - self.r*alpha*np.sin(
+            self.theta) - self.r*self.omega ** 2*np.cos(self.theta),
+                          r_ddot*np.sin(self.theta) + 2*self.r_dot*self.omega*np.cos(self.theta) + self.r*alpha*np.cos(
+                              self.theta) - self.r*self.omega ** 2*np.sin(self.theta))
+        self.r_ddot, self.alpha = r_ddot, alpha
+        return np.array([self.x, self.y])
+
+    def _tangent(self, alpha):
+        self.x, self.y = (self.r*alpha*-np.sin(self.theta) - self.r*self.omega**2*np.cos(self.theta),
+                          self.r*alpha*np.cos(self.theta) - self.r*self.omega**2*np.sin(self.theta))
+        self.alpha = alpha
+        return np.array([self.x, self.y])
+
+    def _slip(self, r_ddot):
+        self.x, self.y = r_ddot*np.cos(self.theta), r_ddot*np.sin(self.theta)
+        self.r_ddot = r_ddot
+        return np.array([self.x, self.y])
+
+    def __repr__(self):
+        return f'Acceleration(joints={self.joints}, r_ddot={self.r_ddot}, alpha={self.alpha})'
+
+    def __str__(self):
+        return f'A_{self.joints[0]}{self.joints[1]}'
```

### Comparing `mechanism-1.1.7/mechanism.egg-info/PKG-INFO` & `mechanism-1.1.8/mechanism.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,447 +1,449 @@
-Metadata-Version: 2.1
-Name: mechanism
-Version: 1.1.7
-Summary: A package that provides a kinematic analysis of mechanisms and cams and custom tooth profile for spur gears.
-Home-page: https://github.com/gabemorris12/mechanism
-Author: Gabe Morris
-Author-email: gabemorris1231@gmail.com
-License: MIT
-Keywords: mechanism,kinematic,cams,linkages,analysis,animations
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
-License-File: license.txt
-Requires-Dist: matplotlib
-Requires-Dist: scipy
-
-# Purpose
-
-This package was created to aid with the designing process of mechanisms involving linkages, cams, and gears. In regard
-to linkages, it is capable of implementing a kinematic analysis with the knowledge of the degrees of freedom for the
-vectors that make up the mechanism. With the aid of numerical solving and iteration, the position, velocity, and
-acceleration of these vectors and points may be acquired.
-
-In regard to cams, this package is capable of supplying coordinates of a cam profile, plotting SVAJ diagrams, and
-getting a cam and follower animation for roller and flat faced followers. In turn, the coordinates may be supplied to a
-machinist or imported into SolidWorks. All that is needed to know is the motion description (i.e. rise 2 inches in 1
-second, dwell for 1.5 seconds, fall 2 inches in 3 seconds). As of right now, the kinds of motion supported are
-naive/uniform motion (how the cam shouldn't be designed), harmonic motion, and cycloidal motion. It is possible that
-this gets updated in the future with better options such as modified sinusoidal motion.
-
-For gears, this package is capable of providing the coordinates of a spur gear tooth profile given a set of properties.
-The analysis is based on the diametral pitch, number of teeth, and pitch diameter if desired over the number of teeth.
-An argument for AGMA standards may be set to `True` if desired.
-
-Install this package via pip: `pip install mechanism`.
-
-# Results/Examples
-
-`fourbarlinkage.py`
-
-![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/fourbarlinkage.gif)
-
-`fivebarlinkage.py`
-
-![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/fivebarlinkage.gif)
-
-`crunode_coupler.py`
-
-![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/crunode_coupler.gif)
-
-`crankslider.py`
-
-![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/crankslider.gif)
-
-`engine.py`
-
-![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/engine.gif)
-
-`non_grashof.py`
-
-![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/non_grashof.gif)
-
-`offset_crankslider.py`
-
-![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/offset_crankslider.gif)
-
-`cam2_example.py`
-
-![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/cam2.gif)
-
-# Linkages, Cranks, Couplers, and Rockers
-
-In order to use the contents of `mechanism.py`, a basic knowledge of vector loops must be known. The structure of the
-vector loops function is shown in several files under the `examples` folder. To gain a greater understanding of this
-package's usage, this walk through is provided.
-
-## Four Bar Linkage Example
-
-![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/fourbarlinkage.PNG)
-
-A four bar linkage is the basic building block of all mechanisms. This is similar to how the triangle is the basic
-building block of all structures. What defines a mechanism or structure is the system's overall number of degrees of
-freedom, and the number of degrees of freedom is determined via Kutzbachâ€™s equation.
-
-![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/fourbarlinkage_dof.PNG)
-
-Kutzbach's equation is: *total degrees of freedom = 3(#links - 1) - 2(J1) - J2* where J1 is the number of full joints
-(also known as a revolute joint) and J2 is the number of half joints. For this four bar linkage, there are 4 full
-joints.
-
-The number of degrees of freedom is: 3(4 - 1) - 2(4) = 1
-
-This means that we need one known input to find the unknowns of the system. This can be explained further with a diagram
-of the vectors that make up the four bar linkage.
-
-![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/fourbarlinkage_loop.PNG)
-
-From the above image, the vector "a" is the crank. The speed at which it rotates will be considered as the input to the
-system, and thus, it is the defining parameter to the system.
-
-The lengths of all the vectors are known. The only two unknowns are the angle that corresponds to vector "b" and "d". It
-is important to note that the objects that make up this package are vectors, and the polar form of the vectors is the
-main interest.
-
-There is only one loop equation which provides two equations when breaking down the vectors into its components. With
-two equations and two unknowns, this system becomes solvable.
-
-### Problem Statement
-
-Consider the four bar linkage shown above. The lengths of a, b, c, and d are 5", 8", 8" and 9". The crank (a) rotates at
-a constant 500 RPM. Use `mechanism` to get an animation of this linkage system and plot the angles, angular velocity,
-and angular acceleration of vector d as a function of time.
-
-### Solution
-
-The four bar linkage is a grashof linkage because it satisfies the grashof condition (9 + 5 < 8 + 8). This means that
-the crank is able to fully rotate. The input can be deduced by integrating and differentiating the constant value of the
-constant angular velocity of the crank.
-
-Always begin with defining the joints and vectors.
-
-```python
-from mechanism import *
-import numpy as np
-import matplotlib.pyplot as plt
-
-# Declare the joints that make up the system.
-O, A, B, C = get_joints('O A B C')
-
-# Declare the vectors and keep in mind that angles are in radians and start from the positive x-axis.
-a = Vector((O, A), r=5)
-b = Vector((A, B), r=8)
-c = Vector((O, C), r=8, theta=0, style='ground')
-d = Vector((C, B), r=9)
-```
-
-Always define the vectors in the polar form. The first argument is the joints, and the first joint is the tail of the
-vector, and the second is the head. Additionally, extra keyword arguments will be passed to plt.plot() for styling.
-
-By not defining the angles for a vector (like `a`, `b`, and `c`) you are saying that this vector will have a varying
-angle and the same is true for the length argument (`r`). If both the length and the angle are defined, as with `c`,
-then the vector is stationary and will remain at this length and angle. If niether `r` or `theta` is specified, then you
-are saying that the vector changes in length and angle, so you should expect two degrees of freedom for the input of
-this vector in the vector loop equations. There should be half as many loop equations as there are unknown. The input
-vector "a" does not need to have its known values at its declaration. Instead, it's values will be accounted for in the
-loop equation. The next thing to do is to define the known input and guesses for the first iteration of the unknown
-values.
-
-```python
-# Define the known input to the system.
-# For a 500 RMP crank, the time it takes to rotate one rev is 0.12s
-time = np.linspace(0, 0.12, 300)
-angular_velocity = 50*np.pi/3  # This is 500 RPM in rad/s
-
-theta = angular_velocity*time  # Integrate to find the theta
-omega = np.full((time.size,), angular_velocity)  # Just an array of the same angular velocity
-alpha = np.zeros(time.size)
-
-# Guess the unknowns
-pos_guess = np.deg2rad([45, 90])
-vel_guess = np.array([1000, 1000])
-acc_guess = np.array([1000, 1000])
-```
-
-The guess values need to be arrays of the same length as the number of unknowns. These arrays will be passed as the
-first iteration. The next thing to do is to define the loop function and create the mechanism object.
-
-```python
-# Define the loop equation(s)
-def loop(x, i):
-    return a(i) + b(x[0]) - c() - d(x[1])
-
-
-# Create the mechanism object
-mechanism = Mechanism(vectors=(a, b, c, d), origin=O, loops=loop, pos=theta, vel=omega, acc=alpha,
-                      guess=(pos_guess, vel_guess, acc_guess))
-```
-
-This example is simpler than most others because there is only one loop equation. For multiple loop equations, it is
-important that the function returns a flattened array of the same length as there are unknown, and the indexing of the
-first array argument to the loop corresponds to the input guess values. The second argument is the input. It is strongly
-encouraged to view the examples for the more rigorous structure of the loop function. The last thing to do is to
-call `mechanism.iterate()`, which is necessary if the input from `pos`, `vel`, and `acc` are arrays. If they are not
-arrays, then it is assumed that the mechanism at an instant is desired. If this is the case, then
-call `mechanism.calculate()` then call `mechanism.plot()` (see `plot_at_instant.py`).
-
-```python
-# Call mechanism.iterate() then get and show the animation
-mechanism.iterate()
-ani, fig_, ax_ = mechanism.get_animation()
-
-# Plot the angles, angular velocity, and angular acceleration of vector d
-fig, ax = plt.subplots(nrows=3, ncols=1)
-ax[0].plot(time, d.pos.thetas, color='maroon')
-ax[1].plot(time, d.vel.omegas, color='maroon')
-ax[2].plot(time, d.acc.alphas, color='maroon')
-
-ax[0].set_ylabel(r'$\theta$')
-ax[1].set_ylabel(r'$\omega$')
-ax[2].set_ylabel(r'$\alpha$')
-
-ax[2].set_xlabel(r'Time (s)')
-ax[0].set_title(r'Analysis of $\vec{d}$')
-
-for a in (ax[0], ax[1], ax[2]):
-    a.minorticks_on()
-    a.grid(which='both')
-
-fig.set_size_inches(7, 7)
-# fig.savefig('../images/analysis_d.png')
-
-plt.show()
-```
-
-This will produce the following output:
-
-![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/fourbar_animation.gif)
-![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/analysis_d.png)
-
-# Cams
-
-There are several kinds of motion types for a cam, but there is an important corollary when designing cams: *The jerk
-function must be finite across the entire interval (360 degrees)* (Robert Norton's *Design of Machinery*). Usually, the
-cycloidal motion type achieves this corollary, but it comes at a cost. It produces an acceleration and velocity that is
-typically higher than the other motion types. More motion types are to come later (hopefully).
-
-## Problem Statement
-
-Design a cam using cycloidal motion that has the following motion description:
-
-* Dwell at zero displacement for 90 degrees
-* Rise 1 inch in 90 degrees
-* Dwell for 90 degrees
-* Fall 1 inch in 90 degrees
-
-The cam's angular velocity is 2*pi radians per second. Show the SVAJ diagram as well as the cam's profile. Size the cam
-for a roller follower with a radius of 1/2" with a maximum pressure angle of 30 degrees. Also size the cam for a flat
-faced follower. Get an animation for both a roller/flat faced follower. Finally, save the coordinates of the profile to
-a text file and show the steps for creating a part in SolidWorks.
-
-## Solution
-
-Begin by creating a cam object with the correct motion description.
-
-```python
-import numpy as np
-from mechanism import Cam
-import matplotlib.pyplot as plt
-
-cam = Cam(motion=[
-    ('Dwell', 90),
-    ('Rise', 1, 90),
-    ('Dwell', 90),
-    ('Fall', 1, 90)
-], degrees=True, omega=2*np.pi)
-```
-
-The motion description is a list of tuples. Each tuple must contain 3 items for rising and falling and two items for
-dwelling. The first item of the tuple is a string equal to "Rise", "Fall", or "Dwell" (not case-sensitive). For rise and
-fall motion, the second item in the tuple is the distance at which the follower falls or rises. For dwelling, the second
-item in the tuple is either the time (in seconds) or angle (in degrees) for which the displacement remains constant. The
-third item in the tuple for rising and falling is equivalent to the second item for dwelling. If degrees is set to true,
-then the last item in each tuple is interpreted as the angle for which the action occurs. A manual input for the angular
-velocity is then required if conducting further analysis via SVAJ.
-
-This is all that's required to call the following methods.
-
-```python
-fig1, ax1 = cam.plot(kind='all')
-fig2, ax2 = cam.svaj(kind='cycloidal')
-plt.show()
-```
-
-This produces the following:
-
-![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/displacement_plot.png)
-![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/svaj.png)
-
-Looking at the acceleration plot, there are no vertical lines. This means that there is no infinite derivative at any
-instant along the cam's profile; the jerk function is finite across each instant, making this an acceptable motion type.
-
-If a roller follower with a 1/2" radius is desired, an analysis depending on the cam's radius of curvature and pressure
-angle can be conducted to determine the base circle of the cam.
-
-```python
-roller_analysis = cam.get_base_circle(kind='cycloidal', follower='roller', roller_radius=1/2, max_pressure_angle=30,
-                                      plot=True)
-fig3, ax3 = cam.profile(kind='cycloidal', base=roller_analysis['Rb'], show_base=True, roller_radius=1/2,
-                        show_pitch=True)
-plt.show()
-```
-
-Output:
-
-![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/pressure_angle.png)
-![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/roller_profile.png)
-
-For a flat faced follower, the radius of curvature at the point of contact should be positive (or greater than 0.25")
-for all theta. There is an option to return the base radius such that the radius of curvature of the cam's profile is
-positive for all values of theta (this is the conservative approach).
-
-```python
-flat_analysis = cam.get_base_circle(kind='cycloidal', follower='flat', desired_min_rho=0.25)
-print(flat_analysis['Rb'])
-print(flat_analysis['Min Face Width'])
-fig4, ax4 = cam.profile(kind='cycloidal', base=flat_analysis['Rb'], show_base=True)
-plt.show()
-```
-
-Output:
-
-![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/flat_profile.png)
-
-The base circle radius was found to be 1.893" and the minimum face width for the follower was found to be 2.55".
-
-To get the roller animation, call this:
-
-```python
-ani, fig5, ax5, follower = cam.get_animation(kind='cycloidal', base=roller_analysis['Rb'], roller_radius=1/2, length=2,
-                                             width=3/8, inc=5)
-fig6, ax6 = follower.plot()
-plt.show()
-```
-
-Output:
-
-![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/cam_roller.gif)
-![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/roller_follower_displacement.png)
-
-The graph above shows the actual follower displacement due to the circle having to always be tangent to the surface of
-the cam. Note that as a result of this physical limitation, the follower will have higher magnitudes of velocity and
-acceleration.
-
-For the flat faced follower,
-
-```python
-ani_flat, fig7, ax7, follower = cam.get_animation(kind='cycloidal', base=flat_analysis['Rb'], face_width=2.75, length=2,
-                                                  width=3/8, inc=5)
-fig8, ax8 = follower.plot()
-plt.show()
-```
-
-Output:
-
-![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/cam_flat.gif)
-![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/flat_follower_displacement.png)
-
-### Getting Coordinates into SolidWorks
-
-Save the coordinates to a text file.
-
-```python
-cam.save_coordinates('cam_coordinates.txt', kind='cycloidal', base=1.3, solidworks=True)
-```
-
-Select `Curve Through XYZ Points`
-
-![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/curve_xyz.png)
-
-The cam profile will always be extended to the front plane due to the manner in which SolidWorks defines the global
-coordinates. Next, select browse and choose the saved coordinate file, making sure that text files are able to be seen.
-
-![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/select_file.PNG)
-
-Create a sketch on the front plane. Select the curve and then convert entities. The sketch is now projected to the front
-plane.
-
-![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/front_plane.PNG)
-
-Notice that the sketch is not closed. Add a line to close the sketch, then extrude the sketch.
-
-![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/solidworks_cam.PNG)
-
-# Gears
-
-To use this feature, a knowledge of gear nomenclature must be known. Here is a figure from Robert Norton's *Design of
-Machinery*:
-
-![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/gear_nomenclature.PNG)
-
-For gears, a general rule of thumb is that the base circle must fall below the dedendum circle because the curve below
-base circle cannot be an involute curve. This package will send a warning if this occurs, and if it is desired to
-continue, the curve below the circle is just a straight line, and undercutting will occur.
-
-For a reference, here are the AGMA (American Gear Manufacturers Association) standards from *Design of Machinery*:
-
-![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/agma.PNG)
-
-## Problem Statement
-
-Design a gear that has a diametral pitch of 32 and has 60 teeth using `mechanism`. The gear follows the AGMA standards.
-Compare the gear to SolidWorks' gear from the tool library.
-
-## Solution
-
-Define a gear object with the known information and save the coordinates to a file.
-
-```python
-from mechanism import SpurGear
-import matplotlib.pyplot as plt
-
-gear = SpurGear(N=60, pd=32, agma=True, size=500)
-fig, ax = gear.plot()
-fig.savefig('../images/gear60.PNG', dpi=240)
-plt.show()
-gear.save_coordinates(file='gear_tooth_coordinates.txt', solidworks=True)
-gear.rundown()
-```
-
-output:
-
-![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/gear60.PNG)
-
-| Property                 | Value    |
-|--------------------------|----------|
-| Number of Teeth (N)      | 60       |
-| Diametral Pitch (pd)     | 32.00000 |
-| Pitch Diameter (d)       | 1.87500  |
-| Pitch Radius (r)         | 0.93750  |
-| Pressure Angle (phi)     | 20.00000 |
-| Base Radius              | 0.88096  |
-| Addendum (a)             | 0.03125  |
-| Dedendum (b)             | 0.03906  |
-| Circular Tooth Thickness | 0.04846  |
-| Circular Space Width     | 0.04971  |
-| Circular Backlash        | 0.00125  |
-
-Keep in mind that the `size` argument refers to the size of the coordinates that make up the involute curve. The more
-points, the sharper it is, but SolidWorks sometimes struggles with points being too close together. To fix this issue,
-make the size smaller. The default value is 1000.
-
-### SolidWorks Results
-
-Follow the same steps to get the curve into SolidWorks from the cam example. Make sure that the units in SolidWorks
-matches the units of the analysis.
-
-![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/gear60_compare.PNG)
-
-The results are a near identical match, and the addendum and dedendum fit perfectly. If analyzed closely, the only
-difference is the tooth thickness. The gray gear (the resulting gear from this package) has a slightly larger tooth
-thickness compared to SolidWorks' gear. This is due to the fact that SolidWorks doesn't use an involute gear tooth
-profile, as gears from the SolidWorks toolbox are for visuals only. Instead, the tooth profile is circular. Their gears
-should not be used for manufacturing as this is not accurate at all. The purpose of the involute tooth profile is that
-the meshing of gears will always produce a constant angular velocity, even when the gears aren't perfectly placed
-tangent to the pitch circles.
+Metadata-Version: 2.1
+Name: mechanism
+Version: 1.1.8
+Summary: A package that provides a kinematic analysis of mechanisms and cams and custom tooth profile for spur gears.
+Home-page: https://github.com/gabemorris12/mechanism
+Author: Gabe Morris
+Author-email: gabemorris1231@gmail.com
+License: MIT
+Keywords: mechanism,kinematic,cams,linkages,analysis,animations
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Programming Language :: Python :: 3.10
+Description-Content-Type: text/markdown
+Requires-Dist: matplotlib
+Requires-Dist: scipy
+
+# Purpose
+[![PyPI version](https://badge.fury.io/py/mechanism.svg)](https://badge.fury.io/py/mechanism)
+[![Downloads](https://static.pepy.tech/badge/mechanism)](https://pepy.tech/project/mechanism)
+[![Downloads](https://static.pepy.tech/badge/mechanism/month)](https://pepy.tech/project/mechanism)
+
+This package was created to aid with the designing process of mechanisms involving linkages, cams, and gears. In regard
+to linkages, it is capable of implementing a kinematic analysis with the knowledge of the degrees of freedom for the
+vectors that make up the mechanism. With the aid of numerical solving and iteration, the position, velocity, and
+acceleration of these vectors and points may be acquired.
+
+In regard to cams, this package is capable of supplying coordinates of a cam profile, plotting SVAJ diagrams, and
+getting a cam and follower animation for roller and flat faced followers. In turn, the coordinates may be supplied to a
+machinist or imported into SolidWorks. All that is needed to know is the motion description (i.e. rise 2 inches in 1
+second, dwell for 1.5 seconds, fall 2 inches in 3 seconds). As of right now, the kinds of motion supported are
+naive/uniform motion (how the cam shouldn't be designed), harmonic motion, and cycloidal motion. It is possible that
+this gets updated in the future with better options such as modified sinusoidal motion.
+
+For gears, this package is capable of providing the coordinates of a spur gear tooth profile given a set of properties.
+The analysis is based on the diametral pitch, number of teeth, and pitch diameter if desired over the number of teeth.
+An argument for AGMA standards may be set to `True` if desired.
+
+Install this package via pip: `pip install mechanism`.
+
+# Results/Examples
+
+`fourbarlinkage.py`
+
+![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/fourbarlinkage.gif)
+
+`fivebarlinkage.py`
+
+![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/fivebarlinkage.gif)
+
+`crunode_coupler.py`
+
+![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/crunode_coupler.gif)
+
+`crankslider.py`
+
+![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/crankslider.gif)
+
+`engine.py`
+
+![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/engine.gif)
+
+`non_grashof.py`
+
+![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/non_grashof.gif)
+
+`offset_crankslider.py`
+
+![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/offset_crankslider.gif)
+
+`cam2_example.py`
+
+![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/cam2.gif)
+
+# Linkages, Cranks, Couplers, and Rockers
+
+In order to use the contents of `mechanism.py`, a basic knowledge of vector loops must be known. The structure of the
+vector loops function is shown in several files under the `examples` folder. To gain a greater understanding of this
+package's usage, this walk through is provided.
+
+## Four Bar Linkage Example
+
+![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/fourbarlinkage.PNG)
+
+A four bar linkage is the basic building block of all mechanisms. This is similar to how the triangle is the basic
+building block of all structures. What defines a mechanism or structure is the system's overall number of degrees of
+freedom, and the number of degrees of freedom is determined via Kutzbach’s equation.
+
+![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/fourbarlinkage_dof.PNG)
+
+Kutzbach's equation is: *total degrees of freedom = 3(#links - 1) - 2(J1) - J2* where J1 is the number of full joints
+(also known as a revolute joint) and J2 is the number of half joints. For this four bar linkage, there are 4 full
+joints.
+
+The number of degrees of freedom is: 3(4 - 1) - 2(4) = 1
+
+This means that we need one known input to find the unknowns of the system. This can be explained further with a diagram
+of the vectors that make up the four bar linkage.
+
+![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/fourbarlinkage_loop.PNG)
+
+From the above image, the vector "a" is the crank. The speed at which it rotates will be considered as the input to the
+system, and thus, it is the defining parameter to the system.
+
+The lengths of all the vectors are known. The only two unknowns are the angle that corresponds to vector "b" and "d". It
+is important to note that the objects that make up this package are vectors, and the polar form of the vectors is the
+main interest.
+
+There is only one loop equation which provides two equations when breaking down the vectors into its components. With
+two equations and two unknowns, this system becomes solvable.
+
+### Problem Statement
+
+Consider the four bar linkage shown above. The lengths of a, b, c, and d are 5", 8", 8" and 9". The crank (a) rotates at
+a constant 500 RPM. Use `mechanism` to get an animation of this linkage system and plot the angles, angular velocity,
+and angular acceleration of vector d as a function of time.
+
+### Solution
+
+The four bar linkage is a grashof linkage because it satisfies the grashof condition (9 + 5 < 8 + 8). This means that
+the crank is able to fully rotate. The input can be deduced by integrating and differentiating the constant value of the
+constant angular velocity of the crank.
+
+Always begin with defining the joints and vectors.
+
+```python
+from mechanism import *
+import numpy as np
+import matplotlib.pyplot as plt
+
+# Declare the joints that make up the system.
+O, A, B, C = get_joints('O A B C')
+
+# Declare the vectors and keep in mind that angles are in radians and start from the positive x-axis.
+a = Vector((O, A), r=5)
+b = Vector((A, B), r=8)
+c = Vector((O, C), r=8, theta=0, style='ground')
+d = Vector((C, B), r=9)
+```
+
+Always define the vectors in the polar form. The first argument is the joints, and the first joint is the tail of the
+vector, and the second is the head. Additionally, extra keyword arguments will be passed to plt.plot() for styling.
+
+By not defining the angles for a vector (like `a`, `b`, and `c`) you are saying that this vector will have a varying
+angle and the same is true for the length argument (`r`). If both the length and the angle are defined, as with `c`,
+then the vector is stationary and will remain at this length and angle. If niether `r` or `theta` is specified, then you
+are saying that the vector changes in length and angle, so you should expect two degrees of freedom for the input of
+this vector in the vector loop equations. There should be half as many loop equations as there are unknown. The input
+vector "a" does not need to have its known values at its declaration. Instead, it's values will be accounted for in the
+loop equation. The next thing to do is to define the known input and guesses for the first iteration of the unknown
+values.
+
+```python
+# Define the known input to the system.
+# For a 500 RMP crank, the time it takes to rotate one rev is 0.12s
+time = np.linspace(0, 0.12, 300)
+angular_velocity = 50*np.pi/3  # This is 500 RPM in rad/s
+
+theta = angular_velocity*time  # Integrate to find the theta
+omega = np.full((time.size,), angular_velocity)  # Just an array of the same angular velocity
+alpha = np.zeros(time.size)
+
+# Guess the unknowns
+pos_guess = np.deg2rad([45, 90])
+vel_guess = np.array([1000, 1000])
+acc_guess = np.array([1000, 1000])
+```
+
+The guess values need to be arrays of the same length as the number of unknowns. These arrays will be passed as the
+first iteration. The next thing to do is to define the loop function and create the mechanism object.
+
+```python
+# Define the loop equation(s)
+def loop(x, i):
+    return a(i) + b(x[0]) - c() - d(x[1])
+
+
+# Create the mechanism object
+mechanism = Mechanism(vectors=(a, b, c, d), origin=O, loops=loop, pos=theta, vel=omega, acc=alpha,
+                      guess=(pos_guess, vel_guess, acc_guess))
+```
+
+This example is simpler than most others because there is only one loop equation. For multiple loop equations, it is
+important that the function returns a flattened array of the same length as there are unknown, and the indexing of the
+first array argument to the loop corresponds to the input guess values. The second argument is the input. It is strongly
+encouraged to view the examples for the more rigorous structure of the loop function. The last thing to do is to
+call `mechanism.iterate()`, which is necessary if the input from `pos`, `vel`, and `acc` are arrays. If they are not
+arrays, then it is assumed that the mechanism at an instant is desired. If this is the case, then
+call `mechanism.calculate()` then call `mechanism.plot()` (see `plot_at_instant.py`).
+
+```python
+# Call mechanism.iterate() then get and show the animation
+mechanism.iterate()
+ani, fig_, ax_ = mechanism.get_animation()
+
+# Plot the angles, angular velocity, and angular acceleration of vector d
+fig, ax = plt.subplots(nrows=3, ncols=1)
+ax[0].plot(time, d.pos.thetas, color='maroon')
+ax[1].plot(time, d.vel.omegas, color='maroon')
+ax[2].plot(time, d.acc.alphas, color='maroon')
+
+ax[0].set_ylabel(r'$\theta$')
+ax[1].set_ylabel(r'$\omega$')
+ax[2].set_ylabel(r'$\alpha$')
+
+ax[2].set_xlabel(r'Time (s)')
+ax[0].set_title(r'Analysis of $\vec{d}$')
+
+for a in (ax[0], ax[1], ax[2]):
+    a.minorticks_on()
+    a.grid(which='both')
+
+fig.set_size_inches(7, 7)
+# fig.savefig('../images/analysis_d.png')
+
+plt.show()
+```
+
+This will produce the following output:
+
+![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/fourbar_animation.gif)
+![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/analysis_d.png)
+
+# Cams
+
+There are several kinds of motion types for a cam, but there is an important corollary when designing cams: *The jerk
+function must be finite across the entire interval (360 degrees)* (Robert Norton's *Design of Machinery*). Usually, the
+cycloidal motion type achieves this corollary, but it comes at a cost. It produces an acceleration and velocity that is
+typically higher than the other motion types. More motion types are to come later (hopefully).
+
+## Problem Statement
+
+Design a cam using cycloidal motion that has the following motion description:
+
+* Dwell at zero displacement for 90 degrees
+* Rise 1 inch in 90 degrees
+* Dwell for 90 degrees
+* Fall 1 inch in 90 degrees
+
+The cam's angular velocity is 2*pi radians per second. Show the SVAJ diagram as well as the cam's profile. Size the cam
+for a roller follower with a radius of 1/2" with a maximum pressure angle of 30 degrees. Also size the cam for a flat
+faced follower. Get an animation for both a roller/flat faced follower. Finally, save the coordinates of the profile to
+a text file and show the steps for creating a part in SolidWorks.
+
+## Solution
+
+Begin by creating a cam object with the correct motion description.
+
+```python
+import numpy as np
+from mechanism import Cam
+import matplotlib.pyplot as plt
+
+cam = Cam(motion=[
+    ('Dwell', 90),
+    ('Rise', 1, 90),
+    ('Dwell', 90),
+    ('Fall', 1, 90)
+], degrees=True, omega=2*np.pi)
+```
+
+The motion description is a list of tuples. Each tuple must contain 3 items for rising and falling and two items for
+dwelling. The first item of the tuple is a string equal to "Rise", "Fall", or "Dwell" (not case-sensitive). For rise and
+fall motion, the second item in the tuple is the distance at which the follower falls or rises. For dwelling, the second
+item in the tuple is either the time (in seconds) or angle (in degrees) for which the displacement remains constant. The
+third item in the tuple for rising and falling is equivalent to the second item for dwelling. If degrees is set to true,
+then the last item in each tuple is interpreted as the angle for which the action occurs. A manual input for the angular
+velocity is then required if conducting further analysis via SVAJ.
+
+This is all that's required to call the following methods.
+
+```python
+fig1, ax1 = cam.plot(kind='all')
+fig2, ax2 = cam.svaj(kind='cycloidal')
+plt.show()
+```
+
+This produces the following:
+
+![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/displacement_plot.png)
+![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/svaj.png)
+
+Looking at the acceleration plot, there are no vertical lines. This means that there is no infinite derivative at any
+instant along the cam's profile; the jerk function is finite across each instant, making this an acceptable motion type.
+
+If a roller follower with a 1/2" radius is desired, an analysis depending on the cam's radius of curvature and pressure
+angle can be conducted to determine the base circle of the cam.
+
+```python
+roller_analysis = cam.get_base_circle(kind='cycloidal', follower='roller', roller_radius=1/2, max_pressure_angle=30,
+                                      plot=True)
+fig3, ax3 = cam.profile(kind='cycloidal', base=roller_analysis['Rb'], show_base=True, roller_radius=1/2,
+                        show_pitch=True)
+plt.show()
+```
+
+Output:
+
+![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/pressure_angle.png)
+![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/roller_profile.png)
+
+For a flat faced follower, the radius of curvature at the point of contact should be positive (or greater than 0.25")
+for all theta. There is an option to return the base radius such that the radius of curvature of the cam's profile is
+positive for all values of theta (this is the conservative approach).
+
+```python
+flat_analysis = cam.get_base_circle(kind='cycloidal', follower='flat', desired_min_rho=0.25)
+print(flat_analysis['Rb'])
+print(flat_analysis['Min Face Width'])
+fig4, ax4 = cam.profile(kind='cycloidal', base=flat_analysis['Rb'], show_base=True)
+plt.show()
+```
+
+Output:
+
+![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/flat_profile.png)
+
+The base circle radius was found to be 1.893" and the minimum face width for the follower was found to be 2.55".
+
+To get the roller animation, call this:
+
+```python
+ani, fig5, ax5, follower = cam.get_animation(kind='cycloidal', base=roller_analysis['Rb'], roller_radius=1/2, length=2,
+                                             width=3/8, inc=5)
+fig6, ax6 = follower.plot()
+plt.show()
+```
+
+Output:
+
+![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/cam_roller.gif)
+![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/roller_follower_displacement.png)
+
+The graph above shows the actual follower displacement due to the circle having to always be tangent to the surface of
+the cam. Note that as a result of this physical limitation, the follower will have higher magnitudes of velocity and
+acceleration.
+
+For the flat faced follower,
+
+```python
+ani_flat, fig7, ax7, follower = cam.get_animation(kind='cycloidal', base=flat_analysis['Rb'], face_width=2.75, length=2,
+                                                  width=3/8, inc=5)
+fig8, ax8 = follower.plot()
+plt.show()
+```
+
+Output:
+
+![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/cam_flat.gif)
+![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/flat_follower_displacement.png)
+
+### Getting Coordinates into SolidWorks
+
+Save the coordinates to a text file.
+
+```python
+cam.save_coordinates('cam_coordinates.txt', kind='cycloidal', base=1.3, solidworks=True)
+```
+
+Select `Curve Through XYZ Points`
+
+![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/curve_xyz.png)
+
+The cam profile will always be extended to the front plane due to the manner in which SolidWorks defines the global
+coordinates. Next, select browse and choose the saved coordinate file, making sure that text files are able to be seen.
+
+![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/select_file.PNG)
+
+Create a sketch on the front plane. Select the curve and then convert entities. The sketch is now projected to the front
+plane.
+
+![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/front_plane.PNG)
+
+Notice that the sketch is not closed. Add a line to close the sketch, then extrude the sketch.
+
+![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/solidworks_cam.PNG)
+
+# Gears
+
+To use this feature, a knowledge of gear nomenclature must be known. Here is a figure from Robert Norton's *Design of
+Machinery*:
+
+![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/gear_nomenclature.PNG)
+
+For gears, a general rule of thumb is that the base circle must fall below the dedendum circle because the curve below
+base circle cannot be an involute curve. This package will send a warning if this occurs, and if it is desired to
+continue, the curve below the circle is just a straight line, and undercutting will occur.
+
+For a reference, here are the AGMA (American Gear Manufacturers Association) standards from *Design of Machinery*:
+
+![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/agma.PNG)
+
+## Problem Statement
+
+Design a gear that has a diametral pitch of 32 and has 60 teeth using `mechanism`. The gear follows the AGMA standards.
+Compare the gear to SolidWorks' gear from the tool library.
+
+## Solution
+
+Define a gear object with the known information and save the coordinates to a file.
+
+```python
+from mechanism import SpurGear
+import matplotlib.pyplot as plt
+
+gear = SpurGear(N=60, pd=32, agma=True, size=500)
+fig, ax = gear.plot()
+fig.savefig('../images/gear60.PNG', dpi=240)
+plt.show()
+gear.save_coordinates(file='gear_tooth_coordinates.txt', solidworks=True)
+gear.rundown()
+```
+
+output:
+
+![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/gear60.PNG)
+
+| Property                 | Value    |
+|--------------------------|----------|
+| Number of Teeth (N)      | 60       |
+| Diametral Pitch (pd)     | 32.00000 |
+| Pitch Diameter (d)       | 1.87500  |
+| Pitch Radius (r)         | 0.93750  |
+| Pressure Angle (phi)     | 20.00000 |
+| Base Radius              | 0.88096  |
+| Addendum (a)             | 0.03125  |
+| Dedendum (b)             | 0.03906  |
+| Circular Tooth Thickness | 0.04846  |
+| Circular Space Width     | 0.04971  |
+| Circular Backlash        | 0.00125  |
+
+Keep in mind that the `size` argument refers to the size of the coordinates that make up the involute curve. The more
+points, the sharper it is, but SolidWorks sometimes struggles with points being too close together. To fix this issue,
+make the size smaller. The default value is 1000.
+
+### SolidWorks Results
+
+Follow the same steps to get the curve into SolidWorks from the cam example. Make sure that the units in SolidWorks
+matches the units of the analysis.
+
+![image not found](https://github.com/gabemorris12/mechanism/raw/master/images/gear60_compare.PNG)
+
+The results are a near identical match, and the addendum and dedendum fit perfectly. If analyzed closely, the only
+difference is the tooth thickness. The gray gear (the resulting gear from this package) has a slightly larger tooth
+thickness compared to SolidWorks' gear. This is due to the fact that SolidWorks doesn't use an involute gear tooth
+profile, as gears from the SolidWorks toolbox are for visuals only. Instead, the tooth profile is circular. Their gears
+should not be used for manufacturing as this is not accurate at all. The purpose of the involute tooth profile is that
+the meshing of gears will always produce a constant angular velocity, even when the gears aren't perfectly placed
+tangent to the pitch circles.
```

### Comparing `mechanism-1.1.7/setup.py` & `mechanism-1.1.8/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-from setuptools import setup, find_packages
-import os
-
-THIS_DIR = r'C:\Users\gmbra\Downloads\Python Programs\mechanism'
-
-VERSION = '1.1.7'
-
-CLASSIFIERS = [
-    'Development Status :: 5 - Production/Stable',
-    'License :: OSI Approved :: MIT License',
-    'Operating System :: Microsoft :: Windows',
-    'Programming Language :: Python :: 3.10'
-]
-
-with open(os.path.join(THIS_DIR, 'readme.md'), 'r') as f:
-    LONG_DESCRIPTION = f.read()
-
-setup(
-    name='mechanism',
-    version=VERSION,
-    author='Gabe Morris',
-    author_email='gabemorris1231@gmail.com',
-    description='A package that provides a kinematic analysis of mechanisms and cams and custom tooth profile for spur '
-                'gears.',
-    long_description=LONG_DESCRIPTION,
-    long_description_content_type='text/markdown',
-    url='https://github.com/gabemorris12/mechanism',
-    license='MIT',
-    classifiers=CLASSIFIERS,
-    packages=find_packages(),
-    install_requires=['matplotlib', 'scipy'],
-    keywords=['mechanism', 'kinematic', 'cams', 'linkages', 'analysis', 'animations'],
-    include_package_data=True
-)
-
-# See this video: https://youtu.be/v4bkJef4W94
-# Don't use the config file though. If you do, you have to use the 'src' folder and that makes things work differently.
-
-# python -m build
-# twine upload dist/*
+from setuptools import setup, find_packages
+import os
+
+THIS_DIR = os.path.dirname(os.path.abspath(__file__))
+
+VERSION = '1.1.8'
+
+CLASSIFIERS = [
+    'Development Status :: 5 - Production/Stable',
+    'License :: OSI Approved :: MIT License',
+    'Operating System :: Microsoft :: Windows',
+    'Programming Language :: Python :: 3.10'
+]
+
+with open(os.path.join(THIS_DIR, 'readme.md'), 'r') as f:
+    LONG_DESCRIPTION = f.read()
+
+setup(
+    name='mechanism',
+    version=VERSION,
+    author='Gabe Morris',
+    author_email='gabemorris1231@gmail.com',
+    description='A package that provides a kinematic analysis of mechanisms and cams and custom tooth profile for spur '
+                'gears.',
+    long_description=LONG_DESCRIPTION,
+    long_description_content_type='text/markdown',
+    url='https://github.com/gabemorris12/mechanism',
+    license='MIT',
+    classifiers=CLASSIFIERS,
+    packages=find_packages(),
+    install_requires=['matplotlib', 'scipy'],
+    keywords=['mechanism', 'kinematic', 'cams', 'linkages', 'analysis', 'animations'],
+    include_package_data=True
+)
+
+# See this video: https://youtu.be/v4bkJef4W94
+# Don't use the config file though. If you do, you have to use the 'src' folder and that makes things work differently.
+
+# python -m build
+# twine upload dist/*
```

