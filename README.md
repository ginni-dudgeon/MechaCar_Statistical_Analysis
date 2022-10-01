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

