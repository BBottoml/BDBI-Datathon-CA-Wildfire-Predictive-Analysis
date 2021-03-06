# BDBI-Datathon-U.S-Wildfire-Predictive-Analysis
2020 BDBI Datathon predictive analysis project for U.S wildfires

## Problem
Wildfires pose significant disruption to daily life for those in affected areas. Although sources like NASA speculate where wildfires may occur, it is simply not feasible to combat every possible wildfire. We need a way to determine which potential wildfires pose the greatest risk to individuals and industry and allocate the necessary resources to fight them. 

## Potential Solution & The Pipeline Solution
Minimize disruption to industry and areas of high population density by preemptively monitoring high risk areas by leveraging predictive analytics. 
To preemptively monitor, we retrieve dynamic, current data from NASA that speculates where wildfires may occur. Based on user refinement, our model looks at a given region and predicts the highest risk regions to inform first responders. Our solution emphasizes the use of dynamic data, low cost initiatives and accounts for economic activity to avoid industry/supply chain disruption. 

## pipeline.py
pipeline.py is our answer to the problem. When the program is ran, it makes a get request to the NASA Active Fire data source to retrieve current information about potential wildfires. From there, we identify wildfires that are suitable for analysis and then proceed to retrieve data about the area based on latitude and longitude. Using our model, we output a CSV file sorted by the most vulnerable locations. We envision first responders and the necessary agencies using this information to allocate resources. 

## Findings
![Image of Severity Score vs. Median Household Income](https://raw.githubusercontent.com/BBottoml/BDBI-Datathon-US-Wildfire-Predictive-Analysis/master/sev_score_vs._median_household_income.PNG)

Ultimately, what we found was that in the most vulnerable locations for wildfires, the median household income is low as you can see in the plot above. This means that the places getting hurt the most are low-income, rural areas where the agriculture industry is most affected. Our findings show that in order to prevent these rural wildfires, more financial resources need to be added so that the agriculture industry does not crumble.

## Complete Presentation
View our complete presentation [here](https://docs.google.com/presentation/d/1jF-VbzMAlVYQEc_hYhQ3EaZn2OGWisH6i93anI_tTao/edit?usp=sharing)
