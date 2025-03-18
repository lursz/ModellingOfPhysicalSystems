Create a Jupyter notebook performing a convergence analysis of the upwind scheme.

Convergence analysis compares how a measure of error (here could be RMSE vs. analytic solution)
changes with changing dt (temporal step, convergence in time) or dx (spatial convergence,
convergence in space). Thus, repeating the calculation for a set of dt or dx, and computing
the error measure in each case is needed. Note that the physical setup and the Courant number 
should remain unchanged, and the Courant number should be set to a value different than zero or
one (as an extension, it is worth checking how the convergence rate differs depending on C).

Create a GitHub Action executing the notebook (see https://nbconvert.readthedocs.io/) 
and uploading the resultant pdf as an action artifact (see https://github.com/actions/upload-artifact).

Scoring:
- 20% narrative explaining the analysis approach, and the goal of the analysis
- 20% Python code implementing the error measure
- 20% Python code implementing the logic repeating the simulations for a range of time or grid steps
- 20% Python code creating a plot with the results of the analysis
- 20% narrative explaining the conclusions (e.g., what one achieves for a given increase of resources)

Essentials: automation leading to vector graphics plot embedded in the pdf with author's name, uploaded as 
GitHub Action artifact. Analysis, plot and resultant pdf should be computed in the cloud.

Submission: sending the location of the repository by e-mail to sylwester.arabas@agh.edu.pl
