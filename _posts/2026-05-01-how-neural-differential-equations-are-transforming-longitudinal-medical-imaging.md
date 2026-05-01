---
layout: post
title: How Neural Differential Equations Are Transforming Longitudinal Medical Imaging
date: 2026-05-01 12:00:00-0500
description: Neural ODEs and neural differential equations offer continuous-time models that align naturally with irregular follow-up and disease progression in longitudinal medical imaging.
tags: neural-odes medical-imaging machine-learning longitudinal-data
categories: research
giscus_comments: false
related_posts: true
toc:
  - name: "Part I — The Language of Change"
    subsections:
      - name: "What is a differential equation?"
      - name: "The derivative, measuring instantaneous change"
      - name: "Ordinary differential equations, one variable one rule"
      - name: "Systems of ODEs, when everything affects everything else"
      - name: "Partial differential equations, change across space and time"
      - name: "Solving differential equations, analytical vs numerical approaches"
      - name: "Why most real world equations cannot be solved by hand"
  - name: "Part II — Classical Numerical Methods"
    subsections:
      - name: "Euler's method, the simplest possible solver"
      - name: "Runge-Kutta methods, getting smarter about approximation"
      - name: "Adaptive step size, letting the solver decide how hard to work"
      - name: "Stiffness, when equations become numerically difficult"
      - name: "The initial value problem, starting conditions and uniqueness"
      - name: "Picard's theorem, when does a solution even exist?"
  - name: "Part III — Stochastic Differential Equations"
    subsections:
      - name: "Randomness in dynamical systems, why determinism is not enough"
      - name: "Brownian motion, the physics the history the mathematics"
      - name: "The Wiener process, formalizing randomness over time"
      - name: "Itô calculus, a new kind of calculus for noisy systems"
      - name: "The Itô SDE, drift diffusion and the dW term"
      - name: "Itô vs Stratonovich, two conventions and when each applies"
      - name: "The Fokker-Planck equation, how probability distributions evolve"
      - name: "Jump processes, when systems change discontinuously"
  - name: "Part IV — Neural Differential Equations"
    subsections:
      - name: "Residual networks as discrete dynamical systems"
      - name: "The Euler connection, ResNets are secretly ODE solvers"
      - name: "Neural ODEs, replacing hand-crafted rules with learned ones"
      - name: "The adjoint sensitivity method, backpropagating through a solver"
      - name: "Memory efficiency, why O(1) depth changes everything"
      - name: "Adaptive computation, depth that scales with problem complexity"
      - name: "Neural SDEs, adding learned stochasticity to the dynamics"
      - name: "The drift network f, learning the trend"
      - name: "The diffusion network g, learning the uncertainty"
      - name: "Neural Jump SDEs, modeling sudden discontinuous events"
      - name: "Continuous Normalizing Flows, the change of variables simplification"
  - name: "Part V — Latent Neural Differential Equations"
    subsections:
      - name: "Why operate in latent space, the dimensionality problem"
      - name: "The Latent ODE, VAE encoder meets ODE decoder"
      - name: "ODE-RNN and GRU-ODE-Bayes, updating beliefs at each observation"
      - name: "The Latent SDE, stochasticity throughout the trajectory"
      - name: "What latent spaces need to look like for ODEs to work"
      - name: "Position parameterized ODEs, sharing dynamics across patients"
      - name: "Temporal flow matching, a newer training objective"
  - name: "Further reading"
---

This post is the result of a growing curiosity about the applications of neural differential equations in healthcare. While biomedical imaging is a domain that piques my interest, I want this blog to serve as a comprehensive yet easy-to-understand introduction to neural differential equations. I hope that you, as the reader, find this to be a more accessible introduction than I did when first diving into this field.

Truthfully, as someone who found physics and mathematics more daunting than my peers growing up, it wasn’t always easy for me to grasp concepts that felt intimidating. With this blog post, I hope to take away some of that complexity for fellow peers and researchers who want to better understand neural differential equations and their applications in research.

I also chose to write this blog to organize my thoughts (or, more accurately, to word-vomit them) as I continue my research. If there are any points you’d like to add or correct, please feel free to reach out to me! I am no expert and am always looking to learn more. Anyway, let’s move on!

