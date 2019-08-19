# Crime Analytics

When deciding where to live in San Francisco over the summer, I found it difficult to find affordable housing. I would be excited to find cheap housing right outside of areas such as the Financial District, only to find that those areas were the ones ridden with crime. Many of my friends had been searching for housing in Chicago and New York and running into similar problems, and this resulted in me thinking about the differences in crime across these cities. After doing some research, I realized that weather can actually be an indicator of crime and wanted to explore this topic further. Since these cities are some of the most populous in the country, I also wanted to see how crime is similar and different between them.

## Methodology
**Tools Used**: R, OpenRefine, Excel, Tableau
Almost all of my analysis and visualizations below are from using R, with a few from Tableau as well. 

**Data Sources**: Weather, San Francisco Crimes (2014-2015), New York Crimes (2014-2015), Chicago Crimes (2014-2015)

**Weather Data**:
I trimmed the data to the 2014-2015 time frame when downloading the dataset, transformed the numbers from Kelvin to Fahrenheit, aggregated by year since the data was given hourly, and got the average temperature for each day. All of this analysis was performed on OpenRefine through the use of GREL and Python functions. I also got data on weather type and utilized OpenRefine to categorize weather description into 6 categories: (Snowy, Rainy, Foggy, Cloudy, Hazy, Sunny). 

**Crime Data**:
I filtered the data for each city to get crimes in 2014 and 2015. I used Excel to sort the data by date and retrieve the day of the week and hour for each crime. Some of the data points that were crucial to my analysis include Date, Category of Crime (eg. assault, theft), City District, and Crime Location (see attached files for more detail).

## Takeaways and Next Steps
Some of the interesting findings from my project:

San Francisco has the opposite seasonal trend in crimes compared to New York and Chicago. This could be due to its more temperate climate.

San Francisco is not as heavy of a "crime hotspot" compared to Chicago and New York, which have high levels of crime for more days and hours of the week. This could be due to San Francisco's lower population.

Crime has interesting hotspots in each city and varies based on time of the year, especially the prevalence of prostitution and different types of theft.

Some improvements/things I would add if I redid this project or expanded on it in the future:

Use more recent data (2017 and 2018)

Try to predict crime based on certain variables (eg. does the district and type of crime have a correlation to the victim's race and/or age)
