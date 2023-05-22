# Airbnb Dataset Analysis and Visualization
This project, implemented in Python using Google Colab, focuses on analyzing and visualizing the Airbnb dataset. The dataset contains information about various Airbnb listings in Amsterdam. The goal of this project is to process the dataset, perform calculations, and create an interactive app for visualizing the data geographically.

* [Project Code](https://colab.research.google.com/drive/1QZ-y2DTPlGMRCGjUYVV5F-7G4c7WSCMr#scrollTo=7G3KvDaeF9YD)  
* [Streamlit app](https://panktir-airbnb-ds-streamlit-app-9qu9wu.streamlit.app/)

## Project Overview
* Downloading and preprocessing the dataset
* Cleaning the data and transforming it into a suitable format
* Performing calculations and currency conversion
* Adjusting prices for inflation
* Selecting a preferred location in Amsterdam
* Calculating the distance between the preferred location and available Airbnb listings
* Visualizing the dataset using Streamlit

## Project Tasks
1. **Data preprocessing:** The dataset is downloaded and processed to ensure proper formatting and eliminate irrelevant information.
2. **Cleaning and transformation:** Unnecessary rows and columns are removed, and the dataset is rearranged to its original format.
3. **Data validation:** String characters are filtered out, and the dataset is verified to contain only numerical values.
4. **Currency conversion:** Prices are converted from US dollars to a chosen currency using appropriate calculations.
5. **Inflation adjustment:** Prices are adjusted based on the annual inflation rate of the chosen currency.
6. **Data type conversion:** The dataset is transformed to enable numerical operations by changing the data type to float32.
7. **Geographical analysis:** A preferred location in Amsterdam is selected, and the distances between this location and available Airbnb listings are calculated.
8. **Optimization with NumPy:** The distance calculation function is converted into a pure NumPy function for improved efficiency.
9. **Performance evaluation:** Execution time is measured using the timeit function to compare the optimized NumPy implementation with the previous version.
10. **Visualization:** The dataset is visualized using Streamlit, displaying prices, locations, and color-coding based on category.

## Technologies and Libraries Used
* Python
* Google Colab
* NumPy
* Streamlit
This project showcases proficiency in data preprocessing, cleaning, calculations, currency conversion, and geographical visualization using Python. The final result is an interactive app that allows users to explore the Airbnb dataset in Amsterdam visually.

[Streamlit app](https://panktir-airbnb-ds-streamlit-app-9qu9wu.streamlit.app/)
