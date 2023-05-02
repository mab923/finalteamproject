# Welcome to our [team project website!](https://mab923.github.io/finalteamproject)

This is a website to showcase our final project for FIN 377 - Data Science for Finance course at Lehigh University.

The basis for this report was analyzing the connection between the changes in interest rates brought on by FOMC meetings on the stock market and bonds. The project analyzes the S&P 500 as an indicator for stock correlation and the VBIRX and VBILX indexes as bond samples. 

# Hypothesis 

We suspect that large increases in interest rates would lead to negative or lower returns in the days before and after an FOMC meeting and vice versa



To see the complete analysis file(s) click [here](https://github.com/mab923/finalteamproject/blob/main/Analysis/Final_Analysis.ipynb).



## Table of contents
1. [Introduction](#introduction)
2. [Methodology](#meth)
3. [Section 2](#section2)
    1. [Subsection](#subsec2-1)
    2. [Subsection](#subsec2-2)
4. [Analysis Section](#section3)
5. [Summary](#summary)

## Introduction  <a name="introduction"></a>

Interest rate changes can have large effects on the economy in both the stock and bond market. We wanted to look deeper into how these securities react to changes in the days leading up to and following a FOMC meeting and corresponding hike. 

## Methodology <a name="meth"></a>

The first step in 
 
Note that for the purposes of the website, you have to copy this code into the markdown file and  
put the code inside trip backticks with the keyword `python`.

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

## Section <a name="section2"></a>
Blah blah

### Subsection 1 <a name="subsec2-1"></a>
This is a subsection, formatted in heading 3 style

### Subsection 2 <a name="subsec2-2"></a>
This is a subsection, formatted in heading 3 style

## Analysis Section <a name="section3"></a>

Here are some graphs that we created in our analysis. We saved them to the `pics/` subfolder and include them via the usual markdown syntax for pictures.

![](pics/plot1.png)
<br><br>
Some analysis here
<br><br>
![](pics/plot2.png)
<br><br>
More analysis here.
<br><br>
![](pics/plot3.png)
<br><br>
More analysis.

## Summary <a name="summary"></a>

Blah blah



## About the team
finalteamproject/pics/6FB5FD7F-9E42-4F5C-BE04-D13CF10E6667.jpeg
<img src="pics/6FB5FD7F-9E42-4F5C-BE04-D13CF10E6667.jpeg" alt="nathan" width="300"/>
<br>
Nathan is a senior at Lehigh studying finance and business analytics.
<br><br><br>
<img src="pics/don2.jpg" alt="don" width="300"/>
<br>
Don is an assistant professor at Lehigh.


## More 

