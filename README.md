# Urban-Oasis-Capstone-Project

## Description 

The following project is an in depth analysis on the effects of water scarcity and their causes can be countered from the implementation of Vertical Farming. To give a brief description of what is vertical farming, here is as follows: Vertical farming is a type of agriculture that involves growing crops in vertically stacked layers, using various technologies such as hydroponics, aeroponics, or aquaponics, inside a controlled environment. The stacked layers can be in the form of shelves, racks, or towers that maximize space utilization and allow for higher crop yields per unit area than traditional farming methods.

In a vertical farm, plants are grown in a soil-free medium or nutrient-rich water solution with artificial lighting, temperature control, and air ventilation systems to mimic natural conditions required for plant growth. The controlled environment helps to eliminate the risks of pests, diseases, and weather-related problems that may affect traditional farming methods.

Vertical farming is considered an innovative and sustainable solution to overcome the challenges of traditional farming, including land and water scarcity, climate change, and food security. It also provides the opportunity to grow fresh and healthy produce in urban areas where access to fresh and healthy food is limited.

Our team from Correlation One's Data Science for All fellowship program wanted to gain insights of not only the increasing benefits of vertical farming compared to traditional farming, but also if vertical farming can help counter the increasing effects of climate change, such as, water scarcity and food shortage. 

## Description of Data used for Analysis  

We retrieved data from the open data website Kaggle.com. Upon our search we decided to use three main datasets: Global land temperature, UN Crop Data, US Geographical Water Use Index.

The global land temperature data consisted of major cities accross the world, Countries, states, and counties. We filtered and extrated the data that only consisted of major US cities and US Counties by State. 

The UN Crop data was gathered to extract and filtered based on the same metrics as the temperature dataset. As for the Water Data, we were able to retrieve a water scarcity index and connected our datasets with the relevant metrics in order to narrow down the places in the US with the high water scarcity percentages. 

## Exploratory Data Analysis - Crop Yield Data

In the crop/yield analysis, we conducted analysis through the usage of Python's Pandas library to determine the correlation between crop yeild and temperature. Dataset containing temperature and yield data for 10 crops accross 118 countries over a 50 year period were extracted, cleaned and manipulated. Additionally, Pearson's coefficient and p-value were calculated to determine the correlation between crop yeilds and temperature. In the jupyter notebooks, you will see that the results revealed a high positive correlation between crop yeild and temperature with some crops more sensitive to temperature changes than others such as, leafy green crops. 

## Exploratory Data Analysis - Temperature Analysis 

Continuing to use Python's Pandas library, the temperature data was imported fromt he global temperature dataset and filtered to include only rows with "United States" as the country and year "2010". Additionally, we transformed the dataframe to the index of datetime "year" that allowed us to group by "city" and "year". Following this, we took the average temperature for each group, created a 248 column dataframe and plotted a line graph of the temperature throughout the year 2010. 

## Exploratory Data Analysis - Water Scarcity Index

The 2015 Countywide US data contained over 3000 rows and 141 columns with many entries left blank. While we converted data types to floats for aggregation purposes, we used a water analysis, again with Python, to identify correlating data and modeling linear regressions to determine which variables had the greates impact on water demand. 

## Linear Regression Model 

As we created multiple linear regression models from our water data, we noticed both irrigation and thermoelectric power affected the models the most. Due to the scope of our analysis, we only abstracted the irrigation model as vertical farming would benefit most from this. We discovered that through vertical farming, fresh water usage through irrigation can be reduced up to 90% of the normal use of water. Thus, allowing for less water for the same results. 

## Limitations

Some of the limitations that we ran into while doing our analysis is the inability to have up to date data available. Meaning, our datasets were only up to the year 2015. Additonaly, to cross analyze all of our data to focus on water scarcity, food shortage, and temperature data, we were only able to conduct a thorough analysis for the year 2010. This included the combining of US Major Cities, US Counties, Water Scarcity, Temperature, and food supply. Through this we ran the Linear Regression Model as seen above. Further analysis needs to occur in order to gain a more accurate understanding of how Vertical Farming can be applied to major cities in the U.S. However, our analysis was a preliminary starting point for people looking on ways to counter water scarcity and food shortage in an age of climate change and globate warming. 
