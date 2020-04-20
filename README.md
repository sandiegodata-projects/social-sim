# social-sim
A socially interaction simulation for studying infection


# Overview

The simulation has these phases:

* Generate a community and social network built from households, people and social connections
* Create a schedule for each person, where the person is, and who the person intercts with, for different times of day
* Simulate infections as people are moved thorugh their schedules. 

The source data is the Current Population Survey for 2019. The simulation selects 40,000 households, approximately 100,000 people, and allocates the households to 4 communities, each with 10,000 households. Each community is further divided into 9 neighborhoods. 

People are assigned to workgroups based on their ocupation codes, with no workgroup being larger than 100 employees. 

Some of the workgroups are restuarants, nighclubs and stores. These are also locations that will be allocated patrons. 

Head household has a head of household, and some have a spouse. 


## Scheduling


## References 

http://jameskitts.com/pubs/Demography_2009.pdf



## Data

Sarah Flood, Miriam King, Renae Rodgers, Steven Ruggles and J. Robert Warren. Integrated Public Use Microdata Series, Current Population Survey: Version 7.0 [dataset]. Minneapolis, MN: IPUMS, 2020. https://doi.org/10.18128/D030.V7.0
