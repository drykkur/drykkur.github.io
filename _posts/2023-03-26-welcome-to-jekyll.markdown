---
layout: post
title:  "Traffic collisions in NYC 2012-2020"
date:   2023-05-10 13:33:49 +0200
categories: jekyll update
---

We are going to show the story of robberies in San Francisco, by analyzing patterns time and location of this crime type. The analysis is build on the historical Police Department Incident Reports from 2003 to 2018 of the crime reports from the San Francisco Police Department. For this analysis we have chosen to focus of the years 2004 to 2017.

#### Time-series plot
On this calendar plot we see an indication of the amount of robberies on each day over the years 2004, 2008, 2013 and 2017. This plot is great for creating an overview of the days, months and years. From looking at the plot, we see that the years with the most robberies are 2008 and 2013, as these are the darkest. One the contrary, the year 2017 is the lightest, and hence the year where fewest robberies occurred in SF. It is a bit more difficult to find patterns in the months and days, however it seems that there are generally fewer robberies happening in the winter months November, December and January.

![Barplot](/assets/calplot.png)
*A calendar plot showing number of robberies commited in San Francisco by day for the 4 covered years. The colour of a day indicates the number of robberies committed that day, as described by the colour legend*

#### Chloropleth map
Below, we see map plots of the different areas in San Francisco, again in the four years; 2004, 2008, 2013 and 2017. The map plots are used to visualize the number of robberies in each district relative to the others by color. From these plots we can confirm what we saw from the calendar plots, that 2008 and 2013 were among the years with the most robberies. We also notice that the districts 'SOUTHERN' and 'MISSION' seems to be the districs that struggle most with robberies over the years. On the other hand, 'RICHMOND' and 'PARK' have stayed the areas with fewest robberies over the years. When comparing these finding to the average income of people living in the different areas of SF, we see that the areas with most robberies correspond to the areas with the lowest average income, whereas the opposite apply to the areas with fewest robberies. The data on income is found [here](https://www.opportunityatlas.org/).

![Chloropleth map](/assets/mapplot.png){:class="img-responsive"}
*A chloropleth map showing number of robberies in San Francisco by area covered by each police district. The colour of an area indicates the number of robberies committed in said area, as described by the colour legend*

#### Interactive plot
Next, we see an interactive bar chart of the total number of robberies in SF each year from 2004 to 2017. The plot is interactive, so hovering over any of the bars will show additional informations including a specific number of robberies and the number of robberies in each of the 10 districts. Again, we are confirmed in the observation that most robberies occur in 2008 and 2013. We also see that the years 2010, 2011 and 2016 were the years with fewest robberies. An overall trend is hard to spot, as the total count is fluctuating from year to year, but we do see a relatively stable robbery count in the years 2014 to 2017.

{% include plot.html %}
*An interactive plot of robberies committed per year in San Francisco. Hovering over the bars displays the exact value for robberies committed that year as well as the number of robberies commited per district.*


From this analysis we have gained insight on the robberies in San Francisco. We have seen how the number of robberies have changed over the years, and how it was still an issue in 2017. We have discovered that the number was stable in the last 4 years of the analysis, but also that it was not improving. Additionally it was seen that further work can be done to reduce the number of robberies in SF, by focusing on the parts of town with low incomes, as the districts here have more robberies than the neighboring districts.

![Percentplot](/assets/percentplot.png)


![colcal](/assets/collissioncalendar.jpg)


![injcal](/assets/injuredcalendar.jpg)


![fatcal](/assets/fatalcalendar.jpg)


{% include collissionmap.html %}


{% include injurymap.html %}


{% include fatalmap.html %}

