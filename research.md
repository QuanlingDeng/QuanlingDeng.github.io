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

## Several projects

**Development of FEM approximations**

(1) A FEM approximated solution lacks the local conservation property on its fluxes. We proposed a simple and efficient postprocessing technique to recover the locally conservative fluxes on control volumes (FEM dual mesh elements). The technqiue solves an elemental Neumann-boundary value problem and it can be naturally implemented in a parallel environment. See [this paper](https://www.sciencedirect.com/science/article/pii/S0377042719301803) for details. 

<table class="fixed">
  <col width="300"/>
  <col width="300"/>
  <tr>
    <td> 
        <div class="card" style="width: 24rem;">
          <img src="images/cv0.jpg" alt="" class="img-responsive"> 
        </div>
    </td>
    <td> 
        <div class="card" style="width: 24rem;">
          <img src="images/cv1.jpg" alt="" class="img-responsive"> 
            </div>
          </div>
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



**Spectral approximation with finite and isogeometric elements**  


**Multiphase flow simulations for flow in poros or poroelastic media**  


**Superfloe parameterisation for sea ice dynamics**  



## Research visits, talks, and other activities
- See [CV here](https://quanlingdeng.github.io/deng.pdf).
