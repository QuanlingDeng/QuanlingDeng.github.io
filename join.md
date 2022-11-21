---
title: Join
layout: default
---

We are looking for highly motivated students (undergraduate, PhB, Honours, Masters, and PhD), who will work on research projects to develope the next generation of models and methods in the field of Computational and Applied Mathematics, broadly in Computational Science within the ANU School of Computing.
There are a large number of potential directions and some of them are: development and application of advanced finite and isogeometric element analysis, machine learning based model solvers and simulators, modeling and superparameterization of sea-ice-ocean-atmosphere dynamics, and wave dispersion/disspation analysis. 

## ANU undergraduates or masters' students looking for research projects
If you are an ANU student interested in Honours or research projects (either for COMP3770/4550/8603/8604/8800/SCNC2101 or simply interest), please email me to express your interest. While emailing me, please include some background information and briefly state the research that you would like to undertake. Feel free to propose your research project ideas. Some current avaliable student projects are: 

- **Soft spectral element method (softSEM) and its application to seismic wave simulation (co-supervision)** 
The high-order spectral element method (SEM) has been widely used in geoscience for simulating seismic waves [1]. However, like the higher-order finite element methods (FEMs), high-order SEMs suffer from high stiffness (large condition numbers) in their discretized systems. Following the softFEM idea [2], we propose to reduce the stiffness of the problem by subtracting a least-squares penalty on the gradient jumps across the mesh interfaces from the standard stiffness SEM bilinear form. We refer to this method as softSEM. The two key goals of softSEM are (1) to reduce the numerical dispersion errors [3], especially for high-frequency waves, leading to more accurate simulation; and (2) to reduce the condition number (i.e., the stiffness) of the discretized system, leading to larger time-marching step size when using explicit schemes and hence computational advantages. The major difficulty of this project is to optimize the softness parameter such that the resulting system is coercive while the above goals are achieved. The project will be supervised by [Dr. Rhys Hawkins](https://cecc.anu.edu.au/people/rhys-hawkins#acton-tabs-link--tabs-0-middle-1) (mainly on seismic wave simulation) and Dr. Quanling Deng (mainly on the development of softSEM). We will provide a basic code (both Python and Matlab codes are available for your choice) for this project. This project is ideal for an Honour’s or Master’s student pursuing 12 or 24 units over two consecutive semesters. 

- **Soft Isogeometric Analysis (softIGA): Development and Application**:
Isogeometric analysis (IGA) is an advanced computational approach that integrates 
finite element analysis (FEA) into computer-aided design (CAD) tools. 
It has been a vital tool in computational mechanics and it is the core technology 
for many commercial companies such as Coreform. 
A major part of the ongoing developments of IGA techniques focuses on improving 
simulation accuracy and reducing simulation costs. This is particularly challenging in modeling non-linear structural mechanics. 
Standard isogeometric analysis suffers from its high stiffness that causes numerical instabilities, 
and consequently, keeps the analysis tool from more accurate and faster simulations. 
One recent idea is to reduce the stiffness by softening the discretized system 
via a jump penalization technique, hence the motivation of the development of the new tool—softIGA. 
In this project, we will also look into real-world applications such as structural vibration modeling.

- **Neural networks for high-dimensional differential eigenvalue problems**
The classic second-order elliptic differential eigenvalue problems can be solved efficiently by using the finite element methods (FEMs) or FEM-based methods. For differential operators living in a high-dimensional space, the eigenvalue problem (numerical spectral approximation) becomes particularly challenging due to the “curse of dimensionality”, a phenomenon that the computational complexity of certain algorithms increases exponentially with the dimension. This project aims to develop neural network models to efficiently approximate the spectrum and eigenfunctions of the differential operator. 

- **Deep learning based permeability characterisation in porous media**:
It has been a well-known challenge to model and simulate of multiphase fluid flow through porous and poroelastic media. 
Related projects are best known for their importance in oil recovery from petroleum reservoirs, 
but they also find applications in novel areas such as hydrofracturing for natural gas recovery.
Australia has about 0.3 percent of the world oil reserves. Most of Australia’s known remaining oil resources are condensate and liquefied petroleum gas associated with giant offshore gas fields. Many researchers in USA and China have been make efforts to develop mathematical models 
and simulation techniques to predict and maximize oil production. One of the major challenges is the lack knowledge of the subsurface permeability in the modeling equations. Permeability measures a fluid’s ability to flow through a porous solid. A standard non-destructive technique to
determine the location of material discontinuities inside solids is to measure sound waves that travelled through the medium. 
Presently, there is an unmet need to use elastic waves to image the permeability distribution of saturated porous solids, such as rocks and bones. 
This project aims to first develop the next generation of mathematical models that describe wave propagation in fluid-saturated porous media
and then design and implement ML-based inversion methods to  the permeability.

- **Parallel computing and machine learning for Arctic sea ice dynamics simulations**:
One major challenge in applying the DEM models to simulate Arctic sea ice dynamics is the heavy computational cost 
when the number of the floes becomes large. This project aims to develop a parallel computing structure that divides the simulation tasks.
This structure is to be used in a high performance computing (HPC) environment with more computational sources 
when running more realistic Arctic sea ice simulations. These research directions would improve the physical modeling and prediction
of Arctic sea ice, so as to improve the understanding of sea ice impacts on global warming.


## ANU students interested in joining the group as a PhD student
Please follow the following guidlines and email me to express your interest.
- Browse ANU School of Computing webpages ([mainly here](https://comp.anu.edu.au/education/03-research/)) and familiarise with the entry requirements.

- If you believe you meet all the entry requirements, please email me your CV and a concise statement about your motivation and the research direction you would like to pursue. Based on this email, we will then probably schedule a meeting.
 
## Non-ANU students interested in joining the group
Please follow the following guidlines and email me to express your interest.

- Browse ANU School of Computing webpages ([mainly here](https://comp.anu.edu.au/education/03-research/)) and familiarise with the entry requirements.

- If you believe you meet all the entry requirements, please email me with background information (mainly your CV) such as courses and projects, academic transcript, and programming skills, and a concise statement about your motivation to undertake a PhD under my supervision. 

- Based on your background information, we will decide whether we can proceed with an interview. After that, based on our meeting, I will then provide more instructions on how to apply to the PhD program under my supervision.

## Scholarship Opportunities

### ANU
- [https://comp.anu.edu.au/education/03-research/](https://comp.anu.edu.au/education/03-research/)

  Due on 31/08/2022 for international students and 31/10/2022 for domestic students

### Non-ANU

- For potential students: [ATSE Elevate Scholarship](https://www.atse.org.au/career-pathways/elevate/elevate-scholarship-guidelines/). 
  
  For female domestic students (Australian, New Zealand citizen and Australian PR)
  
  Due date for 2023 commencement is 30 Sep 2022.


- For current students:

  [Nvidia](https://www.nvidia.com/en-us/research/graduate-fellowships/) 
  Due 9 Sep 3pm PT, recommended to submit as soon as possible

  [Meta](https://research.facebook.com/fellowship/)
  Due 20 Sep, not clear on the time zone, to be safe, I recommend using Canberra time zone
  
### Climate Change Related
  
 - [Climate Game Change Scholarship](https://iceds.anu.edu.au/news-events/news/scholarship-open-support-climate-game-changers-apply-now)
  
 - [COSIMA Ocean Sea Ice Modeling](http://cosima.org.au/index.php/2021/10/06/cosima-offers-scholarships/)


### School of Computing Pioneering Women

- [Pioneering Women Researchers (Both Domestic and International)](https://comp.anu.edu.au/join/pwp/)

