---
title: Research
layout: default
---

[comment]: <> 
(
I am a computational mathematician working closely with computer scientists and engineers. 
My research spans various areas in Computational Science such as Mathematical Modeling and Simulation, 
Scientific Computing, and Numerical Analysis.
In the following, I will briefly outline several ongoing research projects.
)

## Soft Isogeometric Analysis (softIGA): Development and Application

Isogeometric analysis (IGA) is an advanced computational approach that integrates 
finite element analysis (FEA) into computer-aided design (CAD) tools. 
It has been a vital tool in computational mechanics and it is the core technology 
for many commercial companies such as Coreform. 
A major part of the ongoing developments of IGA techniques focuses on improving 
simulation accuracy and reducing simulation costs. 
This is particularly challenging in modeling non-linear structural mechanics. 
Standard isogeometric analysis suffers from its high stiffness that causes numerical instabilities, 
and consequently, keeps the analysis tool from more accurate and faster simulations. 
One recent idea is to reduce the stiffness by softening the discretized system 
via a jump penalization technique, hence the motivation of the development of the new tool—softIGA. 
In this project, we will also look into real-world applications such as structural vibration modeling.

![Pro1](./images/pro1.png)

## Deep learning based permeability characterisation in porous media

It has been a well-known challenge to model and simulate of multiphase fluid flow through porous and poroelastic media. 
Related projects are best known for their importance in oil recovery from petroleum reservoirs, 
but they also find applications in novel areas such as hydrofracturing for natural gas recovery.
Australia has about 0.3 percent of the world oil reserves.
Most of Australia’s known remaining oil resources are condensate and liquefied petroleum gas associated with giant offshore gas fields. 
Many researchers in USA and China have been make efforts to develop mathematical models 
and simulation techniques to predict and maximize oil production.
One of the major challenges is the lack knowledge of the subsurface permeability in the modeling equations. 
Permeability measures a fluid’s ability to flow through a porous solid. A standard non-destructive technique to
determine the location of material discontinuities inside solids is to measure sound waves that travelled through the medium. 
Presently, there is an unmet need to use elastic waves to image the permeability distribution of saturated porous solids, such as rocks and bones. 
This project aims to first develop the next generation of mathematical models that describe wave propagation in fluid-saturated porous media
and then design and implement ML-based inversion methods to  the permeability.
In particular, most of the existing mathematical models does not account for the relative motion of the fluid
and solid as well as the porosity gradients. 
We build a forward simulator that accounts for all the couplings between
the relative motions of the solid matrix and the fluid as well as the distortion of the pore space. 
Once the model is built, the goal is to develop deep learning techniques to enhance the permeability inversion at different scales.
The use of convolutional neural networks (CNNs) and
deep learning techniques (DLTs) on sound wave inversion problems is relatively new in comparison to standard
approaches based on forward simulations and parameter optimisation via minimisation of a misfit functional. 
Once the training stage is completed, CNN can process sound wave data automatically to estimate the permeability field.
The new models and efficient simulators are the necessary foundations to perform poroelastic inversion. 
This will allow us to invert for permeability fields from sound wave data directly, opening the
door for industrially relevant inversion workflows based on poroelasticity and, thus, unlock the potential for fluid
transport property prediction from wavefield recordings, which have been elusive for practitioners heretofore.

![Pro2](./images/pro2.png)

## Parallel computing and machine learning for Arctic sea ice dynamics simulations

One major challenge in applying the DEM models to simulate Arctic sea ice dynamics is the heavy computational cost 
when the number of the floes becomes large.
This project aims to develop a parallel computing structure that divides the simulation tasks.
This structure is to be used in a high performance computing (HPC) environment with more computational sources 
when running more realistic Arctic sea ice simulations.  
These research directions would improve the physical modeling and prediction
of Arctic sea ice, so as to improve the understanding of sea ice impacts on global warming.

![Pro3](./images/pro3.png)
