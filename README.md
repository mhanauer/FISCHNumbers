---
title: "Test"
output: html_document
---

```{r setup, include=FALSE}
knitr::opts_chunk$set(echo = TRUE)
```
Library packages
```{r}
library(MASS)
library(caret)
library(pROC)
library(semTools)
library(lavaan)
library(mediation)
```
We have about five people a week and we need to get each person in for 6 sessions.  It takes about two weeks for everyone to get a session.  What is the total amount of weeks needed to get 100 people through 6 sessions.
```{r}
# It will take 10 weeks for each person to get through the intervention 2 weeks per each data collection not counting the first data session so just  
timeInTreatment = 2*5

# If we are enrolling 5 per week and we want to enroll 5 people it will take us 20 weeks.  Need to add Thanksgiving, finals week twice, spring break, and winter break (3 weeks)
totalWeeksToEnroll = (100/5)+7
totalWeeksToEnroll

# So if we take the last person enrolled at 27 weeks and add 10 it will take about 37 weeks
totalWeeksUntilEnd = totalWeeksToEnroll+timeInTreatment; totalWeeksUntilEnd
```






