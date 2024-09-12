---
title: "Konstanz Weekly 5k Run"
excerpt: "<img src='/images/Running.png'><br/>In this project I explore some data from a weekly 5 kilometer running event I help organise."
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

![Volunteer Ratio](/images/pie.png)

### Seasonal differences
Anyone who runs, knows that is quite different to run at different times of the year. For example, it is a lot easier to find the motivation to go for a run on a nice and sunny summer morning than on a cold and wet winter morning. This is very nicely reflected in the data (see the graph on the left). It even turns out that there are some seasonal differences in running speed (see the graph on the right). While the differences in running speed don't seem too big, 0.5 km/h (the difference between spring and summer) comes out to a finishing time difference of almost 1:30 min which over 5 kilometers is quite a lot.

![Seasonal differences](/images/seasonal_diffs.png)

### Attendance
Now we established that the attendance underlies seasonal changes, let's see if there is an overall trend in participant numbers. The linegraph below shows the developement of finisher number over the 163 organised events. The first thing that (quite literally) spikes out is that one event had many more participants than all others. This was the aforementioned 100th event where we managed to recruit 125 runners to join us. The red line also shows us that attendance in our runs is overall increasing with time. One thing that is a bit harder to see, are the seasonal changes. They are reflected by the periods with higher attendance numbers (e.g. around the 100th-115th and the 145th-160th event) displayed by the blue line.

![Finishers over time](/images/finishers.png)
