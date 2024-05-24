---
layout: archive
title: "Research"
permalink: /projects/
author_profile: true
---

## Bayesian optimization (BO) for origami-inspired folding structures
  - 1D schematic<br>
  
<p align="center">
  <img src="https://Sourabh-Shende.github.io/Figures/GPBO_1D_wo_der.gif?raw=true" width="300" height="200" alt="Schematic" title="Schematic"/>
</p>
<ol>
 <li>Upper panel</li>
 <ul style="list-style-type:square;">
  <li><b>Goal :</b> To optimize expensive function (black dashed curve) in the upper panel</li>
  <li><b>Surrogate :</b> Gaussian process (GP) surrogate model is trained with the points (black dots) and is stochastic, with the uncertainty levels (blue bands) and the mean of GP (solid blue curve) in the upper panel.</li>
</ul>  
 <li>Lower panel</li>
 <ul style="list-style-type:square;">
 <li><b>Scalarization :</b> Acquisition function (green solid curve) in the lower panel scalarizes the surrogate model to give single-valued function</li>
 <li><b>Optimization :</b> Acquisition function (green solid curve) is minimized to find the next training point shown with the red triangle.</li>
 <li><b>Iteration :</b> The expensive function is evaluated at the new training point (red circle) and added to the training data. The process is repeated with the surrogate model mimicking the expensive function better with each iteration. The uncertainty in the surrogate model is also reduced as more training points are added.</li>
</ul><br>
</ol>  

  - Chomper origami folding structure <br>    
<table class="wide:70%" style="border: none">
<tr style="border: none">
   <th align="center" style="width:35%" style="border: none">Problem setup</th>
   <th align="center" style="width:35%" style="border: none">Evolution of objective function</th>
  </tr>
  <tr style="border: none">
  <td align="center" style="border: none">
      <img src="https://Sourabh-Shende.github.io/Figures/chomper_problem_setup.jpg" alt="chomper setup" title="Setup" width="300" height="150"/>  
  </td>
  <td align="center" style="border: none">
    <img src="https://Sourabh-Shende.github.io/Figures/4_Comparison_of_gradient_bayesian_optimal_obj_funct_18D_ts_1.jpg" alt="Objective function evolution" title="Evolution of objective function" width="300" height="200"/><br>   
  </td>
   <tr style="border: none">
   <th align="center" style="width:35%" style="border: none">Number of objective function evaluations</th>
   <th align="center" style="width:35%" style="border: none">Best fold pattern</th>
  </tr>
 </tr>
<tr style="border: none">
  <td align="center" style="border: none">
    <img src="https://Sourabh-Shende.github.io/Figures/FE_solution_comparison_18D.jpg" alt="Objective function evaluations" title="Number of objective function evaluations" width="300" height="200"/>
  </td>
   <td align="center" style="border: none">
    <img src="https://Sourabh-Shende.github.io/Figures/chomper_opt_design.gif" alt="Best fold pattern" title="Best fold pattern" width="300" height="150"/>   
  </td>
  </tr>
  </table>
  <br>
  
  <ul style="list-style-type:square;">
  <li> Traditional gradient-based optimization technique gets trapped in local minima.</li>
  <li> Bayesian (BO) finds optimal design and takes ~34 x fewer FE solution than genetic algorithm (GA)</li>  
</ul><br>

  - Twist chomper origami folding structure<br>
  
<table class="wide:70%" style="border: none">
 <tr style="border: none">
   <th align="center" style="width:35%" style="border: none">Problem setup</th>
   <th align="center" style="width:35%" style="border: none">Evolution of objective function</th>
  </tr>
<tr>
  <td align="center" style="border: none">
     <img src="https://Sourabh-Shende.github.io/Figures/twist_chomper_setup.jpg" alt="chomper setup" title="Setup" width="300" height="150"/>
  </td>
  <td align="center" style="border: none">
    <img src="https://Sourabh-Shende.github.io/Figures/5_Comparison_of_gradient_bayesian_optimal_obj_funct_38D_ts_5.jpg" alt="Objective function evolution" title="Evolution of objective function" width="300" height="200"/>
  </td>
  <tr style="border: none">
   <th align="center" style="width:35%" style="border: none">Number of objective function evaluations</th>
   <th align="center" style="width:35%" style="border: none">Best fold pattern</th>
  </tr>
   </tr>
<tr style="border: none">
 <td align="center" style="border: none">
    <img src="https://Sourabh-Shende.github.io/Figures/FE_solution_comparison_38D.jpg" alt="Objective function evaluations" title="Number of objective function evaluations" width="300" height="200"/>
  </td>
  <td align="center" style="border: none">
    <img src="https://Sourabh-Shende.github.io/Figures/twist_chomper_opt_design.gif" alt="Best fold pattern" title="Best fold pattern" width="300" height="150"/>
  </td>
</tr>
</table>
<ul style="list-style-type:square;">
  <li> Traditional gradient-based optimization technique gets trapped in local minima.</li>
  <li> Bayesian (BO) finds optimal design and takes ~56 x fewer FE solution than genetic algorithm (GA)</li>  
</ul><br>


<b>Companion paper: </b>[Bayesian topology optimization for efficient design of origami folding structures](https://www.sciencedirect.com/science/article/pii/S0045782522001992)



## Gradient-enhanced Bayesian optimization

  - 1D schematic<br>
  
<table class="wide:70%" style="border: none">
 <tr style="border: none">
   <th align="center" style="width:35%" style="border: none">BO</th>
   <th align="center" style="width:35%" style="border: none">Gradient enriched BO</th>
  </tr>
<tr>
  <td align="center" style="border: none">
     <img src="https://Sourabh-Shende.github.io/Figures/GPBO_1D_wo_der.gif" alt="without derivative" title="without derivative" width="300" height="200"/>
  </td>
  <td align="center" style="border: none">
    <img src="https://Sourabh-Shende.github.io/Figures/GPBO_1D_w_der.gif" alt="with derivative" title="with derivative" width="300" height="200"/>
  </td>
 </tr>
</table>

  - 2D schematic<br>

 <table class="wide:72%" style="border: none">
 <tr style="border: none">
   <th align="center" style="width:24%" style="border: none">Objective function</th>
   <th align="center" style="width:24%" style="border: none">GP</th>
   <th align="center" style="width:24%" style="border: none">Gradient enriched GP</th>  
  </tr>
<tr>
  <td align="center" style="border: none">
     <img src="https://Sourabh-Shende.github.io/Figures/Fig2a.jpg" alt="Objective function" title="Objective function" width="200" height="200"/>
  </td>
  <td align="center" style="border: none">
    <img src="https://Sourabh-Shende.github.io/Figures/Fig2b.jpg" alt="GP" title="GP" width="200" height="200"/>
  </td>
 <td align="center" style="border: none">
    <img src="https://Sourabh-Shende.github.io/Figures/Fig2c.jpg" alt="Gradient enriched GP" title="Gradient enriched GP" width="200" height="200"/>
  </td>
 </tr>
</table>

  - Airfoil shape optimization<br>
  
<table class="wide:70%" style="border: none">
 <tr style="border: none">
   <th align="center" style="width:35%" style="border: none">Problem schematic</th>
   <th align="center" style="width:35%" style="border: none">CFD mesh</th>
  </tr>
<tr>
  <td align="center" style="border: none">
     <img src="https://Sourabh-Shende.github.io/Figures/Fig14d.jpg" alt="Problem schematic" title="Problem schematic" width="300" height="200"/>
  </td>
  <td align="center" style="border: none">
    <img src="https://Sourabh-Shende.github.io/Figures/Fig11.jpg" alt="CFD mesh" title="CFD mesh" width="300" height="200"/>
  </td>
  <tr style="border: none">
   <th align="center" style="width:35%" style="border: none">Evolution of objective function</th>
   <th align="center" style="width:35%" style="border: none">Computational time</th>
  </tr>
   </tr>
<tr style="border: none">
 <td align="center" style="border: none">
    <img src="https://Sourabh-Shende.github.io/Figures/FIg12a.jpg" alt="Evolution of objective function" title="Evolution of objective function" width="300" height="200"/>
  </td>
  <td align="center" style="border: none">
    <img src="https://Sourabh-Shende.github.io/Figures/Fig12b.jpg" alt="Computational time" title="Computational time" width="300" height="200"/>
  </td>
</tr>
</table>
  
  - Square twist origami folding structure<br>
  
<table class="wide:70%" style="border: none">
 <tr style="border: none">
   <th align="center" style="width:35%" style="border: none">Problem setup</th>
   <th align="center" style="width:35%" style="border: none">Evolution of objective function</th>
  </tr>
<tr>
  <td align="center" style="border: none">
     <img src="https://Sourabh-Shende.github.io/Figures/Fig16b.jpg" alt="chomper setup" title="Setup" width="300" height="150"/>
  </td>
  <td align="center" style="border: none">
    <img src="https://Sourabh-Shende.github.io/Figures/Fig19a.jpg" alt="Objective function evolution" title="Evolution of objective function" width="300" height="200"/>
  </td>
  <tr style="border: none">
   <th align="center" style="width:35%" style="border: none">Computational time</th>
   <th align="center" style="width:35%" style="border: none">Best fold pattern</th>
  </tr>
   </tr>
<tr style="border: none">
 <td align="center" style="border: none">
    <img src="https://Sourabh-Shende.github.io/Figures/Fig19b.jpg" alt="Computational time" title="Computational time" width="300" height="200"/>
  </td>
  <td align="center" style="border: none">
    <img src="https://Sourabh-Shende.github.io/Figures/square_twist_opt_design.gif" alt="Best fold pattern" title="Best fold pattern" width="250" height="250"/>
  </td>
</tr>
</table>

<b>Companion paper: </b>[Systematic cost analysis of gradient- and anisotropy-enhanced Bayesian design optimization](https://link.springer.com/article/10.1007/s00158-022-03324-8)

## Anisotropy-enhanced Bayesian optimization
  - 2D schematic<br>
  
<table class="wide:72%" style="border: none">
 <tr style="border: none">
   <th align="center" style="width:24%" style="border: none">Objective function</th>
   <th align="center" style="width:24%" style="border: none">Isotropic GP</th>
   <th align="center" style="width:24%" style="border: none">Anisotropy enriched GP</th>  
  </tr>
<tr>
  <td align="center" style="border: none">
     <img src="https://Sourabh-Shende.github.io/Figures/Fig7a.jpg" alt="Objective function" title="Objective function" width="200" height="200"/>
  </td>
  <td align="center" style="border: none">
    <img src="https://Sourabh-Shende.github.io/Figures/Fig7b.jpg" alt="Isotropic GP" title="Isotropic GP" width="200" height="200"/>
  </td>
 <td align="center" style="border: none">
    <img src="https://Sourabh-Shende.github.io/Figures/Fig7c.jpg" alt="Anisotropy enriched GP" title="Anisotropy enriched GP" width="200" height="200"/>
  </td>
 </tr>
</table>

  - Twist chomper origami folding structure<br>
  
<table class="wide:70%" style="border: none">
 <tr style="border: none">
   <th align="center" style="width:35%" style="border: none">Problem setup</th>
   <th align="center" style="width:35%" style="border: none">Evolution of objective function</th>
  </tr>
<tr>
  <td align="center" style="border: none">
     <img src="https://Sourabh-Shende.github.io/Figures/twist_chomper_setup.jpg" alt="chomper setup" title="Setup" width="300" height="150"/>
  </td>
  <td align="center" style="border: none">
    <img src="https://Sourabh-Shende.github.io/Figures/Fig21a.jpg" alt="Objective function evolution" title="Evolution of objective function" width="300" height="200"/>
  </td>
  <tr style="border: none">
   <th align="center" style="width:35%" style="border: none">Computational time</th>
   <th align="center" style="width:35%" style="border: none">Best fold pattern</th>
  </tr>
   </tr>
<tr style="border: none">
 <td align="center" style="border: none">
    <img src="https://Sourabh-Shende.github.io/Figures/Fig21b.jpg" alt="Computational time" title="Computational time" width="300" height="200"/>
  </td>
  <td align="center" style="border: none">
    <img src="https://Sourabh-Shende.github.io/Figures/twist_chomper_opt_design.gif" alt="Best fold pattern" title="Best fold pattern" width="300" height="150"/>
  </td>
</tr>
</table>

<b>Companion paper: </b>[Systematic cost analysis of gradient- and anisotropy-enhanced Bayesian design optimization](https://link.springer.com/article/10.1007/s00158-022-03324-8)

## Deep energy minimization framework for hyperelastic multistable structures

  - Schematic DEM-SF<br>
  
<p align="center">
  <img src="https://Sourabh-Shende.github.io/Figures/NeuralNetworkSchematicv2.jpg?raw=true" width="450" height="300" alt="Schematic" title="Schematic"/>
</p>

  - Buckling of rectangular beam<br>
<table class="wide:99%" style="border: none">
 <tr style="border: none">
   <th align="center" style="width:33%" style="border: none">FEM Compression</th>
   <th align="center" style="width:33%" style="border: none">FEM Buckling (Needs Eignevalue solution)</th>
   <th align="center" style="width:33%" style="border: none">DEM-SF</th>  
  </tr>
<tr>
  <td align="center" style="border: none">
     <img src="https://Sourabh-Shende.github.io/Figures/FEM_Compression_prb5.gif" alt="FEM Compression" title="FEM Compression" width="300" height="200"/>
  </td>
  <td align="center" style="border: none">
    <img src="https://Sourabh-Shende.github.io/Figures/FEM_Buckling_prb5.gif" alt="FEM Buckling" title="FEM Buckling" width="300" height="200"/>
  </td>
 <td align="center" style="border: none">
    <img src="https://Sourabh-Shende.github.io/Figures/DEMSF_prb5.gif" alt="DEM-SF" title="DEM-SF" width="300" height="200"/>
  </td>
 </tr>
</table>

<p align="center">
  <img src="https://Sourabh-Shende.github.io/Figures/MinpotentFEMDEMProb5Elem250ls20inkscape.jpg?raw=true" width="450" height="300" alt="Potential energy" title="Potential energy"/><br>
 <label><b>Minimum potential energy evolution comparison.</b></label>
</p>


  - Bi-stable unit cell<br>
<table class="wide:99%" style="border: none">
 <tr style="border: none">
   <th align="center" style="width:33%" style="border: none">FEM Compression</th>
   <th align="center" style="width:33%" style="border: none">FEM Buckling (Needs Eignevalue solution)</th>
   <th align="center" style="width:33%" style="border: none">DEM-SF</th>  
  </tr>
<tr>
  <td align="center" style="border: none">
     <img src="https://Sourabh-Shende.github.io/Figures/FEM_Compression_prb10ext2.gif" alt="FEM Compression" title="FEM Compression" width="300" height="200"/>
  </td>
  <td align="center" style="border: none">
    <img src="https://Sourabh-Shende.github.io/Figures/FEM_Buckling_prb10ext2.gif" alt="FEM Buckling" title="FEM Buckling" width="300" height="200"/>
  </td>
 <td align="center" style="border: none">
    <img src="https://Sourabh-Shende.github.io/Figures/DEMSF_prb10ext2.gif" alt="DEM-SF" title="DEM-SF" width="300" height="200"/>
  </td>
 </tr>
</table>

<p align="center">
  <img src="https://Sourabh-Shende.github.io/Figures/MinPotenDEMsfgradFEMElem696Prob10ext2.jpg?raw=true" width="450" height="300" alt="Potential energy" title="Potential energy"/><br>
 <label><b>Minimum potential energy evolution comparison.</b></label>
</p><br>

  - Multistable structure<br>

<table class="wide:100%" style="border: none">
 <tr style="border: none">
   <th align="center" style="width:50%" style="border: none">DEM-SF deformation</th>
   <th align="center" style="width:50%" style="border: none">Minimum potential energy evolution</th>   
  </tr>
<tr>
  <td align="center" style="border: none">
     <img src="https://Sourabh-Shende.github.io/Figures/DEMSF_prb9xt3.gif" alt="FEM Compression" title="FEM Compression" width="300" height="200"/>
  </td>
  <td align="center" style="border: none">
    <img src="https://Sourabh-Shende.github.io/Figures/MinPotenDEMtEMProb9ext3Elem1424R_sfgrad_Mat1_lsstudies.jpg" alt="FEM Buckling" title="FEM Buckling" width="300" height="200"/>
  </td>
 </tr>
</table>

  - Load step independence<br>
<table class="wide:100%" style="border: none">
 <tr style="border: none">
   <th align="center" style="width:50%" style="border: none">Problem setup</th>
   <th align="center" style="width:50%" style="border: none">Minimum potential energy evolution</th>   
  </tr>
<tr>
  <td align="center" style="border: none">
     <img src="https://Sourabh-Shende.github.io/Figures/Prob7Elem250Setup.jpg" alt="Setup" title="Setup" width="300" height="200"/>
  </td>
  <td align="center" style="border: none">
    <img src="https://Sourabh-Shende.github.io/Figures/MinpotentDEMProb7blsStudies.jpg" alt="Potential energy" title="Potential energy" width="300" height="200"/>
  </td>
 </tr>
</table>

  - Transfer learning<br>
 <table class="wide:100%" style="border: none">
 <tr style="border: none">
   <th align="center" style="width:50%" style="border: none">Trained design</th>
   <th align="center" style="width:50%" style="border: none">New design</th>   
  </tr>
<tr>
  <td align="center" style="border: none">
     <img src="https://Sourabh-Shende.github.io/Figures/Prob10ext2Elem696Setup.jpg" alt="Trained design" title="Trained design" width="300" height="200"/>
  </td>
  <td align="center" style="border: none">
    <img src="https://Sourabh-Shende.github.io/Figures/Prob9ext2Elem712Setup.jpg" alt="New design" title="New design" width="300" height="200"/>
  </td>
 </tr>
  <tr style="border: none">
   <th align="center" style="width:50%" style="border: none">Loss history</th>
   <th align="center" style="width:50%" style="border: none">Minimum potential energy evolution</th>   
  </tr>
<tr>
  <td align="center" style="border: none">
     <img src="https://Sourabh-Shende.github.io/Figures/LossHistoryWithWithoutTransferLearningprob9ext2.jpg" alt="Loss history" title="Loss history" width="300" height="200"/>
  </td>
  <td align="center" style="border: none">
    <img src="https://Sourabh-Shende.github.io/Figures/MinPotenDEMsfgradFEMElem712Prob9ext2lsstudiestlprb10ext2.jpg" alt="Minimum potential energy evolution" title="Minimum potential energy evolution" width="300" height="200"/>
  </td>
 </tr> 
</table>

## Deep energy minimization framework for phase-field plasticity problem

  - Schematic<br>

<p align="center">
  <img src="https://Sourabh-Shende.github.io/Figures/ForwardFrameworkSchematicInkscape.jpg?raw=true" width="450" height="300" alt="Schematic" title="Schematic"/>
</p>

  - Extension of square specimen<be>

<table class="wide:100%" style="border: none">
 <tr style="border: none">
   <th align="center" style="width:50%" style="border: none">Problem setup</th>
   <th align="center" style="width:50%" style="border: none">Displacement u<sub>1</sub></th>
  </tr>
<tr>
  <td align="center" style="border: none">
     <img src="https://Sourabh-Shende.github.io/Figures/Squaredomain.jpg" alt="Setup" title="Setup" width="200" height="200"/>
  </td>
  <td align="center" style="border: none">
    <img src="https://Sourabh-Shende.github.io/Figures/Square_extension_u1.gif" alt="Displacement u1" title="Displacement u1" width="400" height="200"/>
  </td>
  <tr style="border: none">
   <th align="center" style="width:50%" style="border: none">Displacement u<sub>2</sub></th>
   <th align="center" style="width:50%" style="border: none">Phase field s</th>
  </tr>
   </tr>
<tr style="border: none">
 <td align="center" style="border: none">
    <img src="https://Sourabh-Shende.github.io/Figures/Square_extension_u2.gif" alt="Displacement u2" title="Displacement u2" width="400" height="200"/>
  </td>
  <td align="center" style="border: none">
    <img src="https://Sourabh-Shende.github.io/Figures/Square_extension_slip.gif" alt="Phase field s" title="Phase field s" width="400" height="200"/>
  </td>
</tr>
</table>

