---
title: "The State of Open Access Practices"
excerpt: "I explore Open Access practices in Germany and the world.<br/><a href='https://moejakob.github.io/portfolio/OS_project/'><img src='/images/OA/oa_lock_450.png'></a><br/>"
collection: portfolio
published: true
---
([Find all the code as well as information about data provenance for this project on my Github-Account](https://github.com/moejakob/OS_practices))

## Introduction
Year after year, new scientific discoveries have an impact on people all over the world. Such discoveries may have farreaching consqeuences. For example, they might be the basis for major political policies or for medical treatment procedures all over the world. With scientific research having such strong societal impact, it is pertinent that people all over the planet have equal access to scientific discoveries. One major step towards achieving this goal is to publish research results as Open Access (OA), i.e. to make it freely available for everyone.

Every year, the Centre for Science and Technology Studies (CWTS) Leiden publishes a ranking that among other information includes some statistics on the OA publishing practices of universities world wide. In this project I worked with data from the [CWTS Leiden Ranking OPEN Edition 2023](https://open.leidenranking.com/).

## Exploring Open Access Practices
Open Access has gained a lot of momentum in recent years. As a matter of fact, the overall worldwide open access publication rate (blue line has risen from 28.6% during the period of 2006-2009 to 55.1% during the most recently assessed period (2018-2021). It is notable, that opan access conventions differ between subject areas. In particular, OA rates in the Biomedichal and Health Sciences (orange line) have consistently been higher than in other fields. A reason for those high OA rates may be that this area of research can be viewed being of especially high importance as it can literally decide over life and death.

[![Figure 1: Open Access Rates (%) over Time for Different Scientific fields](/images/OA/overall_oa_rate_over_time.png)](/images/OA/overall_oa_rate_over_time.png)
<figcaption style="text-align: left; font-style: italic;">
    Figure 1: Open Access Rates (%) over Time for Different Scientific fields.
</figcaption>
<br/><br/>
Additionally, OA practices also vary quite strongly by regions. In the map below I have marked the 100 universities with the highes OA rates world wide in the period 2018-2021. It is very notable that only 7 of these 100 universities are outside of Europe (3 in the USA, 2 in Africa and 2 in the Middle East). If we look more closely, we can even see that 69 of the top 100 OA universities are located in only two European countries (58 in the UK and 11 in the Netherlands).

<figure>
  <iframe src="{{ 'https://moejakob.github.io/images/OA/top_100_oa_unis_world_2018-2021.html' | relative_url }}" width="100%" height="600px" frameborder="0"></iframe>
  <figcaption style="text-align: left; font-style: italic;">
    Figure 2: Interactive map of the top 100 Open Access universities worldwide (2018-2021).
  </figcaption>
</figure>

Open Access is often subcategorised into different *colours*. While all articles that are published in any type of OA can be accessed for free, most major publishers have adapted models (**Gold OA** and **Hybrid OA**) that require publication fees from researchers that want to publish their work as an OA article. Other models like **Green OA** and **Bronze OA** don't require publication fees. When we look at the development of OA publication rates by OA colours, we notice that the increase in OA rates is largely driven by **Gold** and **Hybrid Open Access** publications - the two models that require payment from researchers. Since research funding varies from region to region, it is not unexpected that OA practices are mostly centered around Europe rather than poorer countries. I will go into more details about this issue and about the different OA models in a blog post soon.

[![Figure 3: OA publication rates over time for different OA models](/images/OA/oa_colours_rate_over_time_stack.png)](/images/OA/oa_colours_rate_over_time_stack.png)
<figcaption style="text-align: left; font-style: italic;">
    Figure 3: OA publication rates over time for different OA models.
</figcaption>
<br/><br/>
However, it seems that the amount of funding is not the only driving force impacting the OA rates. The interactive map below displays European countries and their overall OA rates in the period 2018-2021. We can see that Germany, one of the wealthiest countries in Europe has an OA rate of 66.7% whereas less wealthy countries like Hungary (77.4%) have significantly higher OA rates. Other factors like national policy making and research culture might have equally (or even stronger) influence on OA publication rates than funding availability.

## Interactive Dashboard Visualizing Open Access Rates
<iframe title="oa_dashboard" src="https://app.powerbi.com/reportEmbed?reportId=f2a080ce-e811-4c08-acdb-3257d4731353&autoAuth=true&ctid=a0668a0b-7f14-4396-ad4d-0ebf06457115" frameborder="0" allowFullScreen="true"></iframe>

<figure>
  <iframe src="{{ 'https://moejakob.github.io/images/OA/oa_map_europe_2018-2021.html' | relative_url }}" width="100%" height="600px" frameborder="0"></iframe>
  <figcaption style="text-align: left; font-style: italic;">
    Figure 4: Interactive map of Open Access rates in european countries (2018-2021).
  </figcaption>
</figure>

Since I am a German myself and have in the past worked at a German university, I am particularly interested in OA practices in my home country. So let's take a closer look:<br/>
These are the top 10 German universities by their open access publishing rate (period: 2018-2021). The number one spot on this list is held by the University of Konstanz (which incidentally is the university at which I was employed in the past 😉). While it takes the top spot among German universities with an OA rate of 79.4% it only just makes it into the top 100 European universities (99th place) and just misses out on a spot in the top 100 OA universities worldwide (105th place).

<figure>
  <iframe src="{{ 'https://moejakob.github.io/images/OA/top_10_oa_unis_germany_2018-2021.html' | relative_url }}" width="100%" height="600px" frameborder="0"></iframe>
  <figcaption style="text-align: left; font-style: italic;">
    Figure 5: Interactive map of the top 10 Open Access universities in Germany (2018-2021).
  </figcaption>
</figure>

If we compare OA rates of German universities to the European average, we see that the German average lies below the European average in every single scientific field and in the overall OA publishing rate. This indicates that, on a European level, Germany has sadly fallen behind in the uptake of open access practices. Changing this will require progressive policy making by the German government and a change in the German research culture.


| Scientific Field                  | Germany    | Europe     |
|:---------------------------------:|:----------:|:----------:|
| Overall                           | 66.7 %     | 71.0 %     |
| Biomedical and Health Sciences    | 72.0 %     | 74.5 %     |
| Life And Earth Sciences           | 68.3 %     | 71.8 %     |
| Mathematics And Computer Science  | 64.9 %     | 68.2 %     |
| Physical Sciences And Engineering | 62.5 %     | 69.4 %     |
| Social Sciences And Humanities    | 59.4 %     | 66.2 %     |

<figcaption style="text-align: left; font-style: italic;">
Table 1: Open Access rates in scientific displins in Germany vs. Europe (2018-2021).
</figcaption>
<br/><br/>
Figures 6 and 7 allow us to look at these numbers in more detail. Specifically, they allow us to see the publishing rates for the different OA models. It is notable that there is one model where the German publishing rate is higher than the European one, namely, the **Hybrid OA** model. This is, infact, not necessarily disirable, as **Hybrid OA** describes a publishing practice that allows publishers to both ask for publication fees **and** subscription fees - a practice also termed double dipping.

<figure>
  <iframe src="{{ 'https://moejakob.github.io/images/OA/oa_rate_fields_colors_europe_2018-2021.html' | relative_url }}" width="100%" height="600px" frameborder="0"></iframe>
</figure>

<figure>
  <iframe src="{{ 'https://moejakob.github.io/images/OA/oa_rate_fields_colors_germany_2018-2021.html' | relative_url }}" width="100%" height="600px" frameborder="0"></iframe>
  <figcaption style="text-align: left; font-style: italic;">
    Figures 6 & 7: Interactive graphics of Open Access rates by field and Open Access colours in Germany and Europe (2018-2021).
  </figcaption>
</figure>

## Correlation between OA Practices and University Statistics
Finally, I want to see how Open Access rates correlate with different university statistics. For the university statistics I used two resources: the [Times Higher Education (THE) World University Ranking](https://www.timeshighereducation.com/world-university-rankings) for university ranking statistics (I used data from the year 2021 so it matches the data from the CWTS Leiden Ranking) and university microdata from the [European Tertiary Education Register (ETER)](https://eter-project.com/) (also from the year 2021).

### CWTS Leiden Ranking and THE University Ranking
Let's first look at a correlation matrix of the correlations between the CWTS Leiden Ranking and the THE University Rankings. I highlighted the most interesting part of the matrix, i.e. the correlations of OA rates and the 6 THE scores (Overall, Teaching, Research, Citations, Industry Income, and International Outlook).

[![Correlation Table of CWTS and THE University Rankings](/images/OA/oa_the_corr_highlight.png)](/images/OA/oa_the_corr_highlight.png)
<figcaption style="text-align: left; font-style: italic;">
Figures 8: Correlation matrix (Pearson's r) of the CWTS and the THE University Rankings. Correlations between OA (model) rates and THE scores are highlighted.
</figcaption>
<br/><br/>
With two exceptions, the matrix shows positive correlations between all THE scores and all CWTS OA rates, indicating that overall, universities that have highe OA rates also score higher on the THE University Ranking scores. A very remarkable exception is the **Gold OA** rate which correlates **negatively** with the THE scores. As we have seen above, **Gold OA** is largely responsible for the strong increase in overall OA publication rates worldwide. While this is counterintuitive, it is somewhat consistent with the results of a study by [Piwowar and colleagues (2018)](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5815332/) that found that **Gold OA** articles are cited **less often** than the overall average. In their discussion they state the following conjecture to explain this fact.

> "Interestingly, Gold articles are actually cited less, likely due to an increase in the number of newer and smaller OA journals. Some of these journals are from regions of the world not historically indexed by WoS, are published in languages other than English, or might be considered to be less prestigious because they have not had time to become established or accumulate citations (Archambault et al., 2013). On the flip side, the citation disadvantage of Gold OA is likely also affected by the continued growth of so-called ‘mega journals’ such as PLOS ONE ( PLOS, 2018)." (Piwowar et al. 2018, p. 17)

The second exception are correlation coefficients related to the THE Industry Income Score. However since they don't show strong correlations in either direction, I will not discuss them further.

### CWTS Leiden Ranking and ETER University Microdata
Secondly, I want to look at correlations between OA rates and some university microdata, specifically total third party funding, number of academic personnel and number of students. Again, I highlighted the part of the correlation matrix that I find most relevant.

[![Correlation Table of CWTS and ETER University Microdata](/images/OA/oa_eter_corr_highlight.png)](/images/OA/oa_eter_corr_highlight.png)
<figcaption style="text-align: left; font-style: italic;">
Figures 9: Correlation matrix (Pearson's r) of the CWTS OA rates and ETER University Microdata. Correlations between OA (model) rates and microdata are highlighted.
</figcaption>
<br/><br/>
Once agein, we observe that **Gold OA** rates correlate negatively with all three university statistics, indicating that universities with more third party funding, more academic personnel and more students display lower Gold OA publication rates. Likely the most interesting positive correlations are those of third party funding with Overall OA rates, as well as Hybrid-, Bronze- and Green-OA rates indicating that universities with higher funding also have higher OA rates (with the exception of Gold OA), potentially giving universities an incentive to encourage their researchers to publish in open access.

### Additional correlation visualisations
The following graphics visualise the correlations between the OA rates with the THE scores and the ETER microdata, respectively.

[![Correlation Table of CWTS and ETER Funding data](/images/OA/oa_funding_corr.png)](/images/OA/oa_funding_corr.png)
<figcaption style="text-align: left; font-style: italic;">
Figures 10: Correlations between the CWTS and the Total amount of third party funding in Mio Euro.
</figcaption>

[![Correlation Table of CWTS and THE Scores](/images/OA/oa_the_corr.png)](/images/OA/oa_the_corr.png)
<figcaption style="text-align: left; font-style: italic;">
Figures 11: Correlations between the CWTS and the THE University Ranking Overall-, Research- and Citation-scores.
</figcaption>
