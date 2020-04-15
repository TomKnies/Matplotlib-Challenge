# Matplotlib-Challenge

# Three observations from my data

Observation 1 - The correlation between the weight of the mouse subject and the final recorded volume of their tumors makes
logical sense now that I've seen the data.  Even though it's not something that would've occurred to me beofre the testing,
the idea that more body mass leads to bigger tumors sounds obvious in retrospect.  The r-squared is pretty strong at .84 so
we can say with reasonable certainty that this conclusion isn't just random noise in our data.  Following the regression
line we can estimate that the tumor volume (mm3) of a mouse after 45 days of treatment will be rougly 21.5 plus the mouse's
weight in grams.  Official line equation is: y = 0.95x + 21.55

Observation 2 - Looking at the results from the overall summary statistics and the later created box and whisker plots for
our four target drug regiments, it appears our Capomulin and a competitor's Ramicane are significantly better than every
other regiment we tested with.  Their means are up to 20% smaller!  Their maxes are smaller than everyone else's means!
Those numbers may not be 100% quote worthy because Capomulin and Ramicane both have a lower outlier or two, but they were
outliers by very small margins by my calculations, and the box plot didn't even mark them as outliers so it's possible I
simply calculated that wrong and they aren't even outliers in the first place.

Observation 3 - Knowing from the data that Capomulin and Ramicane produce lower final tumor volumes than the others, it
occurs to me that this may also be the reason we have the most datapoints on them.  We started with 25 mice on each of the
10 regimens for a total of 250 mice that we tested every 5 days (thus creating a new datapoint).  So by the end we should
have 250 datapoints per regimen (25 mice checked 10 times each) except we clearly do not.  Meaning some of the mice stopped
being checked, presumably because they died from the cancer.  This is sort of another "well duh" moment, but we can likely
say that in addition to being better at reducing tumor volume, Capomulin and Ramicane are also better at keeping those
being treated with it alive.
