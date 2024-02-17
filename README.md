# Green Borough Taxi Analysis

Hi everyone, in this project i will try to discover hidden pattern and insights from the NYC borough taxi trip data by performing data analysis, these findings can be used by taxi cab companies or even individual drivers to improve their profit or minimize operating cost.

# Source Data 
<p align="center">
<img src="images/NYC.png" alt="Image Description" width="300"/>
</p>

The main data that being used in this analysis was gained from the New York City Taxi and Limousine Commission (NYC TLC), each rows represent a green taxi trip. the secondary data that being used was gained from the nyc open data which contains information of trip location and shape data.

# Business Understanding
<p align="center">
<img src="images/Boro-Taxi-4.png" alt="Image Description" width="300"/>
</p>
Boro taxis or green taxi are taxicabs in New York City that are allowed to pick up passengers (street hails or calls) in outer boroughs (excluding John F. Kennedy International Airport and LaGuardia Airport unless arranged in advance) and in Manhattan above East 96th and West 110th Streets.

# Problems to be solved

After diving into the bussiness process, here are some problems that i can help to solve by using the data:
<ol>
  <li>When is the best time to allocate the taxi fleet or drive a taxi?</li>
  <li>Is the borough taxi distribution to other borough is even? </li>
  <li>How to improve the borough taxi business in other borough ?</li>
</ol>

# Data Cleaning

Data cleaning plays a pivotal role in data analysis as the quality and validity of insights are very dependant on data cleaning
<ol>
  <li> Handling Missing Values ?</li>
  <li> Outlier Identification </li>
  <li>How to improve the borough taxi business in other borough ?</li>
</ol>

## Missing Values

![image](https://github.com/bintangrizqikhairullah/Green-Borough-Taxi-Trip-Analysis/assets/101108509/c9ddcc22-5290-411e-8f47-306b9ffe9af1)

The data have 7 columns with missing value, The column "ehail_fee" has all it's value missing, while other columun has an average of 6.35% missing value.The column "ehail_fee" is dropped because all of it's value are missing The rows with missing values are dropped because imputation would probably lead to bias and there are no patterns in these missing value beside it happens in the same observation.

# Data Analysis

# Peak Day Analysis

![image](https://github.com/bintangrizqikhairullah/Green-Borough-Taxi-Trip-Analysis/assets/101108509/a914b97c-1eca-456b-a9f3-e492b7aea27e)

It seems that the taxi trip number rises at the start of weekdays and declines in weekend. From the graphic above, we can also conclude that the number of trips is increasing along the month.

![image](https://github.com/bintangrizqikhairullah/Green-Borough-Taxi-Trip-Analysis/assets/101108509/003b23d7-90be-4af7-ab58-860f3c5c047d)

The data visualization suggest that daily trips on weekdays are higher compared to weekends, this statment also strenghtened by the mann whitney test that resulted in pvalue=0.00027 < alpha=0.05. the huge number of trips on weekdays happens due to a lot of people work on weekdays which is on monday to friday. Not only workers, there are a lot of user that do their activities on weekdays such as student, etc. The number of trips fall off on weekends, this happens because the customer that have been mentioned before, are having holidays. On weekends, customer uses taxi to go to recretional places.

# Peak Hour Analysis

![image](https://github.com/bintangrizqikhairullah/Green-Borough-Taxi-Trip-Analysis/assets/101108509/bcdece7e-1e64-43ac-8d98-4eb65447a66b)

The taxi trip numbers rises when near and in rush hour which is in 6:00 am to 9:00 am when people are commuting to work place and school, and 4:00 pm to 7:00 pm when people are coming back from it. On weekends, the number of taxi trip on midnights is relatively higher than on weekdays.

# Trip Location Analysis

![image](https://github.com/bintangrizqikhairullah/Green-Borough-Taxi-Trip-Analysis/assets/101108509/2e6bce74-b0f3-4d80-bb02-cdc344e5c435)

60% of trips were made in Manhattan, this result suggest that the borough taxi's populraity and use in other borough besides manhattan is still low, this is bad because The borough taxi were intially made to fullfill the demand of taxi for from customer outer borough.

![image](https://github.com/bintangrizqikhairullah/Green-Borough-Taxi-Trip-Analysis/assets/101108509/d0eec5fc-7c4f-488a-8c81-c731e8029ff2)

The graphic above shows that the majority trip's drop off location is the sama as it's pick up location. This means that taxi is commonly  used as short distance transportation.

# Trip Characteristic by Borough Analysis

![image](https://github.com/bintangrizqikhairullah/Green-Borough-Taxi-Trip-Analysis/assets/101108509/33bf4dca-8896-4b87-936b-af2407bed395)

Borough with higher average fare amount, trip distance, and trip duration have lower total trips. This happens because the trip distance trip duration of a trip, the higher the fare will be, this would cause customer to choose more cheap transportaion for long distance travel.

![image](https://github.com/bintangrizqikhairullah/Green-Borough-Taxi-Trip-Analysis/assets/101108509/1108c3b0-f58b-4d8b-9ae0-60d4d1d02332)

The correlation spearman shows that trip duration and trip distance have strong positive correlation with fare_amount. It's also shwon that total trips have strong negative correlation with trip duration, trip distance, and fare amount.

# Reccomendation and conclusion

<ul>
  <li>It's recomended to allocate taxi fleet in the weekdays especially on wednesday, Thursday and friday's rush hour because the taxi demand on the peroids are high and allocate less fleet on sunday to reduce operating cost</li>
  <li>The popularity of green taxi on other borough besides manhattan is still low, especially in staten island and Bronx, the taxi also rarely used to travel between borough, this is because customer in these borough uses taxi for longer duration and farther distance than in manhattan, recalibartaion of taxi's fare rate to make it affordable in these borough or giving discount would increase the trip's number</li>
</ul>
