---
title: "Visualizing Text and Distributions"
author: "Susmitha Gopavaram- 'sgopavaram2200@floridapoly.edu"
date: '2022-06-06'
output: html_document
---

# Data Visualization Project 03

**"We have accomplished all the visualizations that the professor suggested using the hints he provided and the materials he uploaded through links and in the canvas."**

In this exercise we explore methods to visualize text data and practice how to recreate charts that show the distributions of a continuous variable. 


## Part 1: Density Plots

Using the dataset obtained from FSU's [Florida Climate Center](https://climatecenter.fsu.edu/climate-data-access-tools/downloadable-data), for a station at Tampa International Airport (TPA) from 2016 to 2017, attempt to recreate the charts shown below


```r
library(tidyverse)
weather_tpa <- read_csv("https://github.com/reisanar/datasets/raw/master/tpa_weather_16_17.csv")
# random sample 
sample_n(weather_tpa, 4)
```

```
## # A tibble: 4 x 6
##    year month   day precipitation max_temp min_temp
##   <dbl> <dbl> <dbl>         <dbl>    <dbl>    <dbl>
## 1  2016     8     3          0          90       77
## 2  2016     6    10          0.52       88       76
## 3  2016     2    16          0.25       71       55
## 4  2016     1    14          0.02       69       50
```

See https://www.reisanar.com/slides/relationships-models#10 for a reminder on how to use this dataset with the `lubridate` package for dates and times.


(a) Recreate the plot below:

<img src="https://github.com/reisanar/figs/raw/master/tpa_max_temps_facet.png" width="80%" style="display: block; margin: auto;" />

Hint: the option `binwidth = 3` was used with the `geom_histogram()` function.

## **Here is my plot A which I recreated**

![A_plot](https://github.com/susmithareddy-1996/dataviz_final_project/blob/main/figures/3plot_1.jpg)

-----------------------------

(b) Recreate the plot below:

<img src="https://github.com/reisanar/figs/raw/master/tpa_max_temps_density.png" width="80%" style="display: block; margin: auto;" />

Hint: check the `kernel` parameter of the `geom_density()` function, and use `bw = 0.5`.

## **Here is my plot B which I recreated**

![B_plot](https://github.com/susmithareddy-1996/dataviz_final_project/blob/main/figures/3plot_2.jpg)

------------------------------

(c) Recreate the chart below:

<img src="https://github.com/reisanar/figs/raw/master/tpa_max_temps_density_facet.png" width="80%" style="display: block; margin: auto;" />

Hint: default options for `geom_density()` were used. 

## **Here is my plot C which I recreated**

![C_plot](https://github.com/susmithareddy-1996/dataviz_final_project/blob/main/figures/3plot_3.jpg)

--------------------------

(d) Recreate the chart below:

<img src="https://github.com/reisanar/figs/raw/master/tpa_max_temps_ridges.png" width="80%" style="display: block; margin: auto;" />

Hint: default options for `geom_density()` were used. 

## **Here is my plot D which I recreated**

![D_plot](https://github.com/susmithareddy-1996/dataviz_final_project/blob/main/figures/3plot_4.jpg)

------------------------------

(e) Recreate the plot below:

<img src="https://github.com/reisanar/figs/raw/master/tpa_max_temps_ridges.png" width="80%" style="display: block; margin: auto;" />

Hint: use the`ggridges` package, and the `geom_density_ridges()` function paying close attention to the `quantile_lines` and `quantiles` parameters.

## **Here is my plot E which I recreated**

![E_plot](https://github.com/susmithareddy-1996/dataviz_final_project/blob/main/figures/3plot_5.jpg)

------------------------------------

(f) Recreate the chart below:

<img src="https://github.com/reisanar/figs/raw/master/tpa_max_temps_ridges_plasma.png" width="80%" style="display: block; margin: auto;" />

Hint: this uses the `plasma` option (color scale) for the _viridis_ palette.

## **Here is my plot B which I recreated**

![F_plot](https://github.com/susmithareddy-1996/dataviz_final_project/blob/main/figures/3plot_6.jpg)


---------------------------------


## Part 2: Visualizing Text Data

Review the set of slides (and additional resources linked in it) for visualizing text data: https://www.reisanar.com/slides/text-viz#1

**"Trying to visualize text data using Billboard Top 100 Lyrics datasets was part 2 of the project"**

Make sure to include a copy of the dataset in the `data/` folder, and reference your sources if different from the ones listed below:

- [Billboard Top 100 Lyrics](https://github.com/reisanar/datasets/blob/master/BB_top100_2015.csv)

- [RateMyProfessors comments](https://github.com/reisanar/datasets/blob/master/rmp_wit_comments.csv)

- [FL Poly News 2020](https://github.com/reisanar/datasets/blob/master/poly_news_FL20.csv)

- [FL Poly News 2019](https://github.com/reisanar/datasets/blob/master/poly_news_FL19.csv)

(to get the "raw" data from any of the links listed above, simply click on the `raw` button of the GitHub page and copy the URL to be able to read it in your computer using the `read_csv()` function)
