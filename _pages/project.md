---
layout: archive
title: "Research"
permalink: /projects/
author_profile: true
---

<!-- <details> 
<summary></summary>
</details>
-->
<script src='https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.4/MathJax.js?config=default'></script>

<h2>Bayesian optimization (BO) for origami-inspired folding structures</h2>
- <u>1D schematic<br></u>
  
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

<hr width="80%" />

  - <u>Chomper origami folding structure</u> <br>    
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
<hr width="80%" />
  - <u>Twist chomper origami folding structure</u><br>
  
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
<hr width="80%" />
<b>Companion paper: </b>[Bayesian topology optimization for efficient design of origami folding structures](https://www.sciencedirect.com/science/article/pii/S0045782522001992)<br>

<hr width="80%" size="10px" />
## Gradient-enhanced Bayesian optimization (GEBO)

  - <u>1D schematic</u><br>
  
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
  - <u>2D schematic</u><br>
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
 <ul style="list-style-type:square;">
  <li> Gradient enriched GP matches the objective functions gradients and function values at the training points.</li>
  <li> Gradient enriched GP gives a better fit than traditional GP.</li>
  </ul><br> 
<hr width="80%" />
  - <u>Airfoil shape optimization</u><br>
  
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
 <ul style="list-style-type:square;">
  <li> <b>Objective:</b> To find the optimal airfoil shape to minimize drag.</li>
  <li> GEBO with gradient clipping gives ~3 x speedup than traditional BO.</li>
  </ul><br> 
<hr width="80%" />  

  - <u>Square twist origami folding structure</u><br>
  
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
<ul style="list-style-type:square;">
  <li> <b>Objective:</b> To find the optimal fold pattern to maximize actuation.</li>
  <li> GEBO with gradient clipping gives ~3.5 x speedup than traditional BO.</li>
  </ul><br> 
<hr width="80%" />

<b>Companion paper: </b>[Systematic cost analysis of gradient- and anisotropy-enhanced Bayesian design optimization](https://link.springer.com/article/10.1007/s00158-022-03324-8)

<hr width="80%" />
## Anisotropy-enhanced Bayesian optimization
  - <u>2D schematic</u><br>
  
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
<ul style="list-style-type:square;">
  <li> Anisotropy-enhanced GP gives a better fit than traditional GP for functions with dominant design variables.</li>
  <li> Anisotropy-enhanced GP can be used as a dimension reduction technique using automatic relevance determination (ARD).</li>
  </ul><br> 
<hr width="80%" />
  - <u>Twist chomper origami folding structure</u><br>
  
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
<ul style="list-style-type:square;">
  <li> <b>Objective:</b> To find the optimal fold pattern to maximize actuation.</li>
  <li> Anisotropy-enhanced BO with (ARD) reduces the dimension from 38 to 16.</li>
  <li> Anisotropy enhanced BO with (ARD) gives ~2 x speedup than traditional BO.</li>
  </ul><br>
<hr width="80%" />

<b>Companion paper: </b>[Systematic cost analysis of gradient- and anisotropy-enhanced Bayesian design optimization](https://link.springer.com/article/10.1007/s00158-022-03324-8)
<hr width="80%" />

## Deep energy minimization (DEM) framework for hyperelastic multistable structures

  - <u>Schematic DEM-SF</u><br>
  
<p align="center">
  <img src="https://Sourabh-Shende.github.io/Figures/NeuralNetworkSchematicv2.jpg?raw=true" width="450" height="300" alt="Schematic" title="Schematic"/>
</p>
<hr width="80%" />
<ul style="list-style-type:square;">
  <li> <b>Solver: </b>A Fully connected feed-forward neural network approximates the displacement field.</li>
  <li> <b>Loss: </b> Potential energy of the system is minimized as loss (DEM). </li>
  <li> <b>Gradients: </b> Finite element shape functions are used to calculate the gradients of displacement (DEM-SF).</li>
  </ul><br>
  
  - <u>Buckling of rectangular beam</u><br>
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
<ul style="list-style-type:square;">
  <li> FEM gives compression deformation mode without eigenvalue solution. </li>
  <li> FEM requires an eigenvalue solution for perturbation to give buckling deformation mode.</li>
  <li> The deep energy minimization framework when FE shape function (DEM-SF) is utilized to calculate the gradients gives buckling deformation mode.</li>
  <li> The deep energy minimization framework when automatic differentiation (DEM-AD) is utilized to calculate the gradients gives a non-physical solution.</li>
  </ul><br>
<hr width="80%" />
  - <u>Bi-stable unit cell</u><br>
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
<ul style="list-style-type:square;">
  <li> FEM needs an eigenvalue solution to predict the low potential buckling path.</li>
  <li> DEM-SF finds the low potential buckling path without an eigenvalue solution.</li>  
  <li> DEM-SF accurately predicts the second stable state.</li>
  </ul><br>
<hr width="80%" />
  - <u>Multistable structure</u><br>

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
<ul style="list-style-type:square;">
  <li> DEM-SF can accurately predict multiple stable states.</li>
  </ul><br>
<hr width="80%" />
  - <u>Load step independence<br>
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
<ul style="list-style-type:square;">
  <li> DEM-SF finds accurate solutions with larger load steps.</li>
  <li> FEM with larger load steps runs into convergence issues.</li>
  </ul><br>
<hr width="80%" />
  - <u>Transfer learning</u><br>
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
<ul style="list-style-type:square;">
  <li> Transfer learning can be leveraged for new designs to speed up the solution time by at least <b>5x</b>.</li>
  </ul><br>
<hr width="80%" />
## Deep energy minimization framework for phase-field elastic-perfectly plasticity problems

  - <u>Schematic<br>

<p align="center">
  <img src="https://Sourabh-Shende.github.io/Figures/ForwardFrameworkSchematicInkscapeDEMAD.jpg?raw=true" width="450" height="300" alt="Schematic" title="Schematic"/>
</p>
<ul style="list-style-type:square;">
  <li> <b>Solver: </b>A Fully connected feed-forward neural network approximates the displacement and scalar phase field.</li>
  <li> <b>Slip: </b> The scalar phase field, s  $\left(0\leq s\leq 1\right)$, called slip represents the degree of plastic slip in the body such that the bulk material response is degraded in the areas where $s>0$ plastic slip.</li>  
  <li> <b>Loss: </b> Potential energy of the system and the slip irreversibility condition is minimized as loss. </li>
  <li> <b>Gradients: </b> In-built automatic differentiation library of PyTorch is used to calculate the gradients of displacement and phase field (DEM-AD).</li>  
  </ul><br>
<hr width="80%" />

  - <u>Extension of square specimen</u><be>
<ul style="list-style-type:square;">
  <li> <b>Elasticity parameters: </b> Youngs modulus, $E=2.1e5$ ; Poissons ratio, $\nu = 0.3$.</li>
  <li> <b>Plasticity parameters: </b> Unpinning stiffness per area $\gamma = 0.1$; gliding resistance, $\sigma_0 = 120$; characteristic length $\epsilon = 2.5e-2$ .</li>  
</ul><br>
<table class="wide:100%" style="border: none">
 <tr style="border: none">
   <th align="center" style="width:50%" style="border: none">Problem setup</th>
   <th align="center" style="width:50%" style="border: none">Phase field s</th>
  </tr>
<tr>
  <td align="center" style="border: none">
     <img src="https://Sourabh-Shende.github.io/Figures/Squaredomain.jpg" alt="Setup" title="Setup" width="200" height="200"/>
  </td>
  <td align="center" style="border: none">
    <img src="https://Sourabh-Shende.github.io/Figures/SquareExtensionPhaseField.gif" alt="Phase field s" title="Phase field s" width="400" height="200"/>
  </td>
  <tr style="border: none">
   <th align="center" style="width:50%" style="border: none">Mininum potential energy</th>
   <th align="center" style="width:50%" style="border: none">Reaction force</th>
  </tr>
   </tr>
<tr style="border: none">
 <td align="center" style="border: none">
    <img src="https://Sourabh-Shende.github.io/Figures/Fenics23a_30a_DEMAD_138a_Pi_Loss.jpg" alt="potential energy" title="potential energy" width="300" height="200"/>
  </td>
  <td align="center" style="border: none">
    <img src="https://Sourabh-Shende.github.io/Figures/Fenics23a_30a_DEMAD_138a_mid_RF2_Loss.jpg" alt="Reaction force" title="Reaction force" width="300" height="200"/>
  </td>
</tr>
</table>
<ul style="list-style-type:square;">
  <li> FEM with first order fully integrated element gives unrealistic stiff response due to volumetric locking that results in wider shear bands.</li> 
  <li> FEM with second-order selective reduce integration (SRI) is needed to counter the volumetric locking issue and it predicts realistic sharper shear bands.</li>  
  <li> DEM-AD can provide a volumetric locking-free solution and predicts sharper shear bands.</li> 
</ul><br>
<hr width="80%" />

  - <u>Extension of square plate with hole</u><be>
<ul style="list-style-type:square;">
  <li> <b>Elasticity parameters: </b> Youngs modulus, $E=2.1e5$ ; Poissons ratio, $\nu = 0.3$.</li>
  <li> <b>Plasticity parameters: </b> Unpinning stiffness per area $\gamma = 0.025$; gliding resistance, $\sigma_0 = 120$; characteristic length $\epsilon = 2.5e-2$ .</li>  
</ul><br>
<table class="wide:100%" style="border: none">
 <tr style="border: none">
   <th align="center" style="width:50%" style="border: none">Problem setup</th>
   <th align="center" style="width:50%" style="border: none">Phase field s</th>
  </tr>
<tr>
  <td align="center" style="border: none">
     <img src="https://Sourabh-Shende.github.io/Figures/ProbSquareHoleElem8175Setup_page.jpg" alt="Setup" title="Setup" width="200" height="200"/>
  </td>
  <td align="center" style="border: none">
    <img src="https://Sourabh-Shende.github.io/Figures/Slip_FEnics_7_DEMAD_14e3.gif" alt="Phase field s" title="Phase field s" width="400" height="200"/>
  </td>
  <tr style="border: none">
   <th align="center" style="width:50%" style="border: none">Mininum potential energy</th>
   <th align="center" style="width:50%" style="border: none">Reaction force</th>
  </tr>
   </tr>
<tr style="border: none">
 <td align="center" style="border: none">
    <img src="https://Sourabh-Shende.github.io/Figures/SquareHole_Fenics_7_DEMAD_14e3_11a_Pi.jpg" alt="potential energy" title="potential energy" width="300" height="200"/>
  </td>
  <td align="center" style="border: none">
    <img src="https://Sourabh-Shende.github.io/Figures/SquareHole_Fenics_7_DEMAD_14e3_11a_ReactForce.jpg" alt="Reaction force" title="Reaction force" width="300" height="200"/>
  </td>
</tr>
</table>
<ul style="list-style-type:square;">
  <li> FEM and DEM-AD solution accurately predicts the onset of the plastic slip near the hole.</li> 
  <li> FEM with second-order selective reduce integration (SRI) follows the higher minimum potential energy path indicating that it gets trapped in local solution.</li>  
  <li> DEM-AD follows the lower minimum potential energy path.</li> 
</ul><br>
<hr width="80%" />

 - <u>Extension of rectangular plate with two asymmetrical notches</u><be>
<ul style="list-style-type:square;">
  <li> <b>Elasticity parameters: </b> Youngs modulus, $E=2.1e5$ ; Poissons ratio, $\nu = 0.3$.</li>
  <li> <b>Plasticity parameters: </b> Unpinning stiffness per area $\gamma = 0.2$; gliding resistance, $\sigma_0 = 80$; characteristic length $\epsilon = 2.5e-2$ .</li>  
</ul><br>
<table class="wide:100%" style="border: none">
 <tr style="border: none">
   <th align="center" style="width:50%" style="border: none">Problem setup</th>
   <th align="center" style="width:50%" style="border: none">Phase field s</th>
  </tr>
<tr>
  <td align="center" style="border: none">
     <img src="https://Sourabh-Shende.github.io/Figures/ProbRect2HoleassymMeshElem12357Setup.jpg" alt="Setup" title="Setup" width="60" height="240"/>
  </td>
  <td align="center" style="border: none">
    <img src="https://Sourabh-Shende.github.io/Figures/Rect2HoleAssym_Fenics_5_DEMAD_12a.gif" alt="Phase field s" title="Phase field s" width="400" height="200"/>
  </td>
  <tr style="border: none">
   <th align="center" style="width:50%" style="border: none">Mininum potential energy</th>
   <th align="center" style="width:50%" style="border: none">Reaction force</th>
  </tr>
   </tr>
<tr style="border: none">
 <td align="center" style="border: none">
    <img src="https://Sourabh-Shende.github.io/Figures/Rect2HoleAssym_Fenics_5_DEMAD_12a_Pi.jpg" alt="potential energy" title="potential energy" width="300" height="200"/>
  </td>
  <td align="center" style="border: none">
    <img src="https://Sourabh-Shende.github.io/Figures/Rect2HoleAssym_Fenics_5_DEMAD_12a_ReactForce.jpg" alt="Reaction force" title="Reaction force" width="300" height="200"/>
  </td>
</tr>
</table>
<ul style="list-style-type:square;">
  <li> FEM and DEM-AD solution accurately predicts the onset of the plastic slip near the notches.</li> 
  <li> FEM with second-order selective reduce integration (SRI) follows the higher minimum potential energy path that leads to wider shear bands.</li>  
  <li> DEM-AD follows the lower minimum potential energy path that leads to sharper shear bands.</li> 
</ul><br>
<hr width="80%" />
  - <u>Unique calibration of plasticity parameters</u> <be>

<table class="wide:100%" style="border: none">
 <tr style="border: none">
   <th align="center" style="width:25%" style="border: none">BO loss</th>
   <th align="center" style="width:25%" style="border: none">$\gamma$ (True value $= 0.1$)</th>
   <th align="center" style="width:25%" style="border: none">$\sigma_0$ (True value $= 120$) </th>
   <th align="center" style="width:25%" style="border: none">$\epsilon$ (True value $= 2.5e-2$) </th>
  </tr>  
<tr style="border: none">
 <td align="center" style="border: none">
    <img src="https://Sourabh-Shende.github.io/Figures/BO_120_400iter_BO_loss_curve_analysis.jpg" alt="BO loss" title="BO loss" width="300" height="200"/>
  </td>
  <td align="center" style="border: none">
    <img src="https://Sourabh-Shende.github.io/Figures/BO_120_400iter_gamma_curve_analysis.jpg" alt="gamma" title="gamma" width="300" height="200"/>
  </td>
  <td align="center" style="border: none">
    <img src="https://Sourabh-Shende.github.io/Figures/BO_120_400iter_sigma0_curve_analysis.jpg" alt="sigma0" title="sigma0" width="300" height="200"/>
  </td>
  <td align="center" style="border: none">
    <img src="https://Sourabh-Shende.github.io/Figures/BO_120_400iter_epsilon_curve_analysis.jpg" alt="epsilon" title="epsilon" width="300" height="200"/>
  </td>
</tr>
</table>
<table class="wide:100%" style="border: none">
 <tr style="border: none">
   <th align="center" style="width:25%" style="border: none">BO loss</th>
   <th align="center" style="width:25%" style="border: none">$\gamma$ (True value $= 0.3$)</th>
   <th align="center" style="width:25%" style="border: none">$\sigma_0$ (True value $= 70$) </th>
   <th align="center" style="width:25%" style="border: none">$\epsilon$ (True value $= 4e-2$) </th>
  </tr>  
<tr style="border: none">
 <td align="center" style="border: none">
    <img src="https://Sourabh-Shende.github.io/Figures/BO_129_BO_loss_curve_analysis.jpg" alt="BO loss" title="BO loss" width="300" height="200"/>
  </td>
  <td align="center" style="border: none">
    <img src="https://Sourabh-Shende.github.io/Figures/BO_129_gamma_curve_analysis.jpg" alt="gamma" title="gamma" width="300" height="200"/>
  </td>
  <td align="center" style="border: none">
    <img src="https://Sourabh-Shende.github.io/Figures/BO_129_sigma0_curve_analysis.jpg" alt="sigma0" title="sigma0" width="300" height="200"/>
  </td>
  <td align="center" style="border: none">
    <img src="https://Sourabh-Shende.github.io/Figures/BO_129_epsilon_curve_analysis.jpg" alt="epsilon" title="epsilon" width="300" height="200"/>
  </td>
</tr>
</table>
<ul style="list-style-type:square;">
  <li> Bayesian optimization (BO) with displacement data obtained using digital image correlation (DIC) is considered for the calibration of the plasticity parameters.</li>
  <li> Anisotropy is embedded in the Bayesian optimization (BO) framework by using unique kernel length scales for each plasticity parameter.</li>  
  <li> The neural network is initially trained on the DIC displacement data to get a good starting point for the weights</li>
  <li> DEM-AD equipped with transfer learning is utilized to solve the necessary forward problems.</li>
  <li> DEM-AD equipped with transfer learning uniquely calibrates plasticity parameters <b>6x</b> faster than using FEM.</li>   
</ul><br>
<hr width="80%" />
