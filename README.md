# PyBer_Analysis

### Overview
As a Data Analyst for PyBer, a Python-based ride sharing app company, I have been tasked with completing exploratory analysis on a large set of ride-sharing data collected in early 2019.  This analysis will be presented to the company's CEO, V. Isualize, and will inform decisions about improving access to underserved neighborhoods.  I will develop numerous visualizations to better articulate key points of my analysis.

### Results 
#### More Drivers and Rides Results in Lower, More Consistent Fares 
Comparing the key inputs - drivers, rides, and fares by city type - shows that a larger number of drivers and rides correlates with lower, more consistent fares.  Visualizing the summary data in a bubble chart shows that fares Urban city types are more clustered around lower average fares (average fare per ride = $24.53, Standard Deviation = $11.73) than in Rural city types (average fare per ride = $34.62, Standard Deviation = $14.56).  Driver counts in Urban areas are significantly higher than in Rural areas - 1,625 compared to only 125 - which is illustrated by the bubble sizes.

![pyber_ride_sharing_data](https://github.com/benclark62/PyBer_Analysis/blob/main/analysis/Fig1.png) 

The discrepancy between average fares by city type are much more pronounced when viewing per Driver averages instead of per Ride averages.  Urban average fares per ride are 29.1% lower than Rural average fares per ride ($24.53 vs $34.62), but Urban average fares per driver are 70.1% lower than the same measure in Rural areas ($16.57 vs $55.49).  This implies that the supply of drivers meets the demand in Urban areas and can create downward pressure on average fares.  In fact, the count of drivers in Urban areas exceeds the total rides where Rural and Suburan areas both have a Rides : Driver ratio > 1.

![pyber_summary_dataframe](https://github.com/benclark62/PyBer_Analysis/blob/main/analysis/pyber_summary_df.png)

For PyBer, addressing underserved neighborhoods will be a win-win for the company and its customers.  Lower driver counts result in higher average fares, potentially making rides cost-prohibitive for rural customers.  Increasing driver count and forcing average fare down will grow the customer base and ultimately increase revenues for PyBer.  The summary line chart illustrates that despite significantly lower average fares, the Urban city types are driving the vast majority of fares for PyBer - more than twice what is delivered by Suburban and almost ten times Rural fares. 

![pyber_summary_dataframe](https://github.com/benclark62/PyBer_Analysis/blob/main/analysis/PyBer_fare_summary.png)

### Summary
#### How to begin addressing disparities in ride availability
Based on this analysis, I would recommend the following steps to begin addressing ride availability among city types:

- **Launch incentive program to increase driver count in rural areas**.  Availability of drivers appears to be the primary contributor in pushing average fares down, which will increase customers' likelihood to use PyBer.
-**Investigate alternative driver 'uses' in Rural areas**.  Demand for ride sharing in Rural areas may be different than that in an Urban setting.  This could be linked to numerous factors - more tourists in Urban areas, higher car ownership rates in Rural areas, etc. - but the fundamental demand for ride sharing is likely different.  A team should be commissioned to identify new services that could be offered by PyBer drivers in Rural areas that have not been explored yet. 
- **Reevaluate pricing structures**. Understanding that fares will be impacted by factors unique to each city type - namely trip distance - I recommend evaluating a pricing structure that varies by city type.  If the per mile or per minute rate is consistent across all city types, Rural customers will be charged more and less likely to use this service. 
- **Conduct deep dive into driver and trip financial metrics**.  Further analysis will help understand our profitability per driver and per trip.  This will better inform decisions about incentives, long-term growth, and potential for alternative monetization of Rural drivers.
