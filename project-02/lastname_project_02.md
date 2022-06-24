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
