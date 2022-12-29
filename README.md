# Bikesharing

[link to bikesharing story](https://public.tableau.com/app/profile/randy.l.melancon/viz/Challenge_work/ChallengeStory?publish=yes)

# Overview of the analysis: 
Last summer, a friend and I took the trip of a lifetime to New York City and saw all of the sites.  It was a magical experience.  On the flight home, we realized that part of the magical experience came from an unlikely source, citibike.  My friend and I biked everywhere, which really allowed us to get to know the city and interact with people who live there that are using the bikes for their commutes.  

This got us thinking, what if we could start a bike sharing business in our hometown of Des Moines, IA?  A short time upon returning, my friend calls with the news she has found a potential investor who would provide the seed money to explore a bike share program in Des Moines.  The purpose of this analysis is to determine how the bikes are used in New York City to explore ideas of how they could potentially work in Des Moines.  

# Results: Using the visualizations you have in your Tableau Story, describe the results of each visualization underneath the image.

The following analaysis seeks to understand how bikes are used in New York City to see if there is a possible link that would help such a business be successful in Des Moines, IA.  Let's take a look at the ride sharing data and see what we can uncover.

![Cover](https://user-images.githubusercontent.com/107599510/194689272-beb43d40-8695-49f0-b2f8-69d232b2cb22.png)

Citibike is popular in New York City and many people use it to explore New York City.  The business is set up with subscribers who pay a fee of $15/month to use the bike up to 45-minutes per ride for an unlimited number of times each month.  There is also a single 30-minute trip fee of $3.99 per trip or an unlimited amount of 30-minute rides with a day pass that costs $15/day.  

The data analyzed was collected for the month of August in 2019.  During that month, the following data shows the total number of rides taken in NYC.

![#_rides](https://user-images.githubusercontent.com/107599510/194689658-633ccece-ebdb-4933-b8f7-6c894a6719ba.png)

The total number of trips taken in the month of August was 2,344,224!  That averages out to 75,620 trips per day based on a 31 day month.  This is an incredibly popular service and New Yorkers and tourists are taking advantage.  

Let's see what else we can uncover from the data.

![Sharing](https://user-images.githubusercontent.com/107599510/194690347-ac35c15b-2d7e-4fe7-a215-d5d32504bfc6.png)

This chart shows the number of trips by trip duration length.  Most trips last between 0 and 30 minutes with 5 minute duration being the most popular with a count of 146,752 trips.

![Gender](https://user-images.githubusercontent.com/107599510/194690406-5ba2ca15-96b4-4fb2-b4a9-5103acd595b3.png)

The next thing to look at is the gender breakout of users.  There are three categories for gender of users.  They are male, female, and unknown.  During the checkout process, some users must skip entering data about their gender.  The total in the unknown category is 225,521 or 9.62%.  Females make up the second largest user of the bikes at 588,431 or 25.10%.  Males make up the largest segment of users with a total of 1,530,272 or 65.28% of total users.  

![minutes_gender](https://user-images.githubusercontent.com/107599510/194690834-f5feeb33-bb70-4ea6-a27d-8c6a0a30df70.png)

The chart above shows trip duration times broken out by gender.  Similar to previous charts, 0 - 30 minutes are a popular time to rent a bike.  Males had a mode of 5 minute trip durations and females had a mode of 6 minute trip durations.  

![Gender_hour](https://user-images.githubusercontent.com/107599510/194691659-6de257f2-bba7-401d-8b3f-4e299f4cb0b4.png)

This heat map is showing the usage of bikes by hour, day, and gender.  The overall pattern makes sense with more usage around 8 am as well as 5-7 pm during the week.  On weekends, the usage is a little more spread out through the day with more rides occurring between 10am and 5 pm.

![hour_use](https://user-images.githubusercontent.com/107599510/194691744-76c2f9ff-b904-489b-8d15-890b943abd39.png)

This heat map shows the hours and days that bikes are rented the most.  Keeping with the theme of the previous heat map, this one is broken down by total usage and not split out by gender.  It is a little easier to see the pattern of weekday vs weekend usage.  Interesting that wednesday evening shows less usage while thursday afternoon shows heaviest usage during the week.

![customer_day](https://user-images.githubusercontent.com/107599510/194691916-62ebb134-b4c7-495b-8595-3fe9310cba7f.png)

This heat map breaks out customer and subscriber usertypes.  Customers are people who rented a bike during a single transaction while subscribers pay a monthly fee for the service.  It is also broken out by gender to show which days each genders rent the most bikes.  This chart is interesting because it shows that most subscriber use occurs during the week while the heaviest customer usage comes on weekends with unknown gender type renting the most on weekends.  This makes sense that subscribers are most likely residents of NYC and customers are likely not residents.  

To try to begin to understand if a bike sharing business will be as successful in Des Moines as it is New York City, we need to begin to understand the ages of the customers using the bike sharing service.  

![age_trip_old](https://user-images.githubusercontent.com/107599510/194692147-609b5eb8-c73c-4015-a9fa-316feaf3fc74.png)

This chart shows the average trip duration based on year of birth for the customer.  This graph is interesting to look at as there are a few spikes for certain birth years but the overall trend shows that customers are using the bikes for longer durations.  There is also a spike in duration for people who were born around the year 1890?  How is that possible?  This data was taken in 2019.  According to the data set, there are a large number of 129 year olds riding around on bikes for close to 45 minutes in New York City.  Why isn't this advertised as a way to encourage more tourism?  Of course that was sarcasm, there are clearly some issues with the data as it relies on the customer to enter information during rental.  

In order to try to make a little more sense out of the data, I removed records of information with individuals that had a birth year prior to 1946.  1946 was the first year of the baby boomer generation and someone would be 73 years old which felt like a natural cutoff point.  In total, there were originally 1,048,576 value counts of data for birth year.  When the oddity years were removed, the data set had 1,045,183 value counts of birth year.  A total of 3,393 records were removed or 0.003% of the data.  

![age_trip_new](https://user-images.githubusercontent.com/107599510/194693832-ae3ef1c5-4972-4ca1-be10-70b7448ce87d.png)

This chart shows data trip counts by birth year between 1946 - 2003.  This chart shows that a heavy chunk of usage comes from people born beween 1975 - 1995.  There is also a rather large spike of counts for people who were born in the year 1969.  There may be some significance to this or it could just be a prank by people entering their birth year while renting a bike.  


# Summary: Provide a high-level summary of the results and two additional visualizations that you would perform with the given dataset.

In order to see if the bike sharing company would be sucessful in Des Moines, I would be interested in looking at demographic information for Des Moines and compare it to the demographics of the users in New York City.  The demogaphic data from Des Moines isn't included in the data set.  I would look a little further into the habits of subscribers versus customers as well as do more detailed analysis on the starting and ending stations for the bikes.  There might be a relevant pattern for customers and the lengths they travel and I would want to make sure the bikes supported those needs.  I would also want to make sure bikes are avaiable and rotating properly from a usage standpoint at the busiest stations for subscribers.  

