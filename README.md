# Solver-Navier-Stokes-and-advection-convection-equations-Polution-trasport-in-rivers
This is a code that solves the problem of pollutant transport in a river using the Navier-Stokes equations to model the river and the Advection-Convection equations for pollutant transport.  It is solved through the use of finite element techniques, using the FEniCS package.

The problem that solve is the transport of pollution in a part of Santiago River, near of Juanacatlán, Jal, Mex.

Code was thinking to work wiht a mesh generated with a .txt file that generate a .msh file and converte to a .xml file 

If you work with a .geo file, it's necesary adapt the code or chance to .txt

there are some fiscal parameters that can break the solver, in particular diffusivity coefficient (D). If D << 1 could generated numerical noise.

To solve Navier-Stokes (N-S) equations, it's used chorin metod, and an explicit discretization on time. 
To solve Advection-Convection (A-C) equations it's used an explicit discretization on time.

This code obtain the soloution for:
  scalar velocity field
  vectorial velocity field
  scalar pressure field
  scalar pollutions field

Each m time step, a PDF is saved with the solution of these four fields and is stored in their respective folders. When the simulation time is over, all the PDFs are converted into a GIF and the folders are downloaded
