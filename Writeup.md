# Optimizing WTWY Street Team Work 
Evelyn Johnson

## Abstract
The goal of this project was to assist WTWY in optimizing the canvassing work of their street teams. In order to accomplish this, I worked with New York City turnstile
entry and exit data provided by the Metropolitan Transportation Authority (MTA) to find the busiest subway stations and the days of the week with the 
most foot traffic for those stations. After the data was cleaned and compiled into the appropriate dataframes, I created visualizations to communicate my results
using Seaborn. 

## Design
The project was centered around WTWY's directive to optimize the work of their street teams, thereby, attaining the most signatures from those who will 
recieve a free ticket to their gala and increasing the gala's attendance.  Determining the busiest stations and days of the week would enable WTWY to 
deploy their street teams to places where they will have the largest audience and the widest reach.

## Data
The dataset contains entry and exit register values for each turnstile in every subway station for three months from 00:00:00 on 05/29/2021 to 23:59:56 on 08/27/2021. 
A single turnstile is designated by a unique combination of values for C/A, Unit, and SCP. Each turnstile receives six audits per day, normally every four hours. 
The dataset contains information from 2,722,581 audits with 11 features. 

## Algorithms
Data Cleaning Phases:
1. Dropping duplicates with the same C/A, UNIT, SCP, DATE and TIME values
2. Dropping columns not pertinent to the project, specifically, DIVISION and DESC
3. Converting DATE and TIME columns to a single column with a datetime datatype
4. Converting entry and exit data from cumulative values for a device to the value over the course of one day 
5. Assigning outliers for daily entries and exits per device greater than 10,000 to 0 

After the data was cleaned, the turnstile data was organized by individual turnstile and by station. The top ten busiest stations were found 
by daily entries and by daily exits. Using the results of the busiest stations by entry data, the total entries per day of the week were found for each station
using the individual turnstile data for three months.

## Tools
* Sqlite3 for data acquisition
* SQLAlchemy for data retrieval and exploration
* Pandas for data manipulation
* Matplotlib and Seaborn for plotting and visualizations

## Communication
Along with this writeup, I have created a presentation detailing the methodology and results of this project. 


![ten_busiest_stations](https://user-images.githubusercontent.com/84474016/133800265-93f305c2-28df-4bdf-a98a-0e8eae961da4.png)

![ten_busiest_stations_exits](https://user-images.githubusercontent.com/84474016/133800282-46fa46d5-02a2-4f1a-b78c-64e83a85c910.png)

![stations_by_weekday](https://user-images.githubusercontent.com/84474016/133800299-9a8601f6-6124-40a1-974f-ab9ea97be9e4.png)

