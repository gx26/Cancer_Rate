# Second Year Scholarship Application: 
# Cancer Rate Analysis

  Through Internet search, in 2019, nearly 610,000 Americans died of cancer. And there were 1.8 million new cancer patients. Cancer ranks the second in number of deaths among all diseases in the United States, only about 50,000 less than heart disease (National Cancer Institute, “SEER Cancer Statistics Factsheets”). The number of diagnosed cancers continues to maintain at a relatively stable level. Comparing with 2018, the number of men who died of cancer fell by 2%, while the number of women who died of cancer remained the same. But it is important to note that the number of young people in the cancer patients is in an increasing trend in recent years. Cancer is the fourth leading cause of death in the 20-39 age group(American Cancer Society, “Key Statistics for Cancers in Young Adults”). The reason behind this phenomenon may be obesity, or excessive drinking (Piersol). So, as a person in this age group, I want to study some information behind cancer.

## **The overview**

  In the **[project report](Cancer_Rate_Report.docx)**, I analyze and explaine three data sets, codes and graphs, and calso ombine the conclusions made by data with the reality by searching news, article, governmental policy, etc. This report is responsible for the **stroytelling part**.

  The other **[four HTML](https://github.com/gx26/Cancer_Rate)** files are responsible for **visualization** and **predictition** through code.

## **This repository contains**:

- 1. *[Datasets](https://github.com/gx26/Cancer_Rate/tree/master/Datasets)* - A folder contains all datasets（raw and cleaned）

- 2. *[Project Report](Cancer_Rate_Report.docx)* - This report contains my analysis and thoughts on each data set, and searching for policies news, and background on the internet to find the reason behind the conclusions made by data.

- 3. *[Part One](Part1.html)* - This file is about *[Usa_CancerRates_All_ByCounty.csv](https://github.com/gx26/Cancer_Rate/blob/master/Datasets/USA_CancerRates_All_ByCounty.csv)* analysis, because the data set is very clean without null value, it is mainly visualization and feature engineering. Finally, the cleaned dataset was generated in order to analyze all the data sets together in part four.

- 4. *[Part Two](Part2.html)* - This file analyzes the *[us_dataset_powerplants_locations_nature_count.csv](https://github.com/gx26/Cancer_Rate/blob/master/Datasets/US_Dataset_PowerPlants_Locations_Nature_County.csv)*. Because there are few columns in this data set, I decided to draw the geographic information graph by given longitude and latitude. Two interactive graphs are made from Folium package. And at the end I convert latitude and longitude to state and county, so that at part four I can merge three data sets according to county and state.

- 5. *[Part Three](Part3.html)* - This file is an analysis of *[superfund_cleaning.csv](https://github.com/gx26/Cancer_Rate/blob/master/Datasets/superfund_cleaned.csv)*, a dataset that was linked to the EPA provided by Dr.Ami and then crawled down using beautifulsoup. In this file, the relationship between some variables in the data set and superfund sites' score is mainly studied.

- 6. *[Part Four](Part4.html)* - In this file, I first put three data sets together for analysis. For example, whether the number of superfund sites in a state is related to the cancer cases per 100,000 people in this state, whether the type of power plants primary fuel is related to the cancer cases per 100,000 people in this state, etc. Moreover, after some variables were filtered from the merged data set, cancer cases per 100000 people were modeled using XGBoost, Random Forest, CatBoost, etc. Finally, stacking and blending were attempted, and the lowest RMSE, 11.58 was obtained by blending models.

## **Other thoughts**

  there is no doubt that still have a lot of variables affect the number of cancer, such as personal habits: smoking and drinking, and so on, such as per capita medical resources allocation and so on, all of these in the future can be analysis together, and this report to help me model is more accurate, will also be able to find what is the most important variable affecting the number of cancer, to help the government to further policy arrangements.
