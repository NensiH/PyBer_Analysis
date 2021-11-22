# PyBer_Analysis
Ride-sharing app company 'PyBer' needed ride-sharing data analyzed from January 2019-May 2019 to show total rides, total drivers, total fares, average fare per ride, average fare per driver, and total weekly fares for each city type. In this project I'll be helping out Omar(manager of Pyber) to analyze all the rideshare data.

## Overview 
The purpose of our analysis is to create a summary data frame that will show ride sharing data by city type. Data from urban, suburban, and rural cities was provided. Using Python libraries 'Pandas' and 'Matplotlib', a summary chart for each city type's totals and averages was produced. Once we find our data we are going to create a multiple line graph that shows total weekly fares by each city type and our last section was to create visualization of the data in the form of line chart for CEO V.Isualize. This analysis will summarize how data differs by city type and how those differences can be leveraged by senior leadership at PyBer.

## Resources

- **Data**

    - [city_data.csv](Resources/city_data.csv)

    - [ride_data.csv](Resources/ride_data.csv)

- **Software**

    - Jupyter Notebook
    - Python version 3.7
    (matplotlib.pyplot and pandas library)

## Results

PyBer ride-sharing data was combined from [city_data.csv](Resources/city_data.csv) and [ride_data.csv](Resources/ride_data.csv) in order to produce a summary of Total Ride, Total Drivers, Total Fares, Average Fare per Ride, and Average Fare per Driver. After cleaning & formatting the dataframe it looks like :

<img width="610" alt="Screen Shot 2021-11-22 at 3 50 02 PM" src="https://user-images.githubusercontent.com/92277581/142940831-8b2c86c6-26b8-427c-906a-b13e22102c88.png">

Further in analysis we used our Pandas skills and also used two new functions, pivot() and resample() to create a multiple-line graph that showed the total fares for each week by city type. After resetting the index we created the Pivot table by using pivot function which resulted as below:

<img width="297" alt="Screen Shot 2021-11-21 at 1 22 34 PM" src="https://user-images.githubusercontent.com/92277581/142941342-10a55263-97e1-40ac-8272-e3dbd077eafd.png">

Next step is to Resample the data in weekly bins to get the total fares for each week. For resampling, first we have to set the "date" index to datetime datatype. So following is the results of both changing the datatype of date column and resample the data to see total fares for each week:


<img width="271" alt="Screen Shot 2021-11-21 at 12 10 26 PM" src="https://user-images.githubusercontent.com/92277581/142942165-e3ed74a0-5ab6-410e-96df-41bc042c65ee.png">


Last step is, A multiple line chart displaying total fares for urban, suburban, and rural city types for each week between January 1, 2019 and April 29, 2019 was created: 

<img width="704" alt="Screen Shot 2021-11-21 at 12 11 42 PM" src="https://user-images.githubusercontent.com/92277581/142942506-0a92b0a5-d15b-4725-8e31-2983a02e6304.png">

Overall, PyBer ride sharing services significantly differs in rural, suruban, and urban cities given the number of rides, drivers, and fares. Data supports that there is higher usage of PyBer ridesharing services in urban cities.

## Summary

Looking at Pyber summary dataframe as shown in above section, it is noticed that Rural has very less drivers as compared to Suburban and urban cities. So Urban cities have 4x+ more drivers than suburban cities. Suburban cities have 6x + more drivers than rural with almost 4.5x the revenue. The average fare per driver is way too high for Rural compared to Urban. In conclusion, we can effectively say that a rural area will command a higher fare because there are fewer workers that will come to this area, the travel time and distance is most likely longer making the average fare per ride & driver the most out of all city types.
Based on this analysis, my business recommendations to Pyber are: Increasing the amount of drivers in Rural areas to ensure there are enough drivers to meet ride demand. 


