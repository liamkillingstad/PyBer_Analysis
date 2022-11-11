# PyBer Analysis
*Matplotlib Analysis for PyBer Ride-Share company*

## Project Overview 
### Purpose

The purpose of the analysis was to leverage data from the rideshare company "PyBer" pertaining to various aspects of its business model. 

The analysis performed is based on data obtained in the form of a CSV file provided from PyBer. This data has been processed using Python's Pandas to produce a summary dataframe as well as a chart generated using the information in the dataframe to visualize and contextualize the data. 

The analysis performed demonstrates the relationship between variables including the type of the city, the correlation between rides, and drivers and their resepctive fares. The specific tasks and insights that were generated included the following: 

-	The total number of rides by city type. 
-	The total number of drivers by city type.
-	The sum of the fares by city type.
-	The average fare per ride by city type.
-	The average fare per driver by city type.
-	The total fares for each week by city type. 

Categorically, data needed to be cleaned and organized so that we could ultimately produce visual outputs for context and analysis.

### Overview of Methods
The analysis wsas run using Matplotlib. Matplotlib is a Python graphing library and offers statistical graphical representations of the data collected. The library allows the user to manipulate the graphical representations as well and provide richer representations of data. 

Matplotlib has two main graphing methods: 

- Pandas MATLAB and,
- The object-oriented method. 

MATLAB plotting is used for quick and simple plots that require little coding, while the object-oriented method is used for more complex graphs, including those with multiple plots on the same graph and require more coding and interpretation.

MATLAB and the object-oriented method are both extremely useful when it comes to exploratory data analysis ("EDA"). Leveraging EDA at the beginning of a project (particularly with visual representations) can assist in prvoding a targeted plan for how to handle dastasets. Inspecting data quality such as missing values, duplicates, and outliers is an important first step in the analysis process and is required in producing acurate and substantive final analysis.

### Resources
This analysis was performed with the follwoing tools and files:

Related Files:
- [city_data.csv](Resources/city_data.csv)
- [ride_data.csv](Resources/ride_data.csv)

Environment:
- Version 3.9.12

Software:
- Jupyter Notebook 4.11.1


## Results 
From the table *The Summary Data Frame per City Type* we can see the results of the analysis and how city type (rural, urban, or suburban) impacted the the total amount of rides, drivers and fares from January to early May of 2019.

<p align="center">     
<img src=https://github.com/liamkillingstad/PyBer_Analysis/blob/main/PyBear_Chart.png>

*Total Fare by City Type*
From the summary DataFrame, the data was pivoted into a new DataFrame, and then grouped by weeks to show the total fares by city type.

<p align="center">     
<img src=https://github.com/liamkillingstad/PyBer_Analysis/blob/main/Resources/PyBer_fare_summary.png>
</p>

*Some initial observations:*

- All three city types start to rise to a peak at the end for February. For the Urban city type, that oscillating peak lasts through April, while the other city types wane in the month of March.
- The Rural city type increases again leading into the month of April. The Suburban city type starts to peak again at the end of April, while the Rural city type drops off.
- For the total number of drivers, the disparity between urban and suburban cities is ~5x higher for urban and ~31x higher for urban versus rural cities. 
- The total number of rides for urban versus rural cities was ~13x higher while the difference between urban and suburban was only ~2x. 
- Urban cities have the highest total fares ranging from $1,600 per week to $2,500 per week.
- Rural cities have the lowest total fares ranging from $250 per week to $500 per week.
- All cities have pretty steady flow of total fares from week to week with a matching spike in the third week in February.

Overall, there seem to be significant disparaties between the amount and fee strcuture for riders in rural versus urban areas. When it comes to the differences between suburban and rural and suburban and urban areas, however, there seems to be a relatively constant "magnitude" of difference between the various tracked variables (i.e. number of rides, number or drivers, and fares).

## Summary & Recommendation
Urban cities clearly see the most traffic and the highest associated fees. But why?

There are several potential reasons for the disparaties. The results that were generated in the summary DataFrame could be due to Urban city types being more centralized, yielding a lower average fare per ride, while Rural city types are more spread out, which would collect a higher average fare per ride but lower total revenues (due to less total rides). One interesting way to test this hypothesis would be to have PyBer work to include mileage distance data as part of the data collection process and analysis.

Because there are more total drivers than total rides in the Urban city types, Urban drivers may not have enough work to support themselves -- an imbalance between supply and demand. In order to combat the fractured masrket, PyBer could consider investing advertising dollars in the Urban city types to increase the total rides or risk losing Urban drivers. Another idea would be to include a referal program to increase the total rider base. 

If PyBer were to invest in advertising or referral programs in the Urban cities, a subsequent question would be what type of ads would be the most effective and when to run them. After reviewing the Total Fare by City Tpye graph, the end of February kicks off the increase in total fares and would be a good time to launch an advertising or refferal campaign. The idea of referral and adverstising campaigns could be equally beneficial to all city types.

While we have identifed the spike in rides in the third week of Februrary, we do not have a good indication for why this is the case. Based on this information, I would suggest researching this specific spike in activity particularly if we plan to build an advertising strategy around that time period. If the reason for the increased traffic is systemic and/or repeatable, it might be prudent to structure certain events, promotions, or deals around that specific event.

Lastly, Urban cities have the highest ride and driver count and the lowest average fare per driver. I would suggest deeper research to determine if there was a quick fix to generating higher revenues per ride. A way to determine this would be through customer satisfaction ratings and driver ratings. If an  employee rate is high there is likely an ability to charge higher prices and increase total revenue.
