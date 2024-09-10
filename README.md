# Restaurant Location Visualization

## Overview

This project involves crawling data for American McDonald's, Subway, and Starbucks locations, with a focus on Dallas but applicable to any American city. The data is processed and visualized on a map using Python. The main steps include data extraction, cleaning, geocoding, and visualization.

## Project Structure

- **data/**
  - `Restaurants.csv`: Raw data containing information about restaurant locations.
  - `restaurants_geo.csv`: Cleaned data with latitude and longitude values obtained via geocoding.

- **notebooks/**
  - `mcdonalds.ipynb`: Jupyter notebook for crawling data from [McDonald's Restaurant Locator](https://www.mcdonalds.com/us/en-us/restaurant-locator.html).
  - `starbucks.ipynb`: Jupyter notebook for crawling data from [Starbucks Store Locator](https://www.starbucks.com/store-locator?map=39.635307,-101.337891,5z).
  - `subway.ipynb`: Jupyter notebook for crawling data from [Subway Locator](https://www.subway.com/en-us/locator).
  - `geolocation.ipynb`: Jupyter notebook for cleaning data and obtaining geocoded coordinates with Folium.

- **visual/**
  - `map.ipynb`: Python script to generate a map visualization of the restaurant locations using Folium.

## Requirements

- Python 3.x
- pandas
- folium
- requests (for geocoding API)
- [MapQuest API Key](https://developer.mapquest.com/)

## Usage

1. **Prepare Data**

   Ensure that `restaurants.csv` is present in the `data/` directory.

2. **Crawl Data**

   Use the Jupyter notebooks in the `notebooks/` directory to crawl data for McDonald's, Starbucks, and Subway. Execute each notebook to extract data and save it into `restaurants.csv`.

3. **Clean Data and Geocode**

   Use the `geolocation.ipynb` notebook to clean the data and obtain geocoded coordinates. This notebook processes `Restaurants.csv` and saves the results in `restaurants_geo.csv`.

4. **Generate Map Visualization**

   Use the `map.ipynb` script in the `visual/` folder to create an HTML file, `restaurants.html`, which contains an interactive map with restaurant locations plotted using Folium.

5. **View the Map**

   Open `restaurants.html` in your web browser to view the map.

## Example

A sample of usage can be found in `visual/map.ipynb`

## Links

- [McDonald's Restaurant Locator](https://www.mcdonalds.com/us/en-us/restaurant-locator.html)
- [Starbucks Store Locator](https://www.starbucks.com/store-locator?map=39.635307,-101.337891,5z)
- [Subway Locator](https://www.subway.com/en-us/locator)

## Contributing

Feel free to open issues or submit pull requests if you have suggestions or improvements!
