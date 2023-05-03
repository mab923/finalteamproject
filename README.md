# Welcome to our [team project website!](https://mab923.github.io/finalteamproject)

This is a website to showcase our final project for FIN 377 - Data Science for Finance course at Lehigh University.

The basis for this report was analyzing the connection between the changes in interest rates brought on by FOMC meetings on the stock market and bonds. The project analyzes the S&P 500 as an indicator for stock correlation and the VBIRX and VBILX indexes as bond samples. 

# Hypothesis 

Large increases in interest rates would lead to negative or lower returns in the days before and after an FOMC meeting and vice versa



The final analysis file is [here](https://github.com/mab923/finalteamproject/blob/main/Analysis/Final_Analysis.ipynb).

Below is a high-level overview of the steps we took during the project. For a more in depth look into the entire project go to our team website here [team project website!](https://mab923.github.io/finalteamproject)



## Table of contents
1. [Introduction](#introduction)
2. [Data](#data)
3. [Methodology 2](#meth)
    1. [Subsection](#subsec2-1)
    2. [Subsection](#subsec2-2)
4. [Analysis Section](#section3)
5. [Summary](#summary)

## Introduction  <a name="introduction"></a>

Interest rate changes can have large effects on the economy in both the stock and bond market. This project takes a look deeper into how different securities react to changes in the days leading up to and following a FOMC meeting and corresponding hike. The project also takes a look at how the magnitude of a rate change can affect the returns of different stocks and bonds.

## Data Description <a name="data"></a>

We chose to use data from the years 2015 through 2023. We felt this was a large enough sample to draw conclusion from without making the dataset too large. 

In order to properly track the movement of stock price and bond prices we chose the following securities to track:
- Federal Open Market Committee (FOMC)
- S&P 500 - indicator for stock correlation
- Vanguard Intermdiate Long-Term Bond Index Fund (VBILX) -bond sample
- Vanguard Short-Term Bond Index Fund Admiral Shares (VBIRX) - bond sample

The two bond indexes were chosen due to their relatively stable returns and low risk metrics. The two bonds indexes would cover the correlation between bonds and rate hikes for our analysis

The S&P 500 was the logical choice for tracking the stock market due to the high variety in sector, industry, and size of the companies in the index.

The FOMC dataset was used to collect the different rate hikes that occured over the period of 2015-2023

To see the collection of datasets used (raw/clean/final) click [here](https://github.com/mab923/finalteamproject/tree/main/inputs)


## Methodologies <a name="meth"></a>
Blah blah

### Subsection 1 <a name="subsec2-1"></a>
This is a subsection, formatted in heading 3 style

### Subsection 2 <a name="subsec2-2"></a>
This is a subsection, formatted in heading 3 style

## Analysis Section <a name="section3"></a>

Here are some graphs that we created in our analysis. All of the visualization can be found [here](https://github.com/mab923/finalteamproject/tree/main/pics)

![](pics/corr.png)
This correlation matrix displays the correlation coefficients between the variables we created in our EDA process. 
<br><br>
![](pics/p1.png)
<br><br>
This graph depicts the returns of our 3 chosen securities after a interest rate hike. The time variable on the bottom depicts the days leading up to the rate change and the days following. Note the sharp increases in returns in the 1-2 days surronding the announcement of a rate increase.

<br><br>
![](pics/p2.png)
<br><br>
This graph is similar to the one above but depicts the returns after a decrease in interest rates. Its interesting that the decrease in returns surronding the announcement date is not nearly as sharp as the increases. This could be due to investors reluctance to sell assets but willingness to buy new securities.
<br><br>


## Summary <a name="summary"></a>

Blah blah



## About the team
<img src="pics/6FB5FD7F-9E42-4F5C-BE04-D13CF10E6667.jpeg" alt="nathan" width="300"/>
<br>
Nathan is a senior at Lehigh studying finance and business analytics.
<br><br><br>
<img src="pics/don2.jpg" alt="don" width="300"/>
<br>
Margaux is a a senior at Lehigh studying  


## More 

```python
import seaborn as sns 
iris = sns.load_dataset('iris') 

print(iris.head(),  '\n---')
print(iris.tail(),  '\n---')
print(iris.columns, '\n---')
print("The shape is: ",iris.shape, '\n---')
print("Info:",iris.info(), '\n---') # memory usage, name, dtype, and # of non-null obs (--> # of missing obs) per variable
print(iris.describe(), '\n---') # summary stats, and you can customize the list!
print(iris['species'].value_counts()[:10], '\n---')
print(iris['species'].nunique(), '\n---')
```

Notice that the output does NOT show! **You have to copy in figures and tables from the notebooks.**
