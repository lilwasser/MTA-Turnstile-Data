# Metis Project Proposal I: Exploratory Data Analysis

## ABSTRACT:

The goal of this project was to provide insight into the relationship between Metropolitan Transportation Authority (MTA) turnstile activity, specifically its most heavily foot-trafficked stations, and the locations of sexual health clinics in New York. 

To reduce statistical noise and maximize the chances that resources would get used, I focused on MTA traffic after work hours, between 4pm - 8pm, and months that would best equip my client for Spring 2022 traffic trends, so March-June 2021 data.


I developed graphs using matplotlib to best visualize which stations had the most traffic in terms of daily average, overall traffic to best assess which nearby clinics to provide extra funding to. I also analyzed trends in traffic over the course of the chosen Spring time period, which informs my client when to anticipate fluxes in traffic in order to readily stock up on supplies. 


## DESIGN:

### above: The clearly defined client backstory is exceptionally creative and involved, and is addressed in a highly proficient manner.

My client, NYC Department of Health and Mental Hygiene (NYC DOHMH), offers free sexual health services and supplies through their NYC Condom Availability Program. Products are distributed at local businesses, community-based organizations, and health care facilities. The Program gives away more than 30 million free safer sex products every year to over 3,500 locations and across all five boroughs. In anticipation for Spring 2022, my client wants to know which MTA stations garner the most foot traffic outside of typical working hours (4pm - 8pm) and thus 

I plan on exploring the MTA turnstile data to discover which stations have the highest foot traffic in order to help NYC  Department of Public Health identify which existing clinics garner the most foot traffic and therefore should receive additional funding to distribute safe sex supplies. I will look at the top 3 busiest stations and then use location data to see which clinics in those surrounding areas should receive more funding.

In order to prepare for safe sex supply distributions in spring 2022, I am looking at data between March 20 - June 20 2021. I am assuming that people will be more likely seek these types of supplies outside of work hours, so I am looking at MTA exits that are outside of regular working hours (time frame: 4-8pm M-F (workdays)). This will provide insights about the busiest and least busy stations. 

## DATA:

* MTA turnstile data  (March - June 2021)

    * http://web.mta.info/developers/turnstile.html 


* NYC Venues providing safe sex products and resources

    * https://data.cityofnewyork.us/Health/NYC-Condom-Availability-Program-HIV-condom-distrib/4kpn-sezh

## ALGORITHMS:

### Satisfactory: Exploratory data analysis and visualization techniques are effectively used to clean, aggregate, and visualize the data. Patterns and insights obtainable from the data are interpreted correctly.

_*Data Cleaning*_

** In some cases, the turnstiles were being counted in reverse, which led to inaccurate calculations in regards to entry and exit data. I cleaned up these errors early on in data analysis.
** There were some outrageous numbers when it came to entry and exit data for a given turnstile. Even in one of the biggest cities in the world, it would be impossible for a single turnstile in New York to see 1 million entries in a given day. I created limits on these counters to account for outliers in the data.
** I used a function to identify reverse counting, resets, and extra large numbers in the cumulative count for a turnstile.
** I removed all turnstile records that were not reported between the hours of 4 pm to 8 pm.


_*Analysis*_

** I aggregated entry and exit data to create analysis on total station traffic using "merge" function in Pandas.


## TOOLS:

** Python
** SQLAlchemy
** Matplotlib
** Pandas
** Numpy
** SQLite
** Geocode
** Geopy


## COMMUNICATION
### Above: Presentation has exceptional delivery, extremely clear structure, compelling in narrative and selection/construction of visualizations throughout. Slides are beautiful in style and design, carefully curated to draw attention to key information and complement the verbal delivery.

I will present my analysis using Google Sheets.

add a pic here!

My high-level analysis will be presented in a slideshow using visualization created with Matplotlib and Seaborn. The set of Tableau dashboards I created for further analysis can be found here.

Note that there are three dashboards worth exploring. This link takes you to the first dashboard, the Traffic Heatmap. Scroll to the bottom of the screen and click on "Station Comparison" and "Time Series" to explore further. You can also download the workbook and view it in the Tableau Public desktop app.



