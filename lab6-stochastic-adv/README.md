Extend the Monte-Carlo advection solver to two spatial dimensions (e.g., a grid of 32x32 cells).
Define a two-dimensional constant-in-time flow field (with both components not zero). 
Define an 2D initial condition condition.

- 20% for implementing 2D advection
- 20% for analysis of the result vs. analytic solution
- 20% for narrative explaining the goal and conclusions
- 20% plot quality: vector graphics, axes labelled, font size matches text size, reasonable number of lines and colours
- 20% `nbqa pylint` gives no errors

As an extension (so-called [Molenkamp test](https://doi.org/10.1175/1520-0450(1968)007%3C0160:AOFDMA%3E2.0.CO;2)):
- use a non-divergent advector that results in a flow that rotates the signal around the centre of the domain;
- define initial scalar field to be a localised shape in an off-centre location (and zeros elsewhere);
- perform a number of full rotations;
- compare the result with the initial condition for checking accuracy.