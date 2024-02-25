In this notebook, we analyze New York’s Vehicular crash data available at https://data.cityofnewyork.us/Public-Safety/Motor-Vehicle-Collisions-Crashes/h9gi-nx95

The data contains information from all police reported motor vehicle collisions in NYC. The information for this dataset is collated from the police report, called MV104-AN, which is required to be filled out for collisions where someone is injured or killed, or where there is at least $1000 worth of damage.

Data is available from 2012-07-01 onwards, however for this analysis, we will limit ourselves to the period up to 2023-08-15, which is when the data was downloaded.

We find that this data contains over 2 million observations, which allows us to explore several aspects of vehicle crashes in NY's boroughs.

The data dictionary for the data is also available at the URL above.

First, we perform unstructured exploration of the data, and then try to answer the following questions:

We look for which borough has had the maximum number of crashes reported since 2012.

We relate the number of crashes to to the borough's population to find out which borough has the maximum number of crashes for every 100,000 people. Even though the data does not have this information, we can combine the crash data with the population estimates for the boroughs also available from the City of New York's website (https://data.cityofnewyork.us/City-Government/New-York-City-Population-by-Borough-1950-2040/xywu-7bv9)

Borough	Population
Bronx	1446788
Brooklyn	2648452
Manhattan	1638281
Queens	2330295
Staten Island	487155
We look for the leading cause of crashes

We also look for the top-3 causes of crashes, and try to calculate what proportion of all crashes are caused by these top-3 causes.

We then look to some of the more serious implications of crashes by examining how many accidents involved at least one fatality.

We then compute, on average, out of every 1000 accidents, how many have resulted in at least one person dead.

We also look for missing data and try to compute the proportion of accidents in the data that do not have a Borough code.

The fields 'VEHICLE TYPE CODE 1' and 'VEHICLE TYPE CODE 2' represent the first two vehicles involved in the accident. We look for which combinations of vehicles have the most number of accidents.
