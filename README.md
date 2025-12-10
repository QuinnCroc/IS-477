# IS-477 Course Project Report


# Title:
Exploring the Relationship Between Housing Market Trends and Crime Rates Across U.S. Cities

## Contributors:
Quinn Crockling (qdc2@illinois.edu)

Krishan Amin (kamin28@illinois.edu)

## Summary:
This project analyzes the relationship between housing affordability and public safety across different U.S. cities by combining datasets on home prices and crime statistics. The main objective of the project is to explore whether cities with higher housing prices have lower crime rates and how these relationships change based on geography. Our motivation comes from observing that housing costs and neighborhood safety often correlate with each other but are rarely studied together in a reproducible and data-driven way. Understanding this relationship can help city planners, policymakers, and community organizations identify patterns that affect long-term urban development and livability.

The data was collected from multiple sources, including public housing market archives and city-level crime rate records spanning from 2012 to the present. Krishan focused primarily on preparing and cleaning the datasets to ensure consistency in city names, data types, and missing values. He then merged housing and crime files into a unified dataset (merged_housing_crime.csv) that could be easily analyzed. Quinn handled the analytical and visualization components, creating a heatmap to examine correlations between median sale price and various crime categories. This collaboration ensured that both the technical data preparation and analytical interpretation were handled systematically.

The heatmap showed an inverse correlation between home prices and total or violent crime rates, meaning cities with higher property values usually have lower crime levels. This supported our first research question: How do housing prices relate to crime rates across different cities? More modeling and regression analysis will be done to further understand the relationship between the housing prices and crime rates; however, this finding helps establish a strong foundational relationship between the two variables. These early results also show that housing value may be used as a socioeconomic indicator for predicting community safety, although further testing and analysis are needed to confirm this trend across time and regions.

Beyond the analytical results and visualization, a large portion of our project focused on transparency and reproducibility. All data files, cleaning scripts, visualizations, and output artifacts are available through our GitHub repository at https://github.com/QuinnCroc/IS-477. To ensure research integrity, we versioned datasets under the release Housing Market and Crime Datasets (v0.2), allowing others to reproduce our work exactly or extend it with additional variables. Our repository includes organized Jupyter Notebooks, clearly commented Python scripts, and a recorded commit history documenting each step of the workflow. These practices reflect our goal of making this project not just an analysis but a replicable case study showing how public datasets can be responsibly processed and interpreted.

We made sure that our workflow followed reproducible research principles such as clearly labeled data-cleaning scripts, organized Notebooks, and recorded commit histories. Each contribution was documented with specific commit messages and version tags. Together, these procedures make our project a replicable case study in how public datasets can reveal social and economic patterns.

In future versions, we plan to expand on the statistical and predictive aspects of the study. This includes adding regression models to test how housing prices change relative to changes in crime rates while controlling for other socioeconomic factors. We plan to expand the analysis by introducing regression modeling, additional visualization types, and time-series analysis to explore how housing and crime relationships evolve over time. This will allow us to do more than just correlation and begin evaluating potential predictive or causal relationships. Additional visualizations, such as geographic choropleth maps, scatter-plot matrices, and trend lines, will help support the interpretive value of the project. These extensions will allow us to go past correlation and begin exploring potential predictive or causal relationships. Ultimately, this project serves as a foundation for more advanced, policy-relevant research on how affordability and safety interact to shape the urban environments where people live.



