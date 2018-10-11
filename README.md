
# Tableau story -Story of Flight Delays and Cancellations.
# By Anshu Shrivastava
https://public.tableau.com/views/finalproject-v2/Story1?:embed=y&:display_count=yes&publish=yes

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
The Security delays peak on Fridays of the week
# Design: 
I had to limit the data to a particular year (2008). The data is vast and due to file sizes I had performance issues loading the desktop. I tried converting the .csv to excel file but the performance issue wasn't resolved. I had to change some of the data types from number to Date and Month format.  I also converted the variables from dimension to measure and vice versa. The first story shows the busiest airport by origin and chose to portray this through a map. The second story displays the airports and cancellations. I chose the size bubble to show the airports that have most cancellations(ORD). I found it interesting that even though security seems to take a lot of time in the airports but the delays related to it are under 3 min. Next story displays cancellations and diversions by carrier. Story 5 depicts delays related to weather with Bellingham leading. Story 6 displays all different delays related to Weather, NAS, arrival and departure.

# Feedback: 


# Resources: 
https://www.transtats.bts.gov/OT_Delay/OT_DelayCause1.asp?pn=1

