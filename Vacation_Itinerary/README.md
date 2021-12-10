# World Weather Analysis

## Overview

The purpose of this analysis was to create an app that allows users to filter vacation destinations based on weather preferences, thus enabling the identification of potential travel destinations and nearby hotels.  From the list of potential travel destinations, users can then select four cities to travel to, and create a travel itinerary with travel directions between the four cities, as displayed on a marker layer map.  

## Results

The first step in this project was to generate a list of two thousand random latitudes and longitudes, and then identify the closest city using citipy.  Using an API call with OpenWeatherMap, we were able to pull current weather data for each of these cities, notably latitude and longitude, max temp, percent humidity, percent cloudiness, wind speed, and current weather description.  The resulting weather data were then placed into a new DataFrame which was exported as a CSV file.  

![Figure 1](https://raw.githubusercontent.com/AMHembrough/PyBer_Analysis/main/Resources/Resources/Fig1.png) 

The next step in this project was to retrieve customer weather preferences using input statements.  The loc method was then used to filter the city DataFrame for temperature preferences based on the input statements.  A new Dataframe was then created to store the nearest hotel name.  We then added the name of the nearest hotel to each city to the DataFrame.  If a hotel isn’t found that meets the outlined criteria, we skipped to the next city in the DataFrame.  We then dropped rows where a hotel was not found.  An output file was created to store the final DataFrame.  We also created a marker layer map, similar to the one above, to show pop-up markers for each city on the map.  

![Figure 1](https://raw.githubusercontent.com/AMHembrough/PyBer_Analysis/main/Resources/Resources/Fig1.png) 

The final step in this project was to utilize the Google Directions API to create a travel itinerary that shows a transit route between 4 cities chosen from a user’s list of possible travel destinations.  A marker layer map with pop-up markers for each city on the travel itinerary was also created.  

![Figure 1](https://raw.githubusercontent.com/AMHembrough/PyBer_Analysis/main/Resources/Resources/Fig1.png) 

## Summary

Through completion of this project, I was able to learn many new skills including, but not limited to, retrieving weather data via an API call, creating custom marker layer maps, collect data from users using input statements, and so much more! 
