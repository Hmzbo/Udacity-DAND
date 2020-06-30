# Ford GoBike System Data Exploration
## by Hamza Boulahia


## Dataset

The Ford GoBike System data is a dataset providing informations about the trips made in this system from 2017 to 2019. This bike sharing system is located in the greater San Francisco Bay area which cover three regions San Francisco, East Bay, and San Jose.
Each row in this data represent a trip made within the Ford GoBike System, and each column represent a variable describing one aspect of the trip, we have initially a total of 13 columns labeled as follows:
- Trip Duration (seconds)
- Start Time and Date
- End Time and Date
- Start Station ID
- Start Station Name
- Start Station Latitude
- Start Station Longitude
- End Station ID
- End Station Name
- End Station Latitude
- End Station Longitude
- Bike ID
- User Type (Subscriber or Customer – “Subscriber” = Member or “Customer” = Casual)

The dataset has 4,890,404 records.

Wrangling Notes: 
1- For both years 2018, 2019, the data provided by Lyft includes two additional columns; Bike_share_for_all_trip, and Rental_access_method. Those two column are dropped from the master dataset along with the longitude/latitude columns and the bike_id column, because these variable does help us achieve our analysis goals.

2- There are 92,505 trips where the variables: start_station_id, start_station_name, end_station_id, and end_station_name are not available, and since we can't know for sure whether these records are reliable or not, thus we decided to drop those records in order to give a higher reliability for our findings and insights.




## Summary of Findings

- The average duration of trip in general is 14.26 minutes, however we've found that the trips made in this sharing system can be classified in two categories depending on their duration. Firstly we have the Long duration trips which took longer than 28 minutes and represents only 6% of the whole dataset, and secondly we have the Medium length trip which took less than 28 minutes and represents 94% of the dataset.

Furthermore, the average duration of both categories are as follows: 78.43 minutes for the Long duration trips and only 10.18 minutes for the medium duration trips. Moreover, the trips taken by cusotmers, even though representing about 20% of the whole recorded trips, they are on average longer than the double of the average of trips taken by subscribers. This observation suggest that subscribers usually go for more rides but with shorter duration, like going to study, work, gym..etc 

- The number of trips taken in the weekend days throughout 3 years is slightly less than half the number trips taken in the rest of the week, whereas the average duration of trips taken in weekend days is 50% bigger than the average duration taken in the workdays, and this trend is maintained throughout the three years in our dataset. This observation could suggest that the people using the Ford GoBike System would more likely go for a long bike trip during the weekends to hangout or as some kind of workout exercice. While during the workdays, the shorter average trip duration could be explained by the need for short rides, like going to work or going to groceries..etc. 

- The most frequented start station is Bancroft Way at College Ave with more than 85,000 trips starting there during three years. This station is one of four stations that are the closest to the University of California Berkley and many other institutions. In the other hand, the most frequented end station is Folsom St at 3rd St with almost 120,000 trips ending there during three years. This station is in a residential area which suggest that a good number users of this bike sharing system lives near this area, or visit it frequently for any other reason. It's important to note that more than 3 million trip during these three years are made from and to a none highly frequenty stations which means stations with less than 33,000 trips during this period.

-Even though we noticed a huge increase in the number of trips between 2017 and 2018, and a smaller increase between 2018 and 2019, the trends and observation made regarding the average duration of the trips, the variation in number of trips taken during week days and the frequency of the stations are maintained throughout these years.



## Key Insights for Presentation

- Unlike casual users, subscribers usually go for more rides that are on average shorter in duration.

- The users of the Ford GoBike System would more likely go for a long bike trip during the weekends to hangout or as some kind of workout exercice. While during the workdays, the shorter average trip duration could be explained by the needs of users for short rides, like going to work or going to groceries..etc.

- The trends and observation made regarding the average duration of the trips, the variation in number of trips taken during week days and the frequency of the stations are maintained throughout these years.