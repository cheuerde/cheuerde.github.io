---
title: My First Post
author: ''
date: '2024-04-27'
slug: my-first-post
categories: []
tags: []
subtitle: ''
summary: ''
authors: []
lastmod: '2024-04-27T07:52:16+02:00'
featured: no
image:
  caption: 'HALLO'
  focal_point: ''
  preview_only: no
projects: []
---

## Using `plotcli` convenience wrappers

# Density plot


```r
if(!require(plotcli)) install.packages("plotcli")
```

```
## Loading required package: plotcli
```

```
## Loading required package: R6
```

```
## Loading required package: crayon
```

```
## Loading required package: stringr
```

```
## Loading required package: ggplot2
```

```
## 
## Attaching package: 'ggplot2'
```

```
## The following object is masked from 'package:crayon':
## 
##     %+%
```

```
## Loading required package: knitr
```

```
## Loading required package: rmarkdown
```

```
## plotcli loaded. Use plotcli_options() to set global options.
```

```r
library(plotcli)
# Generate sample data
sample_data <- rnorm(1000, mean = 5, sd = 2)

# Create a density plot
plotcli_density(sample_data, color = "blue", braille = TRUE)
```

```
## 
##                                                                                 
##                  ┌────────────────────────────────────────────────────────────┐ 
##              0.2 │                          ⢅⡔⡤⡴⠦                             │ 
##                  │                         ⡳⠒   ⡳⠤                            │ 
##                  │                        ⢐⠣     ⡤⠦                           │ 
##                  │                       ⠰⠶       ⡣⡈                          │ 
##                  │                       ⡇         ⡐⢤⠦                        │ 
##              0.2 │                      ⡳            ⡃⠘                       │ 
##                  │                     ⡰⠣             ⡲⠢                      │ 
##                  │                     ⠘               ⡥                      │ 
##                  │                    ⡱⠑               ⠰⠘                     │ 
##   Density    0.1 │                   ⠰⠥                 ⡂⠖                    │ 
##                  │                   ⠷                   ⡓⠨                   │ 
##                  │                  ⡱⠒                    ⡓⠦                  │ 
##                  │                 ⢁⠤                      ⡓⠦                 │ 
##                  │                ⢁⠦                        ⡤⠢                │ 
##              0.1 │               ⢃⠤                          ⡵                │ 
##                  │              ⡧⠔                            ⡧               │ 
##                  │            ⡐⡩⠑                             ⡀⡖              │ 
##                  │           ⢉⡄                                ⡀⢗             │ 
##                  │        ⢁⢪⡤⠑                                   ⡤⢚⡨          │ 
##              0.0 │⣨⣈⢨⣈⢨⢘⡔⡕⠔                                        ⡀⡕⡴⢪⣈⢨⣈⢨⣈⢨⠬│ 
##                  └────────────────────────────────────────────────────────────┘ 
##                                                                                 
##                   -2.0           1.6           5.1            8.7         12.3  
##                                                                                 
##                                                x                                
## 
```

