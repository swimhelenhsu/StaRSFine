# StaRS FInE, Spring 2019
#### Lily Falk, Sam Hertle, and Whitney Denison
#### February 22, 2019

## Abstract

StaRS FInE is critically important because the subteam deals with one of the last steps in the AguaClara process (filtration). The current outtake pipes are problematic because they clog with chemical deposits, and the best method of cleaning them involves wasting clean water. StaRS FInE's suggested remedy to combat this problem involves designing and implementing a “Christmas tree” design that uses gravity exclusion principles to keep sand out and has larger openings to prevent clogs. The main focus of this semester are testing the model printed last semester with sand and finding the failure velocity with that model.


## Introduction

This is StaRS FInE's second semester since the fall of 2015. The subteam was brought back in the fall of 2018 because of its continued relevance and lack of a sustainable solution. The two methods of cleaning the clogged pipes currently are either pouring buckets of acid into the filter, or by running clean water very quickly through the outlet pipes to clean them (as in Zamorano University). In both of these scenarios, the filter being cleaned can't be used, and there is unnecessary waste of clean water whether it is being used to purge the pipe or to divert water from the filters while they are being cleaned. The team’s goal is to develop and test an outlet system that does not clog with chemical deposits and prevents sand from escaping. Past teams failed because of issues with sand getting into their outlet pipe design during filtration. Encouragingly, they did develop designs that worked during backwash, the filtration velocity was just too great and the water effluent contained a great amount of sand. Because this problem occurs at the filtration outtake, the team must be very conscious of head loss and the major and minor losses coming from the outlet pipe and the design geometry.

The goals of this semester are to test the apparatus that was the result of the work of the Fall 2018 team with sand, discover the failure velocity for this apparatus, and make necessary changes to the spacing of the branches and angles. These changes will be based on the research of Horizontal Filtration's work with their new model, the results of our testing, and the library of AguaClara fluid mechanics calculations. The team must also discover what mode of failure must be guarded against, in other words, does the sand move up as a solid plug or do individual grains make their way through the outlet pipe when filtration speed gets too fast? Last semester's design is promising, but there is still a lot of testing to do before it is ready to be proposed as a solution.

## Literature Review and Previous Work

The work of StaRS FInE has not been investigated outside of AguaClara making the project exciting, and requiring innovation on the part of each team member. In the past the team has found examples related to filters from aqua-ponics and various filtering methods, however the alternate systems are more complicated, and would encounter the same issues that AguaClara filters already face. The StaRS FInE team members are the same this semester as last semester, however last semester the team worked mainly on research, and this semester the project has shifted to fabrication.

Last semester the team encountered a few key insights. First, the team tested at what angle sand falls in a pipe filled with water to determine an optimal angle where sand escaping the gravity exclusion zone is still likely to fall back down. The optimal angle was determined to be 26.64 degrees.  

A christmas tree design was created in onshape and 3D printed to fit inside of a 4-inch tube. Unlike previous teams dating back to 2015, the fall 2018 team ensured that the flow rate, velocity, and wing area of the apparatus all work together to prevent sand from exiting during backwash. This apparatus is still being used this semester as a main tool for research.


## Methods

### Experimental Apparatus Design
The apparatus was designed in Onshape last semester, first including a 3D-printed horizontal filter, and then the 4-Inch diameter PVC pipe that will become the prototype for StaRS FInE testing of the gravity exclusion method for extraction. For more information on this infrastructure, reference the Fall 2018 Report. Below are the Onshape part studio, the Onshape drawings, and the photo of the newly fabricated apparatus. After assembling the apparatus, it was designed to have outlet holes in the filter and in the prototype that match tubing size for the outlet flow rate. The tubes are glued to ensure watertight extraction, as shown below.

<p align="center"> <img
src="https://raw.githubusercontent.com/AguaClara/StaRSFine/master/Images/OnshapeDrawingApparatus.png" width= "350"> </p>
<p align="center">
  Figure 1. The Onshape Drawing of the prototype.
</p>
<p align="center"> <img
src="https://raw.githubusercontent.com/AguaClara/StaRSFine/master/Images/OnshapePartStudioApparatus.png" width= "350"> </p>
<p align="center">
  Figure 2. The part studio design for a more realistic view.
</p>
<p align="center"> <img
src="https://raw.githubusercontent.com/AguaClara/StaRSFine/master/Images/ApparatusRealLife.JPG" width= "350"> </p>
<p align="center">
  Figure 3. The apparatus with extraction tubes attached.
</p>

### Experimental Apparatus Fabrication
The apparatus was fabricated last semester. Upon revisiting the design at the beginning of the semester, Monroe suggested that the team perform calculations to determine if the prototype could withstand flow rates used in the actual plants. Accounting for headless and the flow rate calculated below in the Manual section, the team spent the beginning of this semester planning for and re-fabricating the outlet holes to adjust. The space between the wings in the filter, as show below in figure 4, was minimal. The team used Onshape to determine if increasing the hole size to fit larger diameter outlet tubing was possible. It was determined that the holes were to be offset in order to account for size without disrupting the functionality of the filter.

Eventually, the team used the precision drill to create new holes in the filter and in the PVC tube. The holes were attached to tubing which will be hooked up to a peristaltic pump and ProCoDa box to monitor extraction.


* Design (calculations, constraints):
  * Use LaTeX to format equations in line ($\frac{-b\pm\sqrt{b^2-4ac}}{2a}$) or centered:

  \[\frac{-b\pm\sqrt{b^2-4ac}}{2a}\]

## Future Work
In the next several weeks of research, the team plans to test the apparatus for compatibility with sand and fluidization velocities. If the system is successful, the team will be advancing on the first bridged horizontal filter extraction method. This research could be very helpful to current and new plants.

## Bibliography
Logan, B. E., Hermanowicz, S. W., & Parker,A. S. (1987). A Fundamental Model for Trickling Filter Process Design. Journal (Water Pollution Control Federation), 59(12), 1029–1042.

# Manual
The goal of this section provides all of the guidance that would be necessary for a future team to pick up work where the team left off.

## Fabrication Details
The current apparatus design was revisited. The team noted the small outlet pipe size and did the below calculation to determine that minimum pipe diameter was not met.

| Respective Flow Rate      | Minimum Tube Inner Diameter  
|---------------------------|-----------------------|
| 36.67 milliliter / second | 3.762 millimeter      |

Shaving the glue from the previous tubes, the team detached the tubes. Using the new calculated inner diameter, the team found tubing that matched met the minimum standard and considered how it would affect the design of the 3D printed pine-tree filter which was already fit to the prototype PVC tube by holes drilled. In the OnShape drawing, the team determined that, if the filter was taken from the prototype, respective sized holes could be drilled with the drill press. The holes were designed to be offset from the original holes while still remaining in the bounds of the upper and lower wings. Holes were drilled to match these on the 4-Inch PVC prototype.

## Experimental Checklist
Before running the experiments, the team ensured that the prototype was watertight, in order to collect accurate data regarding the flow rates of injection and extraction.

## Python Code
### Variables
$area$: area of the sand bed
$areamm$: area in mm
$backwashvelocity$: velocity of water in the backwash stream
$filterflow$: Minimum flow rate of the water
$headloss$: Headloss
$temp$: Temperature of operation
$\nu$: Kinematic Viscosity of water based on temperature
$piperough$: k, pipe roughness
$diamtube$: tube diameter


```python
import math
import numpy as np
import pandas as pd
from aguaclara.core.units import unit_registry as u
from aguaclara.core import pipes as pipe
from aguaclara.core import physchem as chem

area = 100*u.cm**2
areamm = area.to(u.mm**2)
backwashvelocity = 11*u.mm/u.s
filterflow = (backwashvelocity*areamm*2)/6
print(filterflow.to(u.ml/u.s))

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


```python
# To convert the document from markdown to pdf
pandoc Name_of_this_file.md -o TeamName_Research_Report.pdf
```
