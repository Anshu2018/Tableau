
# Tableau story -Story of Flight Delays and Cancellations.

# By Anshu Shrivastava
   ## version 1: https://public.tableau.com/views/finalproject-v2/Story1?:embed=y&:display_count=yes&publish=yes
     
   ## version 2: https://public.tableau.com/profile/anshu2510#!/vizhome/finalproject_v3/Story2?publish=yes
     
   ## version 3: https://public.tableau.com/profile/anshu2510#!/vizhome/finalproject_v4/Story2?publish=yes
   ## version 4 (FINAL) : https://public.tableau.com/profile/anshu2510#!/vizhome/finalproject_v5/Story1?publish=yes

# Summary
#### The data set contains information on United State flight delays and performance. 
     The data comes from RITA. Here are some of the common terms and definitions:

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
### My first design consideration was to analyze the volume of flights per origin. I used geolocation plot and size to display the volume. I also used count aggregation on Flight num attribute. Then I wanted to find the number of cancellation per origin, used sum(cancelled) to get this information. I had to convert the cancelled attribute to measures.
### My second design consideration was to analyze the carriers against delays and diversions. I used dual axis to compare the two variables. 
### Next I wanted to see what was the main cause of cancellation. I wanted to analyze this against carriers hence added carriers to categorize. I used different colors to represent the carriers in the bar chart. American Airlines seems to top the cancellations due to weather or carrier.
### Since we were focusing on the weather delays I wanted to also look at average weather delays in minutes by airports. I formatted Month and added to the graph to display if a particular month had higher weather delays. I wanted to break down even further by months to see if the delays had a high and low point during a particular time of the year. A line graph seemed to be a better choice to visually point the high and lows.
### I used the hover tool tip throughout to easily find the details related to carrier, airport or the metric. I also used filter for the viewers throughout the story.
### In order to make it more audience friendly I joined the two .csv files airport,csv and carriers.csv to display the full carrier names and airport names. 
### Calculated fields let you create new fields to use in visualizations.  I used calculated fields in the delays and cancellations by day of the week worksheet. The calculated field called Average delay is average of arrival, departure, NAS, security and late aircraft delays

### The dual axis was added to compare this Average delay calculated field against cancellations over the week.
 

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


