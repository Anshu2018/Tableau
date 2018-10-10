
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
# Design: 
I had to limit the data to a particular year (2008). The data is vast and due to file sizes I had performance issues loading the desktop. I tried converting the .csv to excel file but the performance issue wasn't resolved. I had to change some of the data types from number to Date and Month format. The first story shows the busiest airport. The second story displays the airports and cancellations. I chose the size bubble to show the airports that have most cancellations(ORD). I found it interesting that even though security seems to take a lot of time in the airports but the delays related to it are under 3 min. Next story displays cancellations and diversions by carrier. Story 5 depicts delays related to weather with Bellingham leading. Story 6 displays all different delays related to Weather, NAS, arrival and departure.
# Feedback: 
Please provide me feedback on the following:
https://public.tableau.com/profile/anshu2510#!/vizhome/finalproject-v1/Story1

# Resources: 
https://www.transtats.bts.gov/OT_Delay/OT_DelayCause1.asp?pn=1

