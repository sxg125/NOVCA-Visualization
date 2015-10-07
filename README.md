# Table of Contents
1. [NOVCA-Visualization](#NOVCA-Visualization)
2. [CWRU HPC Specific Guide](#CWRU HPC Specific Guide)

<div id='NOVCA-Visualization'/>
## NOVCA-Visualization
The python script "paraviewGraph.py" is executed to get the unstructured VTK file "vertex.vtu" which is fed to ParaView to get the graph similar to "graph.png".
<div id='CWRU HPC Specific Guide'/>
## CWRU HPC Specific Guide
Login to HPC & load the git module:
```
module load git
```
Clone the Repository:
```
 git clone https://github.com/sxg125/NOVCA-Visualization
```
Go to NOVCA-Visualization directory:
```
cd NOVCA-Visualization
```
Load vtk and python modules:
```
module load vtk
module load python
```
Run the python script:
```
python paraviewGraph.py
```
You will get the "vertex.vtu" file which needs to be fed to the ParaView- [ParaView] (https://sites.google.com/a/case.edu/hpc-upgraded-cluster/home/Software-Guide/paraview). Open the file in ParaView, apply glyph and get the one similar to graph "graph.png".
## References
1. [VTK/Python] (http://www.vtk.org/Wiki/VTK/Examples/Python/Graphs/NOVCAGraph)
2. [VTK/Cxx] (http://www.vtk.org/Wiki/VTK/Examples/Cxx/Graphs/NOVCAGraph)
