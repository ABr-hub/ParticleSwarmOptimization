# ParticleSwarmOptimization
This repo demonstrates a use case (solving required input parameters) for the popular particle swarm optimization and it's solution.

---
### PSO 

Particle Swarm Optimization (PSO) is a population-based optimization algorithm inspired by social behavior observed in bird flocking or 
fish schooling. It was originally developed by James Kennedy and Russell Eberhart in 1995. The basic idea behind PSO is to model the 
optimization process as a swarm of particles moving through a search space to find the optimal solution.

Here's a brief description of how PSO works:

1. ***Initialization***:
    Initialize a swarm of particles with random positions and velocities within a defined search space.
    Evaluate the fitness of each particle based on an objective function.

2. ***Update*** Particle Positions and Velocities:
    Update each particle's velocity and position using its own best-known position and the best-known position of the entire swarm.
    The movement is guided by the particle's own experience and the collective knowledge of the swarm.

3. ***Evaluate Fitness***:
    Evaluate the fitness of the particles' new positions.

4. ***Update*** Personal and Global Bests:
    Update each particle's personal best position if its fitness improves.
    Update the global best position based on the best fitness value found by any particle in the entire swarm.

5. ***Repeat***:
    Repeat steps 2-4 for a specified number of iterations or until a termination criterion is met.

The figure below demonstrates how PSO swarms the various particles around the target area of optimization. The goal of PSO, therefore,
is to find the optimum parameters that solve the problem best.

![image](https://github.com/ABr-hub/ParticleSwarmOptimization/blob/ae4f3612cc8cee0bdd2f4df5c6e749e509f51160/ressources/PSO_Principle.svg)

---
### Sample optimization problem

PSO is frequently applied to address the determination of necessary input parameters in a given equation or function. 
To illustrate, if the objective is to launch a cannonball to a predefined distance, one would take into account the 
physics-based equation depicted in the figure below.
In the case presented here, the PSO algorithm is applied to find the desired optimum initial velocity $v_i$ of the shot and the 
angle $a$ at which it is shot.

![image](https://github.com/ABr-hub/ParticleSwarmOptimization/blob/2e8d4336904b68c562d7243337cf08fc926266ab/ressources/CannonOptimization.svg)

The below simulation demonstrates how the particle swarm searches the optimization space to end up in the optimal solution. 
It is noteworthy that there exist two viable solutions for both the angle and velocity within this problem. Furthermore, 
the particles display a discernible dispersion across the solution space, a phenomenon primarily influenced by the selection 
of hyperparameters. The degree of particle spread can be modulated through the careful adjustment of these parameters.

![](https://github.com/ABr-hub/ParticleSwarmOptimization/blob/a0e40e84aad239bb120d579c1f5b8c142ed1bc2b/ressources/PSO_2Solution.gif)
