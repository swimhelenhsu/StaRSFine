##2/12/2019
#Meeting with Horizontal Filtration
HorFI is
- Testing running water through a horizontal pipe - if water running at representative velocity will the water run through it
- tesing failure velocity
- gonna have multiple shelves
- HorFI in general is working also to come up with alternative filter system for the plants
- extraction vs injection? injection
- bottom shelf is connected to the ground
- variable to control is the output velocity
- share procoda data with each other?



##2/5/2019
#calculating flow rate for filtration
* consider layers of sand: 2 - one above and one below
* deliver water into bottom, pump up, will want to pull
* two pumps: pump in at rate required, "steal" water from top
* design hole (using pipes) so that not much more than a meter of headloss between system and pumps
  - will give minimum size of tubing to handle a third of the flow



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
