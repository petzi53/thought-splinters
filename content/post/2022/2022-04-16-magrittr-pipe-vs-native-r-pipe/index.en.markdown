---
title: magrittr Pipe vs Native R Pipe
author: Peter Baumgartner
date: '2022-04-16'
slug: magrittr-pipe-vs-native-r-pipe
categories: []
tags: []
subtitle: ''
summary: ''
authors: []
lastmod: ''
bibliography:
  - ../../../../static/media/references.bib
featured: no
commentable: yes
side_toc: yes
draft: yes
image:
  placement: 2
  caption: ''
  alt_text: ''
  focal_point: Center
  preview_only: no
---

# Introduction

After some practice, I got familiarized with the {magrittr} r pipe. It is a way to chain commands following each other.

## Resources

-   https://www.rstudio.com/blog/rstudio-v1-4-update-whats-new/

``` r
library(tidyverse)
```

    ## ── Attaching packages ─────────────────────────────────────── tidyverse 1.3.1 ──

    ## ✓ ggplot2 3.3.5     ✓ purrr   0.3.4
    ## ✓ tibble  3.1.6     ✓ dplyr   1.0.8
    ## ✓ tidyr   1.2.0     ✓ stringr 1.4.0
    ## ✓ readr   2.1.2     ✓ forcats 0.5.1

    ## ── Conflicts ────────────────────────────────────────── tidyverse_conflicts() ──
    ## x dplyr::filter() masks stats::filter()
    ## x dplyr::lag()    masks stats::lag()

``` r
iris %>%
  as_tibble %>%
  select(Sepal.Length, Species) %>%
  summary
```

    ##   Sepal.Length         Species  
    ##  Min.   :4.300   setosa    :50  
    ##  1st Qu.:5.100   versicolor:50  
    ##  Median :5.800   virginica :50  
    ##  Mean   :5.843                  
    ##  3rd Qu.:6.400                  
    ##  Max.   :7.900

``` r
my_iris <- as_tibble(iris)
my_iris2 <-  select(my_iris, c(Sepal.Length, Species))
my_iris3 <- arrange(my_iris2, desc(Sepal.Length))
my_iris3
```

    ## # A tibble: 150 × 2
    ##    Sepal.Length Species  
    ##           <dbl> <fct>    
    ##  1          7.9 virginica
    ##  2          7.7 virginica
    ##  3          7.7 virginica
    ##  4          7.7 virginica
    ##  5          7.7 virginica
    ##  6          7.6 virginica
    ##  7          7.4 virginica
    ##  8          7.3 virginica
    ##  9          7.2 virginica
    ## 10          7.2 virginica
    ## # … with 140 more rows

``` r
as_tibble(select(arrange(iris, desc(Sepal.Length)), c(Sepal.Length, Species)))
```

    ## # A tibble: 150 × 2
    ##    Sepal.Length Species  
    ##           <dbl> <fct>    
    ##  1          7.9 virginica
    ##  2          7.7 virginica
    ##  3          7.7 virginica
    ##  4          7.7 virginica
    ##  5          7.7 virginica
    ##  6          7.6 virginica
    ##  7          7.4 virginica
    ##  8          7.3 virginica
    ##  9          7.2 virginica
    ## 10          7.2 virginica
    ## # … with 140 more rows

``` r
iris |> 
  as_tibble()  |> 
  select(Sepal.Length, Species)  |>
  arrange(desc(Sepal.Length))
```

    ## # A tibble: 150 × 2
    ##    Sepal.Length Species  
    ##           <dbl> <fct>    
    ##  1          7.9 virginica
    ##  2          7.7 virginica
    ##  3          7.7 virginica
    ##  4          7.7 virginica
    ##  5          7.7 virginica
    ##  6          7.6 virginica
    ##  7          7.4 virginica
    ##  8          7.3 virginica
    ##  9          7.2 virginica
    ## 10          7.2 virginica
    ## # … with 140 more rows

``` r
# generates error!
# Error in parse(text = x, srcfile = src) : 
#   '=>' is disabled; set '_R_USE_PIPEBIND_' envvar to a true value to enable it
Sys.setenv(`_R_USE_PIPEBIND_` = TRUE) 

mtcars |> 
   . => lm(mpg ~ disp, data = .)
```
