---
title: "PA1_template.Rmd"
author: "Ganesh Prabhupatkar"
date: '2017-12-14'
output: 
  html_document:
    keep_md: true
    self_contained: true
Assignment: Analyzing FitBit Data
#This assignment will be described in multiple parts. You #will need to write a report that answers the questions #detailed below. Ultimately, you will need to complete the #entire assignment in a single R markdown document that can #be processed by knitr and be transformed into an HTML file
---

#Loading and preprocessing the data

### 1.Load the data (i.e. read.csv())
### 2.Process/transform the data (if necessary) into a format suitable for your analysis



#What is mean total number of steps taken per day?

###1.Make a histogram of the total number of steps taken each day

###2.Calculate and report the mean and median total number of steps taken per day


![](PA1_template_files/figure-html/unnamed-chunk-1-1.png)<!-- -->

```
## [1] "Mean Steps per Day = 10766.1886792453"
```

```
## [1] "Median Steps per Day = 10765"
```

#What is the average daily activity pattern?

###1.Make a time series plot (i.e. type = "l") of the 5-minute interval (x-axis) and the average number of steps taken, averaged across all days (y-axis)

###2.Which 5-minute interval, on average across all the days in the dataset, contains the maximum number of steps?

![](PA1_template_files/figure-html/unnamed-chunk-2-1.png)<!-- -->

```
## [1] "Interval with max value = 835"
```

#Imputing missing values
####1.Calculate and report the total number of missing values in   the dataset (i.e. the total number of rows with NAs) 
####2.Devise a strategy for filling in all of the missing values   in the dataset. The strategy does not need to be            sophisticated. For example, you could use the mean/median   for that day, or the mean for that 5-minute interval, etc. 
####3.Create a new dataset that is equal to the original dataset   but with the missing data filled in. 
####4.Make a histogram of the total number of steps taken each    day and Calculate and report the mean and median total      number of steps taken per day. Do these values differ from   the estimates from the first part of the assignment? What   is the impact of imputing missing data on the estimates of   the total daily number of steps?

```
## [1] "Total number of missing values in dataset =  2304"
```

![](PA1_template_files/figure-html/unnamed-chunk-3-1.png)<!-- -->

```
## [1] "Revised Mean Steps per Day = 10589.6937828642"
```

```
## [1] "Revised Median Steps per Day = 10766.1886792453"
```

```
## [1] "Difference of Mean Steps per Day = -176.494896381069"
```

```
## [1] "Difference of Median Steps per Day = 1.1886792452824"
```

```
## [1] "Total difference of Steps per Day = 75363.320754717"
```

#Are there differences in activity patterns between weekdays and weekends?

####1.Create a new factor variable in the dataset with two levels -- "weekday" and "weekend" indicating whether a given date is a weekday or weekend day.

####2.Make a panel plot containing a time series plot (i.e. type = "l") of the 5-minute interval (x-axis) and the average number of steps taken, averaged across all weekday days or weekend days (y-axis). The plot should look something like the following, which was created using simulated data:
![](PA1_template_files/figure-html/unnamed-chunk-4-1.png)<!-- -->
