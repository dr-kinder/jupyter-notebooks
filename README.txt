These are code fragments for _A Student's Guide to Python for Physical
Modeling_ by Jesse M. Kinder and Philip Nelson.

www.amazon.com/Students-Guide-Python-Physical-Modeling/dp/0691223653

Use of these code fragments is subject to the terms of LICENSE.txt.

This file provides a brief description of each fragment.  More details
can be found in the comments of the individual scripts and modules.

------------------------------------------------------------------------- 

CONTENTS
--------

Each Jupyter notebook contains a functional code fragment in single a
code cell.  The name of the notebook is the name of the script, but with
a `.ipynb` extension.  For example, the code sample `projectile.py` is
contained in `projectile.ipynb`.

The folder also contains auxiliary files necessary to run some of the
code samples.

- HIVseries.csv
- g26perrin.npy
- html_movie.py
- simple_oscillator.py
- parametric_oscillator.py
- first_passage.py

The order of appearance of code samples in the text (Second Edition) is
as follows:

* Chapter 2
	- string_format.py
	- string_percent.py
	- for_loop.py
	- while_loop.py
* Chapter 3
	- vectorize.py
	- projectile.py
	- branching.py
	- nesting.py
* Chapter 4
	- import_text.py
	- save_load.py
	- print_write.py
	- simple_plot.py
	- graph_modifications.py
	- line3d.py
	- subplot.py
	- subplots.py
* Chapter 6
	- measurements.py
	- rotate.py
	- average.py
	- histogram.py
	- contour.py
	- matrix_inversion.py
	- quadrature.py
	- simple_oscillator.py
	- solve_ode.py
	- parametric_oscillator.py
	- ivp_comparison.py
	- vortex.py
	- gradient.py
	- streamlines.py
* Chapter 8
	- data_images.py
	- walker.py
	- waves.py
* Chapter 9
	- convolution.py
* Chapter 10
	- first_passage.py
	- data_dictionary.py
	- nd_random_walks.py
* Epilogue
	- surprise.py
* Appendix F
	- scope.py
	- name_collision.py
* Your Turn
	- fancy_plot.py
	- legend.py
	- measurements.py
	- random_walk.py
	- surface.py
	- regression.py
* Additional
	- bar3d.py
	- html_movie.py 
	- perrin.py
	- shading.py
	- sympy_examples.py


DESCRIPTIONS
------------

### string_format.py

Illustrate string formatting using the .format() method.

### string_percent.py

Illustrate string formatting using the % method.

### for_loop.py

Use a for loop to generate solutions to the quadratic equation.

This script illustrates the funamental form of a for loop.  For
alternate solutions to the same problem, see while_loop.py and
vectorize.py.

### while_loop.py

Use a while loop to generate solutions to the quadratic equation.

For alternate solutions to the same problem, see for_loop.py and
vectorize.py.

### vectorize.py

Use vectorized code to generate solutions to the quadratic equation.

For alternate solutions to the same problem, see for_loop.py and
while_loop.py.

### projectile.py

Calculate how long an object is in the air when thrown from a spcified
height with a range of initial speeds assuming constant acceleration due
to gravity:

	0.5 * g * t**2 - v0 * t - y0 = 0

This script illustrates good coding practice in the solution of a simple
problem: parameters with descriptive names, comments, whitespace, and
blocking with '#%%' for debugging in Spyder.

### branching.py

This script illustrates branching with the use of multiple conditional
statements:
	if <condition1>:
		...
	elif <condition2>:
		...
	else:
		...

### nesting.py

Use nested for loops to fill a two-dimensional array of values.

This script illustrates "nesting" --- one for loop inside of another.

### import_text.py

Load data from a text file by reading the file line by line.

This script reads in data from a text file and stores it in a NumPy
array.  It can be adapted to load data from files that are difficult or
impossible to load with NumPy's np.loadtxt function.

### save_load.py

Save array data using NumPy's available methods, then load saved data.

This script demonstrates the various methods of saving and loading data
using NumPy arrays.

### print_write.py

Write same data to a file and print to display.

This script illustrates the similarites between writing to a text file
and printing to the screen.

### simple_plot.py

Create and display a basic plot.

### graph_modifications.py

This script creates a simple plot with two lines, then modifies several
features of the plot, including axis labels, data labels, legend, line
style, tick labels, and title.

### line3d.py

Create a three-dimensional parametric plot.

This script demonstrates how to create three-dimensional plots using the
Axes3D method from the mpl_toolkits.mplot3d module.  See also surface.py.

### subplot.py

Create four plots in the same figure using plt.subplot().

This script demonstrates PyPlot's subplot method, which can be used to
display several plots side-by-side in the same figure.  For another
approach, see subplots.py.  The names are similar, but the behavior of
the plt.subplot and plt.subplots is different.

### subplots.py

Create four plots in the same figure using plt.subplots().

This script demonstrates PyPlot's subplots method, which can be used to
display several plots side-by-side in the same figure.  For another
approach, see subplots.py.  The names are similar, but the behavior of
the plt.subplot and plt.subplots is different.

### measurements.py

Functions to calculate distance between points using different metrics.

This script illustrates the fundamental form of user-defined functions
as well as keyword arguments and default values.

### rotate.py

Define function to rotate a vector in two dimensions.

### average.py

Compute and return the cummulative average of an array.

This script illustrates some principles of functional programming.

### histogram.py

Create histograms of random numbers.

This script illustrates how to use NumPy and PyPlot to create histograms
and bar plots.

### contour.py

Create a labeled contour plot.

This script illustrates how to generate a grid of coordinates for
contour and surface plots.  It also demonstrates some options of
plt.contour and shows how to label contour lines.

### matrix_inversion.py

Invert a simple matrix to solve a system of linear equations.

This script illustrates the use of a special method from the SciPy linear
algebra library, scipy.linalg.

### quadrature.py

Integrate two functions using quad.

This script demonstrates numerical integration using the quad method of
scipy.integrate.  The first function is a built-in NumPy funciton whose
integral can be computed with pencil and paper for comparison.  The
second is a user-defined function.

### simple_oscillator.py

Define function to use in solution of differential equation for a simple
harmonic oscillator.

This script illustrates how to write a function that generates the array
required to integrate a second-order ordinary differential equation.  It
is imported and used in solve_ode.py.

### solve_ode.py

Solution of ODE for harmonic oscillator.

This script imports the function F(y,t) in simple_oscillator.py then
uses the odeint method of scipy.integrate to solve the ordinary
differential equation defined by F(y,t).

See ivp_comparison.py for an example of the solve_ivp method, an
alternative to odeint.

### parametric_oscillator.py

Define a parametric function that accepts 4 parameters then integrate it
using odeint.

This script illustrates two methods for using scipy.integrate's odeint
methods to integrate a function that accepts more than two parameters.

### ivp_comparison.py

Compare different ODE solvers using solve_ivp.

solve_ivp offers an alternative to odeint for solving ordinary
differential equations.  See solve_ode.py for an example of odeint.

### vortex.py

Create a quiver plot.

This script illustrates the use of PyPlot's quiver method.

### gradient.py

Calculate and display the gradient of a two-dimensional Gaussian.

This script illustrates the use of NumPy's gradient function and
demonstrates how to display a vector field.  It displays the gradient as
a quiver plot superimposed on a filled contour plot of the Gaussian.

### streamlines.py

Create streamlines from a vector field.

This script demonstrates the use of PyPlot's streamplot method for
visualizing solutions to a differential equation defined by a vector
field.

### data_images.py

Illustrate differences between image and Cartesian coordinates.

The coordinates used in plotting functions and displaying images follow
different conventions.  This script creates a figure that illustrates
the two conventions.

### walker.py

Make a movie out of the steps of a two-dimensional random walk.

This script demonstrates the use of the FuncAnimation method of
Matplotlib's animation module to create a movie.  If ffmpeg or mencoder
is installed on this computer, the script will save the movie to an mp4
file.

### html_movie.py

Module to generate an HTML document from a collection of images.  When
viewed in a Web browser, the document will display a movie whose frames
are the individual images.

This module is adapted from the scitools library developed by Hans
Petter Langtangen.

### waves.py

Create an HTML animation of a moving Gaussian waves.

This script illustrates a method for combining a series of plots into an
animation using HTML and Javascript.  It uses the html_movie.py module,
which is  adapted from the scitools library developed by Hans Petter
Langtangen.

### convolution.py

This script creates an eLoG (elongated Laplacian of Gaussian) filter
that emphasizes long, vertical lines in a figure.  The effect of the
filter is demonstrated on a plus sign.

### sympy_examples.py

Demonstrate some useful methods available in the SymPy module.

Python may complain about undefined variables if you attempt to run this
script.  init_session() defines several variables, but Python may not be
aware of this.  It is better to run the commands one at a time from the
command line.

### first_passage.py

Define a function to simulate first passage of a random walker.

Simulate a random walker that starts at the origin and takes steps to
the right with probability p and to the left with probability 1-p.
Return the number of steps for the first passage of location x==L, or
give up after N steps.

### data_dictionary.py

Store input and data two different simulations in a dictionary.

This script requires first_passage.py to be in the same directory.

### nd_random_walks.py

Python class to simulate various random walks in N dimensions.

```
RandomWalk -- general random walk class
	LatticeWalk     --  random walk on a D-dimensional lattice
					    default is a cubic lattice in D dimensions
		TriangularWalk  -- 2D triangular lattice
		HoneycombWalk   -- 2D honeycomb lattice
	DirectionalWalk --  random walks of variable step size in D dimensions
				        defaults to constant step length in random directions
		UniformWalk     -- step size drawn from uniform distribution
		GaussianWalk    -- step size drawn from normal distribution
		ExponentialWalk -- step size drawn from exponential distribution
		ParetoWalk      -- step size drawn from power law distribution
```

### surprise.py

This script will create a familar but interesting image.
It may take about a minute to run.

### scope.py

Demonstrate Python's rules of scope --- i.e., how Python looks up
variable names.

### name_collision.py

Illustrate how Python's rules of scope prevent name collisions.

### fancy_plot.py

Add a title and axis labels to a simple plot.

### legend.py

Create a plot with a legend to distinguish multiple curves.

### random_walk.py

Monte Carlo simulation of a two-dimensional random walk.

This script illustrates the use of a random number generator to create a
time series for a random walk.

### surface.py

Create a three-dimensional surface plot.

This script demonstrates how to create three-dimensional plots using the
Axes3D method from the mpl_toolkits.mplot3d module.  See also line3d.py.

### regression.py

Example of linear regression on data from the first passage problem.

first_passage.py must be in the working directory.  The script could
take a while to finish if (samples x nmax) ~ 10**8 or more.

### bar3d.py

Create a 3D histogram ("Lego plot").

This script provides a visual example of the Central Limit Theorem.

### perrin.py

Generate figure displaying Perrin's experimental data on Brownian
motion.  This script requires the data set 04brownian/g26perrindata.npy.

The script illustrates loading and plotting a data set and includes
LaTeX formatting of axis labels and grid lines.

### shading.py

Demonstrate shading of surface plots using Matplotlib's LightSource.

------------------------------------------------------------------------- 
