# MechaCar_Statistical_Analysis

## Linear Regression to Predict MPG

Linear Regression

Data placed into Dataframe

<img width="560" alt="Regression Dataframe" src="https://user-images.githubusercontent.com/105091538/193431553-e4527e9f-360a-471b-95ed-72d9ea6ddf9b.png">

R was used to get the following coefficients.

<img width="634" alt="Coefficients" src="https://user-images.githubusercontent.com/105091538/193431278-5845e6d3-314a-45cb-a5b2-122a4d0c9c2d.png">

Summary of Linear Regression

<img width="831" alt="Summary of Linear Regression" src="https://user-images.githubusercontent.com/105091538/193431290-07b21049-79ae-4565-851f-ce834c2d5141.png">

1. Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?

Coefficients:
mpg: 0 < .05, statistically significant, non-random amount of variance
vehicle length: 0 < .05, statistically significant, non-random amount of variance
vehicle weight: .08 > .05 not statistically significant, random amount of variance
spoiler angle: .31 > .05 not statistically significant, random amount of variance
ground clearance: 0 > .05 statistically significant, non-random amount of variance
AWD: .19>=.05 not statistically significant, random amount of variance

This shows that the vehicle length and amount of ground clearance represent non-random amounts of variance.

2. Is the slope of the linear model considered to be zero? Why or why not?

The slopes of the variables are shown to be non-zero.

3. Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?

This linear model does appear to predict the mpg of the prototypes effectively due to the mpg being statistically significant.


## Summary Statistics on Suspension Coils

## Manufacturing Lot Summary

<img width="507" alt="lot_summary DF" src="https://user-images.githubusercontent.com/105091538/193431816-4ef2d6a9-b91d-4e4a-a5fc-b7d4cdcbff2e.png">

This dataframe shows the mean is 1498.78 and the population mean was 1500.

## Manufacturing Lot Number

<img width="335" alt="total_summary DF" src="https://user-images.githubusercontent.com/105091538/193431852-c65ec9b7-7364-441f-97f6-a8d13e361751.png">

The numbers in this dataframe are similar to the above. 

1. The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?

Lots 1 and 2 appear to meet this design specification. Lot 1 has a variance or around 1 and lot 2 has a variance of 7. However, lot 3 does not appear to meet this. The variance for lot 3 is 170. Collectively the lots may not meet the design specification. 


## T-Tests on Suspension Coils

## T-test for all lots

All Manufacturing Lots: p-value = .6028, alpha = .05
.60 > .05, not statistically significant. Normality is assumed. Mean is within the confidence level.

<img width="527" alt="T test for all lots" src="https://user-images.githubusercontent.com/105091538/193432077-56fbacab-b993-4c10-b8a5-06e6962eccde.png">

## T-test for Lot 1

Lot 1: p-value = 1, alpha = .05
1 > .05, not statistically significant. Normality is assumed. Mean is within the confidence level.

<img width="597" alt="T test for lot 1" src="https://user-images.githubusercontent.com/105091538/193432094-9c136d92-7e1f-4073-a0b4-5907b24e41a1.png">

## T-test for Lot 2

Lot 2: p-value = .6072, alpha = .05
.60 > .05, not statistically significant. Normality is assumed. Mean is within the confidence level.

<img width="614" alt="T test for Lot 2" src="https://user-images.githubusercontent.com/105091538/193432110-da64d571-3e9a-410d-94ba-96891dc9c615.png">

## T-test for Lot 3

Lot 3: p-value = .04168, alpha = .05
.04 < .05, statistically significant. Normality cannot be assumed. Mean is within the confidence level.

<img width="628" alt="T test for lot 3" src="https://user-images.githubusercontent.com/105091538/193432128-12782bba-7625-4b2b-a850-921b9a94662f.png">

Overall the null hypothesis cannot be rejecte due to lots 1 and 2 showing a similar distribution. 

## Study Design: MechaCar vs Competition

There are several metrics that should be considered when comparing MechaCar to competitos. Consumers researching cars would be most interested in include cost, car color, city fuel efficiency, highway fuel efficiency, horsepower, maintenance cost, and safety rating.

What metric or metrics are you going to test?
The most important metrics to test are safety ratings and highway fuel efficiency.

What is the null hypothesis or alternative hypothesis?
The null hypothesis would be zero. The alternative hypothesis would be a number other than zero.

What statistical test would you use to test the hypothesis? And why?
A multiple linear regression using statittics would be the best way to test the hypothesis.

What data is needed to run the statistical test?
The data needed to run a statistical test is a sample of cars from both MechaCar and a competitor. Information included woult be the safety ratings and highway fuel efficiency.

