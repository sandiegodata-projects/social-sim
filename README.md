# social-sim
A socially interaction simulation for studying infection


# Overview

Input to the simulator consists of:

* A list of people, organized into households
* A set of locations where people go, such as home, work, school or shopping. 
* Weekly schedules for each person, with two variants:
** A typical schedule that the person will follow without restriction
** A restricted scheudle that accounts for policy changes, such as closing workplaces or social distancing. 

The simulator runs by placing each person into a location according to the person's schedule and then solves a compartmental infection model to adjust the state of each person. 

# Implementation

It may be sufficient to run the simulation with a timestep of 1 hour, rather than actually solving the system of ODEs for each location. Assuming that there is random mixing at each location, each person has a probability to be infected based on the number of infected people at the location and the susceptability of the person. 

# Data

The source data is the Current Population Survey for 2019. The simulation selects 40,000 households, approximately 100,000 people, and allocates the households to 4 communities, each with 10,000 households. Each community is further divided into 9 neighborhoods. 

People are assigned to workgroups based on their ocupation codes, with no workgroup being larger than 100 employees. 

Some of the workgroups are restuarants, nighclubs and stores. These are also locations that will be allocated patrons. 

Head household has a head of household, and some have a spouse. 

## Components






## Friends Network

Gallup has a [poll on the number of friends pepople have](https://news.gallup.com/poll/10891/americans-satisfied-number-friends-closeness-friendships.aspx).


## Scheduling


## References 

http://jameskitts.com/pubs/Demography_2009.pdf



## Data

Sarah Flood, Miriam King, Renae Rodgers, Steven Ruggles and J. Robert Warren. Integrated Public Use Microdata Series, Current Population Survey: Version 7.0 [dataset]. Minneapolis, MN: IPUMS, 2020. https://doi.org/10.18128/D030.V7.0
