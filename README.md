# python-api-challenge
Weather Analysis Project

# Introduction
This project aims to analyze weather data for various cities and find the nearest hotels for each city using the Geoapify API. It involves collecting weather data for multiple cities, filtering the data to find cities with specific weather conditions, and then using the Geoapify API to find the nearest hotels for those cities.

# Requirements
To run this project, you will need the following:

Python 3.x
Jupyter Notebook
Pandas library
hvplot library
requests library
Geoapify API key

# Project Structure
The project consists of the following components:

1. cities.csv: A CSV file containing weather data for various cities.
2. ideal_cities DataFrame: A data containing cities defined by the ideal conditions.
3. hotel_df DataFrame: A data containing namesof 1st hotel in 10000m radius defined by the city Latitude & Longitude.
4. VacationPy.ipynb: A Jupyter Notebook that includes all the code for data analysis, filtering, and hotel search using the Geoapify API.


# Project Steps

Data Collection: The initial step involves collecting weather data for various cities. The data is stored in a CSV file named cities.csv.

Visualization: The project uses the hvplot library to visualize the cities on a map, where the size of the point marker represents the humidity in each city.

Filtering: The data is then filtered to find cities that meet specific weather conditions, such as a max temperature between 21 and 27 degrees Celsius, wind speed less than 4.5 m/s, and zero cloudiness.

Hotel Search: The Geoapify API is used to find the nearest hotel for each filtered city within a radius of 10,000 meters. The hotel names and other information are added to the hotel_df DataFrame.

Visualization with Hotel Information: The final step involves visualizing the cities on the map again, with the added information of the nearest hotel and country displayed in the hover tooltip.