---
permalink: /code/
layout: single
author_profile: true
title: "Code"
toc: true
toc_label: Content
toc_sticky: true
header:
  overlay_image: /_images/cosmicweb.jpg
  overlay_filter: 0.3
---

# Experience

I mostly write code in Python, occasionally C. In the past few years I have become very familiar with Jax, a Python library for array-oriented numerical computation, with automatic differentiation and JIT compilation to enable high-performance on GPUs. I have substantial experience working with various sampling and optimization methods in high-dimensional parameter space, and I have some machine-learning experience (mostly using Python's scikit-learn library).

I am adept at working with big data sets and running applications in parallel on large super computers. I have significant experience running cosmological N-body simulations using the [GADGET-4](https://wwwmpa.mpa-garching.mpg.de/gadget4/) simulation code, as well as generating linear power spectra with [CAMB](https://camb.readthedocs.io/en/latest/), creating initial conditions with 2nd order Lagrangian Perturbation Theory ([2LPTic](https://cosmo.nyu.edu/roman/2LPT/)), and identifying halos with [ROCKSTAR](https://bitbucket.org/gfcstanford/rockstar/src/main/).

I served as the Allocation Manager for the Large Suite of Dark Matter Simulations (LasDamas) Project on [XSEDE](https://www.xsede.org/) from 2017-2022.

Here are some open-source codes that I have worked on:

## diffsky

I am helping to build a fully differentiable forward modeling pipeline for making predictions of galaxy properties. The diffsky pipeline contains population-level models for predicting galaxy photometry, taking into account dust attenuation, bursty star formation, smooth in-situ star formation, and galaxy merging. The code is written in Jax. The diffsky pipeline brings together several other public codes: [dsps](https://github.com/ArgonneCPAC/dsps), a differentiable stellar population synthesis code; [diffstar](https://github.com/ArgonneCPAC/diffstar), a differentiable model for smooth in-situ star formation; and [diffmah](https://github.com/ArgonneCPAC/diffmah), a differentiable model for smooth halo mass assembly histories. A publication describing the diffsky pipeline is currently in preparation.

[<i class="fab fa-fw fa-github"></i> GitHub](https://github.com/ArgonneCPAC/diffsky){: .btn .btn--primary }

## Halo Mass Corrections

In [Beltz-Mohrmann et al. (2021)](https://ui.adsabs.harvard.edu/abs/2021arXiv210305076B/abstract) I examined the discrepancies in halo masses between dark matter only and hydrodynamic simulations with different baryonic feedback prescriptions. For this work I made use of results from the [Illustris](https://www.illustris-project.org/), [IllustrisTNG](https://www.tng-project.org/), and [Eagle](http://icc.dur.ac.uk/Eagle/) simulations. I determined a correction factor as a function of halo mass that could be used to adjust the halo masses in a given dark matter only simulation to resemble the halos in a given hydrodynamic simulation. I developed a Python module for conveniently implementing these halo mass corrections.

[<i class="fab fa-fw fa-github"></i> GitHub](https://github.com/gbeltzmo/halo_mass_correction){: .btn .btn--primary } 


## Contributions

I have also contributed to the following public codes:

* [ACM](https://github.com/epaillas/acm): a common analysis pipeline for Alternative Clustering Methods in DESI
* [DiffOpt](https://diffopt.readthedocs.io/en/latest/): a collection of tools that are useful for parallelizable optimization of large-parameter, memory-intensive, and/or differentiable models implemented in Jax
* [Corrfunc](https://github.com/manodeep/Corrfunc): a suite of codes to calculate correlation functions and other clustering statistics for simulated and observed galaxies
* [diffmah](https://github.com/ArgonneCPAC/diffmah): a differentiable model for the mass assembly history of individual and populations of dark matter halos
