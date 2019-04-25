# StaRS FInE, Spring 2019
#### Lily Falk, Sam Hertle, and Whitney Denison
#### April 14, 2019

## Abstract

StaRS FInE has worked to develop an improved filter technology for AguaClara outlet pipes.Filtration is the last step in an AguaClara plant. As a result, it is the last opportunity to remove particles that have slipped through all previous treatment processes.
Prior to StaRS FInE, the outtake pipes used in vertical filtration were problematic because small slits in the pipes would clog with chemical deposits. In order to clean the filters and wash away the deposits, clean water was emptied from the larger outlets to increase outflow velocity through the slots to dislodge the chemicals. In the process, clean water was wasted. StaRS FInE designed an alternative to the outtake pipes, triangular in shape, and therefore referred to as the “Christmas tree” design. The design relied on larger openings to prevent clogs, as well as the gravity exclusion principle to prevent sand from exiting the outlet pipes. The focus of StaRS FInE in the spring of 2019 was to test the three dimensional model printed in the fall of 2019 with sand to find what velocity leads to failure in the form of sand in the outlets.

## Introduction

The spring of 2019 was StaRS FInE's second semester working on recent improvements since being disbanded in the fall of 2015. The subteam was brought back in the fall of 2018 because of its continued relevance to AguaClara plants. The filter system used then became clogged throughout the day with chemical deposits, mostly from PaCl, but there was no sustainable solution to the clogging **[do you mean there was not a sustainable solution?]** . Chemical deposits built up on the small slots of the filters, and the plant had to be temporarily shut off periodically for cleaning. During this cleaning (not to be confused with backwash, where the sand particles in the filter are cleaned), clean water would be purged to dislodge the build up on the pipes. Alternatively, buckets of acid could be poured into the filter to clean them, which was also not ideal. In both of these scenarios, the filter could not be used while it was cleaned, and clean water was wasted, whether it was being used to purge the pipe or to divert water from the filters while they were being cleaned with acid. The goal of StaRS FInE was to develop and test an outlet system that prevented sand from escaping and did not clog with chemical deposits. Past teams failed because of issues with sand getting into their outlet pipes during filtration. The past team did develop designs that worked during backwash, however the filtration velocity was too large for the parameters of their design and the water effluent contained a significant amount of sand. Because this problem occurred at the filtration outtake, the team was very conscious of head loss and the major and minor losses coming from the outlet pipe and the design geometry.

The goals for the spring of 2019 were to test the apparatus (designed and 3D printed in the Fall 2018) with sand, discover the failure velocity for this apparatus, and make changes to the spacing of the branches and angles if necessary. The original spacing and angles were based on some of the research of Horizontal Filtration (another AguaClara subteam), the results of testing by past StaRS teams, and the library of AguaClara fluid mechanics calculations. The team also had to discover the possible modes of failure. Failure modes may be caused by flow that is too fast, which may lead to sand moving up as a solid plug or small grains of sand getting into the outlet pipe. Fall 2018's design was promising, but before it was ready to be proposed as a solution, many more tests had to be run.

Gravity exclusion is a principle that explains some interaction between sand and water that informs the research and fabrication of StaRS FInE. The idea is that for two flat surfaces (branches) creating a roof with a specific angle, if sand were to get beneath the branch, it would slide down with gravity and remain outside of the outlet. The water beneath the branches creates enough pressure that the sand remains out of the outlet pipe and in the gravity exclusion zone. This zone is formed by the sand that settles beneath the branches. The biggest challenge with preventing sand from going into the outlet happens during forward filtration, when water is moving quickly through the outlet. In this case, the sand-water interface at the edge of the exclusion zone must be large enough that the force of gravity on the sand is greater than the force of the water moving up through the sand.

## Literature Review and Previous Work

The work of StaRS FInE has not been investigated outside of AguaClara, making the project exciting, requiring innovation on the part of each team member. In the past, the team has found examples related to filters from aquaponics and various filtering methods. That being said, the alternate systems are more complicated, and would have encountered the same issues that AguaClara filters had already faced. The StaRS FInE team members remained the same from the fall of 2018 to the spring of 2019. That being said,**[second time that being said is used in this paragraph, be careful and try for more professional usage and technical writing]** the team focused on research in the fall, whereas the team shifted to fabrication in the spring.

From the reports of the 2015 team, it seems that the necessary wingspan and size of the sand-water interface was not calculated correctly **[be more sure, is it a conclusion that was drawn? Seems seem a bit more iffy]**. This is supported by their lack of success with keeping sand from exiting the filter during higher forward filtration velocities. The size of the spring of 2019's model interface is much larger and there has been greater success in keeping sand out of the outlets.

In the fall of 2018 the team discovered  a few key insights. First, the team tested the angle at which sand falls in a pipe filled with water to determine an optimal angle where sand escaping the gravity exclusion zone is still likely to fall back down. The optimal angle was determined to be 26.64 degrees.  

From the calculations done with the AguaClara fluid calculation Python code library, a "Christmas tree" design was created in OnShape and 3D printed to fit inside of a 4-inch tube. Unlike previous teams dating back to 2015, the fall 2018 team ensured that the flow rate, velocity, and wing area of the apparatus all work together to prevent sand from exiting during backwash. This apparatus is still being used this semester as a main tool for research.



## Methods

### Experimental Apparatus Design
#### Trial 1

The apparatus was designed in OnShape last semester, first including a 3D-printed horizontal filter, and then a 4-Inch diameter PVC pipe that would become the prototype for StaRS FInE testing of the gravity exclusion method for extraction. For more information on this apparatus, reference the Fall 2018 Report. Below are the OnShape part studio, the OnShape drawings, and the photo of the newly fabricated apparatus. After assembling the apparatus, it was designed to have outlet holes in the filter and in the prototype that match tubing size for the outlet flow rate.

-*see above*
<p align="center"> <img
src="https://raw.githubusercontent.com/AguaClara/StaRSFine/master/Images/ApparatusOnshape.png" width= "500"> </p>
<p align="center">
  Figure 1. The OnShape Drawing of the prototype.
</p>
<p align="center"> <img
src="https://raw.githubusercontent.com/AguaClara/StaRSFine/master/Images/FIlterDrawing.png" width= "500"> </p>
<p align="center">
  Figure 2. The part studio design of the 3D printed filter.
</p>
<p align="center"> <img
src="https://raw.githubusercontent.com/AguaClara/StaRSFine/master/Images/ApparatusDrawing.png" width= "500"> </p>
<p align="center">
  Figure 3. The part studio design of the whole prototype.
</p>
<p align="center"> <img
src="https://raw.githubusercontent.com/AguaClara/StaRSFine/master/Images/ApparatusReal.png" width= "700"> </p>
<p align="center">
  Figure 4. The apparatus setup with peristaltic pumps and tubing.
</p>



The experiments up to trial 1 had tested the filter's ability to form sand exclusion zones. Monroe suggested that the team simulate real life AguaClara filter conditions as best as possible. Therefore, it was designed so that the inlet, below the filter would simulate filtration. 

The design also considered the rate at which injection and extraction would occur. AguaClara plant sand filters perform filtration by running water through and extracting from the sand bed at controlled rates. The respective injection and extraction rates were calculated based on backwash velocity and the respective design of the team's apparatus. This is calculated in the Python code in the [manual](#Manual) below. These rates were converted to RPM for the use of peristaltic pumps in ProCoDa, marked as inject and extract. The values for the first trial were as follows:
| Injection Flow Rate     | Extraction Flow Rate
|---------------------------|-----------------------|
| 36.67 mL/s | 18.36 mL/s      |


In the first trial, the team allowed the injection flow (inlet) to fill the tube to the top before the extraction pump (outlet) was turned on. The extraction pump pulled water until the prototype was halfway drained and then the extraction pump would turn off again. At this point, gravity made injection from the top of the apparatus unnecessary and acted as an "injection" source.

The last design consideration was converting between mL/s and RPM on the peristaltic pump that was connected to the inlet and outlet tubing. The team made new set points that converted to RPM values for the pump using ProCoDa, the outlet and inlet flow in mL/s and the tubing sizes (16 for outlet and 18 for inlet). More is detailed about the set points below in the [manual](#Manual). This was a design consideration for the team because the tubing size was adjusted in the apparatus based on the capacity of the peristaltic pump rates and calculations in ProCoDa.


#### Trial 2
In the design of the second experimental apparatus, the team reconsidered the flow rates of injection and extraction pumps. Understanding more about the application of the prototype to real Aguaclara Filters, the team calculated the following:


| Injection Flow Rate | Extraction Flow Rate |
| ------------------- | -------------------- |
| 220.02 mL/s         | 36.67 mL/s           |

After trial 1, the team came to understand that the 6 layers of sand filter would be extracting at the same rate. Therefore, the injection flow rate that the team had used previously was not sufficiently large.

Again, more information about these number can be found in the Python code below in the [manual](#Manual). **[remember to write more technically]**

The team used the same method of filling the prototype to the top before draining and turning off the extraction before the water level reached below the extraction tubes.

#### Trial 3
After considering the second trial, the team again revisited the flow rates. The team had not considered that the flow rate through the filter would be divided by the 3 outlet holes, leading to some error. Therefore, instead of extracting 36.67 mL/s from all three extraction tubes, each would be attached to a pump extracting at 36.67 mL/s. The Python code for the third trial in the [manual](#Manual) explains how the new flow rate was calculated.

| Injection Flow Rate | Extraction Flow Rate |
| ------------------- | -------------------- |
| 220.02 mL/s         | 36.67 mL/s           |

In anticipation of failure, the team first decided to measure whether only one filter outlet could extract at the flow rate. To do so, the team planned on stopping flow from the upper two holes and attaching one pump to the injection tube one pump to the extraction tube. Therefore, the apparatus was designed so that the team could monitor the extraction zone and escape of sand into the outlet more closely.

### Experimental Apparatus Fabrication
#### Trial 1
In the previous semester, the team glued extraction tubes to the apparatus to begin to test design feasibility. Upon revisiting the idea, the team decided the outlet pipe size did not match a minimum inner diameter value.

| Respective Flow Rate      | Minimum Tube Inner Diameter  
|---------------------------|-----------------------|
| 36.67 milliliter / second | 3.762 millimeter      |

<p align="center">
Reference manual below for Python code calculations of these values. </p>

Glue had been used to connect the outlet "pipes" (tubing) to the reactor (the 4-inch diameter PVC pipe). To adjust the apparatus, after shaving the glue from the previous tubes, the team detached the tubes. * Using the new calculated inner diameter, the team found tubing that met the minimum standard and considered it's effect on the design of the 3D printed "pine-tree" filter which already fit to the prototype PVC tube by drilled holes. In the OnShape drawing, the team determined that if the filter was taken from the prototype, respective sized holes could be drilled with the drill press. The holes were designed to be offset from the original holes while still remaining in the bounds of the upper and lower wings. Holes were drilled to match these on the 4-Inch PVC prototype.

With three new outlet tubes of sufficient diameter glued water-tight, the team used two T-joint push-to-connect tubes to attach the outlet to a peristaltic pump of size 16 tubing. The inlet (lower cap) was tapped with push-to-connect that was attached to size 18 tubing in a peristaltic pump.

The team made the mistake of filling the apparatus with sand and then inverting so that exclusion zones could no longer form. The colored sand was chosen to closely monitor the escape of sand from the outlet tubes, but the color dyed the water and the method was unnecessary, leading to regular sand use in future trials.

<p align="center"> <img
src="https://raw.githubusercontent.com/AguaClara/StaRSFine/master/Images/InvertedApparatus.png" width= "350"> </p>
<p align="center">
  Figure 5. The colored sand filling the exclusion zones as the apparatus was inverted.
</p>



#### Trial 2
In the second trial, the team drained the water and sand from the prototype. To better simulate plant conditions, Monroe suggested that the team first fill the prototype with water, and add sand from the top. This would create sand exclusion zones initially, that just needed to be maintained during water flow.**[what just needed to be maintained, the way the sentence was structured made me confused a bit]**

Also, to prevent sand from falling into the injection tube, the team added extremely porous metal mesh between the tube and the push-to-connect.

<p align="center"> <img
src="https://raw.githubusercontent.com/AguaClara/StaRSFine/master/Images/Trial2Water.JPG" width= "350"> </p>
<p align="center">
  Figure 6. Water filling the apparatus before the addition of sand.
</p>

Using newly calculated flow rates from the experimental design passage above, the apparatus was set up the same way as in the first trial, with detail in respect to the order of addition of sand and water. This also prevented the sand from entering the injection tubing because there was a constant water stream that made use of gravity exclusion. When the sand nearly filled the tube, the upper lid was secured and the extraction began.

#### Trial 3
This purpose of this trial was to test the feasibility of the intense newly calculated flow rate. Therefore, the team honed in on one filter wing outlet hole to analyze. The team used plugs at the push-to-connects in lieu of pump tubing to stop the flow from the upper two tubes.

Other than the use of only one extraction hole, the test was conducted in the same way as the earlier trials where the apparatus was filled with water and sand before extraction. After beginning extraction, the injection flow would remain until the water level was close to the opening of the filter outlet hole. The injection and extraction tubes were attached to two peristaltic pumps, set to their effective flow rates in RPM.

<p align="center"> <img
src="https://raw.githubusercontent.com/AguaClara/StaRSFine/master/Images/Trial3SetUp.jpeg" width= "350"> </p>
<p align="center">
  Figure 7. Sand filling the apparatus before extraction.
</p>


### Feasibility of Design and Analysis
Before running the experiments, the team ensured that the prototype was watertight in order to collect accurate data regarding the flow rates of injection and extraction.

#### Trial 1

The initial mistake of inverting the apparatus caused a limitation in the team's understanding of how the design would work in terms of water exclusion zone. The lower of the three triangular partitions was able to form the strongest exclusion zone, which was in fact pulling water without sand.

This trial gave the team an indication of how to move on, but it should be noted that flow rates were not yet indicative of the Aguaclara filtration flow rates (of injection and extraction).

<p align="center"> <img
src="https://raw.githubusercontent.com/AguaClara/StaRSFine/master/Images/Trial1Filter.jpg" width= "350"> </p>
<p align="center">
  Figure 8. The exclusion zone on the lower structure forming.
</p>

<p align="center"> <img
src="https://raw.githubusercontent.com/AguaClara/StaRSFine/master/Images/Trial1Tubes.png" width= "350"> </p>
<p align="center">
  Figure 9. The extraction tubes pulling water without sand from the lower exclusion zone. Note the top tube was pulling sand from the most failed exclusion zone and the middle was pulling air.
</p>

#### Trial 2

The biggest issue with the second trial was that only the top tube pulled water out. This can be explained by a couple of possibilities. There was water leaking through the middle and bottom tubes, suggesting that they were not watertight and so they may have been pulling air only. The existence of air bubbles within the filter was also indication that there is flaw in the design.

<p align="center"> <img
src="https://raw.githubusercontent.com/AguaClara/StaRSFine/master/Images/Trial2Filter.JPG" width= "350"> </p>
<p align="center">
  Figure 10. The filter extraction zones during the second trial. Note the air bubbles in between the layers.
</p>

The top tube did not have any sand in it and the exclusion zones did exist, in a sense which is an essential insight moving forward. This means that at least one of the gravity exclusion zones formed and was capable of operating at the necessary velocity without failure. In agreement with the first trial, the lowest of the three "branches" was successfully pulling water.

<p align="center"> <img
src="https://raw.githubusercontent.com/AguaClara/StaRSFine/master/Images/Trial2Tubes.png" width= "450"> </p>
<p align="center">
  Figure 11. The extraction tubes during the second trial.
</p>

#### Trial 3
In the third trial, the team discovered a very promising result for Aguaclara; the extraction pump could pull water out of one layer of the filter without sand in the output. The minimum failure velocity of the exclusion zones, although not yet found, should be greater than the maximum flow rate out of the filter in true Aguaclara plants.

Although this information is exciting for the team, this trial did not use all three exclusion zones that the original design intended. The optimized filter would pull water from all three of the outlet tubes.

<p align="center"> <img
src="https://raw.githubusercontent.com/AguaClara/StaRSFine/master/Images/ExclusionZonesTrial3.PNG" width= "450"> </p>
<p align="center">
  Figure 12. The exclusion zones during the third trial.
</p>

The difficult issue with air bubbles caused the use of not all extraction tubes, as the air bubbles existed in the upper two partitions that were plugged. The next move for the team would be to take steps to understand more about the pressure differential in the apparatus and determine a different way to extract from the filters.

Another persistent issue is the availability of pumps that can function at a rate as high as the team needs. Also, in the Aguaclara filters, it is not customary to have water deliberately pulled from filters, rather than just having it come out on its own at a rate determined by the rate of water going in.

## Conclusions

Testing the apparatus with sand and water running at filtration speeds made the flaws in the apparatus used for experimentation clear, but not yet the problems with the "Christmas tree" design. The second trial showed that the top branch of the filter can handle high velocities of filtration without sand leaving in the outlet pipes, which is encouraging for predicting the success of this design. The third trial stands to show the strength of the exclusion zones that are formed by this design. There is work to be done regarding optimizing this design and implementing in true Aguaclara plants, but the team is hopeful regarding its progress.

## Future Work
Based on the three trials completed so far this semester, the most pressing goal was to have an experiment where water was pulled from all three tubes. With consideration of plant limitations, the team could move forward to testing failure and finding the filtration velocity where sand begins to be pulled out with the water. If this velocity is reasonably high (i.e. much higher than any velocity expected in an AguaClara plant), the team will have a conversation about next steps necessary to implement the design in actual AguaClara plants. If the failure velocity is low or gravity exclusion zones don't form dependably, the team will need to try other designs. Variations of the design may include more or less branches, bigger spaces between branches, or potentially a new design entirely. The next trial would utilize the filter without extraction pumping, and hopefully begin to combat the issue with air and pressure differential.

**[As someone who is not familiar with this subteam I had a really hard time understanding what the terms were, and why certain things were done. I think you guys can do a much better job at fleshing out the report, specifically at the introduction and previous work so that people who aren't as well versed can follow along better. I know that expanding it may seem self-evident, even redundant, to you but everything is neat and organized in your head, having connections between certain subjects that the audience, such as me, may not have. Overall I liked the report. Where the writing lacked, the diagrams helped me get a general idea of what was going on, but the writing could definitely improve.]**

# Manual
## ProCoDa

The ProCoDa used thus far in the semester has been limited to making sure the input and output peristaltic pumps are running at the correct velocity for their tube size. The team has not yet run an extended experiment regulated by ProCoDa.

For the peristaltic pump calculations, the states were as follows.

### States

#### OFF
The off state was used while the experiments were not run.

#### INJECT
The INJECT state used the set points *Just Water Flow* and *Water Tubing Size* to take into account the inlet flow rate in mL/s and the tubing size from inlet the peristaltic pump.

#### EXTRACT
The EXTRACT state used the set points *Outlet Flow* and *Outlet Tubing Size* to take into account the outlet flow rate in mL/s and the tubing size from the outlet peristaltic pump.

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


```Python
#This code was used for trials 1 and 2
import math
import numpy as np
import pandas as pd
from aguaclara.core.units import unit_registry as u
from aguaclara.core import pipes as pipe
from aguaclara.core import physchem as pc
from aguaclara.core import utility as ut
import aguaclara.design.floc as floc
from aguaclara.research import floc_model as fm

area = 100*u.cm**2
#area of the filter bed for simulations
areamm = area.to(u.mm**2)
backwashvelocity = 11*u.mm/u.s
filterflow = (backwashvelocity*areamm*2)/6
#filterflow is the flow rate of water coming out of each filter
print(filterflow.to(u.ml/u.s))
injectionflow = filterflow*6
#injectionflow is the rate at which the water would come through the filter (all six layers that would be in an aguaclara plant)
print(injectionflow.to(u.ml/u.s))
extractionflow = filterflow*2
#extractionflow is the flow rate at which the team will extract water from the filter because water is coming from above and below the filter
print(extractionflow.to(u.ml/u.s))

headloss = 1*u.m
Length = 1*u.m
temp = 20*u.degC
Nu = pc.viscosity_kinematic(temp)
PipeRough = 0.1*u.mm
KMinor = 2
#to find the diameter of tube for the three tubes that will come out of our filter
diamtube = chem.diam_pipe((filterflow/3), headloss, Length, Nu, PipeRough, KMinor)
print(diamtube.to(u.mm)) #inner diameter of tube we would like to come out

#The below code was revised for trial 3
v_filtration = 11 * u.mm/u.s
#this is the velocity we want to use for extraction of water during the filtration process
N_outlets = 3
#our apparatus has 3 outlet holes
lengthfilter = 10 * u.cm
#the filter has a general cross sectional area of 100
Q_outlet = (v_filtration*lengthfilter**2/N_outlets).to(u.mL/u.s)
print('The flow rate through one filter outlet is', ut.round_sf(Q_outlet,2))

tubing18 = 3.8 * u.mL/u.revolution
Maxspeed = 600 * u.revolution/u.min
Q_pump_max = (Maxspeed * tubing18).to(u.mL/u.s)
print('The max flow rate with one peristaltic pump is', ut.round_sf(Q_pump_max,2))
#What is the max flow from a peristaltic pump with #18 tubing at 600 rpm?
```
## Onshape
Link to the full design:
https://cad.onshape.com/documents/2e536bd8940f20fc75058241/w/42817f17b88f823e779070ce/e/a78ef9a6ae52e13f92aed459?configuration=Angle%3D0.3839724354387525%2Bradian%3BList_NCIYbvAAUq0uK3%3DDefault%3BNumber%3D3.0%3BRadius%3D0.012700000000000001%2Bmeter%3BSpacing%3D0.01905%2Bmeter%3BThickness%3D0.0031750000000000003%2Bmeter%3Bdepth%3D0.10160000000000001%2Bmeter%3Blength%3D0.03429000000000001%2Bmeter

## Materials List
* 4-inch PVC pipe (obtained from available lab materials)
* 3-D printed "Chrismas tree" (printed by Paul)
* Sand (obtained from available lab materials)
* Water from tap
* Peristaltic pump Tubing,size 18 (available in lab)
* Tubing used in apparatus (available lab materials)
* Peristaltic Pumps 100-600 RPM
* PVC Glue
