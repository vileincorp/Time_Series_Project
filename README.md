# Time Series Project
![Time Series](https://marmore-assets-v2.s3.eu-west-1.amazonaws.com/insights/migrated/GCC-Stock-Markets-Positive-earnings-growth-strengthen-business-optimism_1200x600.jpeg)

By Keanan Ginell, Luke Sims, Alvaro Rodriguez
**General Overview:**

We will be forecasting real estate prices for various zip codes in the Washington DC area using data from Zillow Research. In this project, we are acting as a consultant for WASHINGTON MOVES, a real estate investment firm. The firm has posed several questions that we aim to answer:

1. What are the forecasted prices for homes in these zip codes after 2018?
2. What are the percent changes in return on investment in these areas based on the Median House Sales?
3. Which are the top 5 best zip codes for us to invest in?
4. Which model best captures the variance in house pricing in the DC area after 2018?

We have provided the dataset, which can be found in the file "time-series/zillow_data.csv," to simplify the process. The dataset was obtained from Zillow Research Page.

The goal of this project is to assist politicians in making informed decisions about purchasing or selling homes in the area. By identifying the best time to enter the market for home purchase or sale, we aim to help them maximize their returns while serving in Congress.

**Business Understanding:**

Every 2-6 years, elected officials and their families need to navigate the DC real estate market to find suitable investments or properties to reside in. This creates additional stress and can artificially affect the local real estate market, leading to a bubble.

Our company utilizes predictive time series analysis to assist elected officials in making strategic property purchases and sales, enabling them to maximize their returns while serving the nation.

**Data Understanding:**

The data was collected from Zillow's Research Page, encompassing approximately 3.4 million homes across the United States. We narrowed down the dataset to 11,395 homes located in the 21 counties of Washington DC. The timeline of house prices in the dataset spans from 1991 to 2018, with prices ranging from a minimum of $30,200 to $1.6 million (USD).

**Data info:**

- RegionID: Zillow's unique identifier
- RegionName: Zipcodes (renamed as zipcode)
- City: City
- State: State
- Metro: Metropolitan area
- CountyName: County
- SizeRank: Ranking of zipcode sizes
- Other columns represent various data and their median monthly house sales.

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
--------
├── Final Political Presentation (pdf Presentation)
--------
├── Time_Series_Notebook.ipynb
--------
├── Zillow Data (dataset)
--------
└── README.md
