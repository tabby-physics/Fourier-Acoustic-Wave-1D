# 1D Fourier Acoustic Wave Simulation

## Overview

This project implements the one-dimensional acoustic wave equation using the **Fourier Pseudospectral Method** in Python.

The simulation computes spatial derivatives using the **Fast Fourier Transform (FFT)** and compares the results with the classical **Finite Difference Method (FDM)**. The project also demonstrates the effects of **numerical dispersion** on wave propagation.

This implementation is based on concepts learned in the Coursera course **Computers, Waves, Simulations**.

---

## Physics Background

The one-dimensional acoustic wave equation is

\[
\frac{\partial^2 p(x,t)}{\partial t^2}
=
c^2
\frac{\partial^2 p(x,t)}{\partial x^2}
+
s(x,t)
\]

where

- **p(x,t)** = acoustic pressure
- **c** = wave velocity
- **s(x,t)** = source function

The solution is obtained using:

- Fourier Pseudospectral Method for spatial derivatives
- Finite Difference Method for time stepping

---

## Numerical Methods

### Fourier Pseudospectral Method

The spatial derivative is computed in the Fourier domain using the Fast Fourier Transform (FFT):

- Transform the pressure field into the frequency domain.
- Multiply by \((ik)^2\).
- Apply the inverse FFT to obtain the second spatial derivative.

This approach provides very high accuracy and significantly reduces numerical dispersion.

### Finite Difference Method

For comparison, the project also includes:

- 3-point finite difference operator
- 5-point finite difference operator

These methods approximate the second derivative using neighboring grid points.

---

## Features

- 1D acoustic wave propagation
- Fourier Pseudospectral Method
- Fast Fourier Transform (FFT)
- 3-point Finite Difference Method
- 5-point Finite Difference Method
- Wave propagation animation
- Numerical dispersion comparison

---

## Technologies Used

- Python
- NumPy
- Matplotlib
- Jupyter Notebook

---

## Learning Outcomes

Through this project I learned:

- Acoustic wave equation
- Fourier Transform
- Fourier Pseudospectral Method
- Fast Fourier Transform (FFT)
- Finite Difference Method
- Numerical dispersion
- Scientific visualization
- Computational Physics

---

## Future Improvements

- 2D acoustic wave simulation
- Elastic wave propagation
- Staggered-grid methods
- Seismic wave modelling
- Absorbing boundary conditions

---

## Author

**Tabassum Tariq**

Computational Physics | Python | Numerical Methods | Scientific Computing

This repository is part of my Computational Physics learning journey, where I implement numerical methods and physics concepts through Python simulations.
