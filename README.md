# UFOs
Practice and Challenge Assignment for Module 11

## Background
Dana’s webpage and dynamic table are working as intended, but she’d like to provide a more in-depth analysis of UFO sightings by allowing users to filter for multiple criteria at the same time. In addition to the date, you’ll add table filters for the city, state, country, and shape.

## Purpose
The webpage for UFO Sightings might be functional, but there are too many datapoints for the average netizen to scroll through. As a result, Dana asked to have a filter that can search for date, city, state, country, and the shape of the Unidentified Flying Object. The purpose of this project is to build the specified filter and to demonstrate that it is functional. 

## Results
The filters for the website work as demonstrated below:

* Date

![Date](https://github.com/Itgotworse26/UFOs/blob/main/static/images/Date_Search.PNG)


* City

![City](https://github.com/Itgotworse26/UFOs/blob/main/static/images/City_Search.PNG)

* State 

![State](https://github.com/Itgotworse26/UFOs/blob/main/static/images/State_Search.PNG)


* Country

![Country](https://github.com/Itgotworse26/UFOs/blob/main/static/images/Country_Search.PNG)


* Shape

![Shape](https://github.com/Itgotworse26/UFOs/blob/main/static/images/Shape_Search.PNG)


The website would take in data from a file called data.js. In order to search for certain criteria, the user would enter in some criteria in their desired box. The filters would identify which boxes are filled in using the updateFilters() function, and then update the desired filters using a for loop in app.js's filterTable() function. If there are any datapoints inside data.js that matches the user's desired criteria, it will be displayed on the page as rows. If there are no matches, no rows will be displayed. 

An amaterur researcher could develop a list of criteria using date, city, state, country, and the shape of the Unidentified Flying Object to see if there are any patterns. The website is rather useful to see if there are any similarities between different UFO sightings.

## Summary
As demonstrated above, the UFO Sightings website's filters are working. 

However, a notable drawback I am noticing is that when entering in search queries, the search terms have to be exact. One notable example of this is with the state search. I specified for users to enter in a state's abbreviation, because the data uses the state's abbreviation. If someone were to use a state's proper name or a query that does not exactly match the data, the filter would not pick it up.


* State w/ Full Name, But No Results

![State w/ Full Name, But No Results](https://github.com/Itgotworse26/UFOs/blob/main/static/images/State_Search_Full_Name_No_Results.PNG)


A recommendation I would suggest is handling searches that might not exactly match the data. As stated above, the filters cannot handle search queries that do not match the data. Having partial matches or an autocorrect for queries could make the website more accessible. 

Another recommadation I would suggest is allowing the user to sort the data themselves. While the data is currently sorted in descending order by date, allowing users to sort by the other criteria could help with conducting research for similarities between different sightings that might not be close in date. 

The last recommendation I would suggest is being able to update data in real-time. While I am still not familiar with data scraping for Javascript, being able to update data with more recent UFO sightings would be a boon for the the UFO Sightings website. The current dataset is somewhat out-of-date; only going up until the middle January 2010. More recent data could be a bonus to identify patterns from more recent UFO sightings. 