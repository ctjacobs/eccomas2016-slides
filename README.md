# Overview

Slides for the talk entitled "On the validity of tidal turbine array configurations obtained from steady-state adjoint optimisation", given at the [VII European Congress on Computational Methods in Applied Sciences and Engineering (ECCOMAS 2016)](http://www.eccomas2016.org/) in Crete, Greece. Slide files available from the `gh-pages` branch of this repository. The slides are also available to [view online](http://christianjacobs.uk/eccomas2016-slides/).

# Abstract

Extracting the optimal amount of power from an array of tidal turbines requires an intricate understanding of tidal dynamics and the effects of turbine placement on the local and regional scale flow. Numerical models have contributed significantly towards this understanding, and more recently, adjoint-based modelling has been employed to optimise the positioning of the turbines in an array in an automated way and improve on simple man-made configurations (e.g. structured grids of turbines) [(Funke et al., 2014)](http://dx.doi.org/10.1016/j.renene.2013.09.031).

Adjoint-based optimisation of high-resolution and ideally 3D transient models is generally a very computationally expensive problem. Multiple approaches are therefore used in practice to obtain feasible runtimes: using high viscosity values to obtain a steady-state solution, or a sequence of steady-state solutions for "time-varying" setups; limiting the number of adjoint computations; or reformulating the problem to allow for coarser mesh resolution to make it feasible for resources assessment (e.g. [Funke et al., (Submitted)](http://arxiv.org/abs/1507.05795), Culley et al. (2015)). However, such compromises may affect the reliability of the modelled turbines, their wakes and interactions, and thus bring into question the validity of the computed optimal turbine positions.

This work considers a suite of idealised simulations of flow past tidal turbine arrays in a two-dimensional channel. It compares four regular array configurations, detailed by Divett et al. [(Divett et al., 2013)](http://dx.doi.org/10.1098/rsta.2012.0251), with the configuration found through adjoint optimisation in a steady-state, high-viscosity setup. The optimised configuration produces considerably more power than the other configurations (approximately 40% more than the best man-made configuration). The same configurations are then used to produce a suite of transient simulations that do not use constant high-viscosity, and instead use large eddy simulation (LES) to parameterise the resulting turbulent structures. All simulations are performed using OpenTidalFarm [(Funke et al., 2014)](http://dx.doi.org/10.1016/j.renene.2013.09.031).

It is shown that the 'low background viscosity'/LES simulations produce less power than that predicted by the constant high-viscosity runs. Nevertheless, they still follow the same trends in the power curve throughout time, with optimised layouts continuing to perform significantly better than simplified configurations.

# Conference paper

The details of the conference paper associated with this talk are:

C. T. Jacobs, M. D. Piggott, S. C. Kramer, S. W. Funke (2016). **On the validity of tidal turbine array configurations obtained from steady-state adjoint optimisation**. In *Proceedings of the VII European Congress on Computational Methods in Applied Sciences and Engineering (ECCOMAS Congress 2016)*. Pre-print: [http://arxiv.org/abs/1601.08091](http://arxiv.org/abs/1601.08091)
