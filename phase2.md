# Phase Two: Project Report  
Hard Landing – Landing Gear Project  

<p align="center">
    <img src="figures/phase2/other isometric view.png" width="700"></td>
  <p/>

<p align="center">
Aiden Beam, Jack Bessette, Ben Kolecki, Evan Morris, Nordin Jafar 
<p align="center">
Arizona State University
  </p>
<p align="center">
MEE 342  
  </p>


## **Final Design Overview**
This landing gear system is designed for a wide-body commercial aircraft operating under typical taxi, takeoff, landing, and flight conditions. During ground operation, the gear remains in its vertical, locked configuration to support the aircraft, and retracts during flight to reduce aerodynamic drag.

The design is based on a representative aircraft weight consisting of structural mass and payload. For loading assumptions, 90% of the total aircraft weight was taken to be supported by the main landing gear, with the remaining load carried by the nose gear. Since there are two main landing gear assemblies, each gear supports approximately 45% of the total aircraft weight under static conditions.

The system consists of three primary sections:
- **Main strut and wheel assembly**, which carries vertical landing and ground loads  
- **Bogie and fork interface**, which transfers forces from the wheels into the strut  
- **Two-bar linkage mechanism**, which controls retraction and deployment  

The design maintains a clear load path from the wheels through the bogie and into the main strut, ensuring forces are transferred efficiently through the structure.

Multiple loading conditions were considered:
- Landing loads
- Static loads  
- Braking loads  
- Stowed configuration

These cases capture both vertical and combined loading conditions seen in real operation.
Overall, the design focuses on realistic load distribution, efficient force transfer, and identifying critical stress regions.
<br>
<p align="center">
	<img src="figures/phase2/side view.png" width="600"></td>
	<p/>

<br>
This motor will read signals from an Arduino to rotate on its axis, extending and folding up the landing gear. These rotations will occur between two fixed-angle measurements (ensured by mechanical locks) to ensure proper positioning/orientation at all times. Both the motor itself and the top pin on the strut will be fixed to the structure of the plane wing and will not move.
<br>

### **Landing gear deployment/retraction sequence**
<p align="center">
Isometric View
<br>
	
[watch the assembly video](https://github.com/user-attachments/assets/6c1ffd8b-b0af-4d7d-89b4-459098cd728c)

<br>
<p align="center">
Frontal View
<br>
	
[watch the assembly video](https://github.com/user-attachments/assets/f484d572-f8e7-468a-845d-adacea77aa67)

<br>

<p align="center">
	<img src="figures/phase2/StraightFrontView.png" width="500"></td>
	<img src="figures/phase2/FoldedFrontView.png" width="500"></td>
	<p/>
	
</p>
  <p align="center">
<br>

	  
**Full 3D Assembly**
<p align="center">
	<p align="center">
  <img src="figures/phase2/ExplodedView.png" width="600"></td>
<p/>
	<p/>
	
<br>  

## **Description of Major Design Decisions and Changes from Phase 1**<br>

*Increased wheel count to more closely resemble inspiration*  
	-Adding three more wheels makes our model more similar to that of many commercial airliners, whose landing gear we want to replicate. This allows our calculations and simulations to be much more accurate to resemble real world conditions. Also, an even number of wheels allows for a more balanced model, so it will more easily be able to stand and hold weight without an unintended failure. (Along with this includes changes to the entire wheel base to accompany more wheels) <br>
<br>

*Improved harness connecting two-bar linkage to main strut* <br>
	-The updated design is able to handle stronger loads, thus resulting in a higher factor of safety of the overall assembly.<br>
	
<br>

*Changed Location of pin for improved kinematics* <br>
	-Raising the height of the pin supporting the two bar linkage allows for complete horizontal storage of the strut, which should allow for storage of the entire landing gear assembly inside the fuselage. Previously, the landing gear ended at an angle, which would result in parts of the landing gear (wheels especially) being very far away from the neutral axis, and probably resting outside the body of the airplane.
## **Discussion of Design for Assembly and Design for 3D Printing**

Not including the tires, each and every CAD part in our assembly is 3D printable. We will vary the orientation of each part when printing to promote ease of printing, and also to ensure the orientation of the layer lines promotes maximum strength in the direction of loading. In Phase 3, we plan to scale this model down to fit in a 256mm 3D print bed, made with PLA filament.<br>
## **Detailed Explanation of Required Analyses (shaft, gear, fatigue, bearings, interfaces, etc.) with Clear Assumptions and Results**


### **Extended Analysis**

Von-Mises Equivalent stress
<table align="center">
  <tr>
    <td><img src="figures/phase2/1 new equivalent stress.png" width="400"></td>
    <td><img src="figures/phase2/2 new equivalent stress.png" width="400"></td>
  </tr>
  <tr>
</table>
<br>
<br>
Factor of Safety
	<img src="figures/phase2/new FOS.png">
<br>
<br>
Fatigue analysis
<table align="center">
  <tr>
    <td><img src="figures/phase2/Equivalent alternating stress.png" width="400"></td>
    <td><img src="figures/phase2/Fatigue FOS.png" width="400"></td>
  </tr>
  <tr>
	<td align="center"><em>Fatigue Equivalent alternating stress</em></td>
    <td align="center"><em>Fatigue Factor of safety</em></td>
  </tr>	  
</table>
	<br>
	<br>
Added Force

(insert here)
<br>
<br> 
Total Deformation
	
<img src="figures/phase2/new_total_deformation.png">

**Retracted Analysis**
<br>
Equivalent Stress
<img src="figures/phase2/Equivalent stress when up.png">
<br>
Factor of Safety
<img src="figures/phase2/FOS when up.png">
<br>
Deformation
<img src="figures/phase2/Deformation when up.png">
<br>
## **Updated List of Anticipated Risks or Weaknesses to be Addressed in Prototyping**
Smallest factor of safety
<img src="figures/phase2/Minimum_safety_factor.png">
<br>
<br>

## **CAD Drawings - Critical Component and Exploded View**

<table align="center">
  <tr>
    <td><img src="figures/phase2/CriticalComponent.png" width="400"></td>
    <td><img src="figures/phase2/ExplodedView.png" width="400"></td>
  </tr>
  <tr>
	<td align="center"><em>Critical Component</em></td>
    <td align="center"><em>Exploded View</em></td>
  </tr>
  </table>

## **Checklist-(2 astrisks is what we have done)** 

	-full 3D assembly**
	-drawings and views (Need from Ben)**
	-printability **
	-static stress and factor of safety**
	-Fatigue (Need from Aiden) **
	-key/coupling/interface stresses (Need from Aiden) 
	-bearing load check**
	-global safety overview 
<br>
<br>
