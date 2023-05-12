# Time Series Project
![Time Series](https://marmore-assets-v2.s3.eu-west-1.amazonaws.com/insights/migrated/GCC-Stock-Markets-Positive-earnings-growth-strengthen-business-optimism_1200x600.jpeg)

By Keanan Ginell, Luke Sims, Alvaro Rodriguez
# General Overview
We will be forecasting real estate prices of various zip codes using data from Zillow Research in the Washington DC Area. For this project, we will be acting as a consultant for WASHINGTON MOVES real-estate investment firm. The firm has asked us what seems like simple questions:

- What would be the forecasted prices for these homes after 2018?
- What are the percent changes in return on investment in these areas based on the Median House Sales?
- What are the top 5 best zip codes for us to invest in?
- What model best shows the variance in house pricing in the DC area after 2018?

There are many datasets on the Zillow Research Page, and making sure we have exactly what we need can be a bit confusing. For simplicity's sake, we have already provided the dataset for you in this repo -- you will find it in the file time-series/zillow_data.csv.

The goal of this project is to help politicans either purchase their home in the area by observing the best time of entry in the market and for other politicians, would be the best time to sell as they are leaving DC after they are done working in Congress. 

# Business Understanding
Every 2-6 years elected officials from all across the nation and their families have to navigate the DC real estate market to find the best investment/property to reside. This is additional stressor and creates an artificial real estate bubble that can adversely effect the local real estate market. 

Our company uses a predictive time series to help elected officials purchase and sell their property to maximize their returns while they serve the nation.

# Data Understanding
The data was collected from Zillow's Research Page, where there were about 3.4 million homes all over the United States. We narrowed it down to 11,395 homes in the 21 counties of Washington DC. The timeline of the house prices varied from 1991 to 2018 in which the prices ranged from a minimum of $30200 - $ 1.6 million (USD).

Data info:

RegiondID - zillow's own ID
RegionName - Zipcodes, renamed to zipcode
City - City
State - State 
Metro - Metropolitan area
CountyName- - County
SizeRank - ranking of zipcode sizes
The rest - datas and their median monthly house sales

# Models
![SARAIMODEL](https://github.com/vileincorp/Time_Series_Project/blob/main/Images/full_prediction_testing.png)
The house prices in the DC area will be over $700,000 after 2016, with a house price variance of $3000. The house price model is also about 90% effective to the actual model prices, ranging above or below the $3000.

![Average ROIs](https://github.com/vileincorp/Time_Series_Project/blob/main/Images/percentchange%20(1).png)
The yearly percent change for the average return on investments (ROIs) varies from -1% to 2%. The Percent change is at its lowest during 2008 due to the global recession and it hit its peak around 2004, pre-recession. Our client base will also be leaving or entering the DC area every 3-6 years, so we have to take into account that change as well.

![Ideal Zipcodes](https://github.com/vileincorp/Time_Series_Project/blob/main/Images/percentchange_bar%20(1).png)
The top 18 zipcodes for return on investments were based on the mean house prices in their area. The return on investment is dated from the past 22 years beginning in 1996 all the way to 2018. The return on investment ranged from 100 to 800%, where the top five zip codes are 20001, 20002, 20010, 20003, and 20009, respectively.

![Forecasted Model](https://github.com/vileincorp/Time_Series_Project/blob/main/Images/forcasted_2015.png)
The predicted model generates house sale prices after 2018, where the house prices are trending upwards, with a great degree of variance due to upcoming worldwide events. Regardless, the normal degree of variance will still be $3000 from the actual house price.

# Conclusion
- Forecasted prices of these homes trends upwards above 600,000 (USD) after 2018 (within a range of 3000 (USD))
- Percent changes in the median house sales varies from -1% to 2%
- Best five zip codes to invest: 20001, 20002, 20010, 20003,  and 20009, respectively

# Next Steps
![DCMAP](https://github.com/vileincorp/Time_Series_Project/blob/main/Images/dc_maps.png)
- Diplomat Relocation: Helping other diplomats from various countries also find homes in the country where they will be working at specifically

- Corporate Headquarters: Find, assess, and evaluate different homes for specific employees in a corporation once they move to different states after being in Washington DC

- Private Contractors: Non-governmental entities who work closesly with the government; help relocate to different cities after working in DC, or help new contractors coming to DC find a home 

# Repository File Structure
├── Images (for readme, presentation)
├── Final Political Presentation (pdf Presentation)
├── Time_Series_Notebook.ipynb
├── Zillow Data (dataset)
└── README.md
