# 2020 Chesapeake Bay Hackathon _Hack the Bay_ 

1. Introduction

The Chesapeake Bay watershed is home to over 18 million people, spanning 6 states and Washington DC. The Bay is the largest estuary in the United States, providing 500 million pounds of seafood harvest each year. Declining water quality due to pollution and overharvesting in past decades led to poor ecosystem health and the near extinction of economically and culturally important aquatic species. In response to this decline, state and federal partners have invested heavily in restoration efforts, amounting to nearly $1.5 billion of state and federal funding in 2019 alone. Despite many years of costly efforts, warming temperatures, sea level rise, and increasing precipitation due to climate change have hindered the attainment of restoration goals. ([Citation](https://devpost.com/software/enabling-climate-resiliency-for-the-chesapeake-bay))

2. Data Collection

I chose __Water Temperature__ as the indicator. I used the CMC and CBP water quality data set provided by Booz Allen Hamilton. 
For the water temperature, all of the filtered data sets for the analysis and visualization are from the CMC dadabase.
([Link to the raw data](https://github.com/jenli810006995/hack-the-bay))


3. Data Preprocessing

    * Year: I used Python pandas to trim date and time elements from the __Date__ parameter, and filtered 2015 - 2020 as the time window I am interested in.
    * Season: I categorized May to August as __Summer__ , and November to February as __Winter__.
    
4. Exploratory Data Analysis

    * Methodology:
    1. Stationality: Use AF, PACF and Augmented Dickey–Fuller test to check stationality. The water temperature is stationary time-series data. ([Citation](https://github.com/marbakes/pca-arima-fun/blob/master/Data%20Processing%20%26%20Modeling.ipynb))
    2. Summary Statistics: After plotting water temperature within 2015 to 2020, I found the temperature range for the winter has something interesting to look at. Especially after 2017. For Example, the following scale of the winter water temperature reveals the increasing range:
    ![2017 Winter](https://github.com/jenli810006995/Hack_the_Bay_Repo/Images/blob/master/2017_winter_cbp_range.jpg?raw=true)
    ![2018 Winter](https://github.com/jenli810006995/Hack_the_Bay_Repo/Images/blob/master/2018_winter_cbp_range.jpg?raw=true)
    ![2020 Winter](https://github.com/jenli810006995/Hack_the_Bay_Repo/Images/blob/master/2020_winter_cbp_range.jpg?raw=true)
    3. Geospatial Maps:
    ![2015 Summer CBP](https://github.com/jenli810006995/Hack_the_Bay_Repo/Images/blob/master/2015SummerCBPWaterTemperatureHeatmap.png?raw=true)
    ![2015 Summer CMC](https://github.com/jenli810006995/Hack_the_Bay_Repo/Images/blob/master/2015SummerCMCWaterTemperatureHeatmap.png?raw=true)

5. Data Visualization

###### Result

6. Challenges

7. Recommendation

8. Conclusion




