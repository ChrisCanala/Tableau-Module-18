Challenge 18 - Tableau

Link to Tableau Visualization: https://public.tableau.com/app/profile/chris.canala/viz/MyFirstViz_17210967638020/CitiBikeJerseyCityFebuary-April2023?publish=yes

I collected Febuary 2023, March 2023, and April 2023 data from the New York CitiBike data website fo Jersey City.

This data had the fields:

Ride ID, Rideable type,Started at, Ended at, Start station name, Start station ID, End station name, End station ID, Start latitude, Start longitude, End latitude, End Longitude, Member or casual ride
In data.ipynb, I combined the CSV files:

converted the member_casual column to True/False rather than strings
mapped the values of the rideable_type column to single characters rather than full strings
"classic_bike" -> "C"
"electric_bike" -> "E"
"docked_bike" -> "D"
dropped all rows that were missing any data

Analysis:

CitiBike Map

The data shows a map of all of the Stations in Jersey City. Over the three months of data the the hottest station were the ones in downtown Hoboken and Downtown Jersey City. The farther away from those areas the less stations and less popularity. locations for rides remains in central Manhattan for all three months.

Total Statistics

On this dashboard we see the total values for the 3 months and can see some interesting trends.

Majority of the rides are less than 5 minutes with majority of all rides beening less than 20 minutes. It is interesting to look at the avg ride duration of non members as they are nearly double that of memebers which could be due to them being tourists and not as familiar with the area.

Popular Stations

The most popular stations for beginning and ending rides are in downtown Jersey City and downtown Hoboken. This is likely due to the high density of housing and populations within the areas.
Some stations have very similar counts of start and ends which would align with commuters using the same 2 locations to commute to and from work. 

Time & Day Statistics

The data shows that the peak usage occurs during the weekdays around 8 AM and then gets busy again between 6-8PM. We can conclude based upon this info that the most usuage is by commuters to move around quickly and with more ease during times of high traffic.
