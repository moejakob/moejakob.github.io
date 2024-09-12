---
title: "Konstanz Weekly 5k Run"
excerpt: "<img src='/images/Running.png'><br/>In this project I explore some data from a weekly 5 kilometer running event I help organise."
collection: portfolio
---
([https://github.com/moejakob/konstanz5k](Find all the code for this project on my Github-Account))

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

