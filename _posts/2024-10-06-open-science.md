---
title: 'A Case for Open Science'
date: 2024-10-06
permalink: /blog/2024/10/open-science/
tags:
  - science
  - open science
  - equality
---

In [a recent post](https://moejakob.github.io/portfolio/OS_project/) I wrote about the state and the development of Open Access publication practices and showed that over the last 18 years, the rate of scientific papers that were published openly has increased dramatically. In this blog post I want to explain to you, why this is great news. The data analysis I conducted for the other post was focused on Open Access (i.e. making research papers available for everyone for free). Here, I will also write about other practices that play a crucial role in Open Science.

## Why we should make science (more) open?
Scientific research is one of the main drivers of societal evolutions. A great example for this is the development of vaccines. Sera that were developed by scientific research contributed to the complete eradication of the smallpox, a disease that killed an estimated 300-500 million people ([Berche 2022](https://doi.org/10.1016/j.lpm.2022.104117)). According to the [World Health Organisation (WHO)](https://www.who.int/health-topics/poliomyelitis#tab=tab_1) Polio infections dropped from 350.000 cases worldwide in 1988 to 6 cases in 2021. The reason for this was the worldwide distribution of the Polio-vaccine that was first developed by Jonas Salk and had previously quasi eradicated Polio in the western world. Vaccines also helped tremendously in containing the Coronavirus during the recent COVID-19 pandemic.

These achievements (and many others) would never have been possible without scientific research. Hence, to continuously develop our society, science should be conducted as efficiently as possible. At the same time, every person on the planet should be able to audit the process behind new developments that may affect their life and other researchers should be able to reliably reproduce and replicate scientific studies leading to new discoveries (on a side note: check out this very interesting [Youtube-Video about the replication crisis in psychology](https://www.youtube.com/watch?v=QGWeVbYduOI)). Making science more open can help us achieve these goals.

## How to make science more open?
This question requires me to delve into the process of scientific publication a little bit. Original research is always based on data which can be analysed be the scientists who draw conclusions from these analyses. They write everything about their experiments and their data-analysis into a paper and then they try to get this paper published by a publisher. For a paper to be published it goes through a peer-review process where other scientists from the same field read the study to see if the original authors of the paper have done all the right things. So here are a few things you can do to make your own research more open.

### Publish your research data
The reliability of this process strongly depends on everything about this study being available to other scientists. It would be quite simple for a researcher to make up a result that just suits their needs and write it up into a paper. The easiest way to prove that you didn't is to publish your original research data together with your results so that everyone can (at least in theory) reproduce your results.

### Publish a documentation of your methods
Describing the method you used in your experiment is normally required to pass the peer-review process and publish your paper. But it can sometimes still be quite difficult to completely reconstruct the methodology of an experiment from a few paragraphs written in a paper. So if you really want to make sure your experiment is reproducible, you should document your experiments (e.g. in an electronic labnotebook like Labfolder) and publish this documentation along with your paper and your data.

The same holds true for the method of your data analysis. Describing the process of analysing your data and especially describing your statistical model is far from being a trivial task. So the easiest way to tell people what you did is to just show them by publishing an R- or Python-script that you wrote for your analysis.

### Open up the peer review
Researchers have a lot on their plate. Their priority is doing their own research. Yet they are expected to review papers from other researchers in their field. Some researchers may see this as something of a nuisance and won't give the review the thoroughness it deserves (and needs). This is possible, because the peer-review is traditionally a double blind process, meaning that reviewrs don't know the names of the authors and vice versa. Some journals now offer, to openly publish the whole review process including the names of the reviewrs along with the paper to ensure a high quality peer-review (if you ever wanted to see what a peer-review looks like, [here is an example](https://elifesciences.org/articles/87513/peer-reviews#content).

### Publish your paper open access
Traditionally, university libraries had subscriptions to research journals so they researchers could read the papers published in them. If your university didn't have a subscription to a specific journal, you could either buy an individual paper for a lot of money or you couldn't use the (potentially crucial) information written in those journals. This creates a problem of inequality because not all universities have big funding organisations standing behind them. So especially universities in poorer countries may not be able to afford all the important journal subscriptions. Luckily, publishing research papers open access is now more common than not doing so - especially in major scientific locations in Europe and North America and the open access publishing rates are still rising.

## Potential pitfalls of Open Science
Overall I strongly believe that the advantages of Open Science outweigh its disadvantage. That being said, researchers should still be cautious when they practice Open Science. For example, most open access articles are now published as *gold open access*, meaning that publishers ask for a publication fee (a.k.a. article processing charges (APCs)). In reputable journals like Nature, these fees may be in the high four figure range for a single article. On the one hand this is problematic because this model merely shifts the inequality problematic from some poorer universities not having access to scientific discoveries to them not being able to publish their own research in open access journals. In recent years, an even bigger issue has arisen from this model. So called predatory publishing. So called predatory journals actively invite researchers to publish in their journals. To publish in those journals, these publishers ask the researchers to pay the APCs up front. The articles are then published with little to no editorial process (in particular without peer review), which means you can basically publish anything you want in those journals, even if it has no scientific basis. Here is a really good TEDx Talk by Bradley Allf about this topic:

{% include youtube.html id="73goVcQw0QI" %}

Another issue arises when we're talking about openly sharing your research data. I already described some of the benefits of sharing your data. But there are two major considerations that you should make before doing so:

1. **Are you allowed to share your data?** This issue is most prevalent in health- and social sciences, where you may work with personal (patient) data. Most countries have data protection laws that prohibit the sharing of personal data without consent of the respective person. Therefore, when you're working with personal data and want to share it, it is crucial that you pseudonymise or even anonymise the data before sharing it in the repository of your choice.
2. **Is it morally acceptable to share your data?** This might for example be of interest for nuclear physicists, whose research data could be abused to build weaponry.

## Conclusion
To sum up all that you have just read:

Practicing Open Science has many benefits and will (hopefully) become the research standard soon. However, doing so will take careful consideration and even some extra effort from the researchers side.

## Bonus
Here is a video of me, slamming some science at an Open Science Slam that my former colleagues and I organised in January 2024:

<iframe width="560" height="315" src="https://www.youtube.com/watch?v=1w5T1OGeF30" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
