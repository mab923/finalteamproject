# Fin 377 Final Team Project
### Margaux Brennan, Isabel Prado, Natan Rosen


## Table of contents
1. [Introduction](#introduction)
2. [Methodologies](#meth)
    1. [Find Data](#find)
    2. [Cleaning Data](#clean)
    3. [Merging Data](#merge)
3. [Visualizations](#viz)
4. [Analysis](#anal)
5. [Summary](#sum)
6. [Helpful Links](#help)
7. [Team](#team)

## Introduction   <a name="introduction"></a>
Our research aims to investigate the correlation between changes in monetary policy and market performance. We have chosen to inspect this through the lense of changes in the Reserve Requirement by the Federal Open Market Committee (FOMC) and returns from the S&P 500, Vanguard Intermediate Long-Term Bond Index Fund (VBILX) and Vanguard Short-Term Bond Index Fund Admiral Shares (VBIRX).

Our inquiry seeks to determine whether an increase or decrease in the reserve requirement rate or the the magnitude of that change, is linked to positive or negative returns in the stock market, long-term bond market (via Vanguard Intermediate-Term Bond Index Fund), or short-term bond market (using Vanguard Short-Term Bond Index Fund Admiral Shares).

## Why we Chose this Topic
The FOMC's decisions on whether to raise or lower interest rates have far-reaching effects on the economy. We aim to provide a framework that allows investors to time their investments more effectively around the FOMC's scheduled meetings. We believe that our findings will be of particular interest to institutional investors who seek to enhance their capital gains while minimizing losses through making thousands of trades with small gains that altogether compound into a substantial profit.

Therefore, by examining the impact of FOMC's official announcements on the performance of different indexes, investing in stocks or bonds immediately surrounding the press release of a FOMC meeting could be a potentially reliable method for institutional investors to increase their capital gains and minimize losses. We strongly believe that the insights gained from the project will provide a deeper understanding of the correlation between the reserve requirement rate and market returns.

## Methodologies <a name="meth"></a>
To investigate the relationship between the stock and bond markets in the context of the S&P 500 firms. To achieve this, we will carry out an event study. We have determined that we will utilize data spanning over a period of eight years - from 2015 to 2022.

### 1. Find Data <a name="find"></a>
The data set will consist of daily market return data on days t-10 to t+10, where t represents the date of the reserve requirement change.

We will require data on market performance information sourced from the S&P 500, VBILX, and VBIRX. As well as information on the change in Reserve Requirement from the Federal Reserve Board for information on changes in monetary policy during our specified time period. This information will allow us to study the impact of monetary policy decisions and potential correlation between the policy and stocks & bonds

- Federal Open Market Committee (FOMC)
- S&P 500 - indicator for stock correlation
- Vanguard Intermediate Long-Term Bond Index Fund (VBILX) -bond sample
- Vanguard Short-Term Bond Index Fund Admiral Shares (VBIRX) - bond sample

### 2. Clean Data <a name="clean"></a>
After gathering the data, we performed cleaning and exploratory analysis to prepare it for analysis. We used the describe function to understand find count, mean, std, among other key factors. Then we looked for missing values in the data; we found the missing data was minimum but we used the dropna function to have a clean version of the data. We then converted object variables to numeric values. We also explored the outliers and discussed the findings. However, we decided not to eliminate the outliers because it would affect our results. To confirm the results we printed the dtypes. Finally, we used the pairplot to visualize the relationships between the variables in the dataset.


### 3. Putting the Data Together <a name="merge"></a>
We created a row in our data frame for every date in the fifteen days prior and after a change in the FOMC rate. From our sourced data we merged together the returns and trading volume of all three indexes we wished to examine, as well as the change in rate.

From there we created our own event time variable that allowed us to view each event in isolation. From there we were able to average all our results across indexes to receive an overarching answer to our question.

### 3. Visualizations <a name="viz"></a>
We created two different types of figures to analyze our findings.

A. Correlation Matrix
<img src="pics/corr.png?raw=true"/>
<br>
From this plot we can easily see the strength of correlation between increases and decreases of the FOMC rate and the returns on each index.
 
 B. Line Plots
 
 Plot #1
 <img src="pics/p1.png?raw=true"/>
 <br>
 From this plot we are able to determine the effects of an increase in the FOMC rate on the returns of each of our indexes over our 10 day span.
 
 Plot #2
 <img src="pics/p2.png?raw=true"/>
 <br>
 From this plot we are able to determine the effects of a decrease in the FOMC rate on the returns of each of our indexes over our 10 day span.
 
 Plot #3
 <img src="pics/p3.png?raw=true"/>
 <br>
 From this plot we are able to analyze the impact of the negative and positive rates on the returns of the S&P 500
 
 Plot #4
 <img src="pics/p4.png?raw=true"/>
 <br>
 From this plot we are able to analyze the impact of the negative and positive rates on the returns of  VBIRX
 
 Plot #5
 <img src="pics/p5.png?raw=true"/>
 <br>
 From this plot we are able to analyze the impact of the negative and positive rates on the returns of VBLIX
 
 ## Analysis <a name="anal"></a>
 
While some of the analysis we gathered supported our initial assumptions, it's clear that we have to reject our hypothesis after looking through the data and visualizations. While there were moments in the graphs where the increase in a rate led to a decrease in returns, the relationship was not linear and experienced too much volatility to consider a serious finding. While we still believe that this relationship exists, especially when looking at stocks, it's clear that we need to include more samples in our data as well as look at the data from different viewpoints. One phenomenon that we observed that did back up our assumptions was that the s&p 500 index was significantly more volatile in the periods we were analyzing than either of the two bond indexes. This makes intuitive sense as bonds are a lot less liquid and people generally like to hold onto their bonds for longer. One suspicion our group has based on the graphs we saw was that people are more likely to speculatively buy a stock they think is going to go up, then they are to sell a stock they already own. People are much more likely to believe that the stock they are choosing will be a winner versus admitting to themselves the stock they own is a loser. Not only does this make sense psychologically, but the data backs this assumption up reasonably well. One idea we had for improving our analysis would be to create a categorical variable with 4 bins: small hike, large hike, small decrease, and large decrease. This would give us the ability to look at the returns in relation to the size of the increase versus just the average. Another idea for improving the study would be to separate the meeting dates and rate hikes into seasons or periods of the year. This would allow us to extract the true correlations versus returns that were shifting strictly because of season or market patterns.

## Summary <a name="sum"></a>


Our hypothesis was both challenged and supported by our findings in this project. The correlation matrix offered some support to our hypothesis but also was surprising with its correlation of the S&P 500 returns. Similarly, the return graphs showed some semblance of a pattern with returns and rates, but not necessarily the one that we predicted. We suspect that more variables and indexes would have to be chosen for the experiment to show some real results if it were to be done again. We also misunderstood the relationship that exists between interest rates and bonds when we started this project. Our initial assumption was that when rates increase the bond prices will similarly increase because people want less risky investments. This is true to a sense but if you are already holding a bond, then a hike in interest rates actually devalues your bond. It is a complicated relationship that warrants its own study in itself.



# Thanks For Reading

## Helpful Links: <a name="help"></a>

The final analysis file is [here](https://github.com/mab923/finalteamproject/blob/main/Analysis/Final_Analysis.ipynb)
To see the collection of datasets used (raw/clean/final) click [here](https://github.com/mab923/finalteamproject/tree/main/inputs)
All of the visualization can be found [here](https://github.com/mab923/finalteamproject/tree/main/pics)
Presentation of Project [here](https://docs.google.com/presentation/d/1FVA0dMcFhYUgkXvHzQWL9D_ouhccAGN5Ac7-nf0jBTs/edit#slide=id.g1b76803da3e_0_5)

Below is information about the members of the team

## Team <a name="team"></a>

<img src="pics/6FB5FD7F-9E42-4F5C-BE04-D13CF10E6667.jpeg" alt="nathan" width="300"/>
<br>
Nathan is a senior at Lehigh studying finance and business analytics.
<br><br><br>
<img src="pics/margaux.JPG" alt="margaux" width="300"/>
<br>
Margaux is a senior at Lehigh studying Finance 
<br><br><br>
<img src="pics/isabel.jpeg" alt="isabel" width="300"/>
<br>
Isabel is a senior at Lehigh studying finance and business analytics.
