# Bikesharing Challenge

The purpose of this challenge is to show our understanding of how to use Tableau to create worksheets and stories from analyzing data. These stories will help us in presenting findings in data analysis to non-technical professionals (stakeholders, project managers, retail team members etc.) without them needing the expertise of programming languages such as Python, SQL, or Javascript. Tableau is a very useful tool for creating visualizations from analyzing large datafiles.

[link to dashboard](https://public.tableau.com/views/NYCChallenge/BikeshareStory?:language=en-US&publish=yes&:display_count=n&:origin=viz_share_link)

## Overview of Bikesharing Data

In this project we were impressed by visiting various landmarks in New York City by bicycles with Citi Bike. We decide that we want to start our own business which would be similar to Citi Bike, however we need to complete an analysis of many different factors of play when opening a Bike Business. 

We have decided to use Tableau to analyze trends of Citi Bikes business to notice areas of opportunity for our business in Des Moines. Examples of these trends are the checkout times for users, the gender of bike users, the length of trips etc.

## Bikeshare Analysis Results:

### Converting Tripduration column to a date and time field

The first step in our analysis was to use Pandas through Jupyter notebook to convert the "Tripduration" column from an integer datatype to a "time" data type. We complete this as shown in the image below. As you can see the tripduration column has been changed from a integer value to a data and time value seperated by hour, minute, and seconds.

![TripDuration field](https://user-images.githubusercontent.com/92459399/153729052-c559084f-3222-4b1c-9b01-c4266759bf03.PNG)

Our next step was to use tableau to create charts and visualizations to use in our analysis and user story.

### Checkout Times for Users

As you can see there is a line graph displaying the number of bikes checkout times by the duration for all users. The graph is filtered by the hour and minutes and we can come to some conclusions
- Most people on average ride their bikes for a maximum of 20 minutes per trip
- Some users ride their bikes for a maximum of 40 minutees
- Very few people ride for longer than 1 hour

![Checkout Times for Users](https://user-images.githubusercontent.com/92459399/153729542-96087e41-e204-4495-935d-87692100994d.PNG)

### Checkout Times by Gender

As displayed below there is a line graph displaying the number of bikes that are checked out by duration by the hour. Each line is a display of the gender of the riders. From this we can make the following conclusions.
- Which riders by gender made the most trips in the hour
- which riders took the longer trips on average by gender (male or female)
- which riders were of unknown orientation and their length of the trips

![Checkout Times by Gender](https://user-images.githubusercontent.com/92459399/153729428-8a233b1f-1d4b-4a0f-b54e-5aa6632b0cec.PNG)

### Trips by Weekday for Each Hour

We created a heat map for this particular analysis. The heat map shows the number of bike trips for each hour per day of the week. We can come to the following conclusions with this chart.
- which days of the week and hours are the busiest
- from a quick analysis we can make a basic conclusion that for most days 7-8am and 5-6pm are the busiest times in the week 

![Trips by Hour per Week](https://user-images.githubusercontent.com/92459399/153730212-76f3c0a6-8d8b-4edf-a33f-5d78ca1511f1.PNG)

### Trips by Gender (Weekday per Hour)

Once again we create a heat map to analyze the trips per hour throughout the week. In this analysis however we also seperate by the gender of the rider. we can come to some conclusions from this chart
- The demane for male riders is much higher throughout the week than female riders
- the demand for male riders is highest in weekdays around 7-8am and 5-6pm

![Trips by Gender (Weekday per Hour)](https://user-images.githubusercontent.com/92459399/153730267-28b87728-ba57-4e4e-90f1-41c03b84049d.PNG)

### User Trips by Gender (Weekday per Hour)

For this analysis we also use a heatmap with a slightly different setup. We show the number of bike trips for each type of user (customer or subscriber) and the gender for each day of the week. At a quick glance we can come to the following conclusions
- The demand for subscribers is higher than that of customers of Citi Bike
- The demand of Male subscribers is by far much higher than that of other genders of subscribers (female or unknown)

![User Trips by Gender per Weekday](https://user-images.githubusercontent.com/92459399/153730618-24340f59-fa34-4ab3-9a90-8cfa9393e987.PNG)

### Additional Visualizations

For the additional visualizations it makes sense to analyze the gender distribution of riders as for a few of the analysis we noticed that male riders were in general higher than female or unknown gender of riders. Is this because the overall population of riders is male or is it due to the population of female riders is spread out over even time frames? from looking at our Gender Breakdown Pie Chart we see the following
- Male riders make up more than 50% of the population of riders in NYC
- Female riders are roughly 25% of the total population

![Gender Breakdown](https://user-images.githubusercontent.com/92459399/153730754-6b11453a-0df8-4b3a-8179-19e0f00e6b5e.png)

The peak hour chart is below and we can make a few assumptions from this chart as well.
- As in the previous charts 5-6pm is a popular time for riders
- 7-8pm is also the second most busy time for riders
- 1-2am would be the ideal time to perform any bike maintenance as it is the least busy time

![August Peak Hours](https://user-images.githubusercontent.com/92459399/153730819-8666ef11-4b98-4dcf-ad4f-e957f9ab9a5c.PNG)

## Summary and Conclusion of Analysis

from this analysis we can come to the following conclusions:

1. Peak hours for riders throughout the week is 7-8am and 5-6pm
2. the overall population of male riders is much higher than that of female riders. This points towards who the primary customers should be focused around.
3. The busiest days of the week are Weekdays (specifically Monday, Tuesday, Thursday, and Friday) in comparison to weekends. This could also tell us of potential business opportunities around riders (rehydration stands, bike-athon etc.) to take into consideration for the future

