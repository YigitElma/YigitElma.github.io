---
title: "Numerical Simulation of Particle Trajectories in Ion Thruster Grid Region Plasma using a PIC-DSMC Code"
img: IonThruster.webp
collection: project
date: 2022-12-05
---

PLEASE CHECK LATER FOR CONTENT
I WILL COMPLETE THIS PAGE AS SOON AS POSSIBLE

There are many types of propulsion systems used in space applications. The most known category is liquid fueled high thrust rocket engines which are used during the ascend phase of the mission. Generally, these engines fire around 100-120 seconds with extremely high amounts of thrust. Another category is electrified propulsion which uses ionized Xenon gas. Even though they have negligible thrust compared to liquid fueled counterparts, they become beneficial for their efficiency and precision during course correction burns. Long space missions using multiple gravity assists or communications satellites rely on them for their special properties.

Some electric propulsion methods include pressure-feed thrust where the pressure results from the repulsive electric force between ionized gas molecules. The type of system that we are interested in is ion thrusters. They generate plasma by exciting the initially neutral Xenon gas and accelerate it between anode and cathode grids, more specifically screen and acceleration grids. High electric potential causes strong electric field in this region. The grid region is the exact equivalent of the converging-diverging nozzle in liquid fueled engines, except that there is electric force rather than thermodynamic effects during compressible flow.

![Electric Potential](images/electricPotential.png)

A custom finite element code is written in C++ to compute electric potential from Poisson's equation, derive resultant electric field, create ion and neutral macroparticles, move them with electric force and apply collisions or reflections if necessary. ***"PIC"*** stands for *Particle in Cell* method in which motion of the particles executed continuously but a weighting procedure is used to assign them to nearby mesh nodes to be able to solve the finite element equations. ***DSMC*** is acronym for *Direct Simulation Monte-Carlo*. In my opinion, it is a fancy way of saying probability:smile: However, it is extremely useful when an analytical model will be computationally heavier. For our case, we use DSMC to find whether or not a collision has occured, assignment of initial velocity of ions using Maxwellian Velocity Distribution and position assignment for particles to enter into the domain.

Two types of solvers are used to extract electric potential at mesh nodes from discretized Poisson's equation. To optimize the code using the symmetries of the system, we only simulate the triangular prism volume, and use cylindirical coordinates to construct equations. Neumann and Dirichlet boundary conditions are used to specify grid walls and boundaries of the simulation domain.