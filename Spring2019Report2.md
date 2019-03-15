# StaRS FInE, Spring 2019
#### Lily Falk, Sam Hertle, and Whitney Denison
#### March 15, 2019

**[Sidney: Hey team! I will be using bolded square brackets to comment on your manual.]**

## Abstract

StaRS FInE was critically important because the subteam dealt with one of the last steps in the AguaClara process - filtration. The outtake pipes first used in vertical filtration were problematic because over time they became clogged with chemical deposits. In order to clean the filters and wash away the deposits, clean water was emptied from the larger outlets to increase outflow velocity through the slots to dislodge the chemicals. In the process, clean water was wasted. StaRS FInE worked on a design that had the potential to combat this problem by making use of a “Christmas tree” design. The design relied on larger openings to prevent clogs, as well as the gravity exclusion principle to prevent sand from exiting the outlet pipes. The focus of StaRS FInE in the spring of 2019 was to test the three dimensional model printed the previous semester with sand and find what velocity leads to failure in this model.

## Introduction

The spring of 2019 was StaRS FInE's second semester since the fall of 2015. The subteam was brought back in the fall of 2018 because of its continued relevance to AguaClara plants. The filter system in place at this time became clogged throughout the day with chemical deposits, and there was no sustainable solution. Chemical deposits built up on the small slots of the filters, and eventually the plant had to be temporarily shut off for clean water to be pulled through and disposed of. Alternatively, buckets of acid could be poured into the filter to clean them, which was also not ideal. In both of these scenarios, the filter could not be used while it was cleaned, and there was unnecessary waste of clean water whether it was being used to purge the pipe or to divert water from the filters while they were being cleaned. The goal of StaRS FInE was to develop and test an outlet system that did not clog with chemical deposits and prevented sand from escaping. Past teams failed because of issues with sand getting into their outlet pipes during filtration. The past team did develop designs that worked during backwash, however the filtration velocity was too large for the parameters of their design and the water effluent contained a significant amount of sand. Because this problem occurred at the filtration outtake, the team was very conscious of head loss and the major and minor losses coming from the outlet pipe and the design geometry.

The goals of this semester were to test the apparatus designed and 3D printed in the Fall 2018 with sand, discover the failure velocity for this apparatus, and make changes to the spacing of the branches and angles if necessary. These changes were based on the some of the research of Horizontal Filtration (another AguaClara subteam), the results of testing, and the library of AguaClara fluid mechanics calculations. The team also had to discover the possible modes of failure. Failure modes may be caused by flow that is too fast, which may lead to sand moving up as a solid plug or small grains of sand getting into the outlet pipe. Fall 2018's design was promising, but before it was ready to be proposed as a solution a lot more tests had to be run.

## Literature Review and Previous Work

The work of StaRS FInE has not been investigated outside of AguaClara making the project exciting, and requiring innovation on the part of each team member. In the past the team has found examples related to filters from aquaponics and various filtering methods. That being said, the alternate systems are more complicated, and would encounter the same issues that AguaClara filters already face. The StaRS FInE team members are the same this semester as last semester, however last semester the team worked mainly on research, and this semester the project has shifted to fabrication.

Last semester the team encountered a few key insights. First, the team tested at what angle sand falls in a pipe filled with water to determine an optimal angle where sand escaping the gravity exclusion zone is still likely to fall back down. The optimal angle was determined to be 26.64 degrees.  

A "Christmas tree" design was created in OnShape and 3D printed to fit inside of a 4-inch tube. Unlike previous teams dating back to 2015, the fall 2018 team ensured that the flow rate, velocity, and wing area of the apparatus all work together to prevent sand from exiting during backwash. This apparatus is still being used this semester as a main tool for research.


## Methods

### Experimental Apparatus Design
#### Trial 1
The apparatus was designed in OnShape last semester, first including a 3D-printed horizontal filter, and then the 4-Inch diameter PVC pipe that will become the prototype for StaRS FInE testing of the gravity exclusion method for extraction. For more information on this infrastructure, reference the Fall 2018 Report. Below are the OnShape part studio, the OnShape drawings, and the photo of the newly fabricated apparatus. After assembling the apparatus, it was designed to have outlet holes in the filter and in the prototype that match tubing size for the outlet flow rate.

<p align="center"> <img
src="https://raw.githubusercontent.com/AguaClara/StaRSFine/master/Images/ApparatusOnshape.png" width= "350"> </p>
<p align="center">
  Figure 1. The OnShape Drawing of the prototype.
</p>
<p align="center"> <img
src="https://raw.githubusercontent.com/AguaClara/StaRSFine/master/Images/FIlterDrawing.png" width= "350"> </p>
<p align="center">
  Figure 2. The part studio design of the 3D printed filter.
</p>
<p align="center"> <img
src="https://raw.githubusercontent.com/AguaClara/StaRSFine/master/Images/ApparatusDrawing.png" width= "350"> </p>
<p align="center">
  Figure 3. The part studio design of the whole prototype.
</p>
<p align="center"> <img
src="https://raw.githubusercontent.com/AguaClara/StaRSFine/master/Images/ApparatusReal.png" width= "500"> </p>
<p align="center">
  Figure 4. The apparatus setup with peristaltic pumps and tubing.
</p>


For experiments conducted thus far, the filter's ability to form sand exclusion zones was tested. Monroe suggested that the team best simulate real life AguaClara filter conditions. Therefore, it was designed so that the inlet, below the filter to simulate filtration.

The design also considered the rate at which injection and extraction would occur at. Essentially, the respective injection and extraction rates were calculated based on backwash velocity and the respective design of the team's apparatus. This is calculated below in Python code in the [manual](#Manual). The values for the first trial were as follows:
| Injection Flow Rate     | Extraction Flow Rate
|---------------------------|-----------------------|
| 36.67 mL/s | 18.36 mL/s      |

In the first trial, the team allowed the injection flow to fill the tube to the top before the extraction pump was turned on. The extraction would pull water until the prototype was halfway drained and then the extraction would be turned off again. This would allow gravity to act as the flow from above the filter, as well as the injection as the flow below.

The last design consideration was converting between mL/s and RPM on the peristaltic pump that was connected to the inlet and outlet tubing. Using ProCoDa, the outlet and inlet flow in mL/s and the tubing sizes (16 for outlet and 18 for inlet), the team made new set points that converted into RPM values for the pump. More is detailed about the set points below in the [manual](#Manual).
#### Trial 2
In the design of the second experimental apparatus, the team reconsidered the flow rates of injection and extraction. Understanding more about the application of the prototype to real Aguaclara Filters, the team calculated the following:
| Injection Flow Rate | Extraction Flow Rate |
| ------------------- | -------------------- |
| 220.02 mL/s         | 36.67 mL/s           |

The team used the same method of filling the prototype to the top before draining and turning off the extraction before the water level reached below the extraction tubes.

### Experimental Apparatus Fabrication
#### Trial 1
The current apparatus design was revisited. The team noted the small outlet pipe size and did the below calculation to determine that minimum pipe diameter was not met.

| Respective Flow Rate      | Minimum Tube Inner Diameter  
|---------------------------|-----------------------|
| 36.67 milliliter / second | 3.762 millimeter      |

<p align="center">
Reference manual below for python code calculations of these values. </p>

Shaving the glue from the previous tubes, the team detached the tubes. Using the new calculated inner diameter, the team found tubing that matched met the minimum standard and considered how it would affect the design of the 3D printed pine-tree filter which was already fit to the prototype PVC tube by holes drilled. In the OnShape drawing, the team determined that, if the filter was taken from the prototype, respective sized holes could be drilled with the drill press. The holes were designed to be offset from the original holes while still remaining in the bounds of the upper and lower wings. Holes were drilled to match these on the 4-Inch PVC prototype.

With three new outlet tubes of sufficient diameter glued water-tight, the team used two T-joint push-to-connect tubes to attach the outlet to a peristaltic pump of size 16 tubing. The inlet (lower cap) was tapped with push-to-connect that was attached to size 18 tubing in a peristaltic pump.

The team made the mistake of filling the apparatus with sand and then inverting so that exclusion zones were given no real chance to form.

<p align="center"> <img
src="https://raw.githubusercontent.com/AguaClara/StaRSFine/master/Images/InvertedApparatus.png" width= "350"> </p>
<p align="center">
  Figure 5. The colored sand filling the exclusion zones as the apparatus was inverted.
</p>

#### Trial 2
In the second trial, the team drained the water and sand from the prototype. To better simulate plant conditions, Monroe suggested that the team first fill the prototype with water, and add sand from the top. This would create sand exclusion zones initially, that just needed to be maintained during water flow.

Using the newly calculated flow rates, the apparatus was set up the same way as in the first trial, with detail in respect to the order of addition of sand and water. This also prevented the sand from entering the injection tubing because there was a constant water stream disallowing it. When the sand nearly filled the tube, the upper lid was secured and the extraction started.

### Feasibility of Design and Analysis
Before running the experiments, the team ensured that the prototype was watertight in order to collect accurate data regarding the flow rates of injection and extraction.

#### Trial 1

The initial mistake of inverting the apparatus was a limitation of the team's understanding of how the design would work in terms of water exclusion zone. The lower of the three triangular partitions was able to form the strongest exclusion zone, which was in fact pulling water without sand.

This trial gave the team an indication of how to move on, but should be noted that flow rates were not indicative of the Aguaclara filtration flow rates (of injection and extraction).

<p align="center"> <img
src="https://raw.githubusercontent.com/AguaClara/StaRSFine/master/Images/Trial1Filter.jpg" width= "350"> </p>
<p align="center">
  Figure 6. The exclusion zone on the lower structure forming.
</p>

<p align="center"> <img
src="https://raw.githubusercontent.com/AguaClara/StaRSFine/master/Images/Trial1Tubes.png" width= "350"> </p>
<p align="center">
  Figure 7. The extraction tubes pulling water without sand from the lower exclusion zone. Note the top tube was pulling sand from the most failed exclusion zone and the middle was pulling air.
</p>

#### Trial 2

The biggest issue with the second trial was that only the top tube pulled water out. This can be explained by a couple of possibilities. There was water leaking through the middle and bottom tubes, suggesting that they were not watertight and so they may have been pulling air only. There could also be a problem with how we join the three tubes together, either with it not being airtight or with an unequal distribution of suction from the peristaltic pump. Encouragingly, the top tube did not have any sand in it. This means that at least one of the gravity exclusion zones formed and was capable of operating at the necessary velocity without reaching either failure mode.

## Future Work
In the next several weeks of research, the team plans to test the apparatus for compatibility with sand and fluidization velocities. If the system is successful, the team will be advancing on the first bridged horizontal filter extraction method. This research could be very helpful to current and new plants.

# Manual
The goal of this section provides all of the guidance that would be necessary for a future team to pick up work where the team left off.

## ProCoDa

The ProCoDa used thus far in the semester has been limited to making sure the input and output peristaltic pumps are running at the correct velocity for their tube size. The team has not yet run an extended experiment regulated by ProCoDa.

## Python Code
### Variables
$area$ : area of the sand bed

$areamm$ : area in mm

$backwashvelocity$ : velocity of water in the backwash stream

$filterflow$ : Minimum flow rate of the water

$headloss$ : Headloss

$temp$ : Temperature of operation

$\nu$ : Kinematic Viscosity of water based on temperature

$piperough$ : k, pipe roughness

$diamtube$ : tube diameter


```python
import math
import numpy as np
import pandas as pd
from aguaclara.core.units import unit_registry as u
from aguaclara.core import pipes as pipe
from aguaclara.core import physchem as chem

area = 100*u.cm**2
#area of the filter bed for simulations
areamm = area.to(u.mm**2)
backwashvelocity = 11*u.mm/u.s
filterflow = (backwashvelocity*areamm*2)/6
#filterflow is the flow rate of water coming out of each filter
print(filterflow.to(u.ml/u.s))
injectionflow = filterflow*6
#injectionflow is the rate at which the water would be coming through the filter (all six layers of filter through the filter)
print(injectionflow.to(u.ml/u.s))
extractionflow = filterflow*2
#extractionflow is the flow rate at which the team will extract water from the filter because water is coming through from above and below the filter
print(extractionflow.to(u.ml/u.s))

headloss = 1*u.m
Length = 1*u.m
temp = 20*u.degC
Nu = chem.viscosity_kinematic(temp)
PipeRough = 0.1*u.mm
KMinor = 2
#to use to find diameter tube for the three tubes that will go in
diamtube = chem.diam_pipe((filterflow/3), headloss, Length, Nu, PipeRough, KMinor)
print(diamtube.to(u.mm)) #inner diamter of tube we would like to come out

```
