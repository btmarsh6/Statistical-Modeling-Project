# Final-Project-Statistical-Modelling-with-Python

## Project/Goals
In this project, I examine the locations and capacities of the Mobi bikeshare system in Vancouver, BC. I compare this data to data from Yelp and Foursquare, looking for points of interest (POIs) around each bike station. My goal is to determine if there is a relation between the number and types of POIs around each station and the bike capacity of that station. I attempt to build a statistical model of the relationship.

## Process
I begin with pulling data about each bike station from the City Bike API. Specifically, I take the station location, name and total number of bike slots.

Next, I looked at the categories from the Yelp and Foursquare APIs and decided which types of POIs I thouhgt were most likely to have an impact on bike traffic. I chose the following categories:
* Bars, Restaurants and Cafes
* Arts & Entertainment
* Landmarks, Outdoors & Sports
* Retail (specifically grocery, beer/liquor, drug, convenience, clothing, electronics, book, and department stores)
* Municipal Buildings/Services (schools, hospitals, libraries, community centers and SkyTrain stations)

I retrieved these POIs from both Foursquare and Yelp within a 300 m radius of each bike station. After retrieving them, I sorted through the data to delete duplicates, including for example places listed as both bars and restaurants, or stores listed as both department and clothing stores.

## Results
(fill in what you found about the comparative quality of API coverage in your chosen area and the results of your model.)

## Challenges 
One challenge I encountered was the result limit and request limits for Foursquare and Yelp API requests. My model would be improved by including more categories of POIs. This model does not account for things like office spaces that might attract commuter traffic, and is only a selection of types of retail and municipal buildings that might attract riders to an area.

## Future Goals
(what would you do if you had more time?)
