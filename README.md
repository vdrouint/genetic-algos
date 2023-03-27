# genetic-algos
A ground-up implementation of a genetic algorithm on Python, for future use in a QAOA-type quantum algorithm and optimized adiabatic evolution for general purposes. 

In the bitwise_genetic notebook, you can have fun implementing a bit-wise genetic algorithm to find the minimum of a D-dimensional function. You can feed a N bit string, which will be compiled into a custom float-N (base 2). GO and play around with it!

In genetic_adiabatic_dwave, you can use another genetic algorithm version to optimize the annealing path for a complicated spin glass problem. The goal there is to obtain a good solution faster than with the simple, linear annealing path. 

In prepare-AF-state-w-Pulser, you can use another genetic algorithm version to optimize the annealing path to best prepare an AF state on a chain. It certainly works competitively with other optimizers, like Bayesian optimization. In the future, this will be implemented on solving MIS problems on general unit-disk graphs.

In the future, more notebooks could be added to further probe genetic algorithms and optimization of analog quantum processes. See below for some ideas.

1. Optimizing a reverse annealing schedule. The fidelity criteria could be creating a statistical ensemble of degenerate states (all with same energy but optimizing for the smallest variance). This uses D-Wave.
2. Adiabatic path optimizer but with the Pulser simulator. Paths are spline interpolated from a series of points. Less constraints on the paths. Compare with the Bayesian optimization notebook. (**done**)
3. Adiabatic path optimizer with Pulser simulation for neutral atoms. Find lowest energy solution for a given graph to solve MIS problem on the general graph.
4. Bit-wise optimized for QAOA sequence to solve maxcut problems or other problems on graphs using the Pulser platform.
