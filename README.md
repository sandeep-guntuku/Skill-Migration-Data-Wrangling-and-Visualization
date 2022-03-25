# Skill-Migration-Data-Wrangling-and-Visualization
## Migration of LinkedIn members at the country-skill level, 2015-2019

## Data Source:

Data has been sourced from the citation “Talent Migration Data” by World Bank Group & LinkedIn Corporation, licensed under CC BY 4.0., published by The World Bank at https://datacatalog.worldbank.org/search/dataset/0038044/Talent-Migration---LinkedIn-Data-

Table downloaded from Overview tab “CSV: Skill Migration”. Data has been taken for all countries and categories for the years 2015-2019.

## Background:

This dataset is part of the LinkedIn - World Bank Group partnership, which helps governments and researchers understand rapidly evolving labor markets with detailed and dynamic insights.

## Characteristics:

The main characteristic of this dataset is that it allows leaders to benchmark and compare labor markets across the world; analyze skills and migration; and leverage real-time data to make policy changes.

## Variables:

The original dataset has the following variables:

Country Code and Country Name : Every country name and corresponding country code over the world has been included in the data.

Income Category: The Income Category based on the country concerned.

Region: The region based on the country concerned.

Skill Group ID, Category and Name: The ID, Category and Name of the Skill Group based on the migration of LinkedIn members.

net_per_10K_2015, net_per_10K_2016,…net_per_10K_2019: Discrete values of years for which the respective data has been collected.

## Data Cleaning:
Data needs to be cleaned and made tidy before performing any visualizations.

To avoid scientific notation and Read the data from csv file.

Dropping the null columns created with indexes 13 till 29 and Dropping rows/records with NA values.

Here, I have used kable for displaying the top 10 rows as the dataset has 17000 rows.

## Data Wrangling:
The dataset is untidy as it violates the tidy data principles because:

Each variable does not have its own column.
Each observation does not have its own row.
For tidying the dataset below steps are followed:

#### Using pivot_longer:

We have column names 2015, 2016, 2017, 2018, 2019 that contain values and not variables.

Hence, Using PIVOT LONGER, created two new columns named “Year” and “Net_per_10K_Value” for tidying the dataset.

Used kable to display the first ten records in the tidy dataset.

## Data Visualization:
Created a vector of 4 countries having different income categories and updated the values into datafil for better visualizations.

## Conclusion:
1. Skill migration is more predominant in country Afghanistan and less predominant in country United States.

2. Skill migration is more predominant in Europe and Central Asia region and less predominant in Latin America & Caribbean region.

3. Skill migration is more predominant in Low Income groups and less predominant in High Income Groups.

4. United States has more skill migration in Tech Skills and Disruptive Tech Skills.

5. Afghanistan has more skill migration in Specialized Industry Skills and Business Skills.
