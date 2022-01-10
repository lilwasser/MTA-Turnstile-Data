#### Minimum Viable Product (MVP) Template


I will be examining 3 months of MTA turnstile data and a dataset from NYC OpenData on HIV condom distribution locations. My primary goal is to look at the highest traffic stations, day of week, and times. The timeframe in the datasets I am looking at is between March 20 - June 20 2021 in order to prepare for safe sex supply distributions in Spring 2022. I am assuming that people will be more likely seek these types of supplies outside of work hours, so I am looking at MTA exits that are between 4-8pm M-F (workdays). This will provide insights about the busiest and least busy stations during this time.


I plan on exploring the MTA turnstile data to discover which stations have the highest foot traffic in order to help NYC Department of Public Health identify which existing clinics garner the most foot traffic and therefore should receive additional funding to distribute safe sex supplies. I will use location data to better inform NYC Department of Public Health of the most heavily trafficked stations during the week and the clinics nearby those busy stations to ensure that resources are getting distributed to the most people.

The MVP will be a jupyter notebook containing a bar chart showing which are the top 3 stations in terms of heaviest foot traffic during the week, and then a bar chart that breaks that data down by days of the week during a given time span. This will provide a simple answer to the question of which clinics should receive more funding because I can use location data to plot the clinics around those 3 stations.

I will perform this exploratory data analysis using SQLite and Python's Pandas package, and interpret it throguh Seaborn and Matplotlib packages to create visualizations.<img width="570" alt="Screen Shot 2022-01-10 at 5 13 02 PM" src="https://user-images.githubusercontent.com/89549841/148852771-e452066d-c7c1-44fe-b2cf-744861a21aea.png">
