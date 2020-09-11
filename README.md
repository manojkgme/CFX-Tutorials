# CFX Tutorials
 Tutorials created for the ocean engineering under graduate students. The tutorial details different stages involved in the simulation of wave structure interaction using the CFX software in the ANSYS CFD Suite. Two different problems are considered in this tutorial.
1. **Wave interaction with horizontal plate.**
2. **Wave interaction with cylinder.**

Any computational fluid dynamics (CFD) simulation involves the following stages.  

1. **Establishing/Understanding the domain to be simulated.**  
In this stage, the physical area/region to be simulated in considered. It is important to have a larger outlook at this stage. The actual scale of the physical process, various regions of interest, measurement locations etc, are identified and estiblished at this stage.<br />
Video sets
[video 0]
2. **Determining/Specifying the area and physics to be simulated.**  
In many cases, during simulation we can get away with simulating only a part of the physical domain. For example, in the case of a large wave flume that is 30.0 m long, we might not have to simulate the entire physical domain in very high resolution to study a process/event. Instead a small area can be simulated by adopting techniques such as weak coupling and system modelling. By using these techniques the simulation physics and domain can be optimized.<br /> 
Video sets  
[video 1]
[video 2]
3. **Creating the geometry**  
The geometry can be created either using a 3D modelling software or using the meshing tool. In this tutorial, the geometry is created using Autodesk(R) inventor and exported as an IGES file. This geometry is then imported into the meshing tool (ICEM CFD).<br />
Video sets  
[video 3]
[video 4]
4. **Creating the mesh**  
The geometry imported into ICEM CFD is then meshed based on the problem and boundary conditions. While using turbulence models, the boundary effects should be modelled properly for a stable simulation. This can be achieved by optimizing the mesh for [Y plus](https://www.computationalfluiddynamics.com.au/tips-tricks-turbulence-wall-functions-and-y-requirements/#:~:text=The%20y%2B%20value%20is%20a,are%20within%20a%20certain%20range.) values. In this tutorial, a structured mesh approach using the blocking technique is used. The boundaries of the simulation are also specified at this stage. The boundary specification makes it easier to specify the boundary conditions while setting up the simulation.  
The mesh is then exported to a format that can be read by the solver. Since ICEM CFD is a genric meshing tool, it can export the mesh to any format, specific to the solver you want to use. In this case, since we are using the CFX Pre solver, the mesh is exported to *.msh* format.<br />
Video sets  
[video 5]
[video 6]
5. **Setting up the simulation**
Here, the mesh is imported into the solver and the analysis type is specified. In a CFD simulation, the fluids and boundary conditions are specified at this stage along with various simplified physics approximations and order of various solvers. The data management aspects and controls for the solver are also specified at this stage.  
Once the simulation is setup properly, this can be run either on a local machine or a server/High Performace Computing (HPC) facility.<br />
Video sets  
[video 7]
[video 8]
6. **Post processing the results**  
The results from the solver are post processed using the CFD post software. The software also handles visualization and manipulation.<br />
Video sets  
[video 9]
[video 10]