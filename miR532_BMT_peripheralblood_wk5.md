---
title: "miR532_BMT_peripheralblood_wk5"
author: "Patrick Lac"
date: "April 12, 2020"
output: 
  html_document: 
    keep_md: yes
---





Let's begin by importing our data:


```r
metadata <- read.csv("F:/Git/PLac Analyses/miR-532 project/miR532_BMT/Data/200412_MetaData.csv")
JL_data <- read.csv("F:/Git/PLac Analyses/miR-532 project/miR532_BMT/Data/200412_JL_Data.csv")
MB_data <- read.csv("F:/Git/PLac Analyses/miR-532 project/miR532_BMT/Data/200412_MB_Data.csv")
PL_data <- read.csv("F:/Git/PLac Analyses/miR-532 project/miR532_BMT/Data/200412_PL_Data.csv")
```

Next lets attach the different peripheral blood data together:

```
##   ï..Sample          Original.label Treatment Weeks.post.transplant WBC  RBC
## 1     MIG.1 BMT1.MIG (NEP cage 1/2)   control                     5 5.2 9.57
## 2     MIG.2 BMT1.MIG (REP cage 1/2)   control                     5 3.6 9.37
## 3     MIG.3 BMT1.MIG (BEP cage 2/2)   control                     5 6.5 9.58
## 4     MIG.4 BMT1.MIG (REP cage 2/2)   control                     5 6.2 9.74
## 5     MIG.5 BMT2.MIG (cage 2/2 BEP)   control                     5 4.5 9.84
## 6     MIG.6 BMT2.MIG (cage 2/2 LEP)   control                     5 3.0 9.83
##    HGB  HCT MCV  MCH MCHC PLT MPV  RDW Percent.Lym Percent.Mon Percent.Gra
## 1 14.7 45.7  48 15.4 32.2 473 6.8 15.7          NA          NA          NA
## 2 14.3 43.0  46 15.3 33.3 605 6.5 15.5          NA          NA          NA
## 3 14.6 44.4  46 15.3 32.9 453 6.7 15.3          NA          NA          NA
## 4 15.1 45.7  47 15.5 33.1 540 7.3 15.3          NA          NA          NA
## 5 14.6 45.8  46 14.9 32.0 631 6.5 16.0          NA          NA          NA
## 6 14.4 44.8  46 14.6 32.2 900 6.0 15.8          NA          NA          NA
##   Number.Lym Number.Mon Number.Gra  GFP
## 1        2.3        0.3        2.6 85.2
## 2        2.1        0.3        1.2 86.8
## 3        3.0        0.5        3.0 88.7
## 4        3.6        0.5        2.1 87.8
## 5        2.6        0.4        1.5 82.3
## 6        1.4        0.2        1.4 82.2
```

We will make a copy of the total data for manipulation:

What are the dimensions of our data?

```
## [1] 368  21
```

## Peripheral bleeds 5 weeks post-transplant:
Next we will filter for CBC data at 5 weeks post-transplant


Let's check the dimensions of our subsetted data:

```
## [1] 48 21
```

Let's make dotplots for our CBC counts:

![](miR532_BMT_peripheralblood_wk5_files/figure-html/wk5.WBC-1.png)<!-- -->



![](miR532_BMT_peripheralblood_wk5_files/figure-html/wk5.RBC-1.png)<!-- -->



![](miR532_BMT_peripheralblood_wk5_files/figure-html/wk5.HGB-1.png)<!-- -->



![](miR532_BMT_peripheralblood_wk5_files/figure-html/wk5.HCT-1.png)<!-- -->



![](miR532_BMT_peripheralblood_wk5_files/figure-html/wk5.PLT-1.png)<!-- -->



![](miR532_BMT_peripheralblood_wk5_files/figure-html/wk5.MCV-1.png)<!-- -->



![](miR532_BMT_peripheralblood_wk5_files/figure-html/wk5.MCH-1.png)<!-- -->



![](miR532_BMT_peripheralblood_wk5_files/figure-html/wk5.MCHC-1.png)<!-- -->



![](miR532_BMT_peripheralblood_wk5_files/figure-html/wk5.RDW-1.png)<!-- -->



![](miR532_BMT_peripheralblood_wk5_files/figure-html/wk5.MPV-1.png)<!-- -->



![](miR532_BMT_peripheralblood_wk5_files/figure-html/wk5.Percent.Lym-1.png)<!-- -->



![](miR532_BMT_peripheralblood_wk5_files/figure-html/wk5.Percent.Mon-1.png)<!-- -->



![](miR532_BMT_peripheralblood_wk5_files/figure-html/wk5.Percent.Gra-1.png)<!-- -->



![](miR532_BMT_peripheralblood_wk5_files/figure-html/wk5.Number.Lym-1.png)<!-- -->



![](miR532_BMT_peripheralblood_wk5_files/figure-html/wk5.Number.Mon-1.png)<!-- -->



![](miR532_BMT_peripheralblood_wk5_files/figure-html/wk5.Number.Gra-1.png)<!-- -->

### Now let's arrange the plots:
#### Figure 1
![](miR532_BMT_peripheralblood_wk5_files/figure-html/figure1-1.png)<!-- -->


#### Figure 2
![](miR532_BMT_peripheralblood_wk5_files/figure-html/figure2-1.png)<!-- -->


### Notes
The four miR-532 mice with high granulocytes had lower peripheral blood engraftment (37-45% GFP+)
Two of these four mice had low lymphocyte and monocyte counts.
The other two mice had relatively high monocyte counts, but lower than average lymphocyte counts.

ID, GFP+ %, Lym, Mon, Gra
miR532-29, 43.2,  1.8, 0.9, 7.5
miR532-14, 45.5, 1.1, 0.3, 5.6
miR532-30, 37.4, 2.0, 0.8, 4.3
miR532-8, 44.3, 0.9, 0.2, 4.0
          
#### Making a figure for just WBC, RBC, and platelets
![](miR532_BMT_peripheralblood_wk5_files/figure-html/figure3-1.png)<!-- -->