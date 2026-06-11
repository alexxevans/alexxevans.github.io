---
layout: page
title: Generative AI for Cold Atom Interferometry
description: Modelling quantum apparatus for the AION dark-matter and gravitational-wave experiment.
img: assets/img/1.jpg
importance: 1
category: research
related_publications: false
---

As part of my MRes at Imperial College London, I modelled the quantum apparatus used in **AION** (Atom Interferometer Observatory and Network) — a national UK project aiming to detect ultra-light dark matter and gravitational waves through cold-atom interferometry. The model enabled Bayesian inference over the apparatus to find the ideal set of parameters for optimal atom cooling.

**Highlights**

- Ran **2¹⁹ atomic simulations** with parameters drawn from a Sobol sequence on the Imperial College HPC — roughly **22 years of total compute** across 500 concurrent instances.
- Applied **normalising flows and diffusion** to generate cooled atoms for given parameter sets; generated samples were indistinguishable from ground truth to a random forest classifier.
- Developed novel techniques: for normalising flows, an initial denoising phase significantly reduced manifold overfitting; for diffusion, stabilising an approximation of the trace of the Hessian (Jacobian of the score) mitigated overfitting.
- Applied **Bayesian optimisation** to maximise an objective derived from probability of transmission, average velocity, and atom dispersion.

*Techniques:* Diffusion · Normalising Flows · Deep Neural Networks · Decision Trees · Bayesian Optimisation
*Key libraries:* JAX · PyTorch · HyperOpt · XGBoost

This work was presented at **STEM for Britain 2025** in the UK Parliament and to nominees for the RAEng Africa Prize.
