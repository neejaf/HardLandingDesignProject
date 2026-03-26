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

## Description of Major Design Decisions and Changes from Phase 1

### Increased wheel count to better match real configurations
- Added three additional wheels to more closely reflect typical commercial airliner landing gear
- Improves realism of load distribution in simulations
- Results in a more stable and balanced system under load
- Wheelbase was updated to accommodate the additional wheels

### Reinforced linkage-to-strut connection
- Strengthened the connection between the two-bar linkage and main strut
- Allows the assembly to handle higher loads
- Increases the overall factor of safety

### Pin relocation for improved kinematics
- Raised the pin supporting the two-bar linkage
- Allows full horizontal stowage of the strut
- Enables more realistic retraction within the fuselage
- Eliminates previous angled configuration that would place components outside the aircraft envelope

## **Discussion of Design for Assembly and Design for 3D Printing**
Phase 3, we plan to scale this model down to fit in a 256mm 3D print bed, made with PLA filament. Certain dimesnsions will be adjussted to account for 3D print tolerances to ensure intented kinematics is possible.

### Design for Assembly
- Assembly is kept simple using pin connections for all joints
- Parts are split into manageable components (strut, bogie, linkage, etc.)
- Small clearances are included to avoid binding during motion

### Design for 3D Printing
- All parts are sized to fit within the printer build volume
- Basic clearances are included to account for print tolerance
- Parts are oriented to reduce the need for supports where possible
- Design prioritizes functionality over strength since this is a demonstration model
<br>

## **Analysis**
- As mentioned before, four loading cases are evaulated: landing impact, static load, braking (rejected takeoff), and stowaway configuration. These cases represent the primary or critical conditions the landing gear is expected to experience.
- Loads are derived by assuming the main landing gear supports approximately 90% of the total aircraft weight, distributed equally between the two main gear assemblies. This approach follows standard landing gear design practices.
- For landing conditions, a load factor (n ≈ 2–3) is applied to account for impact during touchdown. Braking conditions introduce horizontal forces due to friction at the wheels, while the static case considers steady vertical loading. The stowed configuration evaluates the effect of gravity and constraints during retraction.
- For each case, forces and constraints are applied to approximate real-world conditions, and resulting stresses, deformations, and reaction forces are analyzed to evaluate structural performance and factor of safety.

### Landing (Tilted Oleo @ 9 degrees - 3.4MN Load)
Von-Mises Equivalent Stress Results - 220.81 MPa
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
<td><img src="figures/phase2/Minimum_safety_factor.png" width="400"></td>
<br>
<br>

## **CAD Drawings - Critical Components and Exploded View**

<table align="center">
  <tr>
    <td><img src="figures/phase2/CriticalComponent.png" width="400"></td>
	<td><img src="figures/phase2/CriticalComponent2.png" width="400"></td>
    <td><img src="figures/phase2/ExplodedView.png" width="400"></td>
  </tr>
  <tr>
	<td align="center"><em>Oleo</em></td>
	<td align="center"><em>Bogie</em></td>
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
