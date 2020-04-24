---
title: "miR532_BMT_peripheralblood_wk5"
author: "Patrick Lac"
date: "April 12, 2020"
output: 
  html_document: 
    keep_md: yes
---





Let's begin by importing our data:



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

![](miR532_BMT_peripheralblood_files/figure-html/wk5.WBC-1.png)<!-- -->



![](miR532_BMT_peripheralblood_files/figure-html/wk5.RBC-1.png)<!-- -->



![](miR532_BMT_peripheralblood_files/figure-html/wk5.HGB-1.png)<!-- -->



![](miR532_BMT_peripheralblood_files/figure-html/wk5.HCT-1.png)<!-- -->



![](miR532_BMT_peripheralblood_files/figure-html/wk5.PLT-1.png)<!-- -->



![](miR532_BMT_peripheralblood_files/figure-html/wk5.MCV-1.png)<!-- -->



![](miR532_BMT_peripheralblood_files/figure-html/wk5.MCH-1.png)<!-- -->



![](miR532_BMT_peripheralblood_files/figure-html/wk5.MCHC-1.png)<!-- -->



![](miR532_BMT_peripheralblood_files/figure-html/wk5.RDW-1.png)<!-- -->



![](miR532_BMT_peripheralblood_files/figure-html/wk5.MPV-1.png)<!-- -->



![](miR532_BMT_peripheralblood_files/figure-html/wk5.Percent.Lym-1.png)<!-- -->



![](miR532_BMT_peripheralblood_files/figure-html/wk5.Percent.Mon-1.png)<!-- -->



![](miR532_BMT_peripheralblood_files/figure-html/wk5.Percent.Gra-1.png)<!-- -->



![](miR532_BMT_peripheralblood_files/figure-html/wk5.Number.Lym-1.png)<!-- -->



![](miR532_BMT_peripheralblood_files/figure-html/wk5.Number.Mon-1.png)<!-- -->



![](miR532_BMT_peripheralblood_files/figure-html/wk5.Number.Gra-1.png)<!-- -->

### Now let's arrange the plots:
#### Figure 1
![](miR532_BMT_peripheralblood_files/figure-html/wk5.fig1-1.png)<!-- -->

#### Figure 2
![](miR532_BMT_peripheralblood_files/figure-html/wk5.fig2-1.png)<!-- -->

### Notes
The four miR-532 mice with high granulocytes and lower peripheral blood engraftment (37-45% GFP+) at week 5:

At week5  
ID, GFP+ %, Lym, Mon, Gra  
miR532-29, 43.2,  1.8, 0.9, 7.5  
miR532-14, 45.5, 1.1, 0.3, 5.6  
miR532-30, 37.4, 2.0, 0.8, 4.3  
miR532-8, 44.3, 0.9, 0.2, 4.0  

At week11  
ID, GFP+ %, Lym, Mon, Gra  
miR532-29,  
miR532-14, 43.1, 3.0, 0.5, 5.8  
miR532-30,  
miR532-8, 55.0, 2.3, 0.4, 2.6   

## Peripheral bleeds 11 weeks post-transplant:
Next we will filter for CBC data at 11 weeks post-transplant

```
##    ï..Sample          Original.label Treatment Weeks.post.transplant  WBC   RBC
## 28     MIG.1 BMT1.MIG (NEP cage 1/2)   control                    10  5.0 10.84
## 29     MIG.2 BMT1.MIG (REP cage 1/2)   control                    10 11.1 10.81
## 30     MIG.3 BMT1.MIG (BEP cage 2/2)   control                    10  3.4 11.07
## 31     MIG.4 BMT1.MIG (REP cage 2/2)   control                    10  3.8 11.22
## 32     MIG.5 BMT2.MIG (cage 2/2 BEP)   control                    11  4.5 10.77
## 33     MIG.6 BMT2.MIG (cage 2/2 LEP)   control                    11  6.3 10.13
##     HGB  HCT MCV  MCH MCHC PLT MPV  RDW Percent.Lym Percent.Mon Percent.Gra
## 28 16.4 50.4  46 15.1 32.5 614 6.4 15.3          NA          NA          NA
## 29 15.5 47.7  44 14.4 32.6 567 6.7 15.9          NA          NA          NA
## 30 16.0 48.0  43 14.5 33.4 720 6.0 14.6          NA          NA          NA
## 31 16.0 49.3  44 14.3 32.5 790 6.4 15.5          NA          NA          NA
## 32 14.8 47.0  44 13.8 31.5 756 6.6 15.9          NA          NA          NA
## 33 14.4 44.3  44 14.2 32.6 799 6.1 15.4          NA          NA          NA
##    Number.Lym Number.Mon Number.Gra  GFP
## 28        3.1        0.4        1.5 86.7
## 29        4.3        0.7        6.1 87.5
## 30        2.2        0.2        1.0 88.9
## 31        2.4        0.2        1.2 84.8
## 32        0.5        0.3        3.7 73.6
## 33        2.8        0.5        3.0 66.5
```

Let's check the dimensions of our subsetted data:

```
## [1] 48 21
```

Let's make dotplots for our CBC counts:

![](miR532_BMT_peripheralblood_files/figure-html/wk11.WBC-1.png)<!-- -->



![](miR532_BMT_peripheralblood_files/figure-html/wk11.RBC-1.png)<!-- -->



![](miR532_BMT_peripheralblood_files/figure-html/wk11.HGB-1.png)<!-- -->



![](miR532_BMT_peripheralblood_files/figure-html/wk11.HCT-1.png)<!-- -->



![](miR532_BMT_peripheralblood_files/figure-html/wk11.PLT-1.png)<!-- -->



![](miR532_BMT_peripheralblood_files/figure-html/wk11.MCV-1.png)<!-- -->



![](miR532_BMT_peripheralblood_files/figure-html/wk11.MCH-1.png)<!-- -->



![](miR532_BMT_peripheralblood_files/figure-html/wk11.MCHC-1.png)<!-- -->



![](miR532_BMT_peripheralblood_files/figure-html/wk11.RDW-1.png)<!-- -->



![](miR532_BMT_peripheralblood_files/figure-html/wk11.MPV-1.png)<!-- -->



![](miR532_BMT_peripheralblood_files/figure-html/wk11.Percent.Lym-1.png)<!-- -->



![](miR532_BMT_peripheralblood_files/figure-html/wk11.Percent.Mon-1.png)<!-- -->



![](miR532_BMT_peripheralblood_files/figure-html/wk11.Percent.Gra-1.png)<!-- -->



![](miR532_BMT_peripheralblood_files/figure-html/wk11.Number.Lym-1.png)<!-- -->



![](miR532_BMT_peripheralblood_files/figure-html/wk11.Number.Mon-1.png)<!-- -->



![](miR532_BMT_peripheralblood_files/figure-html/wk11.Number.Gra-1.png)<!-- -->

### Now let's arrange the plots:
#### Figure 3
![](miR532_BMT_peripheralblood_files/figure-html/wk11.fig1-1.png)<!-- -->

#### Figure 4
![](miR532_BMT_peripheralblood_files/figure-html/wk11.fig2-1.png)<!-- -->
