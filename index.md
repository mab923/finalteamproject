# Fin 377 Final Team Project
### Margaux Brennan, Isabel Prado, Natan Rosen

## Introduction
Our research aims to investigate the correlation between changes in monetary policy and market performance. We have chosen to inspect this through the lense of changes in the Reserve Requirement by the Federal Open Market Committee (FOMC) and returns from the S&P 500, Vanguard Intermdiate Long-Term Bond Index Fund (VBILX) and Vanguard Short-Term Bond Index Fund Admiral Shares (VBIRX).

Our inquiry seeks to determine whether an increase or decrease in the reserve requirement rate or the the magnitude of that change, is linked to positive or negative returns in the stock market, long-term bond market (via Vanguard Intermediate-Term Bond Index Fund), or short-term bond market (using Vanguard Short-Term Bond Index Fund Admiral Shares).

## Why we Chose this Topic
The FOMC's decisions on whether to raise or lower interest rates have far-reaching effects on the economy. We aim to provide a framework that allows investors to time their investments more effectively around the FOMC's scheduled meetings. We believe that our findings will be of particular interest to institutional investors who seek to enhance their capital gains while minimizing losses through making thousands of trades with small gains that alltogether compound into a substainial profit.

Therefore, by examining the impact of FOMC's offical announcements on the performance of different indexes, investing in stocks or bonds immediately surrounding the press release of a FOMC meeting could be a potentially reliable method for institutional investors to increase their capital gains and minimize losses. We strongly believe that the insights gained from the project will provide a deeper understanding of the correlation between the reserve requirement rate and market returns.

## Methodology
To investigate the relationship between the stock and bond markets in the context of the S&P 500 firms. To achieve this, we will carry out an event study. We have determine that we we will utlize data spanning over a period of eight years - from 2015 to 2022.

### 1. Find Data
The data set will consist of daily market return data on days t-15 to t+15, where t represents the date of the reserve requirement change.

We will require data on market performance information sourced from the S&P 500, VBILX, and VBIRX. As well as information on the change in Reserve Requirement from the Federal Reserve Board for information on changes in montetary policy durong our specified time period. This information will allow us to study the impact of monetary policy decisions and potential correlation between the policy and stocks & bonds

### 2. Clean Data

### 3. Putting the Data Together
We created a row in our data frame for every date in the fifteen days prior and after a change in the FOMC rate. From our sourced data we merged togethter the returns and trading volume of all three indexes we wished to examine, as well as the change in rate.

From there we created out own event time variable that allowed us to view each event in isolation. From there we were able to average all our results across indexes to receive an overarching answer to our question.

### 3. Analysis
We created three different types of figures to analyze out findings.
 1. Correlation Matrix
 2. Scatter Plot
 3. Event Study Graph

## Potential Issues 

## Our Team

