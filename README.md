# NOVCA-Visualization

The execuatable "CreateGraph", which by complining using cmake, is executed to get the unstructured VTK file "testVertex.vtu" which is fed to ParaView to get the graph similar to "graphCXX.png".

# CWRU HPC Specific Guide
Login to HPC & load the git module:
* module load git

clone the Repository:
* git clone https://github.com/sxg125/NOVCA-Visualization

Checkout the VTKCxx branch:
* git checkout VTKCxx

Go to NOVCA-Visualization directory:
* cd NOVCA-Visualization

Load vtk,depends and cmake modules:
* module load vtk
* module load depends
* module load cmake

Comiple the Code:
* mkdir buid
* cd build
* ccmake ..
* make

Run the Executable:
* ./CreateGraph

You will get the "testVertex.vtu" file which needs to be fed to the ParaView (https://sites.google.com/a/case.edu/hpc-upgraded-cluster/home/Software-Guide/paraview). Open the file in ParaView, apply glyph and get the one similar to graph "graphCXX.png".
