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

*INSERT TABLE*

*INSERT COMMENT*

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
Urban cities clearly see the most traffic and the highest associated fees. The results generated in the summary DataFrame could be due to Urban city types being more centralized, yielding a lower average fare per ride, while Rural city types are more spread out, which would collect a higher average fare per ride but lower total revenues. One interesting way to test this hypothesis would be to have PyBer work to include mileage distance data as part of the data collection process and analysis.

Because there are more total drivers than total rides in the Urban city types, Urban drivers may not have enough work to support themselves. PyBer may want to consider investing advertising dollars in the Urban city types to increase the total rides or risk losing Urban drivers.

One solution could be to invest in the exsiting driver base. If PyBer were to invest into advertising dollars in the Urban city type, the next question is when would ads be the most effective? After reviewing the Total Fare by City Tpye graph, the end of February kicks off the increase in total fares and would be a good time to launch an advertising campaign, which would also strategically help the other two city types.

There is a matching peak in third week in February for each city type. Based on this information I would suggest to research this peak in more detail that can help determine what caused the jump. Therefore, the analsis can be used as a business strategy in the future. For example, if the total amount of fares were increased due to certain event, PyBer could use future events for promotion of their services.

Urban cities have the highest ride and driver count and the lowest average fare per driver, that is $16.57. I would suggest deeper research on this area by finding out what is the employee satisfaction rate and the company profit on this number (total fare amount is $39,854.38). If employee rate is high and PyBer is profitable, that would indicate a good bussiness strategy for urban cities. In addition, I would suggest to take a closer look into the peaks and dips that appear from late February to early April in order to find out what is causing them. This could reveal important information for future business planning.

