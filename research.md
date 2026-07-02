---
layout: page
title: Research
permalink: /research/
---

## Overview
My PhD research mainly revolves around data-efficient machine learning through optimal transport and optimization algorithms, with a particular focus on active learning and coreset selection. 

## Current Projects

### Low-Budget Active Learning Through Entropic Optimal Transport
We address low-budget active learning, where a model should be trained on a small selection only called the coreset. The learning problem formalizes as a combinatorial optimization problem over the hypersimplex, which is provably challenging for existing integer optimization methods and convex relaxations, for complexity and geometry reasons.

We leverage entropic optimal transport, using the Sinkhorn divergence as the coreset selection criterion, which admits computationally efficient gradient evaluations. This opens the way to using gradient-based algorithms to rapidly compute solution candidates, further improved by a swap-based local search, with guarantees on the solution quality. 

Paper submitted and will be published soon on arxiv.

### NetSurvival.jl: A Julia Package for Relative Survival Analysis 
Co-developed **NetSurvival.jl** during my M2 internship, which is a Julia package implementing relative survival analysis algorithms in a modern, high-performance Julia ecosystem. The package provides a pure Julia implementation of established estimators together with documentation, testing, and performance comparisons against existing R software. 

This work was presented at **JuliaCon 2024** in **Eindhoven, Netherlands**.  
Paper: [NetSurvival.jl: A glimpse into relative survival analysis with Julia](https://arxiv.org/pdf/2408.15655)

---

See the [publications page]({{ '/publications/' | relative_url }}) for related papers, or the [CV]({{ '/cv/' | relative_url }}) for a full overview of my academic background.
