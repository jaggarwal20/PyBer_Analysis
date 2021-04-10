# PyBer_Analysis

## Table of Contents
- [1.0 Project Overview](#Project-Overview)
  * 1.1 Purpose
  * 1.2 Resources
 
- [2.0 Results](#Results)

- [3.0 Summary](#Summary)


<a name="Project-Overview"></a>
## Project Overview
### 1.1 Purpose
Summarize the ride sharing data for January to April 2019 by city type (urban, rurual, and suburban).

1. Create a pivot chart for each city type on a weekly basis
2. Create a line chart plotting the fares for each city type

### 1.2 Resouces
- Data Source: schools_complete.csv and students_complete.csv
- Software: Python 3.6.1, Jupyter Notebook
- Libraries: Pandas, Matplotlib

<a name="Results"></a>
## Results
* The overall summary of the fares, total drivers, and total riders using the groupby function. The total rides and drivers is higher in Urban city types. 
  
  ![alt text](Resources/summary_city_type.png)
  
* Create a pivot table displaying total fare by city type for each date from January to April 2019. 
 
  `df.pivot_table('fare', index = 'date' , columns = 'type')`
 
  `df.loc[date range]`
 
  ![alt text](Resources/pivot_table.png)
 
* Summarize the data on a weekly basis by using resample().

 ![alt text](Resources/pivot_table_weekly.png)
 
* Plot the fares vs weekly date on a line chart. 

![alt text](Resources/total_date_by_city.png)

The ride sharing shows that majority of the business is in urban city types with over 1000 rides and over 2000 drivers.  The average fare prices was less than the suburban and rural city types, but due to the amount of rides there is a higher total fares in the urban city type. The least amount of drivers and riders are in the rural city types, and this correlates with the average fare and average driver fare to be higher than the other city types.  

<a name="Summary"></a>
## Summary

The three recommendations for the CEO are: 

1. Increase the price of fares in the urban cities since the demand is higher, compared to the other city types.  This will increase profit and also allow for the drivers to have an increase in fare per ride. 
2. Reduce the number of drivers during the middle of the month as the peaks are towards the end and beginning of the month. 
3. The total fares for rural city types is overall flat, while there are fluctuations in the urban and suburban city types.  Invest more time and money in those to city types in order to draw more demand.  
