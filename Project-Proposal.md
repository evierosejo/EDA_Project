### EDA Project Proposal

#### Question/Need:

The purpose of my project is to find the places and times that allow WTWY street teams to work most efficiently.
Optimal places are subway stations with the most foot traffic. Optimal times are the busiest days of the week and 
times of the day for those subway stations. 
Finding these subway stations will allow the street teams to: 
  1. Gather the most signatures in order to increase gala attendance, and  
  2. Spread awareness of WTWY by reaching the largest audience possible 

both in the shortest amount of time, directly benefitting the WTWY organization.


#### Data Description:
My primary source of data will be the MTA turnstile data for June, July, and August of 2021. 
These months are the most current and complete, meaning data has been collected for the entire month. 
If time allows, my secondary source of data will be the public use dataset for the 2010/2011 Regional Household Travel Survey 
collected by the New York Metropolitan Transportation Council. This data includes demographic information and travel data from 
19,000 households in NY, NJ and CT. Using this secondary source of data, I will be able to explore which subway stations are more often frequented
by residents of NYC rather than tourists, enabling an analyis of the subway stations that are frequented by people who are more likely 
able to attend WTWY's gala. 

The unit of analysis will be the subway station, "STATION" in the MTA turnstile database. 
I expect to do most of my analysis with the date, time, entry and exit data. 


#### Tools:
I plan to gather and store the data for my selected months from the raw MTA turnstile data with the get_mta.py file in SQLite, compiling it into a SQL database. 
I will then conduct SQL queries from the database into python via SQLAlchemy in a Jupyter Notebook. 
I am planning on using pandas for my exploratory data analysis, and both mathplotlib and seaborn to create visualizations in python.

#### MVP Goal:
For this project, my MVP might be a mathplotlib visualization for the top ten busiest subway stations of all MTA stations. 

