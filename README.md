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

![image](https://github.com/ABr-hub/Drawings/blob/54b9f1b913f9104237bc38907ef5eb812f4aa56d/EnvelopeSpectrumAnalysis.drawio.svg)
![image](https://github.com/ABr-hub/Drawings/blob/7853b6cb0d272d8e6935271420ccad13aba95cc6/FailureIdentificationCNN.drawio.svg)
