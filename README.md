# SimulatedAnnealing

This project represents a basic implementation of Simulated Annealing, a global search optimization algorithm.

The program uses a certain number of particles (can be changed by user) and a certain temperature. It will randomize the 
particles' coordinates in space.

It will then "guess" the lowest energy arrangement of the particles, given a random arrangement.
- after the initial guess, the program will make incremental changes to the particle positions and measure the new energy.
- if the new potential energy is lower than the old potential energy, then the new arrangement becomes the "best" guess.
- if the new potential energy is higher than the old potential energy, then the new arrangement has a small chance (depending
on the temp) if the new arrangement becomes the "best" guess
   - this condition prevents the program from getting trapped in local minima.
   

Current issues:
- occasionally results in overflow issues
- the results don't change much after about 50-60 iterations
  - unsure if the true global minima has been found or if the program is just trapped in some local minima
