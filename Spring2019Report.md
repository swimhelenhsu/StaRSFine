# StaRS FInE, Spring 2019
#### Lily Falk, Sam Hertle, and Whitney Denison
#### February 22, 2019

## Abstract
Briefly summarize your previous work, goals and objectives, what you have accomplished, and future work. (100 words max)

## Introduction
Explain how the completion of your challenge will affect AguaClara and the mission of providing safe drinking water (or sustainable wastewater treatment!). If this is a continuing team, how will your contribution build upon previous research? What needs to be further discovered or defined? If this is a new team, what prompted the inclusion of this team?

## Literature Review and Previous Work
Discuss what is already known about your research area based on both external work and that of past AguaClara Teams. Connect your objectives with what is already known and explain what additional contribution you intend to make. Make sure to add APA formatted in-text citations. If you mention the author(s) in your sentence, you can simply give the year of publication. [(Logan et. al. 1987)](http://www.jstor.org/stable/pdf/25043431.pdf?acceptTC=true)


## Methods
Explain the techniques you have used to acquire additional data and insights. Reserve fine detail for the Manual at the end of the report, but use this section to give an overview with enough detail for the reader to understand your Results and Analysis. Describe your apparatus, and have a justification for every decision you made and every parameter you chose in the design of the apparatus. Be especially careful to detail the conditions your experiments were conducted under, as this information is especially important for interpreting your results

Below, some example sections are given. Sectioning the report is meant to keep similar information together.  Continue making sections as necessary, or delete sections if you do not need them. Feel free to add subsubsections to further delineate the information. For example, under the Experimental Apparatus section below, the EStaRS team might consider having sections such as "Filter Design" and "Filter Fabrication".

### Experimental Apparatus
Explain your apparatus setup using enough detail such that future teams can recreate your apparatus. Make sure to explain why you built it this way. Create a schematic drawing of the apparatus (not a photo) that has clearly labeled components, flow paths, sensors, and reactor geometry.

* Design (calculations, constraints):
  * Use LaTeX to format equations in line ($\frac{-b\pm\sqrt{b^2-4ac}}{2a}$) or centered:

  \[\frac{-b\pm\sqrt{b^2-4ac}}{2a}\]

* Schematic (label parts)
  <p align="center">
    <img src="/Images/Example Schematic.png" height=300>
  </p>

  <p align="center">
    Figure 1. Above is an example schematic drawing of the Summer 2018 High Rate Sedimentation apparatus. It is labeled with components, flow paths, sensors, and reactor geometry.
  </p>

* Image (from lab, label parts)
  <p align="center">
    <img src="/Images/Example Lab Image.JPG" height=300>
  </p>
  <p align="center">
    Figure 2. Any photos taken in the lab should be clearly labeled and captioned as well.
  </p>

* Materials (manufacturer, dimensions, and other specifications)
* Complications in construction
* If already constructed: write a brief summary of important constraints, include any revisions to apparatus, also reference the prior report where construction is described

### Procedure- dont do yet
Discuss your experimental procedure. How did you run your experiment? What were you testing? What were the values of relevant parameters?

## Results and Analysis- dont do yet
Present an observation (results), then explain what happened (analysis).  Each paragraph should focus on one aspect of your results. In that same paragraph, you should interpret that result.
In other words, there should not be two distinct paragraphs, but instead one paragraph containing one result and the interpretation and analysis of this result. Here are some guiding questions for results and analysis:

When describing your results, present your data, using the guidelines below:
* What happened? What did you find?
* Show your experimental data in a professional way.

```python
import aguaclara.research.procoda_parser as pp
import matplotlib.pyplot as plt
import numpy as np

time, influent_turbidity, effluent_turbidity = pp.get_data_by_time(
      path="Data", columns=[0, 3, 4], start_date="6-14-2018",
      start_time="15:40", end_time="23:30")
elapsed_time = (np.array(time)-time[0])*24

fig, ax1 = plt.subplots()
ax1.set_xlabel("Time (hours)")
ax1.set_ylabel("Effluent Turbidity (NTU)")
line1, = ax1.plot(elapsed_time, effluent_turbidity, color="blue")

ax2 = ax1.twinx()
ax2.set_ylabel("Influent Turbidity (NTU)")
ax2.set_ylim(60,120)
line2, = ax2.plot(elapsed_time, influent_turbidity, color="green")

plt.legend((line1, line2), ("Effluent", "Influent"))
plt.savefig("Turbidity.png")
```
<p align="center">
  <img src="/Images/Turbidity.png">
</p>
<p align="center">
  Figure 3. Descriptive captions are very important for figures. Rather than including a title above your figure, write a caption below.
</p>

### Figure requirements
 - Create the graph using python (not Excel)
 - If the x axis is time then make zero time reflect the beginning of the test.
 - Use a white background for all graphs.
 - Most data will have both x and y values and thus should be presented using an xy scatter plot.
 - Label all axes and include units where appropriate.
 - Axis scale labels should be in the margin of the graph and not inside the graph border.
 - Eliminate parts of the range in both x and y axis that aren't used or that aren't meaningful.
 - Place a caption with a brief description below the graph. Add this caption using the wiki formatting, not in your graphing software.
 - Use data symbols to show data points unless there is so much data that the symbols overlap. If the data symbols overlap it is better to connect the data points with a line and not show the data symbols.
 - When presenting multiple plots on a single graph make sure that it is easy to distinguish the plots using the legend.
 - If curve fitting is used explain why and include the equation (elsewhere in the report).
 - If a model or theoretical curve is presented it should be a smooth curve without data points.
 - Use the same font in the graphs as you use in the text of the report.
 - Insert the graph in your report after the first reference to it in the text. Inserted the graph after the next paragraph break
 - Scale the size of the graph so it is large enough to see the data and read the text without having to follow a link to see a larger image. Avoid using hyperlinks on images because that causes the export to Microsoft Word option to not include the image.

After describing a particular result, within a paragraph, go on to connect your work to fundamental physics/chemistry/statics/fluid mechanics, or whatever field is appropriate. Analyze your results and compare with theoretical expectations; or, if you have not yet done the experiments, describe your expectations based on established knowledge. Include implications of your results. How will your results influence the design of AguaClara plants? If possible provide clear recommendations for design changes that should be adopted. Show your experimental data in a professional way using the following guidelines:
* Why did you get those results/data?
* Did these results line up with expectations?
* What went wrong?
* If the data do not support your hypothesis, is there another hypothesis that describes your new data?

## Conclusions
Explain what you have learned and how that influences your next steps. Why does what you discovered matter to AguaClara?

Make sure that you defend your conclusions with facts and results.

## Future Work
Describe your plan of action for the next several weeks of research. Detail the next steps for this team. How can AguaClara use what you discovered for future projects? Your suggestions for challenges for future teams are most welcome. Should research in this area continue?

## Bibliography
Logan, B. E., Hermanowicz, S. W., & Parker,A. S. (1987). A Fundamental Model for Trickling Filter Process Design. Journal (Water Pollution Control Federation), 59(12), 1029–1042.

# Manual
The goal of this section is to provide all of the guidance that would be necessary for a future team to pick up your work where the team left off.

## Fabrication Details
The current apparatus design was revisited. The team noted the small outlet pipe size, and did the below calculation to determine that minimum pipe diameter was not met.

| Respective Flow Rate      | Minimum Tube Inner Diameter  |
|---------------------------|-----------------------|---|---|---|
| 36.67 milliliter / second | 3.762 millimeter      |

Shaving the glue from the previous tubes, the team detached the tubes. Using the new calculated inner diameter, the team found tubing that matched met the minimum standard and considered how it would affect the design of the 3D printed pine-tree filter which was already fit to the prototype PVC tube by holes drilled. In the OnShape drawing, the team determined that, if the filter was taken from the prototype, respective sized holes could be drilled with the drill press. The holes were designed to be offset from the original holes while still remaining in the bounds of the upper and lower wings. Holes were drilled to match these on the 4-Inch PVC prototype.
## Experimental Checklist
Before running the experiments, the team ensured that the prototype was water tight, in order to collect accurate data regarding the flow rates of injection and extraction.
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
