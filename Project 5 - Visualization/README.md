# (Airline On-Time Performance Data Exploration)
## by (Bui Tuan Anh)


## Dataset

> This project explores a dataset that reports flights in the United States, including carriers, departure time, arrival time and delays time along with status of cancelled, reasons for delays, cancelled, from January 2007 to December 2007.

Data source: https://community.amstat.org/jointscsg-section/dataexpo/dataexpo2009
Description about data source: https://www.transtats.bts.gov/DatabaseInfo.asp?QO_VQ=EFD&Yv0x=D

> There are 5 table, **df_flights** contain records about flights, **df_airports** contain records about airports, **df_carriers** contain records about carriers,  **df_plane_data contain** records about plane, **df_variable_descriptions** contain records about variable descriptions in the **df_flights**.

> The dataset has **7,453,215 flights** details with **29 features** all has descriptions in df_variable_descriptions. The data ranges from **Jan 1, 2007** to **December 15, 2007**.

> The variables in the df_flights contains information about flights like **date** (Year, Month, DayofMonth, DayOfWeek), **time in schedules** (CRSDepTime, CRSArrTime), **actual time** (DepTime, ArrTime), **duration** (CRSElapsedTime, ActualElapsedTime, AirTime), **origin**, **destination**, **cancellation status** (and cause of cancellation), **delay** (and cause of delay), etc.

Data wrangling:

* Some of the variables such as ArrTime and DepTime were converted from float to hh:mm datetime format.
* Some Nan value in  AirTime so I choose fill with 0 value because there are so many cancelled flights mean don't have airTime

## Summary of Findings


* Sounthwest Airlines has the highest flights (15.7%) followed by American Airlines (8.5%).
* More than 50% of flights have air time between 50 and 150 minute.
* William B Hartsfield-Atlanta Intl is busiest airport 2007
* The biggest reason for the flights to be cancelled is the Carrier causes followed by Weather causes.
* Distribution of distance is between 0 and 3000 miles.
* 2,16% of all the flight has been cancelled
* In 2007 seem most of the cancelled flight is because of Carrier, very few flights are cancelled due to security reasons.
* Saturday a little less flights than others.
* Seem Cancelled cause by Carrier is highly likely happen in Monday.
* Southwest Airlines Co is the carrier have most flight but also have the percentage of cancelled highest. After is United Air Lines Inc. 
* From top 10, Delta Air Lines Inc is the carrier with lowest percentage of cancelled flight



## Key Insights for Presentation

In the presentation Part_II_slide_deck_template.slides.html, I'm showing the analysis of cancelled flights.

> Proportion of cancelled flights
> Distribution of Cancelled flights
> Cancelled flights by Airlines