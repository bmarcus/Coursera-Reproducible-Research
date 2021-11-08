---
title: "Reproducible Research: Peer Assessment 1"
output:
  html_document:
    keep_md: true
---
## Loading and preprocessing the data (also unzip raw data)

```r
# set working directory to "/Users/brad/Documents/development/repos/coursera/reproducible research/project 1"
setwd("/Users/brad/Documents/development/repos/coursera/reproducible research/project 1/RepData_PeerAssessment1")

# Download the raw data file (zipped)
# Raw File location: https://d396qusza40orc.cloudfront.net/repdata%2Fdata%2Factivity.zip

rawFile <- "https://d396qusza40orc.cloudfront.net/repdata%2Fdata%2Factivity.zip"
currDir <- getwd()
rawFileFullPath <- paste(getwd(),"//raw data//repdata_data_activity.zip",sep="")

download.file(url = rawFile,
              destfile= rawFileFullPath,
              method="curl")


# Extract the zip file
# unzip the data file and rename it locally
unzip(zipfile = rawFileFullPath, exdir=".//raw data")
```


## What is mean total number of steps taken per day?



## What is the average daily activity pattern?


## Imputing missing values



## Are there differences in activity patterns between weekdays and weekends?
