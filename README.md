# :oncoming_taxi:  PyBer Analysis  :blue_car:  :red_car:


## Purpose
PyBer is a ride-sharing app company that uses Python-based programming.  PyBer wishes to improve access to ridesharing services and determine affordability for underserved neighborhoods using data that highlights the timeframe from January 2019 to April 2019.   

In the initial assignment, an exploratory analysis on ride-sharing data was done.  One file primarily pertained to ride ID/date/fare/city name information while the other pertained to jurisdiction/driver count information.  

In the challenge assignment, Python scripts are used along with Pandas libraries, Matplotlib, and Jupyter Notebook to make more sense of the dataframes and the relationships among the variables.  This included merged information about the total rides and drivers, total fares, average fare per ride and driver, and total fare by city/jurisdiction type.  


### Resources
**Data Sources:**
- [ride_data.csv](https://github.com/Super-Manda/PyBer_Analysis/blob/main/Resources/ride_data.csv)
- [city_data.csv](https://github.com/Super-Manda/PyBer_Analysis/blob/main/Resources/city_data.csv)

**Methods:**
- Jupyter Notebook 6.4.8
- Python 3.10
- Matplotlib Library 3.5.1
- Pandas Library 1.4.2 


## Analysis
Python and Pandas are used to create a summary dataframe of the ride-sharing data by city/jurisdiction type, while Pandas and Matplotlib are also used to create a line graph is presented that shows the total weekly fares for each jurisdiction type. 

## Results

### **Summary Dataframe**

![Summary_Dataframe](https://github.com/Super-Manda/PyBer_Analysis/blob/main/Analysis/Dataframe_summary.png)

In urban areas, the average fare per ride ($24.53) is actually lower than the average fare per driver ($16.57).  This is the opposite in the other areas, where average fare per driver ($55.49 in rural towns and $39.50 in suburbs) exceeds average fare per ride ($34.62 in rural towns and $30.97 in suburbs).  Urban areas boast the highest number of drivers and rides.  The lower fares in urban areas are, therefore, offset by the brisk business, which means that urban areas still bring in the most amount of revenue compared to suburban and rural areas.  

 
### **Percent of Total Fares by City/Jurisdiction Type** 
![%Total_Fares_by_CityType](https://github.com/Super-Manda/PyBer_Analysis/blob/main/Analysis/Fig5.png)

- Urban areas accounted for 62.7% of total fares.  Suburban areas accounted for 30.5% of total fares.  Rural areas accounted for 6.8% of total fares.


### **Percent of Total Rides by City/Jurisdiction Type** 
![%Total_Rides_by_CityType](https://github.com/Super-Manda/PyBer_Analysis/blob/main/Analysis/Fig6.png)

- Urban areas had 68.4% of total rides, while suburbs had 26.3% and rural areas had 5.3%.  Therefore, relatively, it may be logical to slightly increase the number of drivers available in suburbs and rural towns so that those customers can be better served, but it would be too premature to conclude that the increased fare amount in the suburbs and rural towns could drive away customers who truly need the service because this dataset doesn’t account for the duration of the trips.  The current high gas prices will also be a factor in whether anyone would want to sign up to drive for Pyber and whether people would ride.  


### **Percent of Total Drivers by City/Jurisdiction Type** 
![%Total_Drivers_by_CityType](https://github.com/Super-Manda/PyBer_Analysis/blob/main/Analysis/Fig7.png)

- Urban areas employed 80.9% of total drivers, while suburbs employed 16.5% of total drivers and rural towns employed 2.6% of total drivers.  Without the trip duration, it would be hard to give the specifics of how to match the ostensibly excess drivers of the urban areas with the ostensible demand of the suburbs and rural towns, but at face value, the data shows that there are good paying customers out there who could use more drivers.  


### **Total Fare by City/Jurisdiction Type**
![TotalFare_by_JurisdictionType](https://github.com/Super-Manda/PyBer_Analysis/blob/main/Analysis/PyBer_fare_summary.png)

- On a weekly basis, the average sum of fares for rural is $230.22, the weekly average sum of fares for suburban is $1051.96, and the weekly average sum of fares for urban is $2180.34.  This suggests that increasing drivers alone cannot solve the problem; it must also be coupled with new business, particularly in rural towns.

- Total Fare by City/Jurisdiction Type can also show date trends.  For example, the last week of February and the first week in April appears popular in any jurisdiction.  The least popular rural week is the second week of January ($67.65 weekly sum of fares), followed by the third week in February ($95.82).  In the suburbs, the least popular weeks may coincide with New Year’s and Easter/Passover preparations.      

- The first and third weeks of January are relatively less popular in urban areas compared to what they relatively are within the trends for suburbs.  This may be because the snow requires homeowners to dig out, and people may discover that they have cars that do not start or they cannot drive to work because they fell down and hurt themselves.  In urban areas, they may have city sanitation workers who do much of the salting and digging, so less can go wrong on those weeks.  So it may make sense to have urban drivers occasionally pick up the suburban people in those instances, since they’re destined for the city anyway.  


## Key Questions:

### Who might our customers be, and are they apt to be repeat customers?
- In suburban areas, it stands to reason that more people can afford cars, and in rural areas, it stands to reason that mass transit and paratransit is less available, so people may have to drive their own cars to meet their activities of daily living.  If a person can no longer drive, they may opt to live in the cities unless they have a caretaker.  

- The purpose of ridesharing is likely different in the city than in the suburbs or rural towns.  In the cities, it may be primarily used to take people beyond the city limits where mass transit routes have ended, or it may be used to quickly transport businesspeople or tourists from place to place who cannot wait around for the next train or bus.  

- In suburbs or rural areas, it seems more logical that ridesharing would serve people with short-term issues, whose car is at the mechanic being fixed, for example (unless PyBer wants to branch into delivering restaurant food to repeat customers’ doors or something to get new business).  As a mere ridesharing service, the customers may be more random and less likely to be repeat customers, regardless of the fare, in suburbs and rural towns.  In cities, if people like the service they receive, they may wish to be a repeat customer in the near future, unless they’re a tourist.

### Will increasing the supply of drivers meet or increase the demand for them?  

- Regarding the number of drivers, one must determine whether we’re looking at the chicken or the egg: are they low because there is a high need for them going unfulfilled, or are we properly staffed in the outskirts because the rides are long (and hiring any more drivers would leave some drivers without clients, thus forcing them to give up driving).  One must think about this operation more from the perspective of maintaining these drivers as employees/subcontractors than from the perspective of maintaining these same customers, given that it’s established that many of the customers could be random.    

- It may make sense to conclude that increasing the supply of drivers alone would not increase the demand for them in those areas unless population is also increasing in those areas simultaneously; thus, the high price of the ride must offset the fact that this driver will no longer wish to make a living as a driver if he/she cannot earn enough of money per week.  The data does support that we can increase drivers in suburbs and rural areas, but that should probably be done in conjunction with efforts to increase business too.  

### What is the trip duration?
- This will help us determine affordability.


## Recommendations

### 1. Maintain or expand business in urban areas: Keep the same number of drivers in urban areas for now, but have them pick up more rides. 
- **How do we expand business?**  Current events makes it easy to predict the supply and demand of drivers and riders.  For example, Senate Bill S2934 (https://www.njleg.state.nj.us/bill-search/2022/S2934 ) aims to decriminalize psilocybin (magic mushrooms) in this state, putting magic mushrooms on the road to legalization, which goes on top of past legislation that has already legalized cannabis (marijuana).  These could be some of our potential customers who may call for PyBer rides anywhere in the state.  In addition, it means more of an expense for the company to screen PyBer drivers for these additional substances before hire.  Although adding some more drivers in suburban and rural areas makes good sense, there may be diminishing returns of hiring new drivers in general.  Therefore, the idea of making the drivers in urban areas more productive, since they already do a considerable amount of business, could be mutually beneficial because there’d be no new costly hiring processes.  Part of making the drivers in urban areas more productive may also be to give them some incentive to pick up the suburban and rural people who are destined to the urban cities.


### 2. Hire more drivers in the rural and suburban areas

- Regarding how much to increase the drivers by, it’s clear from the dataframe that there are 13x more rides in the urban cities than the rural towns.  The number of drivers in the urban cities is 2405, so dividing that by 13 means that the number of rural drivers should not exceed 185 once business increases.  Since there are only 125 rural rides now, this seems like a good number of rural drivers to aim for in the short-term.  

- Likewise, there are 2.6x more rides in urban cities compared to suburbs.   This means that the number of suburban drivers should not exceed 925, and since there are only 625 rides now, that seems like a good number of suburban drivers to aim for in the short-term.  

- The only reason why the ratio of rides to drivers can go so low in the urban areas is because the riders are spending less time in the vehicle, as cities are laid out closer together.  In the suburbs and rural areas, once the riders enter the vehicle, it likely takes longer to arrive at the destination, so they’re spending more time with the driver.  It would not be wise to go beyond a 1:1 ratio for suburban and rural ride to driver ratio in general, as business increases, because ultimately, the urban cities are simply planned differently. 
 
### 3. Gear advertising toward rural and suburban clients to gain more business; also consider hiring a telephone operator to book and dispatch drivers in those areas.  

- We may have some urban clients who are tourists and businesspeople.  In contrast, we may have some suburban and rural people whose car is temporarily in the shop, but we may also have more elderly people who have grown up in town all their life, but now they cannot drive anymore.  Similar to Eat24, it may make sense to have “cash points” accrue that can be used toward a reduced rate ride in the future to try to foster repeat customers, but it may also make sense to have the zip code trigger different types of advertising.  

- Also, if the market is elderly or disabled, then establishing a phone call hotline option in addition to the standard online booking of the vehicle may help them access the PyBer service.  In that case, it may be possible to hire 1-2 telephone operators who will help to draw that market and increase business.  Many competitors only allow booking through a cell phone or online, and it could be assuming too much that our client has a smart phone or that a rural farm area has cell towers near it.   

- Relative to increasing fares, it makes more sense to try to increase business first and only resort to increasing fares if the marketing campaigns fail to increase business and/or the inflation becomes unbearable.  In that case, a hidden fare increase, such as a fuel surcharge may be more desirable than outright raising fares in terms of the consumer’s impression of the company.  The consumer will not likely want to see prices go up.


### 4. Consider fare pricing in suburban and rural areas after extra drivers are placed there and after more data is gathered about trip duration.  

- If the service is not affordable, consider whether to slightly reduce fares on a trial basis (choose weeks to try it out when business is normally low to average) to establish if that brought more customers in.  If it did not, return to normal rates, because it’s not the affordability causing the issue.  

