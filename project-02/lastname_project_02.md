---
title: "Report for Data Visualization Mini-Project 2"
author: "Susmitha Gopavaram -sgopavaram2200@floridapoly.edu"
date: '2022-06-15'
output: html_document
---


# Data Visualization Project 02

**"Among the Data sets in the list, this one caught my eye. In addition to the name, age, gender, country, state, city and state (where available), the data set has the expected time, finish time and pace, overall place, division place, gender place and age place of 26410 finishers of the 2017 Boston Marathon"**.

**The link for the chosen Dataset is:**

[Marathon_finishers](https://github.com/susmithareddy-1996/dataviz_final_project/blob/main/data/marathon_results_2017.csv)

**Cleaning the data set**

During data cleansing, all the existing data in a database is reviewed and deleted or updated if it is outdated, incomplete, incorrect, improperly formatted, duplicate, or irrelevant. Data cleansing usually involves cleaning up data compiled in one area.

Here I use na.omit() to drop my null values in the data set

In the process of cleaning data I want to drop Proj.Time column because it dosen't have any numerical values 

> ## **Finishers by Age and Gender**
 
 **Which finishers took the top spot?**

In general, both male and female endurance runners experience significant declines in performance with advancing age, but the magnitude is greater for female runners.

Among the finishing age ranges for men and women, the youngest was 18 and the oldest was 83.

![Plot1](https://github.com/susmithareddy-1996/dataviz_final_project/blob/main/figures/plot1)

Among younger runners, females outnumber males, but this bias reverses when it comes to older runners, who tend to run at an age that is suitable for both genders. Here I created a Interactive Plot in X axies we give the Age and y axies we took count to know the number of Males and Female runner's and their count

Study findings show that runners slowed by a linear rate of about one percent each year when they were 40 to 70 years old. By the late 70s, the rate of decline for runners started declining by about 1.5 percent, and between 90 and 95, the decline accelerated to two to three percent.

![Plot2](https://github.com/susmithareddy-1996/dataviz_final_project/blob/main/figures/plot2)

Based on this graph, the average finish time in males over 54 is higher than that of all remaining ages.

------------------------

> ## **Top Country Participants**

In this case, I intend to create a global spatial graph for 27-year-old participants around the world. 

want to Know top countries Participants?

![Plot3](https://github.com/susmithareddy-1996/dataviz_final_project/blob/main/figures/plot3.jpg)

