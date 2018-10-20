CFDTool™ - An Easy to Use CFD Toolbox for MATLAB®
=================================================

![CFDTool Screenshot](https://raw.githubusercontent.com/precisesimulation/cfdtool/master/cfdtool-screenshot.png)


About
-----

[CFDTool](https://www.cfdtool.com)™ is a
[MATLAB](https://www.mathworks.com/products/matlab.html)®
[Computational Fluid Dynamics (CFD)](https://en.wikipedia.org/wiki/Computational_fluid_dynamics)
Toolbox for modeling and simulation of fluid flows
with coupled heat transfer.

Based on [FEATool Multiphysics](https://www.featool.com)™, CFDTool is
specifically designed to make fluid dynamics and heat transfer
simulations both easy and enjoyable.

The CFDTool MATLAB Toolbox includes the following features:

- completely stand-alone and self-contained toolbox
- fully integrated and easy to use Graphical User Interface (GUI)
- modeling and simulation in 1D, 2D, and axisymmetric/cylindrical coordinate systems
- seamless [OpenFOAM](https://www.openfoam.com)® CFD solver integration
- built-in geometry and CAD tools
- automatic mesh and grid generation
- pre-defined equations and boundary conditions for incompressible fluid flows and heat transfer
- simulation of laminar and turbulent flows (k-epsilon and k-omega turbulence models with OpenFOAM)
- stationary and time-dependent analysis types
- postprocessing and visualization


System Requirements
-------------------

Verified to work with Windows, Mac, and Linux systems running MATLAB
R2009b and later.


Installation
------------

Download and extract the CFDTool archive.

- For MATLAB 2012b and later double click on the
  **[CFDTool.mlappinstall](https://github.com/precisesimulation/cfdtool/blob/master/CFDTool.mlappinstall?raw=true)** file, or use the _Get More Apps_ button in
  the MATLAB _APPS_ toolbar. Once the app has been installed, a
  corresponding icon will be available in the toolbar to start
  CFDTool. (Note that MATLAB may not give any indication of the app
  installation progress or completion.)

- For MATLAB 2009b-2012a, copy the **[cfdtool.p](https://github.com/precisesimulation/cfdtool/blob/master/cfdtool.p?raw=true)** file to a
  directory accessible to MATLAB (optionally, copy a corresponding
  _gridgen2d_ binary to enable faster and improved mesh generation,
  _lnx_ file extension for Linux and _exe_ for Windows systems,
  respectively), and then enter

      cfdtool

  on the MATLAB command line to start the application.


OpenFOAM® CFD Solver
--------------------

The optional OpenFOAM CFD solver integration makes it easy to perform
both laminar and turbulent high performance CFD simulations directly
in MATLAB. OpenFOAM CFD simulations often results in a magnitude or
more speedup for instationary simulations compared to the built-in
flow solvers. Additionally, with the multi-simulation solver
integration in CFDTool it is possible to compare and better validate
simulation results obtained using both the built-in and OpenFOAM CFD
solvers.

The OpenFOAM solver binaries are currently not included with CFDTool
and must be installed separately. The OpenFOAM MATLAB solver
integration has been verified with OpenFOAM version 5. For Windows
systems it is recommended to install and use the pre-compiled
blueCFD-core (2017) binaries from
[blueCAPE](http://bluecfd.github.io/Core). For Linux and MacOS systems
the distribution from the
[OpenFOAM Foundation](https://openfoam.org/download) is
recommended. It is necessary that the _simpleFoam_, _pimpleFoam_,
_potentialFoam_, and _collapseEdges_ binaries are installed and
properly set up so they can be called from system script files (bash
scripts on Linux and MacOS and bat/vbs on Windows).


Basic Use
---------

CFDTool and its GUI has been specifically designed to be as easy to
use as possible, and making learning CFD by experimentation possible.

The modeling process is divided into six different steps or modes

- **Geometry** - Definition of the geometry to be modeled
- **Grid** - Subdivision of the geometry into smaller cells suitable
  for computation
- **Equation** - Specification of material parameters and coefficients
- **Boundary** - Boundary conditions specify how the model interacts
  with the surrounding environment (outside the geometry)
- **Solve** - Solution and simulation of the defined model problem
- **Post** - Visualization and postprocessing

These modes can be accessed by clicking on the corresponding buttons
in left hand side _Mode_ toolbar. The different modes may have
specialized and different _Tools_ available in the corresponding
toolbar. Advanced mode options may also be available in the
corresponding menus.

A number of pre-defined fluid flow and heat transfer tutorial examples
are available under the **File** > **Load Example...** menu option.

Basic use and how to set up and model laminar flow past a cylinder is
explained in the video tutorial linked below (click on the image to
start the tutorial).

[![CFDTool Video Tutorial](https://img.youtube.com/vi/ZnnXl7ryBMI/0.jpg)](https://www.youtube.com/watch?v=ZnnXl7ryBMI)


License
-------

(C) Copyright 2013-2018 by Precise Simulation Ltd.
All Rights Reserved.

CFDTool™ and FEATool™ are trademarks of Precise Simulation
Ltd. MATLAB® is a registered trademark of The MathWorks, Inc.
OPENFOAM® is a registered trade mark of OpenCFD Limited, producer and
distributor of the OpenFOAM software via www.openfoam.com. All other
trademarks are the property of their respective owners. Precise
Simulation Ltd and its products are not affiliated with, endorsed by,
sponsored by, or supported by these trademark owners.

The license agreement for using CFDTool is included with the
distribution and can also be accessed from the _Help_ menu in the
application.

Carefully read the license terms and conditions before installing or
using the programs or documentation. Installing or using the programs
means you have accepted and agree to be bound by the terms and
conditions of this agreement. if you do not accept them, uninstall,
remove and completely delete the programs and documentation.
