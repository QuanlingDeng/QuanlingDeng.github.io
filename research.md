---
title: Research
layout: default
---

## Research interests
- Mathematical modeling and simulation: fluid flow through poroelastic media, ocean and atmosphere dynamics, sea ice floe dynamics.

- Scientific computing and numerical analysis: parallel computing, preconditioners, post-processing, PDE numerical solvers such as FDM, FVM, FEM, IGA, DG, HHO, Runge--Kutta methods, and generalized-alpha methods, operator splitting schemes, dispersion and spectral analysis, a priori and a posteriori error analysis.

- Uncertainty quantification and data assimilation: stochastic models, Kalman filters, Ornstein-Uhlenbeck process.

- Artificial intelligence and machine learning: particle swarm optimization, physics-informed neural networks, supervised learning.

## Publications 
- See [Google Scholar Profile](https://scholar.google.com/citations?user=PBGaQ44AAAAJ&hl=en), or
- See [ResearchGate Profile](https://www.researchgate.net/profile/Quanling-Deng), or
- See [CV here](https://quanlingdeng.github.io/deng.pdf).


## Several research lines

* * *
**Development of FEM approximations**

(1) A FEM approximated solution lacks the local conservation property on its fluxes. We propose a simple and efficient postprocessing technique to recover the locally conservative fluxes on control volumes (FEM dual mesh elements). The technqiue solves an elemental Neumann-boundary value problem and it can be naturally implemented in a parallel environment. See below figures for control volumes for rectangular and triangular elements. See [this paper](https://www.sciencedirect.com/science/article/pii/S0377042719301803) for details. 

<table class="fixed">
  <col width="200"/>
  <col width="200"/>
  <tr>
    <td> 
        <div class="card" style="width: 20rem;">
          <img src="images/cv0.jpg" alt="" class="img-responsive"> 
        </div>
    </td>
    <td> 
        <div class="card" style="width: 20rem;">
          <img src="images/cv1.jpg" alt="" class="img-responsive"> 
        </div>
    </td>
 </tr>
</table> 
  
  
(2) Quadratic and higher-order FEMs suffer from high stiffness (large condition numbers) in their discretised systems. We propose to reduce the stiffness of the problem by subtracting a least-squares penalty on the gradient jumps across the mesh interfaces from the standard stiffness bilinear form. The two key advantages of softFEM over the standard Galerkin FEM are to improve the approximation of the eigenvalues in the upper part of the discrete spectrum and to reduce the condition number of the stiffness matrix. The resulting approximation technique is called softFEM since it reduces the stiffness of the problem. See below a figure which compares the quadratic softFEM with FEM on spectral and eigenstate errors. See [this paper](https://www.sciencedirect.com/science/article/pii/S0898122121003382) for details. 

<table class="fixed">
  <col width="600"/>
  <col width="300"/>
  <tr>
    <td> 
        <div class="card" style="width: 40rem;">
          <img src="images/softfem.jpg" alt="" class="img-responsive"> 
        </div>
    </td>
 </tr>
</table> 

* * *

**Spectral approximation with finite and isogeometric elements**  

(1) The spectral approximation by isogoemetric analysis has outliers (large eigenvalue errors) in the high-frequency region. We propose a boundary penalty technique to remove the outliers and consequently reduce the stiffness (condition numbers) of the discretised system; See below a figure where the large spectral errors have been significantly reduced. See [this paper](https://www.sciencedirect.com/science/article/pii/S0045782521002449) for details. 

<table class="fixed">
  <col width="600"/>
  <col width="300"/>
  <tr>
    <td> 
        <div class="card" style="width: 40rem;">
          <img src="images/iga.jpg" alt="" class="img-responsive"> 
        </div>
    </td>
 </tr>
</table> 


(2) In general, when the domain of the model problem is irregular, the discontinuous Galerkin (DG) methods perform better than the standard FEMs. We develop hybrid high-order (HHO) DG method to approximate the spectra of the second-order elliptic operator on irregular domains. See below the HHO approximated eigenmodes on a circular and an L-shaped domain. See [this paper](https://www.ams.org/mcom/0000-000-00/S0025-5718-2018-03405-6/) for details.

<table class="fixed">
  <col width="200"/>
  <col width="200"/>
  <tr>
    <td> 
        <div class="card" style="width: 20rem;">
          <img src="images/circle_ef1.jpg" alt="" class="img-responsive"> 
        </div>
    </td>
    <td> 
        <div class="card" style="width: 20rem;">
          <img src="images/lshape_ef1.jpg" alt="" class="img-responsive"> 
        </div>
    </td>
 </tr>
 <tr>
    <td> 
        <div class="card" style="width: 20rem;">
          <img src="images/circle_ef7.jpg" alt="" class="img-responsive"> 
        </div>
    </td>
    <td> 
        <div class="card" style="width: 20rem;">
          <img src="images/lshape_ef3.jpg" alt="" class="img-responsive"> 
        </div>
    </td>
 </tr>
</table> 

* * *

**Multiphase flow simulations for flow in porous or poroelastic media**  

It is a challenging task to simulate the fluid flow through porous or poroelastic media. The main challenges are (1) complicated coupling between the Darcy fluid flow and the transport and (2) local conservative fluxes are required to maintain physical saturation (bounded from 0 to 1). We develop a simulation tool based on FEMs with our local conservation postprocessing technique. See below the left column for two-phase flow through porous media while the right column for flow through poroelastic media. See [this paper](https://link.springer.com/article/10.1007/s10915-017-0493-9) for porous media while [this paper](https://www.sciencedirect.com/science/article/pii/S0021999117304692) for poroelastic media.

<table class="fixed">
  <col width="200"/>
  <col width="200"/>
  <tr>
    <td> 
        <div class="card" style="width: 20rem;">
          <img src="images/tpfsat1.jpg" alt="" class="img-responsive"> 
        </div>
    </td>
    <td> 
        <div class="card" style="width: 24rem;">
          <img src="images/sat1.jpg" alt="" class="img-responsive"> 
        </div>
    </td>
 </tr>
 <tr>
    <td> 
        <div class="card" style="width: 20rem;">
          <img src="images/tpfsat2.jpg" alt="" class="img-responsive"> 
        </div>
    </td>
    <td> 
        <div class="card" style="width: 24rem;">
          <img src="images/sat2.jpg" alt="" class="img-responsive"> 
        </div>
    </td>
 </tr>
</table> 
  

* * *

**Superfloe parameterisation with data assimilation for sea ice dynamics**  

The discrete element method (DEM) is providing a new modeling approach for describing sea ice dynamics. It exploits particle-based methods to characterize the physical quantities of each sea ice floe along its trajectory under Lagrangian coordinates. One major challenge in applying the DEM models is the heavy computational cost when the number of the floes becomes large. We develop an efficient Lagrangian parameterization algorithm to reduce the computational cost of simulating the DEM models while preserving the key features of the sea ice. The new parameterization takes advantage of a small number of artificial ice floes, named the superfloes, to effectively approximate a considerable number of the floes, where the parameterization scheme satisfies several important physics constraints. See below figures on the superfloe parameterisation. See [this paper](https://arxiv.org/abs/2105.13569) for details. 

<table class="fixed">
  <col width="200"/>
  <col width="400"/>
  <tr>
    <td> 
        <div class="card" style="width: 20rem;">
          <img src="images/floes.jpg" alt="" class="img-responsive"> 
        </div>
    </td>
    <td> 
        <div class="card" style="width: 30rem;">
          <img src="images/floesuper.jpg" alt="" class="img-responsive"> 
        </div>
    </td>
 </tr>
</table> 

* * * *

## Research visits, talks, and other activities
- See [CV here](https://quanlingdeng.github.io/deng.pdf).
