# Phase One: Project Report  
Hard Landing – Landing Gear Project  

<p align="center">
  <img src="figures/phase1/iso2cad.png" alt="System sketch">
</p>

Aiden Beam, Jack Bessette, Ben Kolecki, Hunter Sam, Evan Morris, Nordin Jafar  
Arizona State University  
MAE 342  

## Executive Summary

 This project aims to design and 3D print a retractable and deployable rigid-strut landing gear, intended for kinematic evaluation and preliminary structural and failure analysis. The design implicitly represents a wide-body commercial aircraft main landing gear.
Some simplifications to note are that the design replaces hydraulic actuation with a motor-powered linkage mechanism that supports and deploys the rigid strut. This allows the team to focus on the mechanical motion of the system and how loads are carried through the structure. The landing gear is analyzed at full scale using hand calculations and simulation tools such as ANSYS to evaluate stresses, motion, and potential failure modes under realistic loads.

## System Function and Decomposition
**Primary Function**

The primary function of this landing gear is to provide rigid structural support for an aircraft during all ground operations. This includes taxiing, takeoff, and landings of all intensities. When deployed, the main rigid strut, or oleo, and wheel assembly are designed to absorb and redirect the loadings from landing into the airframe. The rigid design was selected so the Hard Landing team may prioritize understanding the mechanical motion and loading paths through a landing gear. Moreover, this allows the team to ensure the gear maintains its integrity while simulating realistic aircraft loading conditions in the aerospace industry. 
In addition to the structural support the structure must provide, landing gear must reliably retract and deploy over repeated cycles. When the aircraft is airborne, a motor will rotate and fold the landing gear assembly into the wheel well housing, all under a single degree of freedom. A single degree of freedom ensures a smooth retracting and deploying transition along a repeated kinematic path. The overall result of a retracting landing gear allows the assembly to reduce aerodynamic drag to optimize fuel efficiency and overall flight performance. 



<p align="center">
  <img src="figures/phase1/components.png" alt="System sketch">
</p>
<table>
  <tr>
    <td align="center">
      <img src="figures/phase1/isocadproto.png" alt="CAD model">
    </td>
    <td align="center">
      <img src="figures/phase1/frontfacecadproto.png" alt="Hand sketch">
     </td>
  </tr>
</table>

**Decomposition**

The landing gear system is composed of a small number of rigid components connected by pin joints to allow rotation during deployment and retraction (see scaled figure).
Sketch dimensions are intended for prototype demonstration. Primary components (as shown in figure)

**Wheel Leg / Oleo**  
Main rigid strut of the landing gear. Carries the wheel assembly and primary loads  

**Long Bar**  
Part of the linkage mechanism. Controls the motion of the wheel leg during retraction and deployment.

**Short Bar**  
Works with the long bar to guide the rotation path. Helps constrain the mechanism motion.

**Clamp**  
Connects the linkage to the wheel leg. Transfers motion and loads between the linkage and main strut  

Note - Pin joints are assumed at all rotating connections but are not shown in detail. Wheels and small hardware are omitted for clarity. The simplified component layout allows the mechanism motion and load paths to be analyzed without unnecessary complexity.

## Kinematics
<p align="center">
  <img src="figures/phase1/kinematicmotion.png" alt="System sketch">
</p>


**Description**
-The landing gear mechanism is a planar linkage system composed of rigid members connected by pin joints. Based on the linkage layout, the system has one degree of freedom (1 DOF), meaning the entire motion is governed by a single input. Detailed kinematic derivations are provided in scanned notebook form
(click figures to expand)

<p align="center">
  <a href="figures/phase1/hunterkinematicspg1.jpg">
    <img src="figures/phase1/hunterkinematicspg1.jpg" width="150">
  </a>
  &nbsp;&nbsp;&nbsp;
  <a href="figures/phase1/hunterkinematicspg2.jpg">
    <img src="figures/phase1/hunterkinematicspg2.jpg" width="150">
  </a>
</p>

## Preliminary Failure Mode Review

**Static overload (primarily in the main leg)**  
-Design aims to incorporate a factor of safety high enough to not fail under typical or atypical loading.

**Fatigue / cyclic loading (bearings, smaller beams)**
-Repeated extension and retraction causes wear on bearings and other load-bearing joints.  
Design aims to use materials and designs capable of handling repeated loading and to prescribe routine maintenance.

**Misalignment**  
-Tires contacting the ground at angles other than vertical may cause uneven loading.  
Design aims to incorporate components that lock the system in fully extended or retracted positions.

**Temperature-based failure**  
-In warmer environments, elevated temperatures could result in deformation or material degradation.

## Analysis Methods
**Beam Theory**
A primary study of the lending gear can be performed through beam analysis. The main strut, or oleo, can be treated as a beam and the supporting strut can be trivialized to a two force member. The team can study the strut under combined axial and bending loads to determine the locations of maximum bending and shear stress from loadings during landing. This simplified model is limited by its inability to account for the dynamic interaction between the two legs of the supporting strut as well as the pins in the structure. Ultimately, beam theory best serves as a primary validation tool for the primary strut of the landing gear.


**ANSYS / Simulation Analysis**  
After creating individual parts and an assembly in SOLIDWORKS, the design can be imported to ANSYS so real world loadings can be applied to the housing and our structure. We will then analyze the beam under loading conditions that model what would be seen in the real world. ANSYS will help us identify and evaluate the failure modes of our system. Allowing us to make design improvements to our prototype and understand the impact of elements such as hydraulics in the industry 


## Critical Design Parameters
The success of the “Hard Landing” gear structure relies on the implementation of various critical design parameters. These parameters correspond to the structural integrity of the landing gear under load and ensure the mechanism operates as the kinematic relationships describe. 

**Pin to Clamp Length, ℓCD**

-The length front the pin at the top of the strut to the clamp, ℓ, is a critical parameter that directly impacts the angles that the supporting linkage bars must reach. Additionally, the location of the clamp along the oleo will determine the amount of torque the motor needs to rotate the free end with the wheel. 

**Motor Torque and Rotation Requirements**

-The hydraulics in the inspiration for “Hard Landing” have been replaced with rigid supports and rotation powered by a motor. The required torque of the stepper motor, along with the angle it must rotate to, must be calculated to bring the oleo to a 90 degree angle with the landing surface.

**Factor of Safety**

-A reasonably high factor of safety must be established after determining the highest stress components to avoid static overload and failure due to large loadings upon landing. 

**Supporting Strut Lockout**

-When the landing gear is deployed the angle between the short and long bar must be straight at 180 degrees. If this linkage is not at a straight angle, it will not effectively support the loading on the landing gear. The lengths of these bars and the pin at their linkage must be optimized to ensure they do not collapse under loading during landing. 

