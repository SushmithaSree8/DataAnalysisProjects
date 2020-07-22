# FordGoBike/BayWheels System Data
## by Sushmitha Sree Gumireddy


## Dataset

FordGoBike (later BayWheels) is a Bay Area bike sharing system. In this project, the trip data of FordGoBike from 2018 to 2019 will be explored. The data is available on 'https://s3.amazonaws.com/baywheels-data/index.html'. After wrangling the final cleaned dataset has 4370704 trip data with 18 features. The features of interest in the project are  demand for bikes (i.e number of bike trips), the duration of the trip, the weekday, month, year of the trip, user type, bike_share_for_all_trip and rental_access_method.


## Summary of Findings

From the univariate exploration, it was found that distribution was right skewed with wide range of data. The log transformation was similar to normal distribution. Additionally it was observed that the number of trips increased from 2018 to 2019. More number of trips were taken on weekdays than on weekends, using app than clipper, by subscriber than customer and for not all bike trip than all bike trip.

The bivariate exploration was conducted to observe the relation between each set of features. It was found that there is higher probability for longer trips on weekends than on weekdays. Moreover customers tend to take longer trips than subscribers. Another interesting observation was that though the number of trips made by subscriber user type decreased on weekends, the number of trips made by customer user type increased or stayed constant. In the data none of the customers took an all bike trip.

The findings from multivariate exploration are:
1. The mean duration of customer user type is higher than subscriber on each day as expected from bivariate plots. It is interesting however that the mean duration of subscribers remains almost constant while that for customers increases on weekend.

2. From the bivariate plots, it was seen that bike share for entire trip had slightly lower duration than trips not using bike share for entire trip. However when interated with weekend dummy variable, it was seen the difference is greater on weekends than on weekdays


## Key Insights for Presentation

The key insights that will be presented are:
1. The distribution of duration is right skewed with majority of values in range 100 to 3000 seconds
2. The number of trips taken on weekdays is greater than on weekends
3. The number of trips taken by subscribers is greater than by customers
4. Interaction between weekday, user type and duration: The mean duration of customer user type is higher than subscriber on each day of week.Moreover although the mean duration of subscribers remains almost constant, that for customers increases on weekend
5. Interaction between weekday, bike_share_for_all_trip and duration: Trips without bike share for entire trip had greater duration than trips without bike share for entire trip on both weekdays and weekends. However the difference is more pronounced on weekends than on weekdays
For the slide deck, the plots are improved aesthetically by using appropriate title and labels.