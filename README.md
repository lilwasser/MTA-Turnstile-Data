# Metis Project Proposal I: Exploratory Data Analysis



## QUESTION/NEED:

### What is the framing question of your analysis, or the purpose of the model/system you plan to build?


Where can NYC commuters find seasonal flu vaccination sites that are located nearby their subway stations during non-work hours  (7-9am, 4-6pm) between Nov 1 2019 - Jan 31 2020, and how might clinics use this information to open pop-up sites to garner the most foot traffic?



## DATA DESCRIPTION:

### Who benefits from exploring this question or building this model/system?


Health clinics that want to open other pop-up clinic locations to target the most foottraffic in NYC would benefit from this question, as well as NYC residents wanting to get vaccinated outside of typical work hours (7-9am, 4-6pm).


### What dataset(s) do you plan to use, and how will you obtain the data?

MTA Turnstile Data  (Nov 1 2019 - Jan 31 2020)

http://web.mta.info/developers/turnstile.html 



NYC Locations Providing Seasonal Flu Vaccinations (Dec 2019 - Jan 2020)
(We are entering cold and flu season, in addition to contending with coronavirus)

https://data.cityofnewyork.us/Health/New-York-City-Locations-Providing-Seasonal-Flu-Vac/w9ei-idxz

    
I plan to collect the data using SQLAlchemy and visualize with Plotly.


### What is an individual sample/unit of analysis in this project? What characteristics/features do you expect to work with?


An individual sample for the MTA dataset would include which stations have the most foot traffic (entrances and exits) during non-work hours (7-9am, 4-6pm). 
An individual sample for the Flu Vaccination dataset would include the address, borough, and children (when can children get vaccinated). 


### If modeling, what will you predict as your target?


I would expect to find heavier foot traffic around flu vaccination sites that are close to subway stations. 



## TOOLS:


### How do you intend to meet the tools requirement of the project?

I plan to do data analysis with SQLAlchemy and Pandas on the datasets. Since the data is geolocated, I would want to use a tool like geopy or plotly to visualize the data on a map. Both datasets include locations that can clearly be found on a map (lat/long, address, subway station).



### Are you planning in advance to need or use additional tools beyond those required?


Plotly. 



## MVP GOAL:

### What would a minimum viable product (MVP) look like for this project?


I will use a correlation analysis to understand the foot traffic near subway stations and use that to predict which clinics would garner the most success in vaccinating NYC commuters, and also predict where pop-up clinics might be best located in time for the 2021 flu season. 
