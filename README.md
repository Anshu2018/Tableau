
# Tableau story -Story of Flight Delays and Cancellations.
# By Anshu Shrivastava
version 1: https://public.tableau.com/views/finalproject-v2/Story1?:embed=y&:display_count=yes&publish=yes
version 2: https://public.tableau.com/profile/anshu2510#!/vizhome/finalproject_v3/Story2?publish=yes
version 3: 

# Summary
The data set contains information on United State flight delays and performance. The data comes from RITA. Here are some of the common terms and definitions:

FlightNum :	flight number
AirTime : 	in minutes
ArrDelay : 	arrival delay, in minutes
DepDelay :	departure delay, in minutes
Origin : 	origin IATA airport code
Dest :	destination IATA airport code
Cancelled : 	was the flight cancelled?
CancellationCode	: reason for cancellation (A = carrier, B = weather, C = NAS, D = security)
Diverted	1 = yes, 0 = no
CarrierDelay :	in minutes
WeatherDelay :	in minutes
NASDelay :	in minutes
SecurityDelay	: in minutes
LateAircraftDelay	: in minutes

The busiest airport is Atlanta followed by Chicago. Even though Atlanta has most flights the cancellations are not as high as Chicago. Chicago has 3 times more cancellations compared to Atlanta.
If we look at the carriers, the American Eagle Airlines has the maximum cancellations followed by American Airlines. On the other hand Southwest Airlines has maximum diversions and is in the top four airlines for cancellations as well. The main reason for cancellation seems to be weather followed by Carrier.
Bellingham leads in weather delays. The month of December has most arrival and departure delays which could be due to snow or icy conditions, with minimum delays during the month of September and October.
National Aviation Systems(NAS) delay and weather delay is minimum for Hawaiian airlines. National Aviation System delay is maximum for Jet Blue airlines.
The Average taxi out in the month of February and June is higher than the average Taxi in time.
The Security delays peak on Fridays of the week. The maximum number of flights take off in the month of March and July.

# Design: 
I had to limit the data to a particular year (2008). The data is vast and due to file sizes I had performance issues loading the desktop. I tried converting the .csv to excel file but the performance issue wasn't resolved. I had to change some of the data types from number to Date and Month format.  I also converted the variables from dimension to measure and vice versa. The first story shows the busiest airport by origin and chose to portray this through a map. The second story displays the airports and cancellations. I chose the size bubble to show the airports that have most cancellations(ORD). I found it interesting that even though security seems to take a lot of time in the airports but the delays related to it are under 3 min. Next story displays cancellations and diversions by carrier. Story 5 depicts delays related to weather with Bellingham leading. Story 6 displays all different delays related to Weather, NAS, arrival and departure.
I used average aggregation on delays that are measured in minutes. For example: weather delays, arr Delay, dep Delay etc. For Cancellations I used Sum aggregate to get total number of cancellations.
I used hierarchies on monthly data and grouped it by month and weekdays.
In the story Delays Overview used dual axis to compare two variables in the same plot.  Used the dual axis on Flight cancellations or diversions by carrier worksheet as well.
 Calculated fields let you create new fields to use in visualizations.  I used calculated fields in the delays and cancellations by day of the week worksheet. The calculated field called Average delay is average of arrival, departure, NAS, security and late aircraft delays. 
The dual axis was added to compare this Average delay calculated field against cancellations over the week.
I used interactive filters for pairing down lots of visual elements. For example Airports, carriers, month etc.

# Feedback: 

Hello Anshu
Here are some of my humble suggestions:
Story 3:
I am afraid, I would suggest removing story 3. Under 3 min delay does not add a much
Story 4:
I would be sorting bar graph under "Cancellation Reasons"  for clarity.
Help: https://www.ryansleeper.com/3-ways-to-make-beautiful-bar-charts-in-tableau/
Story 5:
For clarity, I would suggest adding minutes to  title "Weather delay by origin "


# Resources: 
https://www.transtats.bts.gov/OT_Delay/OT_DelayCause1.asp?pn=1


