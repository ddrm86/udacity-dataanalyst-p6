# P6: Make Effective Data Visualization

### SUMMARY

This visualization shows the number of traffic accidents in Madrid per day of the week, during the period 2009-2014. 

The number of traffic accidents in Madrid is lower during the weekends, especially on Sundays. Friday is the day of the week with more accidents, although the difference with respect to the rest of the weekdays seems to be narrowing over time.

Hover the mouse over the points to get the exact numbers.


### DESIGN

**First version**

The data is presented in chronological order, one measure per year. Thus, a line chart with the pertinent years in the _x_ axis and the number of accidents in the _y_ axis effectively shows the evolution of the number of traffic accidents over time.

Since I want to show the differences in the number of accidents between the days of the week, it is a multiline chart, where every line represents a day of the week. Lines are in different colors so the audience can distinguish between days of the week, and the legend tells what color corresponds to each one. I considered labeling each line with its day, to avoid having to jump from the chart to the legend and back multiple times, but some lines are too tight together.

Since the data is not continuous, a scatter plot is added on top of the multiline chart so the audience can locate every data point in the chart and easily estimate the number of accidents for a particular day of the week and year. A tooltip text is added for every data point to get the exact figure. I decided to override the default tick format, that represent the numbers in thousands (e.g. 1.2k), since the numbers are not large and can be easily read.

I pondered starting the _y_ axis in 1000 or 1200 to avoid wasting so much space and making the lines less cluttered, but since is an often discouraged practice I decided to leave it that way for this version and seek feedback.

**Second version**

Based on the feedback received, I decided to make the _y_ axis start at 1200. Also, I added a short explanatory description with the main findings of the visualization, instructions on how to interact with it and the source of the data.

**Third version**

A friend indicated to me that some lines where hard to follow due to overlapping and similar colors used. Instead of changing color hues to shapes as suggested, I decided to swap the colors of the lines for Wednesday and Friday, to avoid having similar colors (red and orange) for Tuesday and Wednesday, which overlap in several places.

He also suggested using percentage changes or log-transformed values instead of absolute numbers to show in a more faithful way the increasing and decreasing of the number of accident between years. But, since that makes the visualization harder to read for a non-technical audience, and it is not the main message I want to convey, I decided to leave it as it is.

**Fourth version**

The visualization is now centered on the web page, as suggested by the feedback received.


### FEEDBACK

**First version**

_ChaksUdacity_

> Good topic you have chosen...
> Bringing awareness on traffic incidents and how day of the week impacts.
> Since your minimum number is starting roughly at 1200, it may be good to start at this number and you are not twisting the message provided if your aim is to highlight the number of accidents on friday compared to other days (may be everyone in a hurry for a great weekend!)
> 
> Hope this helps!

_Myles_

> Hi David
> 
> 
> What I noticed (combined with relationships that I noticed): 
> 
> There is a clear distinction between traffic accidents on the weekend vs weekdays (i.e. one that doesn't overlap at all), with fewer accidents on the weekend.
> 
> There is a clear distinction between traffic accidents on Saturdays vs Sundays (i.e. one that doesn't overlap at all), with fewer accidents on Sundays.
> 
> During weekdays, there is a clear distinction between traffic accidents on the Fridays vs all other weekdays
> 
> 
> What questions I have about the data: 
> 
> There is no description of the source of the data and how it was gathered, apart from that, overall, it is a very clear presentation of the information that it is intended to convey.
> 
> Is there something you don’t understand in the graphic?: 
> 
> No 

> I think that the visualization looks better when the 'y' axis begins at 1000 as you say. That is not typical but [Mythbusters: Should you start your axes at zero?](http://gravyanecdote.com/uncategorized/mythbusters-should-you-start-your-axes-at-zero/) and [When It’s OK to NOT Start Your Axis at Zero](http://stephanieevergreen.com/non-zero-axis-rules/)

> Overall, a very nice job!!

_Daniel_

**Second version**

> What do you notice in the visualization? The first thing that comes to mind is the lack of a common trend over the analysed period. There seems to be an overall decline in traffic accidents but the dynamics within the period 2009-2014 differ substantially. These trends are hard to appreciate as the lines cross each other. I would rather use lines with different format (e.g. dotted, dashed lines, etcetera).

> What questions do you have about the data? Three points stand out. First, it would be interesting to have a weekly average to see how far away are traffic accidents in different days with respect to the 'normal' or average value. And secondly, why focus on absolute numbers and not percentages? Of course, with a little bit of more context this question could be answered but it is not clear to me why you would prefer to look at the number of deaths rather than percentages. For instance, if deaths decline from 1200 to 1000 the absolute change is the same as from 400 to 200, even though in percentage terms is completely different. An option to include this is to use indices or maybe better you could use log-transformed traffic accidents. The good thing about this is that you can still specify in the vertical axis the number of accidents to which the different log values refer. In this way, you can have both information on absolute and percentage changes. Finally, the third point is concerned with the underlying data of the graph. The trends you observe might be due to increasing/decreasing population, increasing/decreasing traffic intensity due to fluctuating economic activity, etcetera. It would be interesting to present these data in relative terms. In other words, present data on the number of traffic accidents per capita, or per people driving (if this information is available?), etcetera.

> I think the are three main take-away messages. One is that, in general, the total number of traffic accidents have declined during the period 2009-2014. Secondly, the dynamics within the analysed period differ greatly and call for an explanation. And thirdly, Saturday and Sunday stand out with their low number of traffic accidents while Friday presents the highest value.

**Third version**

_Myles_

> Hi David,

> I would still center everything, as it is distracts from the visualization to have to look at one side of the screen.

> Apart from that it looks great (it is also interesting, which I guess is the key issue ... I would have bet on Monday having the most accidents).

> Nice work!

### RESOURCES

* http://datos.madrid.es/egob/catalogo/207831-2-accidentes-trafico.xls
* https://github.com/PMSI-AlignAlytics/dimple/wiki/dimple.chart
* https://discussions.udacity.com/
* http://gravyanecdote.com/uncategorized/mythbusters-should-you-start-your-axes-at-zero/
* http://stephanieevergreen.com/non-zero-axis-rules/
