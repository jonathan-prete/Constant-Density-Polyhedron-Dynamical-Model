# Constant-Density-Polyhedron-Dynamical-Model

The MATLAB model here presented performs trajectory propagations based on the Constant Density Polyhedron algorithm proposed by Werner[1].

# DynamicalModel.mlx
Use script 'DynamicalModel.mlx' to compute trajectories. A list of sample orbits can be found below.

# importSTLmodel.mlx
Use script 'importSTLmodel.mlx' to import 3D astronomical body shapes in STL format. More astronomical bodies in STL format can be found here: https://nasa3d.arc.nasa.gov/models
After importing the STL model, a workspace is created containing the triangulation data of the body shape.
Note that the function 'selectBody.mlx' must be changed as well to include the new body shape. 

# Sample Orbits
state_vector = [-1689.9 4086.1 5136.9 -6.0545 -4.4489 1.541].*10^3;   %Earth ISS orbit
state_vector = [8000 0 0 0 0 7.05556].*10^3;                          %Earth Circular orbit
state_vector = [8000 0 0 0 9 0].*10^3;                                %Earth elliptical orbit
 
state_vector = [7000 0 0 0 0.39128 0 ];                               %Toutatis high altitude circular orbit
state_vector = [2600 0 0 0 0.6315 0 ];                                %Toutatis low altitude circular orbit
state_vector = [3000 0 0 0 0.75 0 ]                                   %Toutatis elliptical orbit
state_vector = [3000 0 0 -0.9 0.4 0 ];                                %Toutatis landing trajectory
 
state_vector = [350 0 0 0 0.17 0];                                    %Bennu elliptical orbit
state_vector = [350 0 0 0 0.127 0];                                   %Bennu circular orbit
state_vector = [346.41 0 200 0 0.1184 0];                             %Bennu low altitude circular orbit with inclination
 
state_vector = [0 1600 0 -0.2 -0.2 0.1];                              %HW1 landing trajectory
state_vector = [0 2000 0 0.4766 0 0];                                 %HW1 low altitude Circular orbit 
state_vector = [0 5500 0 0.2933 0 0];                                 %HW1 high altitude circular orbit 

# Reference
[1] Exterior gravitation of a polyhedron derived and compared with harmonic and mascon gravitation representations of asteroid 4769 Castalia. Robert A. Werner and Daniel J. Scheeres 1996
