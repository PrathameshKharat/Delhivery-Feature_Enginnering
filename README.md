# Delhivery-Feature_Enginnering
Delhivery is the largest and fastest-growing fully integrated player in India by revenue in Fiscal 2021. The Data team builds intelligence and capabilities using this data that helps them to widen the gap between the quality, efficiency, and profitability of their business versus their competitors.

Business Insights : 

1. Most trips use "Carting" (~8K) transportation type as opposed to "FTL" (~4K).
2.  Bengaluru, Mumbai and Gurgaon are both the top source and destination cities. Bhiwandi, Delhi, Hyderabad, Chennai, Pune and Chandigarh are also some of the top contributors. So we see that the Southern, Western and Northern corridors have the top contributing cities.
3. The top contributor states (both source and destination) are  : Maharashtra is the highest, followed by Karnataka, Haryana, Tamil Nadu and Telengana, Delhi, Gujarat, UP and West Bengal. Again we see Western, Southern and Northern corridors have significant contribution to the traffic.
4.  The greatest amount of time was spent in intra-state trips within Maharashtra,Karnataka, Tamil Nadu, Telengana, UP.
5. The greatest amount of distance was covered on inter-state trips in Karnaataka, Maharashtra, amil Nadu, Telengana and Andhra.
6. Similarly, the greatest amount of time was spent in intra-city trips within Bangalore, Mumbai, Hyderabad. A significant time is also spent in inter-city trips from Mumbai to Bhiwandi and Guragon to Delhi. These routes also contributed to the greatest amount of distance covered on trips.
7. Hourly distribution of number of trips in a day : minimum trips occuring during the day hours (8 AM to 1 PM) and maximum occuring during late night or early morning hours (8 PM to 2 AM).
8. Week Day : we see that maximum number of trips are happening on Wednesday and minimum on Sunday.
9. OSRM seems to be calculating time taken as less than what time it actually takes. This might be because in actual scenario, there might be delays caused by unprecedented traffic or other delays.
10.  OSRM seems to be calculating distance as less than what distance is actually covered. So, OSRM is underestimating time and overestimting the distance.
11. The time taken by full truck load deliveries is on average, a lot higher (>300 hours) (this is because the distance covered by trucks is also mucvh higher since they don't make stops) than the cart deliveries (<100 hours). The full truck load deliveries cover much longer distances on average (>150 kms) than carting deliveries (~ 25 kms).
12. Hourly distribution of trip time and distances : Time and distances follow similar trends against the hour of the day. Maximum time and distance deliveries are likely to be made during peak morning hours of 10 AM to 12 PM as well as 5 PM, 7 PM and 1 AM. 
13. Weekday distribution of trip time and distances : On average, time taken is slightly more on weekdays and Sunday as compared to Saturday. However, they are very similar. Distances covered is also lowest on Saturday.
14. Route type of top 3 Destination states : Maharashtra has 86% Carting and 14% FTL, Karnataka has 86% Carting and 14% FTL, Haryana has 81% Carting and 19% FTL.
15.  Route type of top 3 Source states : Maharashtra hs 85% Carting and 15% FTL, Karnataka has 88% Carting and 12% FTL, Haryana has 75% Carting and 25% FTL.


Recommendations :
1. Since there is significant dfference between the time and distances calculated by OSRM with actual time and distances, it might make sense to revisit the information which is fed to the routing engine for trip planning. We need to check for discrrepancies with transporters nd to check if the routing engine is configured for optimum performance. 

2. We have seen that the Western, Southern and Northern corridors have significant traffic, however, not so much in Eastern, Central and North Eastern corridors. Increasing the presence in these corridors is worth investigating.

3. There is a need to plan resources (specifically during regional festivities) in the states/cities which have highest contribution to traffic. 

4. Road network can be taken into consideration to increase the number of FTL deliveries inter state and to connect the states where there is lower traffic. 

5. Since intra state or intra city trips are more likely to be using "carting" as mehod of transport, the number of hubs could be increased in those cities and states which have highest contribution to traffic.
