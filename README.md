# Vehicle Routing

> Note: in compliance with Brown's Academic Code, the actual code is not uploaded.

[Presentation](/reports/presentation.pdf) | [Problem Description](/reports/Transportation%20and%20Logistics.pdf)

A local search solver for the [vehicle routing problem](https://en.wikipedia.org/wiki/Boolean_satisfiability_problem) (VRP) implemented in Python.

## Features

1. Greedy preprocessing to generate initial route assignment
1. Neighborhood portfolio for robust local search
1. Simulated annealing metaheuristic to encourage exploration

## Usage

To use the solver

```bash
python <input-file>
```

The input file format is described in the [Problem Description](/reports/Transportation%20and%20Logistics.pdf). Some examples are provided in the [input](/input) folder.

You can also export the solution into a file using the `VRPSolution`'s `export` method. The results can be visualized with this [online tool](http://cs.brown.edu/courses/csci2951-o/p5vis.html).

Optionally, you can use [PyPy](https://www.pypy.org/) instead of Python to massively speed up performance.

## Caveats

In case this isn't clear, the solver searches for improving solutions but does not guarantee optimality in any way. This is standard for VRP solvers as the problem is NP-hard.

## Credits

This VRP solver was created by [Alex Ding](https://github.com/alexander-ding/) and [Aaron Wang](https://github.com/aaronwangj) for Brown University's [CSCI 2951-O](http://cs.brown.edu/courses/csci2951-o/) course in Spring 2022.
