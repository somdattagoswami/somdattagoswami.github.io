---
layout: archive
title: "Codes Published"
permalink: /codes/
author_profile: true
---

## Fracture modeling using Physics Informed Neural Network

![](../images/GitHub.png) [Source](https://github.com/somdattagoswami/DEM-PhaseField)

The **P**hysics **I**nformed **N**eural **N**etworks are trained to solve supervised learning problems while respecting any given law of physics described by general non-linear partial differential equations. The developed PINN approach takes a different path by minimizing the variational energy of the system to resolve the crack path within the framework of phase field modeling approach. One major advantage of the variational energy formulation resides in the fact that it requires derivatives of lower order than in the conventional residual minimization approach. Hence, this approach is computationally efficient. The concept of **Transfer Learning** and **Adaptive Refinement Technique** has been integrated with the developed PINN approach.

Companion paper:  
  
  1. [Transfer learning enhanced physics informed neural network for phase-field modeling of fracture](https://doi.org/10.1016/j.tafmec.2019.102447)
  1. [An energy approach to the solution of partial differential equations in computational mechanics via machine learning:Concepts, implementation and applications](https://doi.org/10.1016/j.cma.2019.112790)
  1. [Adaptive fourth-order phase field analysis using deep energy minimization](https://doi.org/10.1016/j.tafmec.2020.102527)

<p align="center">
    <img src="https://github.com/somdattagoswami/somdattagoswami.github.io/blob/master/images/Picture1.png?raw=true" width="650" height="400">
</p>

## Adaptive phase field modeling of fracture using Isogeometric analysis
![](../images/GitHub.png) [Source](https://github.com/somdattagoswami/IGAPack-PhaseField)

- While the phase field approach has numerous advantages for solving complicated fracture paths, the practical application is severely limited due to the computational cost. This is due to the fact that to ensure a numerically stable crack propagation, the size of the elements must be sufficiently small to adequately resolve the damage region.
- Fracture analysis exhibits varying material properties in a local zone. Uniform refinement of the domain requires a significant computational effort when trying to capture quantities of local interest. Hence, an **Adaptive Mesh Refinement Technique** is developed to refine the mesh locally and adaptively, for an accurate and efficient solution. 
- The solution scheme for both the second and the fourth-order phase field model, and is implemented using PHT-splines within the framework of Isogeometric analysis. Both cubic and quadratic stress degradation functions have been used.

Companion paper: [Adaptive fourth-order phase field analysis for brittle fracture](https://www.sciencedirect.com/science/article/pii/S0045782519307005)

<p align="center">
  <img src="https://github.com/somdattagoswami/somdattagoswami.github.io/blob/master/images/CubeWithHole.gif?raw=true" width="500" height="400">
</p>

## Dual mesh approach of fracture modeling using Isogeometric analysis
![](../images/GitHub.png) [Source](https://github.com/somdattagoswami/IGAPack-DualMeshPhaseField)

- PHT splines are C0 continuous at patch boundaries. Hence, these are not suitable for fourth-order phase field modeling with multiple patch geometries, without making any special considerations. 
- The second-order phase field model even though requires C0 smooth basis functions over the whole domain, yet has stringent mesh size requirements. 
- Consequently, a dual-mesh approach for the second-order phase field model is devised, which uses a coarser discretization for the displacement field and a finer discretization for the phase field. 
- The smaller element size in the phase field mesh ensures a numerically stable crack growth, while larger elements in the elastic mesh reduce the computational cost significantly. 
- A recovery-based *a posteriori* error estimator drives the adaptive refinement on the elastic mesh, while a critical threshold value of the phase field parameter determines the need for refinement on the phase field mesh.

Companion paper: [Adaptive phase field analysis with dual hierarchical meshes for brittle fracture](https://www.sciencedirect.com/science/article/abs/pii/S0013794419302814)

<p align="center">
  <img src="https://github.com/somdattagoswami/somdattagoswami.github.io/blob/master/images/Media1.gif?raw=true" width="700" height="500">
</p>

## Monolithic solver for phase-field fracture integrated with fracture energy based arc-length method and under-relaxation
![](../images/GitHub.png) [Source](https://github.com/rbharali/IGAFrac)

- Robust monolithic solver with adaptive under-relaxation and arc-length method.
- Snap-back behaviour is captured with a phase-field fracture energy-based dissipation constraint.
- PHT-splines within IGA framework is utilized for adaptive mesh refinement

Companion paper: [A robust monolithic solver for phase-field fracture integrated with fracture energy based arc-length method and under-relaxation](https://www.sciencedirect.com/science/article/pii/S0045782522001992)

<p align="center">
  <img src="https://github.com/somdattagoswami/somdattagoswami.github.io/blob/master/images/monolithic.gif?raw=true" width="700" height="500">
</p>

## Neural operator learning of heterogeneous mechanobiological insults contributing to aortic aneurysms
![](../images/GitHub.png) [Source](https://github.com/somdattagoswami/Operator-Learning-for-aortic-aneurysms)

- Framework to predict thoracic aortic aneurysm progression by integrating a constrained mixture model for arterial growth and remodeling with a deep neural-network surrogate model
- Consists of 3D finite element simulations of thoracic aneurysm development arising from randomly distributed losses of elastic fiber integrity and dysfunctional mechanosensing.
- Demonstrated improved performance of employing convolutional neural networks in our DeepONet construction.

Companion paper: [Neural operator learning of heterogeneous mechanobiological insults contributing to aortic aneurysms](https://royalsocietypublishing.org/doi/10.1098/rsif.2022.0410)

## A comprehensive and fair comparison of two neural operators (with practical extensions) based on FAIR data
![](../images/GitHub.png) [Source](https://github.com/lu-group/deeponet-fno)

- Practical extensions of DeepONet and FNO that make them more accurate and robust.

Companion paper: [A comprehensive and fair comparison of two neural operators (with practical extensions) based on FAIR data](https://www.sciencedirect.com/science/article/pii/S0045782522001207?via%3Dihub)

## Learning two-phase microstructure evolution using neural operators and autoencoder architectures
![](../images/GitHub.png) [Source](https://github.com/vivek-brown/NPJCOMPUMATS-03747)

- Learning the dynamics of evolution of a two phase mixture suring spinodal decomposition.
- Integrating the developed autoencoder integrated operator newtork with high fidelity solver.

Companion paper: [Learning two-phase microstructure evolution using neural operators and autoencoder architectures](https://www.nature.com/articles/s41524-022-00876-7)

## Deep transfer operator learning for partial differential equations under conditional shift
![](../images/GitHub.png) [Source](https://github.com/katiana22/TL-DeepONet)

- Framework for transfer learning problems under conditional shift with deep neural operators. 
- The proposed framework can be employed for fast and efficient task-specific PDE learning and uncertainty quantification. 
- Leverage principles of the RKHS and the conditional embedding operator theory to construct a new hybrid loss function and fine-tune the target model.

Companion paper: [Deep transfer operator learning for partial differential equations under conditional shift](https://www.nature.com/articles/s42256-022-00569-2)
