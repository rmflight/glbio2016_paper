---
title: "Visualizing Effect of Data Transformations on Errors"
author: "Robert M Flight"
date: "2016-01-01 21:00:58"
output: html_document
---






# Introduction

Data transformations are frequently applied to different -omics data to change
properties of the data and make it more amenable to various statistical assumptions.
Included in the types of changes that are made include changing the error structure,
frequently from multiplicative errors that are commonly present in any data
generated by counts at a detector (essentially all -omics data) to additive errors,
which are more easily handled by most statistical methods.

# Methods



## Data

Simulated data was generated from an initial set of 10000 points drawn from 
a log-normal distribution with a mean in log-space of 1 and a standard deviation
of 1 (see histogram in Figure X). These data points are the **pure** initial 
data to which different types of error are added. From this set, 100 replicates are 
generated with either *additive*, *proportional* or *mixed* (both additive and
proportional) error.



<img src="glbio2016_manuscript_files/figure-html/pure_histogram-1.png" title="" alt="" width="672" />

### Additive Error



<img src="glbio2016_manuscript_files/figure-html/add_plot-1.png" title="" alt="" width="672" />

Additive error was added where the standard deviation was 2. A plot
of two replicates is shown in Figure X.

### Proportional Error



<img src="glbio2016_manuscript_files/figure-html/prop_plot-1.png" title="" alt="" width="672" />

Proportional error was added where the standard deviation was 0.1. A plot
of two replicates is shown in Figure X.

### Mixed Error



<img src="glbio2016_manuscript_files/figure-html/mix_plot-1.png" title="" alt="" width="672" />

Mixture of additive and proportional error was added with standard deviations
of 2 and 0.1 respectively.

## Transformations



# Results



# Conclusion


# Session Information


```
##  setting  value                       
##  version  R version 3.2.2 (2015-08-14)
##  system   x86_64, linux-gnu           
##  ui       RStudio (0.99.825)          
##  language (EN)                        
##  collate  en_US.UTF-8                 
##  tz       America/New_York            
##  date     2016-01-01
```



|package                     |*  |version    |date       |source                                   |
|:---------------------------|:--|:----------|:----------|:----------------------------------------|
|assertthat                  |   |0.1        |2013-12-06 |CRAN (R 3.2.2)                           |
|circlize                    |   |0.3.2      |2015-10-21 |CRAN (R 3.2.2)                           |
|colorspace                  |   |1.2-6      |2015-03-11 |CRAN (R 3.2.2)                           |
|ComplexHeatmap              |   |1.7.1      |2015-10-10 |Github (jokergoo/ComplexHeatmap@e502955) |
|cowplot                     |*  |0.6.0      |2015-12-19 |CRAN (R 3.2.2)                           |
|DBI                         |   |0.3.1      |2014-09-24 |CRAN (R 3.2.2)                           |
|dendextend                  |   |1.1.2      |2015-10-31 |CRAN (R 3.2.2)                           |
|dendsort                    |   |0.3.2      |2014-09-29 |CRAN (R 3.2.2)                           |
|devtools                    |   |1.9.1.9000 |2015-11-18 |Github (hadley/devtools@b4edf3e)         |
|digest                      |   |0.6.8      |2014-12-31 |CRAN (R 3.2.2)                           |
|dplyr                       |*  |0.4.3      |2015-09-01 |CRAN (R 3.2.2)                           |
|evaluate                    |   |0.8        |2015-09-18 |CRAN (R 3.2.2)                           |
|fakeDataWithError           |*  |0.0.1      |2015-10-19 |local                                    |
|formatR                     |   |1.2.1      |2015-09-18 |CRAN (R 3.2.2)                           |
|GetoptLong                  |   |0.1.0      |2015-03-09 |CRAN (R 3.2.2)                           |
|ggbiplot                    |   |0.55       |2015-10-19 |Github (rmflight/ggbiplot@7325e88)       |
|ggplot2                     |*  |2.0.0      |2015-12-18 |CRAN (R 3.2.2)                           |
|GlobalOptions               |   |0.0.8      |2015-08-18 |CRAN (R 3.2.2)                           |
|gtable                      |   |0.1.2      |2012-12-05 |CRAN (R 3.2.2)                           |
|htmltools                   |   |0.2.6      |2014-09-08 |CRAN (R 3.2.2)                           |
|knitr                       |   |1.11       |2015-08-14 |CRAN (R 3.2.2)                           |
|labeling                    |   |0.3        |2014-08-23 |CRAN (R 3.2.2)                           |
|lazyeval                    |   |0.1.10     |2015-01-02 |CRAN (R 3.2.2)                           |
|magrittr                    |   |1.5        |2014-11-22 |CRAN (R 3.2.2)                           |
|memoise                     |   |0.2.1      |2014-04-22 |CRAN (R 3.2.2)                           |
|munsell                     |   |0.4.2      |2013-07-11 |CRAN (R 3.2.2)                           |
|plyr                        |   |1.8.3      |2015-06-12 |CRAN (R 3.2.2)                           |
|R6                          |   |2.1.1      |2015-08-19 |CRAN (R 3.2.2)                           |
|RColorBrewer                |   |1.1-2      |2014-12-07 |CRAN (R 3.2.2)                           |
|Rcpp                        |   |0.12.2     |2015-11-15 |CRAN (R 3.2.2)                           |
|reshape2                    |   |1.4.1      |2014-12-06 |CRAN (R 3.2.2)                           |
|rjson                       |   |0.2.15     |2014-11-03 |CRAN (R 3.2.2)                           |
|rmarkdown                   |   |0.8.1      |2015-10-10 |CRAN (R 3.2.2)                           |
|scales                      |   |0.3.0      |2015-08-25 |CRAN (R 3.2.2)                           |
|shape                       |   |1.4.2      |2014-11-05 |CRAN (R 3.2.2)                           |
|stringi                     |   |1.0-1      |2015-10-22 |CRAN (R 3.2.2)                           |
|stringr                     |   |1.0.0      |2015-04-30 |CRAN (R 3.2.2)                           |
|visualizationQualityControl |*  |0.0.20     |2015-12-16 |local                                    |
|whisker                     |   |0.3-2      |2013-04-28 |CRAN (R 3.2.2)                           |
|yaml                        |   |2.1.13     |2014-06-12 |CRAN (R 3.2.2)                           |


# Create Markdown

