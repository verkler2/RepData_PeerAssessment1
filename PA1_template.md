Question 1: Loading and preprocessing the data
The data must be in the user's current working directory for the code to run correctly. The unzip function extracts the data from the zip file, before it is read into R. The object classes contained within each of the variables are defined, so as to speed up the reading process.

unzip("activity.zip")
initialData <- read.csv("activity.csv", colClasses=c("numeric", "Date", "numeric"))
An initial look at the data confirms its dimensions and contents.

head(initialData)
##   steps       date interval
## 1    NA 2012-10-01        0
## 2    NA 2012-10-01        5
## 3    NA 2012-10-01       10
## 4    NA 2012-10-01       15
## 5    NA 2012-10-01       20
## 6    NA 2012-10-01       25
