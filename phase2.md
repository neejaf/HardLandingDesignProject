# Phase Two: Project Report  
Hard Landing – Landing Gear Project  

<p align="center">
  <img src="figures/phase2/Full_assembly_ss.png">
</p>

<p align="center">
Aiden Beam, Jack Bessette, Ben Kolecki, Evan Morris, Nordin Jafar 
<p align="center">
Arizona State University
  </p>
<p align="center">
MEE 342  
  </p>
<br>
<br>

## **Final Design Overview**
<br>
This aircraft landing gear was modeled based off a simplified version of a large airliner landing gear. During taxi, takeoff, and landing the landing gear will be in its vertical, locked position, and during flight will retract to allow increased aerodynamic performance. Our design consists of three main sections: the strut/wheels that provide the main support for the aircraft, and the two bar linkage connected to a motor that controls the motion of the entire system. <br>
<br>
<p align="center">
  <img src="figures/phase2/front_view.png">
</p>
<br>
This motor will read signals from an Arduino to rotate on its axis, extending and folding up the landing gear. 
<br>
<br>

	
**Landing gear deployment/retraction sequence**
<p align="center">
  [watch the assembly video](![Image](https://github.com/user-attachments/assets/40a034cb-c734-499a-afc4-3781faa09988))
</p>
  <p align="center">
<br>
	  <br>
	  
**full 3D assembly**
<p align="center">
[watch the assembly video](https://github.com/user-attachments/assets/a2dc4aa6-550e-4249-b24c-30bdd2203265)
	</p>
<br>
<br>

  
## **Description of Major Design Decisions and Changes from Phase 1**<br>
Increased wheel count to more closely resemble inspiration  
	-Adding three more wheels makes our model more similar to that of many commercial airliners who's landing gear we want to replicate. This allows our calculations and simulations to be much more accurate to resemble real world conditions. Also, an even number of wheels allows for a more balanced model, so it will more easily be able to stand and hold weight without an unintended failure.

  
  
## **Detailed explanation of required analyses (shaft, gear, fatigue, bearings)**
interfaces, etc.) with clear assumptions and results

- Discussion of design for assembly and design for 3D printing
  <br>
<br>
<p align="center">
Von-Mises Equivalent stress
  <img src="figures/phase2/Equivalent stress.png">
<br>
<br>
Factor of Safety
	<img src="figures/phase2/Factor of saftey.png">
<br>
<br>
Mesh
	<img src="figures/phase2/Mesh.png">
	<br>
	<br>
Added Force

<img src="figures/phase2/Force acting.png">
<br>
<br> 
Total Deformation
	
<img src="figures/phase2/Total_Deformation.png">
	
## **Updated list of anticipated risks or weaknesses to be addressed in prototyping**
Smallest factor of safety
<img src="figures/phase2/Minimum_safety_factor.png">
<br>
<br>

## **Checklist-(2 astrixs is what we have done)** 

	-full 3D assembly**
	-drawings and views
	-printability
	-static stress and factor of safety**
	-Fatigue
	-key/coupling/interface stresses
	-bearing load check
	-global safety overview
<br>
<br>
