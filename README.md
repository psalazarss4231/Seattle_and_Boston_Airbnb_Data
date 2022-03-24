# Seattle_and_Boston_Airbnb_Data
Proyect Write a Data Science Blog Post
# Project Write a data science blog post
# Airbnb Data for Seattle and Boston


1. [ Introduction. ](#intro)
2. [ Section 1. ](#section1)
3. [ Section 2. ](#section2)
4. [ Section 3. ](#section3)
5. [ Conclusion. ](#conclusion)





















<a name="intro"></a>
## 1. Introduction

Since 2008, Airbnb is a business of guests and hosts, providing the opportunity to stay in a more exclusive and highly personalized way and has had a great boom worldwide, even more so with the growing trend of digital nomads and the new generations that do not they are interested in putting down roots in a place, thus preferring to rent a lodging that is cozy (feel at home) while they enjoy the experiences of new places.


<a name="section1"></a>
## 2. Section 1. Business understanding


Some of the busiest cities are Seattle and Boston, so it would be interesting to investigate the factors that can influence a stay through Airbnb, for which we are interested in answering the following questions using the CRISP-DM methodology.

1- What is the occupancy rate in Seattle and Boston?
2- What is the occupancy rate in Seattle and Boston by neighborhood?
3- What is the average price per night in Seattle and Boston?
4- What is the average price per week?
5- What are the most expensive and cheapest times of the year in Seattle and Boston?
6- What are the prices for one night per neighborhood?
7- What are the busiest times of the year in Seattle and Boston?
8- Do the two cities have differences in terms of times of the year or prices?
9- In the busiest times do prices go up?
10- Is there currently an upward trend in terms of accommodation and its prices?
11- Could you predict the price of a new hosting with current features?

<a name="section2"></a>
## 3. Section 2. Prepare data

For the data preparation process, we collect, evaluate and proceed to clean, focusing on the variables of our interest with the Numpy and Pandas libraries.
## 4- Data modeling
We plot all the data relevant to the initial questions using packages like matplotlib and seaborn.

<a name="section3"></a>
## 4. Section 3 Evaluation of the results
From the initial questions we came to the following conclusions:

1- What is the occupancy rate in Seattle and Boston?
The occupancy rate in the city of Seattle is quite high with 67%, however, we observe that for Boston it is only 49%, which makes us think that factors such as price could affect these indicators.

Seattle

![Q 1](/images/1.png "Q 1")


Boston

![Q 1_2](/images/1_2.png "Q 1_2")


2- What is the occupancy rate in Seattle and Boston by neighborhood?
And of course, if I were an investor I would like to have a property in Interbay with 84%, which is why we observe that not only is the city important, but also the location or neighborhood where the property is located in order to compete for added value. and not for price.

Seattle

![Q 2](/images/2.png "Q 2")




3- What is the average price per night in Seattle and Boston?
At this point we verified that the night in Seattle is much more affordable with $135/night than in Boston, which can reach the price of up to $200/night.

Seattle

![Q 3](/images/3.png "Q 3")


Boston

![Q 3_2](/images/3_2.png "Q 3_2")


4- What are the most expensive and cheapest times of the year in Seattle and Boston?
We can see that the most expensive times to visit Seattle are June and August, however, for Boston it is the month of September. We observed a certain relationship with the vacation periods of most of the students.
Regarding the cheapest times to travel to both Seattle and Boston, they are in the months of January, sure to be very cold in winter.

5- What are the prices for one night per neighborhood?
In Seattle there are neighborhoods where you can rent for $90 / night and neighborhoods and other quite expensive ones that reach up to $198 / night, so we can see how there are several options according to the budget of each visitor, and that the Interbay neighborhood with the highest rate of occupancy as it has a very competitive cost per night $118, for which we begin to see clues if it is possible to predict the prices of a lodging.

Seattle

![Q 5](/images/5.png "Q 5")


Boston

![Q 5_2](/images/5_2.png "Q 5_2")




6- What are the busiest times of the year in Seattle and Boston?
The lowest number of visits in is in January of each year, however, it is necessary to review the number of visits in January 2017, since it is significantly lower.
For Boston, the lowest number of visits is in September, which coincides with the most expensive time to stay in Boston.

7- Do the two cities have differences in terms of times of the year or prices?
The two cities coincide in the cheapest prices to travel, but not in the most expensive prices, nor in the months of less or greater occupation.

Seattle

![Q 7](/images/7.png "Q 7")


Boston

![Q 7_2](/images/7_2.png "Q 7_2")


8- In the busiest times do prices go up?
No, apparently there is no relationship between the highest prices and the busiest times in the two cities.

9- Is there currently an upward trend in terms of accommodation and its prices?
We do not observe that there is an increase in prices or visits, for the most recent months
11- Could you predict the price of a new hosting with current features?
We see better results with Random Forest than with linear regression, the highest result is an explanation of 56% of the dependent variable (price) with the other predictor variables such as 'bathrooms', 'bedrooms', 'beds', 'latitude ', 'longitude', 'reviews_per_month', 'accommodates', 'guests_included', 'host_is_superhost', 'neighbourhood_group_cleansed', 'property_type', 'room_type', 'bed_type', 'price', 'security_deposit', 'cleaning_fee', 'extra_people', 'instant_bookable', 'cancellation_policy' and it is a very good start, taking into account that in real life it is quite difficult to obtain determination coefficients greater than 50%, however, more variables can be extracted from the texts and the model performance.


<a name="conclusion"></a>


## 5. Conclusion

We see a considerable difference between the occupancy rates of Seattle and Boston, with Seattle having a higher occupancy rate and in turn a lower average price per occupancy per night.
There are times of the year with higher occupancy such as July, August and September, however we do not see a rise in prices for it.
The regression model using Radom Forest gave good results r2=0.56, however with more analysis of other variables we could improve it.
