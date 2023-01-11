---
title: "Reproducible Research: Peer Assessment 1"
output: 
  html_document:
    keep_md: true
---


## Loading and preprocessing the data


```r
data <- read.csv("activity/activity.csv")
```

## What is mean total number of steps taken per day?


```r
steps <- aggregate(data$steps, by = list(data$date), sum, na.rm = TRUE)

mean(steps$x, na.rm = TRUE)
```

```
## [1] 9354.23
```

## What is the average daily activity pattern?



## Imputing missing values



## Are there differences in activity patterns between weekdays and weekends?
