---
layout: archive
title: "Codes published"
permalink: /codes/
author_profile: true
---

## Fracture modeling using Physics Informed Neural network

![](../images/GitHub.png) [source](https://github.com/lululxvi/deepxde)

DeepXDE is a deep learning library for solving differential equations on top of [TensorFlow](https://www.tensorflow.org/).

Use DeepXDE if you need a deep learning library that

- solves partial differential equations (PDEs),
- solves integro-differential equations (IDEs),
- solves fractional partial differential equations (fPDEs),
- solves inverse problems for differential equations,
- approximates functions from a dataset with/without constraints,
- approximates functions from multi-fidelity data.

DeepXDE is extensible to solve other problems in scientific computing.

#![](../images/deepxde.png)

## Adaptive phase field modeling of fracture using Isogeometric analysis
![](../images/GitHub.png) [source](https://github.com/somdattagoswami/IGAPack-PhaseField)

- Phase field modeling of fracture is a popular approach in the category of continuous fracture modeling approach. This approach aims to simultaneously solve for the displacement field and fracture region by energy minimization and no assumption for the evolution of the cracks is needed, thereby generalizing the Griffith's theory for brittle fracture.  
- While the phase field approach has numerous advantages, the practical application is severely limited due to the computational cost. In order to ensure a numerically stable crack propagation, the size of the elements must be sufficiently small to adequately resolve the damage region.
- Fracture analysis exhibits varying material properties in a local zone. Uniform refinement of the domain requires a significant computational effort when trying to capture quantities of local interest. To make the computational model efficient, we propose an adaptive mesh refinement approach, where we design a refinement scheme to refine the mesh locally and adaptively, for an accurate and efficient solution. 
- The solution scheme for both the second and the fourth-order phase field model is implemented using PHT-splines within the framework of Isogeometric analysis. Both cubic and quadratic stress degradation functions have been used.

Companion paper: [Adaptive fourth-order phase field analysis for brittle fracture](https://www.sciencedirect.com/science/article/pii/S0045782519307005)

![](../images/CubeWithHole.gif)

## Dual mesh approach of fracture modeling using Isogeometric analysis
![](../images/GitHub.png) [source](https://github.com/somdattagoswami/IGAPack-DualMeshPhaseField)

- PHT splines are C0 continuous at patch boundaries. Hence, thesis are not suitable for fourth-order phase field modeling with multiple patch geometries. 
- The second-order phase field model requires C0 smooth basis functions over the whole domain. Consequently, a dual-mesh approach for the second-order phase field model is devised, that allows to relax the stringent mesh refinement criteria. 
- The dual-mesh uses a coarser discretization for the displacement field and a finer discretization for the phase field. The smaller element size in the phase field mesh ensures a numerically stable crack growth, while larger elements in the elastic mesh reduce the computational cost significantly. 
- Also, independent refinement strategies for both the fields are employed. A recovery-based *a posteriori* error estimator drives the adaptive refinement on the elastic mesh, while a critical threshold value of the phase field parameter determines the need for refinement on the phase field mesh.

Companion paper: [Adaptive phase field analysis with dual hierarchical meshes for brittle fracture](https://www.sciencedirect.com/science/article/abs/pii/S0013794419302814)

![](../images/Media1.gif)
