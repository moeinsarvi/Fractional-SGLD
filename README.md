# Fractional Stochastic Gradient Langevin Dynamics

This repository contains a theoretical survey and literature review completed as a course project for High Dimensional Probability. The report explores the mathematical foundations of fractional Langevin dynamics and proposes a conceptual framework for temperature-dependent generalization bounds.

## Project Context
This project is a theoretical exploration and literature survey rather than an empirical study. The primary objective was to demonstrate a rigorous understanding of advanced concepts in stochastic processes, heavy-tailed distributions, and non-convex optimization theory. While no novel mathematical proofs or experimental results are claimed, the report synthesizes current state-of-the-art theories and identifies a clear research gap regarding generalization bounds in heavy-tailed dynamics.

## Overview
Standard Stochastic Gradient Langevin Dynamics (SGLD) relies on Gaussian noise (Brownian motion) to transition from single-point optimization to Bayesian posterior sampling. However, in highly non-convex landscapes, this approach often suffers from metastability—exponentially slow escape times from deep local minima.

Recent literature demonstrates that stochastic gradient noise often exhibits infinite variance, converging instead to a class of heavy-tailed $\alpha$-stable (Lévy) distributions. These fractional dynamics, characterized by discontinuous jumps, allow optimization trajectories to leap directly out of deep valleys, significantly accelerating convergence.

## Key Concepts Surveyed
* **Metastability in SGLD:** The relationship between spectral gaps, inverse temperature ($\beta$), and mixing times in standard Gaussian-driven dynamics.
* **Heavy-Tailed Dynamics:** The transition from Brownian motion to symmetric $\alpha$-stable Lévy processes, defined by stochastic differential equations (SDEs) with fractional drift and diffusion operators.
* **Temperature Scaling:** Recent theoretical frameworks showing that temperature dynamics (rather than spatial dimensionality) can control generalization gaps in standard Langevin processes.

## Theoretical Hypothesis
The report concludes by outlining a theoretical proposal: bridging the convergence benefits of Lévy-driven noise with recent temperature scaling laws. We hypothesize that because the heavy-tailed nature of fractional noise reduces the algorithmic reliance on high temperatures to escape local minima, the tail index $\alpha$ could theoretically be leveraged to derive tighter, noise-aware generalization bounds compared to worst-case Gaussian assumptions.

## Document
The full literature review and mathematical formulations can be found in the attached report:
* [Fractional SGLD Literature Review](./Fractional_SGLD_Literature_Review.pdf)