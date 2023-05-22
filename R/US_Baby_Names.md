## Project Description

# Purpose
The purpose of this project is to explore and analyze 100+ years of US baby names data using R Studio in Gitpod. By examining naming trends, letter popularity, letter combinations, and usage of vowels and consonants, we aim to gain insights into the cultural and linguistic aspects of names over time.

# Project Tasks
During this project, I leveraged R Studio in Gitpod to perform a comprehensive exploration and analysis of 100+ years of US baby names data. Here is an overview of the main tasks I accomplished:

1. **Data Import and Preparation:** Imported the dataset from data/names.csv.gz using the read_csv function from the readr package. Prepared the data for analysis by cleaning, transforming, and structuring it in a suitable format.

2. **Naming Trends:** Explored the most popular names for different decades and identified naming trends over time. Visualized the top names for each sex using column plots and bar plots.

3. **Stability and Trendiness Analysis:** Investigated the stability and trendiness of names by analyzing variations in popularity over the years. Calculated trendiness scores based on birth frequencies and identified stable and trendy names.

4. **Letter Popularity:** Explored the popularity of letters in names by analyzing the distribution of first and last letters. Visualized the trends in letter usage over time and identified popular letter combinations.

5. **Vowels vs Consonants:** Investigated the usage of vowels and consonants in names to uncover naming trends. Categorized names based on letter types and visualized the distribution of births by combinations of first and last letter types.

6. **Data Integration:** Incorporated actuarial life tables from the Social Security Administration to estimate the probability of individuals being alive based on their birth year. Joined the life table data with the baby names data to analyze the probability of survival and age distributions for specific names.

7. **Visualization and Reporting:** Created visually appealing and informative plots using the ggplot2 package to present the findings of each analysis. Generated clear and concise reports to communicate the insights derived from the data.

# Technologies and Libraries Used
Throughout this project, I utilized the following technologies and libraries:

**R Studio:** Integrated development environment (IDE) for R programming.
**Gitpod:** Online development environment for Git-based projects.
**R Programming Language:** Used for data manipulation, analysis, and visualization.
  - Tidyverse:Collection of R packages for data manipulation and visualization, including dplyr, ggplot2, and stringr.
  - readr: R package for reading and parsing data files.
  - zoo: R package for working with regular and irregular time series data.
