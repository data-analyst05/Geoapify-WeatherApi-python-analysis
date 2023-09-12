# WeatherPy Analysis & VacationPy Analysis using Weather API and Geoapify API

# WeatherPy Analysis

## Overview

WeatherPy is an analytical tool that examines the relationship between the latitude of cities worldwide and their weather patterns. By visualizing and interpreting these relationships, we can gain a better understanding of how our planet's geography impacts our climate.

## Dependencies

- Python
- Matplotlib
- Pandas
- NumPy
- Requests
- Scipy
- Citipy
- OpenWeatherMap API

## Instructions

1. **Setup & Initialization**:
    - Clone the repository to your local machine.
    - Make sure all dependencies mentioned above are installed.

2. **API Key**:
    - Sign up for a free account on [OpenWeatherMap](https://openweathermap.org/api) to obtain an API key.
    - Store your API key in a file named `api_keys.py` with the variable name `weather_api_key`.

3. **Execution**:
    - Run the WeatherPy script: `python WeatherPy.ipynb`.

4. **Outputs**:
    - After executing the script, it will generate scatter plots showcasing relationships between latitude and various weather conditions.
    - It will also output the data used to create these plots in a CSV format (`output_data/cities.csv`).

## Key Findings

1. **Latitude vs. Temperature**:
    - As expected, the temperature increases as one approaches the equator and decreases as one moves away from it, especially towards the northern hemisphere.

2. **Latitude vs. Humidity, Cloudiness, and Wind Speed**:
    - These relationships are more complex and may not show a simple linear trend when plotted against latitude. Further analysis and more factors may be needed to draw concrete conclusions.

3. **Linear Regression Analysis**:
    - The northern and southern hemispheres were analyzed separately for each of the relationships to provide a more detailed perspective. 

## Acknowledgments

Special thanks to OpenWeatherMap for providing the weather data and to Citipy for assisting in city lookup based on geographic coordinates.

# VacationPy Analysis

## Overview

VacationPy is a Python-based analytical tool that helps users identify ideal vacation destinations based on their preferred weather conditions. By leveraging weather data from various cities across the globe, VacationPy suggests destinations that match the user's criteria and visualizes them on a Geoapify map, showing hotels in the vicinity.

## Dependencies

- Python
- Pandas
- Matplotlib
- Jupyter Notebook
- hvplot
- Requests
- Geoapify API

## Instructions

1. **Setup & Initialization**:
    - Clone the repository to your local machine.
    - Make sure all dependencies mentioned above are installed.

2. **API Keys**:
    - Obtain a Geoapify API key with access to Geoapify Maps and Places from [Geaapify](https://www.geoapify.com/maps-api).
    - Store these keys appropriately within the script `api_keys.py` as environment variables.

3. **Execution**:
    - Open Jupyter Notebook and run the `VacationPy.ipynb` notebook.

4. **Set Your Preferences**:
    - Within the script, you'll have the option to specify your preferred temperature range and other weather conditions.

5. **Outputs**:
    - The script will render a Geoapify map with markers on suggested destinations.
    - Hovering over these markers will display the name of the nearest hotel.

## Key Features

1. **Weather Preference Filtering**:
    - Users can input their ideal weather conditions, and VacationPy will filter out cities that match these criteria.

2. **Hotel Lookup**:
    - For each potential vacation destination, the nearest hotel is identified and displayed on the map.

3. **Interactive Visualization**:
    - Geoapify Maps integration provides an intuitive and user-friendly way to visualize potential destinations.

## Future Enhancements

- Integration with travel booking APIs to provide direct links for hotel reservations.
- Expansion of criteria to include other factors such as points of interest or local events.
- Integration with user accounts to save past searches and preferences.

## Acknowledgments

Special thanks to OpenWeatherMap for providing the weather data, Geoapify Maps for visualization, and Geoapify Places for assisting in hotel lookup based on geographic coordinates.

