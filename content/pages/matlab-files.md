---
content_type: page
description: This section provides supporting MATLAB files for the course.
learning_resource_types: []
ocw_type: CourseSection
title: MATLAB Files
uid: 80a41719-c571-5a2d-7b39-ba2514ef5b68
video_files:
  video_thumbnail_file: null
video_metadata:
  youtube_id: null
---

Many of the MATLAB programs linked below are from the {{% resource_link "e61e4b80-fccf-457e-8bf4-64c136b8f23b" "_Computational Science and Engineering_" %}} ("CSE") Web site. Many more great MATLAB programs can be found there.

*   **Four linear PDE solved by Fourier series:** mit18086\_linpde\_fourier.m ({{% resource_link 327c2253-074f-0051-2050-cfd78937ec5e "M" %}})  
    Shows the solution to the IVPs u\_t=u\_x, u\_t=u\_xx, u\_t=u\_xxx, and u\_t=u\_xxxx, with periodic b.c., computed using Fourier series. The initial condition is given by its Fourier coefficients. In the example a box function is approximated.
*   **Compute stencil approximating a derivative given a set of points and plot von Neumann growth factor:** mit18086\_stencil\_stability.m ({{% resource_link 5d904bd2-074f-e0e6-efc7-db7ca08b9d98 "M" %}})  
    Computes the stencil weights which approximate the n-th derivative for a given set of points. Also plots the von Neumann growth factor of an explicit time step method (with Courant number r), solving the initial value problem u\_t = u\_nx.  
    Example for third derivative of four points to the left:  
    \>> mit18086\_stencil\_stability (-3:0,3,.1)
*   **Error convergence for the 1d Poisson equation:** mit18336\_poisson1d\_error.m ({{% resource_link fd7113ec-bdbd-0e4d-eff4-8ae25eb8c81e "M" %}}) (CSE)  
    Sets up a sequence of 1d Poisson problems, and plots the error convergence on log-log scale.
*   **Sets up and solves a sparse system for the 1d, 2d and 3d Poisson equation:** {{% resource_link "9b9761cc-da0f-4066-959b-23cbf9e7e58b" "mit18086\_poisson.m" %}} (CSE)  
    Sets up a sparse system by finite differences for the 1d Poisson equation, and uses Kronecker products to set up 2d and 3d Poisson matrices from it. The systems are solved by the backslash operator, and the solutions plotted for 1d and 2d.
*   **Computes the LU decomposition of a 2d Poisson matrix with different node ordering:** {{% resource_link "8fff34ff-9446-41e8-a11c-fa754a148605" "mit18086\_fillin.m" %}} (CSE)  
    Sets up a 2d Poisson problem and computes the LU decomposition of the system matrix, firstly with lexicographic ordering, then with red-black ordering and then with symamd ordering.
*   **Demo for elimination with reordering:** moe.m ({{% resource_link 68faedac-f665-3b38-2139-f97869042fe8 "M" %}})  
    Visualizes elimination with various reordering methods for a 2d Poisson problem. Reordering methods are reverse Cuthill-McKee, minimum degree, symamd, and nested dissection.
*   **Computes the incomplete LU factorization of a 2d Poisson matrix for different tolerances:** {{% resource_link "16ad60e9-6938-428c-a760-a28d2d3e2898" "mit18086\_ilu.m" %}} (CSE)  
    Sets up a 2d Poisson problem and computes the LU factorization and the incomplete LU factorization for different tolerances. Run times, condition numbers and nonzero pattern are plotted for comparison.
*   **Smoothing and convergence for Jacobi and Gauss-Seidel iteration:** {{% resource_link "449e0577-ce7b-484d-8ad7-51dba87707ab" "mit18086\_smoothing.m" %}} (CSE)  
    Sets up a 1d Poisson problem with an oscillatory right hand side and applies Jacobi and Gauss-Seidel iteration to it. One can observe how the error gets smoothed very quickly, but the actual convergence to the correct solution is very slow.
*   **Multigrid solver for 1d Poisson problem:** {{% resource_link "4fc578af-78a9-4e72-a2f7-c1de3ec5aa99" "mit18086\_multigrid.m" %}} (CSE)  
    Sets up a 1d Poisson test problem and solves it by multigrid. The method uses two grid recursively using Gauss-Seidel for smoothing and elimination to solve at coarsest level. The number of pre- and postsmoothing and coarse grid iteration steps can be prescribed.
*   **Conjugate gradient method for 2d Poisson problem:** {{% resource_link "ae364612-d575-4b11-9aaa-60c70f4f5d3e" "mit18086\_cg.m" %}} (CSE)  
    Sets up a 2d Poisson problem and solves the arising linear system by a conjugate gradient method. The error over iteration steps is plotted.
*   **Finite differences for the one-way wave equation, additionally plots von Neumann growth factor:** {{% resource_link "16437cb6-1ff8-45dd-9788-026528b2abb9" "mit18086\_fd\_transport\_growth.m" %}} (CSE)  
    Approximates solution to u\_t=u\_x, which is a pulse travelling to the left. The methods of choice are upwind, downwind, centered, Lax-Friedrichs, Lax-Wendroff, and Crank-Nicolson. For each method, the corresponding growth factor for von Neumann stability analysis is shown.
*   **Nonlinear finite differences for the one-way wave equation with discontinuous initial conditions:** {{% resource_link "f0af0a75-3d29-4687-b04e-358d10b06b5a" "mit18086\_fd\_transport\_limiter.m" %}} (CSE)  
    Solves u\_t+cu\_x=0 by finite difference methods. Of interest are discontinuous initial conditions. The methods of choice are upwind, Lax-Friedrichs and Lax-Wendroff as linear methods, and as a nonlinear method Lax-Wendroff-upwind with van Leer and Superbee flux limiter.
*   **Finite differences for the wave equation:** {{% resource_link "f28ff12e-8837-4087-86fe-69d6a236b3ad" "mit18086\_fd\_waveeqn.m" %}} (CSE)  
    Solves the wave equation u\_tt=u\_xx by the Leapfrog method. The example has a fixed end on the left, and a loose end on the right.
*   **Level set method for front propagation under a given front velocity field:** {{% resource_link "62dc6f79-2edf-40c4-bebd-1921f889d4f7" "mit18086\_levelset\_front.m" %}} (CSE)  
    Uses the level set method with reinitialization to compute the movement of fronts under a given velocity field.
*   **Finite differences for the incompressible Navier-Stokes equations in a box:** {{% resource_link "0a117a32-56eb-4eb6-96fd-97e9ab389b97" "mit18086\_navierstokes.m" %}} (CSE)  
    Solves the 2D incompressible Navier-Stokes equations in a rectangular domain with prescribed velocities along the boundary. The standard setup solves a lid driven cavity problem.  
    This Matlab code is compact and fast, and can be modified for more general fluid computations. You can download a Documentation for the program. ({{% resource_link "bdc3a691-ab9b-4d12-bc4e-62e9d85e63bf" "PDF" %}})
*   **Spectral methods for the incompressible Navier-Stokes equations on a torus:** {{% resource_link "122f5402-c154-474f-843e-50d71bc4c97b" "mit18336\_spectral\_ns2d.m" %}} (CSE)  
    Solves the 2D incompressible Navier-Stokes equations in vorticity/stream function formulation on the torus, using spectral methods.