---
layout: post
title:  "Traffic collisions in NYC 2012-2020"
date:   2023-05-10 13:33:49 +0200
categories: jekyll update
---

New York City is one of the busiest cities in the world, with millions of residents and visitors relying on its extensive network of roads and highways to go about their daily lives. With so many vehicles on the roads, accidents are an unevitable but much too common occurrence. These accidents can have serious consequences, ranging from property damage to severe injuries and sadly also fatalities.
Data can be a powerful tool for understanding and addressing the patterns of these collisions, and we are going to be analyzing a dataset about [Motor Vehicle Collisions in NYC](https://data.cityofnewyork.us/Public-Safety/Motor-Vehicle-Collisions-Crashes/h9gi-nx95), to identify patterns and trends that could help prevent future accidents and improve road safety. This dataset contains extensive information about the circumstances surrounding the collisions, including the locations and times of incidents and also the contributing factors and types of vehicles involved.
This extensive dataset allows us to uncover insights such as seasonal and geographical trends. Additionally, we can make recommendations such as the safest places to drive and whether or not improvements have been made over the years.
So follow along as we uncover the story behind trafic collisions in NYC, and try to work towards a safer transportation system for the city.


### Exploring NYC vehicle collisions and their consequences

New York City hosts almost 9 million residents, making it one of the most populated cities in the world. The city consists of five main boroughs, including Brooklyn, Queens, Manhattan, Bronx and Staten Island. 1,371,448 vehicle collisions have been recorded in the city since 2013 in all of the five districts. 
It is relevant to investigate, where these collisions happen, and to do this we created three different maps where each borough is outlined along with either the number of collisions, injuries or fatalities. These maps are interactive, so the numbers can be seen by hovering over each of the districs.

{% include collissionmap.html %}  
*An interactive chloropleth map showing number of collisions in each of NYC's five boroughs. The colour of an area indicates the total number of collisions occured in said area, as described by colour legend. Hover over a borough to see the exact values*

The first map plot shows the number of collisions. The darker the area is, the more collisions are happening, and as we saw before, most of the incidents happen in Brooklyn. However, Brooklyn, Bronx, Queens and Manhattan are all quite similar in color, and the only real outlier is Staten Island. This shows that Staten Island is experiencing far fewer collisions than the other forur boroughs. The reasons for this will be discussed in further detail later.

Now let's compare this to the map plot below, which shows the number of injuries that result from these collisions.

{% include injurymap.html %}
*An interactive chloropleth map showing number of injuries resulting from collisions in each of NYC's five boroughs. The colour of an area indicates the total number of injuries occured in said area, as described by colour legend. Hover over a borough to see the exact values*


From this plot we see that the color differences are a bit bigger, indicating that there is a larger difference in the number of injuries between the different boroughs. This is especially the case for Bronx/Manhattan and Brooklyn/Queens. Notice also how the geographical location makes boroughs more prone to have similar numbers of incidents.

Let's see if this is also the case for the number of fatalities in the next plot.

{% include fatalmap.html %}
*An interactive chloropleth map showing number of fatalities resulting from collisions in each of NYC's five boroughs. The colour of an area indicates the total number of fatalities occured in said area, as described by colour legend. Hover over a borough to see the exact values*

We immediately notice that the color difference has become smaller, meaning that the difference between the different boroughs has become smaller. But is this because the number of fatalities in Staten Island is higher or because the number of fatalities in the other boroughs are lower?


So far, we have investigated the differences between the boroughs in total numbers. However, we have not taken into account that they all have very different numbers of residents. Many vehicle collisions might just be a result of a high populations and not necessarily anything that can be improved, so let's have a look at the numbers.

Brooklyn, with 31.22% of NYC residents, is the borough with most people living there. On the contrary, only 
5.64% of New Yorkers live in Staten Island. The rest of the boroughs are in between, Queens with 26.91%, Manhattan with 19.01% and Bronx with 17.22%.

Why is this interesting? To answer that question, let's have a look at the plot below. This plot shows the percentage of total collisions, injuries and fatalities in each of the five boroughs in NYC. The blue line is used for reference, and shows the percentage of the population living in each of the boroughs.

![Percentplot](/assets/percentplot.png)
*A line plot showing the percentage of total occurances for each borough. The x-axis consists of the boroughs in descending population order. The lines' meaning is described in the colour legend.*

From the plot above, we see multiple interesting things. First of all, Brooklyn seems to be highly exposed to serious consequences following a collision, as the number of fatalities and especially injuries is very high. It is by far the borough that is most prone to injuries, as 36.09% of those are happening here. 
Brooklyn is closely followed by Queens, which is sadly overrepresented in fatalities when comparing to the number of collisions and injuries. 
Moving on to Manhattan we see a different trend, where the injury- and fatality percent is lower compared to the number of residents. However, in this borough we see by far the highest number of collisions compared to the number of residents. 
Bronx and Queens are both less prone to collisions, injuries and fatalities compared to the other boroughs.  

When interpreting these results, we should consider the types of accidents that each of the boroughs are prone to as a result of the circumstances surrounding them.
We see that there is certainly a clear overrepresentation of fatalities in the two boroughs Brooklyn and Queens. In addition to having the most residents, both boroughs have a higher number of major roads, such as highways. This likely means that accidents happen at higher speeds, which can increase the likelihood of severe accidents. The opposite may apply to Manhattan, where the roads are generally much smaller and the amount of traffic is so heavy that going at high speed is almost impossible. The high number of vehicles might be the cause of the many collisions, while the slow speed can be why fewer of them result in injuries and fatalities.

### Do we see a trend over time?

NYC is continuously working on improving the road safety for pedestrians and drivers in the city. One example of this is [Automated Enforcement](https://www.nyc.gov/content/visionzero/pages/automated-enforcement), where cameras are being installed to catch people crossing red lights and people going more than 10mph over the speed limit in certain zones. The question is, however, do these precautions result in fewer and/or less severe vehicle collisions? And are some boroughs progressing better than the others?  
The plots below show the total number of collisions, injuries and fatalities in each of the different boroughs in the years 2012-2022.

missing image


From the plot above we see the number of collisions for each borough per year.  First of all, we see how the distribution confirms what we say previously, that Brooklyn has the most collisions and Staten Island has the least. 
One thing that really stands out in all of these plots, is the afct that the number of collisions drop drastically in the year 2020 for all boroughs. Not surprising, this is the effect of the Covid19 pandemic, where the roads were left near empty in a long period of time. What is more surprising is the fact that the number of collisions is kept low in the years following the lockdown. A possible explanation for this is that a lot of people were working from home and did not need to commute to work, and also that there were very few tourists in the city in the following years.

Another thing to notice is that Manhattan was successful in lowering the number of collissions by a good amount in the years 2015-2019. Possibly, this is a result of the [Vision Zero Pedestrian Safety Action Plan](https://www.nyc.gov/html/dot/downloads/pdf/ped-safety-action-plan-manhattan.pdf), which contains a detailed analysis of the high-risk areas and plans for improvement.

So how do these trends compare to the number of injuries? Let's have a look at that below.

missing image


This plot surprisingly shows a different trend. We still see a sudden decrease in 2020 for all boroughs, however the number quickly bounce back to the same level as before Covid for most of them. This indicates that even though there are now fewer collisions, they have become more severe so more people are getting injured. Sadly, as we are about to see on the next plot, this is also the case for the number of fatalities. 

missing image

From the plot above we see that the number of people getting killed as a result of vehicle collisions has not gotten lower over the years. If anything, we are seing an upward trend especially in Brooklyn and Bronx. The reson for this should most likely also be found in the Covid19 Pandemic. Based on [this article](https://www.nytimes.com/2021/01/01/nyregion/nyc-traffic-deaths.html), it seems that many people, including young and inexperienced drivers, turned to the roads for a feeling of freedom. This, combined in an increase in drug- and alcohol abuse is likely to have caused the sudden increase.

Now, let's take a deeper look into how vehicle collisions and its consequenses have occured over time. For this, we have chosen to include calendar plots, that can be seen below.

The first one indicates the number of collisions each day of every year, and makes it easy to interpret which periods or days experience more collisions.

![colcal](/assets/collissioncalendar.jpg)

*A calendar plot showing the number of collisions occuring per day for the 9 covered years. The colour of a day indicates the number of collisions occuring that day, as described by the colour legend* 

We very clearly see the effects of Covid on this plot as well. Around the middle of May, the number of collisions decreased by a large amount, and for all of April there were only a few occurences. The trend of there being much fewer collisions than usual continued all through 2022 as well. It is, however, clear that the first week of Covid stands out. This is most likely a result of people being very cautious about being outside of their home and not yet feeling the boredom as described previously. Another interesting thing we see from this plot is outliers. The most prominent outlier is on 21. January 2014. On this day there was a [major snowstorm](https://www.cbsnews.com/newyork/pictures/snowstorm-jan-21-2014/), and it is the effect of this that can be seen as the very dark spot.

One thing is collisions, but another is the human consequenses. Let's have a look at how injuries are distributed over the years.

![injcal](/assets/injuredcalendar.jpg)

*A calendar plot showing the number of injuries resulting from collisions per day for the 9 covered years. The colour of a day indicates the number of injuries occuring that day, as described by the colour legend* 


This plot confirms what we found previously, that the number of injuries actually increased after Covid. Now we can see in more detail what actally happened. The first weeks, from the middle of March to the end of April, there are very few injuries. However, this starts to change around May-June, where the number increases again. Here is stays consistent all the way through 2021 and 2022. About the outlier from before at 21. January 2014, we see no significant increase, so luckily none of the collisions seem to have been severe. However we do see a new outlier on 18. May 2017, where there was a [car attack](https://www.nytimes.com/2017/05/18/nyregion/times-square-crash.html) on Times Square that left 22 people injured in that incident alone.

Lastly, let's have a look at the fatalities.


![fatcal](/assets/fatalcalendar.jpg)

*A calendar plot showing the number of fatalities resulting from collisions per day for the 9 covered years. The colour of a day indicates the number of fatalities occuring that day, as described by the colour legend* 

It is difficult to even find a trend on this plot. We do see a confirmation of what we found earlier, that more people were killed in the middle of the pandemic. Especially the summer months of 2020 was high in fatalities. The very clear outlier that is seen on 31. Otober 2017 is the [Truck Attack](https://www.nytimes.com/2017/10/31/nyregion/police-shooting-lower-manhattan.html) on a bikelane that left 8 people dead.

[Explainer notebook can be found here](https://github.com/drykkur/drykkur.github.io/blob/4ca1cc65eca5fe4377f3e9a03f4cd7739b59e609/src/explainer.ipynb).


### Some discussion/conclusion

Through this analysis we have found a lot of interesting conclusions about the patterns in vehicle collisions in NYC. We found both geographical and time-dependent patterns, both providing valuable knowledge. 

First of all, we saw from the map plots that by far most collisions happen in Brooklyn. This was not only true for the total number, but also for the percentage. The line chart showed how Brooklyn and Queens turned out to be the boroughs where far most injuries and fatalities occur measured in percent. The cause is thought to be the infrastructure in these parts of NYC, as they have a higher number of speedways and highways. Manhattan is victim of having the highest collision percent of all boroughs, however all the while having lower injury- and fatality percent, the expected reason being the large amount of traffic in that borough. 

The unexpected main character of this analysis proved to be the Covid19 pandemic. From the calendar plots we saw how the number of collisions dropped drastically in the middle of March, and stayed there for a few weeks. However, what was even more interesting, is the fact that the number of injuries and fatalities resulting from vehicle collisions increased a lot in the months and years following the pandemic. This all happened despite the successful attempt to lower the number of collisions in the years leading up to 2020 with the Vision Zero Action Plan, and shows how even the best efforts can be destroyed by unexpected events.




















