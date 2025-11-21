# IS-477 Interim Status Report
All datasets used for this project are available in the following GitHub release:

[Housing Market and Crime Datasets (v0.2)](https://github.com/QuinnCroc/IS-477/releases/tag/v0.2-datasets)

This release includes:
- **city_market.archive.6.zip** — contains detailed housing market data across multiple U.S. cities from 2012–present.
- **crime_100_250.csv**, **crime_250_plus.csv**, **crime_40_60.csv**, **crime_60_100.csv** — segmented datasets containing crime rate data (violent, property, and total crime) by city size category.

These datasets were merged, cleaned, and analyzed to explore the relationship between housing affordability and public safety across different U.S. cities.

## Updated Timeline

During Week 1–2, we finalized the topic and research questions focused on housing prices and crime rates. In Weeks 3–4, we collected and cleaned datasets to ensure consistency in city names and to remove missing or invalid values. Weeks 5–6 involved merging both datasets and performing initial visualizations, such as heatmaps. In the upcoming weeks, we plan to add more visualizations, perform regression analysis to test relationships, and prepare the final written report and presentation by the project deadline.

## Changes to Project Plan and Progress

Since Milestone 2, our project plan has evolved to focus more on data accuracy and city-level consistency. Initially, we intended to analyze raw datasets separately, but after receiving feedback from Milestone 2, we changed our approach to merge housing and crime data earlier in the process. This allowed us to generate more accurate visualizations and identify clearer relationships. We also changed our scope by focusing on a smaller subset of U.S. cities to reduce data complexity and improve performance. Additionally, we added new visualization techniques, such as correlation heatmaps, to support our analysis. Overall, these changes have improved both our workflow and data reliability.

## Krishan Amin's Contributions

For this stage of the project, I focused on data acquisition, cleaning, and the integration process. My primary responsibility was to gather and prepare both datasets, which were the United States Crime Rates by City Population and the US Cities Housing Market Data – Live Dataset, so that they could be accurately merged and analyzed. The data preparation phase required attention to file structures, formats, and consistency across tens of thousands of records. By uploading, standardizing, cleaning, and merging the files, this allowed for the later visualizations and statistical analysis.

I began by locating and downloading both datasets from Kaggle, making sure that they covered data from 2012 to the present to match the project’s requirements. I explored the data contents by printing the columns, inspecting data types, and identifying key variables for merging, such as CITY, STATE, and unique identifiers. Since the two datasets came in different formats,  a .tsv file for housing and multiple .csv files for crime, I used Pandas to standardize how each file was loaded and processed in Python. For the crime dataset, I combined several smaller files (crime_40_60.csv, crime_60_100.csv, crime_100_250.csv, and crime_250_plus.csv) into one unified dataset called crime_combined.csv. This ensured that all city-level data, regardless of population size, could be treated as a single source for future merging.

Next, I focused on cleaning the data. This included dropping incomplete rows, trimming extra spaces, and standardizing capitalization in city names to prevent mismatches during the merge. I used string methods like .str.strip() and .str.title() to make sure “Los Angeles,” “los angeles,” and “LOS ANGELES” were identified as the same city. I also removed columns with repetitive or missing identifiers and made sure that each record had consistent state and city information. Once the cleaning was complete, I used the pd.merge() function to connect the housing dataset and the crime dataset on their shared CITY field, making sure that the merge used an “inner join” to include only cities that existed in both datasets. This resulted in a comprehensive combined dataset with over 1.2 million rows, titled merged_housing_crime.csv.

Once I merged the files, I verified the work by checking the number of merged rows, printing sample data, and confirming that all relevant numeric columns were properly aligned. I also began converting numeric fields, such as housing prices and crime rates, from string to float by removing commas and dollar signs. These conversions were important to make the data usable for correlation analysis and visualization later in the project. By doing this,  the dataset was clean, consistent, and ready for statistical analysis.

These steps are crucial to building the analytical base for the project. Without accurate merging and data validation, meaningful correlations between housing affordability and public safety could be inaccurate. Next, I will assist in refining variable selection for regression analysis and validating how crime types correlate with housing costs across different regions. Overall, this work has provided a strong and reliable foundation for the project’s analytical and visualization stages.



