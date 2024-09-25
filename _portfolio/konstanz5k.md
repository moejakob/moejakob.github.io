---
title: "Konstanz Weekly 5k Run"
excerpt: "In this project I explore some data from a weekly 5 kilometer running event I help organise.<br/><a href='https://moejakob.github.io/portfolio/konstanz5k/'><img src='/images/Running.png'></a>"
collection: portfolio
---
([Find all the code for this project on my Github-Account](https://github.com/moejakob/konstanz5k))

I like running. It's probably my biggest hobby. I like to run by myself, in the forests, along the lake and probably most of all in the mountains. But I also like running with other people and helping them to join the (amazing) running community. I do this by organising a trailrunning group at the University Sport and I also help organising a weekly 5 kilometer running event here in Konstanz.🏃🏃

For my first project to be featured on this website, I wanted to do something about running and I decided to analyse some data about the weekly running event I help organising. For reasons of data protection, I will not explicitly mention the running event. But those of you who know me probably know which event I'm talking about.🌳😉

## Procuring the data
We recently celebrated our 3rd "birthday", meaning that we have organised over 150 runs for the community. Each of them has their own result page online, so downloading them manually would be **a lot** of work. Therefore I used webscraping to download the results for all runs. Overall, the dataset has just over 4000 rows of data which have a lot of different information:

* the **event number**
* the **date** of the event
* the anonymised ID and times of the **first male** and **female finisher**
* the **position** of the runner
* the runners **gender** and **agegroup**
* the runners **club affiliation** (if they had one)
* how many **times the runner has run** at a run organised by our organisation which organises weekly runs all over the world*
* how many **times the runner has volunteered** at a running event*
* the runners **finishing time**
* an **age graded performance** metric that is adjusted for gender and agegroup

## Exploratory data analysis
Before we get to some of the more interesting stuff (I promise there will be pretty graphs!📊😉) let me hit you with some hard facts:

Since we started organising this event more than 3 years ago (so far we have organised **163 runs**), a total of **1220 different runners** have participated (and finished) in one of our runs. The average attendannce lies at around **32 runners per week**. Now of course there were some days with more runners (like our 100th run with **125 participants**!) and some cold winter days with fewer participants (one time, there were only 8 runners, yikes that must have been a rough day for running!🌨️🌨️).

On average, it takes our runners **30:37 minutes** to finish the 5 km - quite good if you ask me! Of course, some of them were quite a bit faster. The **course record for the men is 16:51**, the course record for the **women 18:36**, both absolutely **rapid** times!!! However, not just the times are impressive but also the consistency with which some of the runners attend our event. There is one runner who has run in 104 out of 163 runs that we organised - that's almost two thirds of the runs.

Now that you know some of the key facts, I hope I woke your curiosity. So let's uncover some of the trends and patterns hidden in this data.

### Volunteer ratio
The first thing I wanted to know is how many of the runners who have participated in our event have ever volunteered at an event by the same global organisation. And the very pleasant answer to that is: more than half!! All the people who willingly offer their time to volunteer at our running events make it possible to organise them week in, week out - they are absolute legends!

[![Volunteer Ratio](/images/pie.png)](/images/pie.png)

Unsurprisingly, there is a correlation between the number of times people have participated as a runner and the number of times they have volunteered. Generally, the longer you're part of the community, the more time you have to rack up both runs and volunteer credits.

[![Volunteer-Run Correlation](/images/volunteer_ratio.png)](/images/volunteer_ratio.png)

### Seasonal differences
Anyone who runs, knows that is quite different to run at different times of the year. For example, it is a lot easier to find the motivation to go for a run on a nice and sunny summer morning than on a cold and wet winter morning. This is very nicely reflected in the data (see the graph on the left). It even turns out that there are some seasonal differences in running speed (see the graph on the right). While the differences in running speed don't seem too big, 0.5 km/h (the difference between spring and summer) comes out to a finishing time difference of almost 1:30 min which over 5 kilometers is quite a lot.

[![Seasonal differences](/images/seasonal_diffs.png)](/images/seasonal_diffs.png)

### Attendance
Now we established that the attendance underlies seasonal changes, let's see if there is an overall trend in participant numbers. The linegraph below shows the developement of finisher number over the 163 organised events. The first thing that (quite literally) spikes out is that one event had many more participants than all others. This was the aforementioned 100th event where we managed to recruit 125 runners to join us. The red line also shows us that attendance in our runs is overall increasing with time. One thing that is a bit harder to see, are the seasonal changes. They are reflected by the periods with higher attendance numbers (e.g. around the 100th-115th and the 145th-160th event) displayed by the blue line.

[![Finishers over time](/images/finishers.png)](/images/finishers.png)

### Average speed
We can also see if there are any overall trends when it comes to average speed. The red line on the graph below indicates that overall there isn't really a strong trend here. However, there are still a few things we can interpret fro this graph. Firstly, it seems that in the last 20-30 weeks, the average speed has gotten more consistent (the peaks and troughs on the blue line aren't as far apart). One reason for this could be the rising numbers in attendance. With a larger sample size (i.e. with more runners per week) the average speed will converge closer to the true mean of the population. And secondly, it looks like in the first ~20 weeks, the average speed was a bit higher than later. A reason for this could be that the event in Konstanz was founded by club runners. Therefore the first attendees were likely also club runners who tend to be faster than non-club runners.

[![Speed over time](/images/avg_speed_over_time.png)](/images/avg_speed_over_time.png)

Let's just double check if that last statement (that club runners tend to be faster than non-club runners) is true. It sure looks like it in the violinplot below.

[![Speed of club runners](/images/avg_speed_club.png)](/images/avg_speed_club.png)

Finally, let's see how running performance differs by age group. In the dataset there are basically two performance metrics. One is average speed (which is derived from the finishing time) and the other one is an age graded metric that adjusts the performance for gender and age group. Let's compare them side by side.

[![Age group performance](/images/agegroups.png)](/images/agegroups.png)

Now this **a lot** of information so let's unpack it bit by bit. Let's first decode the age group abbreviations (on the horizontal axis). The letter stands for the gender and the numbers for the age(range). 

Let's look at the top graph first. This one shows the (more intuitive) average speed for each age group. The black line in the middle of each box shows the mean. There are a few patterns that we can read from this graph:
1. Men (on the right half of the graph) tend to be faster than women (on the left side of the graph).
2. Once they are past their childhood, both men and women tend to get slower over time.
3. For men this decrease in average speed happens pretty gradually, while there seems to be a pretty clear cut between the female age groups F30-34 and F35-40. The reasons for this are less obvious than the previous two patterns. One guess that you could venture is that it is related to having children or to hormonal changes. But to know this for sure, we would need some additional data about the female runners.

Now let's look at the bottom graph. This one shows the age average graded performance metric for each age group. The idea behind this metric (which was calculated by the running organisation not be myself) is to make running performance comparable across different genders and age groups. So overall we would expect the graph to be flatter. At least for the men (again, on the right side of the graph), this is definitely the case. Only the older age groups and one of the very young age groups look like they differ a bit from the other age groups. One reason for this could just be a relatively low attendance by members of this age group and those who do probably have a strong interest in running and will accordingly perform quite well.

The female age groups on the other hand still show a pretty similar pattern to the one in the graph about average speed. The only reason I can think of why this is the case, is that the algorithm used to compute the age graded performance metric is not optimised for female age groups. A bias towards males and majority groups is a known issue in technology related fields like machine learning and could play a role here as well.

### Predicting running performance
The final thing I want to do is to train a Random Forest Regression to predict running performance based on a handful of variables. We have seen that there are a few variables that affect the running performance. I trained separate models to predict **average running speed** and **age graded performance**. To predict these metrics, I included four predictors in the models: **gender**, **agegroup**, **club affiliation** (as a binary variable "club_bi") and the **month** in which the event was held.

With these four variables I was able to train a decent model that could predict average running speed with a mean squared error of 3.44. This means that on average the predicted values deviate by about 15.5% from the true values. This isn't super precise when we think about predicting running times but it's also not that terrible. With an R-squared value of 0.52, the model actually fit the data quite okay and was able to explain a large part of the variance in the data.

The model trained for the age grade performance on the other hand performed pretty poorly. Most notably, it had an Out-Of-Bag score of -0.18 which indicates that it performed worse than if it had just predicted the mean of the dependent variable. Even after tweaking the hyper-parameters I was not able to significantly improve the model performance.

One reason why I like random forests is that they allow you to look at the importance of the features quite easily. So let's do that to find out which variable is most helpful in predicting running performance. What we can see in the graphs below is that for the average running speed prediction, the variable **gender** is relatively the most important in predicting performance, followed by the **club affiliation**. Both variables showed clear differences in running speed in the exploratory data analysis, so this doesn't really come as a surprise. What is more surprising, is that **gender** and **agegroup** are the two best predictors for the age graded metric. Remember, this metric is actually meant to make running performance comparable across genders and agegroups so we would expect them to be less impactful when predicting this metric. However, given the fairly poor fit of the model, drawing any conclusions from it wouldn't be very smart.

[![Feature importances](/images/feature_importances.png)](/images/feature_importances.png)
