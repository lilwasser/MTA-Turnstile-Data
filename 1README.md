# Metis Project Proposal I: Exploratory Data Analysis

https://data.cityofnewyork.us/Health/NYC-Condom-Availability-Program-HIV-condom-distrib/4kpn-sezh


## QUESTION/NEED:

### What is the framing question of your analysis, or the purpose of the model/system you plan to build?

Where can NYC commuters find free safer sex supplies and resources at venues located nearby the most heavily used subway stations during non-work hours (M-F: 4-8pm) between March 20 - June 20 2021?

I plan on exploring the MTA turnstile data to discover which stations have the highest foot traffic in order to help NYC  Department of Public Health identify which existing clinics garner the most foot traffic and therefore should receive additional funding to distribute safe sex supplies.

In order to prepare for safe sex supply distributions in spring 2022, I am looking at data between March 20 - June 20 2021. I am assuming that people will be more likely seek these types of supplies outside of work hours, so I am looking at MTA exits that are outside of regular working hours (time frame: 4-8pm M-F (workdays)). This will provide insights about the busiest and least busy stations. 


## DATA DESCRIPTION:

### Who benefits from exploring this question or building this model/system?

My fictitious client, NYC Department of Public Health, wants to provide more funding to the top 3 exisiting clinics that distribute free sexual health supplies and garner the most foot traffic outside of typical work hours (M-F: 7-9am, 4-7pm) based on MTA exits data.


### What dataset(s) do you plan to use, and how will you obtain the data?

MTA turnstile data  (March 20 - June 20 2021)

http://web.mta.info/developers/turnstile.html 


NYC Venues providing safe sex products and resources (March 20 - June 20 2021)

https://data.cityofnewyork.us/Health/NYC-Condom-Availability-Program-HIV-condom-distrib/4kpn-sezh

    
I plan to collect the data using SQLAlchemy and visualize with Plotly.


### What is an individual sample/unit of analysis in this project? What characteristics/features do you expect to work with?


An individual sample for the MTA dataset would include which stations have the most foot traffic (entrances and exits) during non-work hours (7-9am, 4-7pm). Units: entries, exits, date, time, station.
An individual sample for the Safe Sex dataset would include the address, borough, hours (Monday, Tues, Wed, Thurs, Fri, Sat, Sun), supplies (check T/F: condoms, FC2 (female condoms), lubricant)
### If modeling, what will you predict as your target?


I would expect to find heavier foot traffic around safe sex sites that are close to subway stations. 


## TOOLS:


### How do you intend to meet the tools requirement of the project?

I plan to do data analysis with SQLAlchemy and Pandas on the datasets. Since the data is geolocated, I would want to use a tool like geopy or plotly to visualize the data on a map. Both datasets include locations that can clearly be found on a map (lat/long, address, subway station).



### Are you planning in advance to need or use additional tools beyond those required?


Plotly. 



## MVP GOAL:

### What would a minimum viable product (MVP) look like for this project?


I will use a correlation analysis to understand the foot traffic near subway stations and use that to predict which clinics would garner the most success in providing supplies to NYC commuters, and also predict where pop-up clinics might be best located for 2022.
