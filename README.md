# Cyclistic_bike_Share-Analysis


Overview Of Bike-Share Offering
Launched	Bicycles [Geo -Tracked]	Stations Across Chicago	Membership
2016	5824	692	"Single Ride Pass
Full Day Pass
Membership Pass"


Goal Of the Analysis with Ask-Prepare-Process-Analyze-Share-Act
Ask Phase

Case Study Roadmap - Ask Guiding questions
 ● What is the problem you are trying to solve?
 ● How can your insights drive business decisions? 
Key tasks
 1. Identify the business task 
2. Consider key stakeholders
 Deliverable: 
A clear statement of the business task
The main goal of the analysis is How do annual members and casual riders use Cyclistic bikes differently.
Download the trip data of  here https://divvy-tripdata.s3.amazonaws.com/index.html.  

Prepare And Process Phase:


We need to combine the data from 2022 in which we have 12 .csv files for that we will be using python to do that task 
We Concatenate all the files to one file we will work on this [Note: when combining all the files make sure it has same column files if it didn’t have the same column names then make sure you rename the columns based on that. 
We add extra columns like date, day, month, day of week which is useful for further analysis.
We calculate ride length based on columns started_at and ended_at to get the time difference and use it for further analysis
Now we have the respective values we can delete any any blank values or null values with this lines.
Finding Key Parameters Using Pandas
Count of Casual members with the Cyclistic members:
Having Casual members of 196964 approx. 1.9M and 309671 approx. 30M members are shows that majority of people are members of Cyclistic so there is high chance to upgrade the casual members to the members of cyclistic .  
Preference of Rides In a Week


Here 1 represents the Sunday going up to 7 for the Saturday Based on Count People prefer going on rides on Saturdays and Fridays.  
Descriptive Analysis:
Calculate the mean of ride_length
Mean of the Ride_Length = 1025.710490552392 [ ..in seconds]


Calculate the max ride_length 
Max Ride = 2061244.0000000002 [..in seconds]


Calculate the mode of day_of_week 
Most Rides happened on = 7 (Saturday)


Average Ride Length
 Average ride_length
casual     00:23:37
member   00:12:55

Average of Ride Length based on week Per Membership:


From this we can say that casual members prefer to travel on the weekends for more places and members are travelling more places in weekdays either for work or travel. 
Lets visualize this reading using Matplotlib.
Comparing with No Of Riders vs Day Of week shows casual people has highest no of riders in Saturday and members has highest in Thursday.

2022 in Numbers

Here,  we can see the casual people are travelling more duration and has average length of 20 minutes and Members has the average length of 12 minutes.

https://public.tableau.com/views/GoogleDataAnalyticsCapStoneProject-CyclisticBikeShareAnalysis/RideDurationComparison?:language=en-US&:display_count=n&:origin=viz_share_link

2022 Cyclistic Ride Duration Comparison
Use the power of data storytelling through interactive charts! I Used a Bar chart to visualize your large sets of data while maintaining their hierarchy and relationship. This chart is interactive, which means you can click and zoom in on a specific section or subsection.

Key Analysis
Summary

                                                       
 Total Trips in 2022 - Month

                           
https://public.tableau.com/views/GoogleDataAnalyticsCapStoneProject-CyclisticBikeShareAnalysis/TotalTripsin2022-Month?:language=en-US&:display_count=n&:origin=viz_share_link
From this we can see that there is more no of riders during the months of June and July and slowly decreasing in November and December 
People tend to use cycles during sunny days. same goes for casual and our members. 
 Rideable Type Preference in 2022

     
https://public.tableau.com/views/GoogleDataAnalyticsCapStoneProject-CyclisticBikeShareAnalysis/RideableTypePreference?:language=en-US&:display_count=n&:origin=viz_share_link
People tend to use electric bike during the 2019 - 2020 cyclistic has more riders want to use the Docked Bike.
During the 2020 our members has shifted towards the classic bike after a ride in usage of electric bike in 2022 Our riders Preference has shifted towards the electric bike showing 56% of our members used the electric bike and also there is significant people who has used our classic bike 
we can attract casual riders by increasing the stock of electric bike since more casual people are preferring to use the electric bikes. 

Rides In A Day

What measures can a company take to innovate and grow in the industry by considering the key KPI of their business
https://public.tableau.com/views/GoogleDataAnalyticsCapStoneProject-CyclisticBikeShareAnalysis/RideInday?:language=en-US&:display_count=n&:origin=viz_share_link
 As you can our riders usually prefer rides from morning peak times and afternoon peak times which tells that reason for using our services to travel to their offices.
Both casual and members has the same preference but during the weekdays the casual people will use our rider during the afternoon times. 
However, when it comes to weekends there are more casual people than members using our rides during the afternoon times.


Weekdays Vs Weekends

What our Riders will prefer Weekday vs Weekends ? 

https://public.tableau.com/views/GoogleDataAnalyticsCapStoneProject-CyclisticBikeShareAnalysis/WeekDayVsWeekends?:language=en-US&:display_count=n&:origin=viz_share_link

The above Pi-chart shows that comparison of our rider type with the days of week 62% of our casual rider prefer to travel on weekdays and 37% prefer to travel on weekends
Members prefer to travel during weekdays having high preference of 75% when compared to weekend which has only 24%.

Season Preference

https://public.tableau.com/views/GoogleDataAnalyticsCapStoneProject-CyclisticBikeShareAnalysis/Seasons?:language=en-US&:display_count=n&:origin=viz_share_link

The Pie-chart shows the rider preference WRT to the Seasons
The casual and member both prefer to travel in the summer months when compared to winter.
It is natural that many people prefer car or bus during winter times rather than cycles. 
After summer most people want to ride in cycles during autumn Season it is the perfect season to enjoy the rides by the cycles.
Top Popular Stations
This section describes the what places our riders prefer to travel from and Popular places they want want to travel to
Top 10 Start Stations

https://public.tableau.com/views/GoogleDataAnalyticsCapStoneProject-CyclisticBikeShareAnalysis/Top10StartStations?:language=en-US&:display_count=n&:origin=viz_share_link
The above map tells top 10 popular places our riders frequently travel from one among them is Streeter Dr. & Grand Ave. is near a very popular pier in Chicago and a Museum, I would conclude people use the bikes for fun and to get to and between points of interest. Lake Shore Dr. & Monroe St. and Lake Shore Dr. & North Blvd. are near Grant Park which is a great place to go bike riding, so I’m inclined to conclude that the reason customers use it if for leisure.  
The other place is DuSable Lake Shore Drive and Monroe Street area: 
This area is situated along Lake Michigan, offering beautiful views of the lake and the city skyline. Biking along the lakefront provides a scenic and enjoyable experience.
Overall, the DuSable Lake Shore Drive and Monroe Street area offers a combination of natural beauty, recreational opportunities, and convenience for cyclists, making it a popular spot for biking in Chicago.
   
Top 10 End Stations


https://public.tableau.com/views/GoogleDataAnalyticsCapStoneProject-CyclisticBikeShareAnalysis/Top10EndStations?:language=en-US&:display_count=n&:origin=viz_share_link
Here it Shows that Top end locations are popular places where our riders travel within the places and not to go to the different destinations.         
"Casual Riders: Start and end their journeys near parks, museums, along the coast and other recreational sites.
Members: Start and end their trips close to universities, residential and commercial areas."


Key Takeaways: 


"Takeaway 1:
"	"The casual riders are taking more times in their rides when compared to the members so, there is high chance that we can convert them to our member by giving them Extended Ride times so they can explore the city at their own pace.
Multi-Ride Packages Introducing packages or subscriptions that allow casual riders to purchase multiple rides at a reduced rate. This can encourage them to use our service more frequently."

"Summer-Only Bike Models: Introducing special summer bike models that are lightweight, equipped with features like water bottle holders, and designed for warm-weather riding. Offer these bikes exclusively to members
Early Access to Summer Events: Provide members with early access to summer events and festivals. They can reserve bikes in advance for these events, ensuring a seamless experience."	"Takeaway 2: 
"

"Takeaway 3:
"	"Guided Tours: Collaborating with local museums and cultural institutions to provide guided bike tours. Offer discounts to members, making it an exclusive benefit. These tours can be educational and informative, enhancing the museum experience.
 Lake Cleanup Initiatives: Promote environmental responsibility by organizing lake cleanup events. Members who participate can earn rewards or discounts on their memberships."



Outlook
By stocking more electric bikes and the charging stations in the popular places can be more useful in the future and by using this key takeaways we can convert our casual riders to the cyclistic members.
“Life is like riding a bicycle. To keep your balance, you must keep moving”
Further Reading
Supplementary material
Cyclistic PDF
R Script
Other links

Contact
For further information, please reach out to us at Cylistic.com.

