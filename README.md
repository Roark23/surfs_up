# surfs_up
## Purpose
We're consulting a Surf'n'Shake shop to help determine where we should put a location and if one is even viable in Oahu. To ensure that we will choose the best location, we need to make some data-driven decisions. This analysis focuses on the temperature and rainfall for the past 7 years from 2010 to 2017, specifically for June and December. These two months are far enough apart to ensure that we have a good condition year-round. To gather enough data, I am analyzing data from six weather stations in Oahu, Hawaii. The analysis will analyze temperaturefor June and December from 2010 to 2017 as well as rainfall for June and December from 2010 to 2017.

## Results
It was crucial to sample data from different months of the year to determine if there were vast variations in the results. Specifically, the temperature data was sampled for the months of June and December in Oahu, Hawaii, to determine if the surf and ice cream shop business would be sustainable year-round.

By utilizing Python, Pandas functions and methods, and SQLAlchemy, the date column was filtered from the Measurements table in the hawaii.sqlite database in order to retrieve all the temperatures for the month of June and December. After gathering this data, I converted the temperatures into a list and then created a DataFrame from the list> Finally, we could generate summary statistics to understand the results.

### June vs. December Temperature Results

June Summary Statistics:

![June_Summary_Statistics](/Resources/June_temp.png)

December Summary Statistics:

![December_Summary_Statistics](/Resources/Dec_temp.png)

We can use this to better understand if a Surf'n'Shake shop is viable year round in Oahu. These results indicate key differences in weather between June and December:

1. Key Differences

- There are more data points capturing temperature in June (1574 data points) versus December (1405 data points).

- The lowest temperature is marked with an 8-degree difference (June: 64F, December: 56F), but the high temperature is marked with a 2-degree difference (June: 85F, December: 83F).

2. Dispersion of the data

- The average temperature in June is 74.9 and in December is 71.0, showing little variance.

- Rainfall quantity is more spread out in December (std = 0.5) than in June (std = 0.33).

- June’s mean and median are 0.13 inches and 0.02 inches respectively.

- December’s mean and median are 0.21 inches and 0.03 inches respectively.

- Maximum rainfall in December is 6.42 inches and 4.43 inches in June.

- Minimum rainfall in December is 0 inches and 0 inches in June.

## Summary
As we can see from the data results, the temperature does change throughout the year but maybe not as much as one anticipated. There is potential for a Surf'n'Shake shop to be open year round and be successful. A major impact on the success of the shop will be determined by how much precipitation there is. 

### Precipitation Factor
The shop obviously will not be as successsful during rainy days. By creating a few additional queries, I was  able to gather data relevant to the precipitation in Oahu during June and December:

![June_Precipitation](/Resources/June_precipitation.png)

![December_Precipitation](/Resources/Dec_precipitation.png)

While there are more days of rain in June, December experiences the heaviest amount of rain. However, the precipiation levels are congruent with other successful surf'n'shake shops. This further analysis supports starting a shop as the precipitation levels are not too high to impact whether the Surf'n'Shake shop will be successful year round.

### Temperature Factor

![Temperature_vs_Frequency](/Resources/Temperature_vs_Frequency.png)

I created a histogram to plot the underlying frequency distribution of the various temperature observations. Through recording temperatures, throughout the year, at the most active weather station, we can see temperatures ranging from 75F – 77F occured the most frequent. 

### Conculsion
This weather is still optimal for the Surf'n'Shake shop and would further support the notion of opening up a shop year round. While the precipiatation is a factor that would hurt business, the data gathered shows evidence that there is not an excess amount of precipitation that would take away from the success of the Surf'n'Shake shop. 
