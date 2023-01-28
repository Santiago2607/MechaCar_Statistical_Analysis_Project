# MechaCar_Statistical_Analysis_Project

## Overview

For this project, our main duty is to help Jeremy, leader of the data analytics team at AutosRUs, to analyze and figure out why the newest prototype, the MechaCar, is suffering from production troubles. 

In order to perform this analysis, we are going to use 'R', one of the best data analytics tools, to create linear regression functions, summary statistics on suspension coils, T-Test on suspension coils, and design some comparisons between the MechaCar and the Competition, to be able to support the company and help it with the production of its product. 

## Results

### Linear Regression to Predict MPG

For the first part of the project, we were able to create a linear regression function to analyze the mpg of the company and get data such as the coefficients, residuals, intercepts, r-value, and p-value, as shown below.

![image](https://user-images.githubusercontent.com/113261292/215286024-29c73020-927b-42ff-bded-5b66ac84b810.png)

Using this data we can say that:

1. The variables/coefficients that provided a non-random amount of variance to the mpg values in the dataset are the vehicle_length and ground_clearance, due to their low p-value that represents a high level of significance.

2. The slope of the linear model is not considered to be zero since the independent variables have a great effect on the dependent variables in the function. 

3. This linear model can be considered to predict mpg of MechaCar prototypes effectively because of the r-value, 0.7149, which means that there is a 71% of succesfully predictions that can be made.   

### Summary Statistics on Suspension Coils

For the second part of the project, we were able to create two dataframes with valuable information that can help us determine the mean, median, variance, and standard deviation of the manufacturing lot and suspension coil from the PSI column.

1. Total Suspension Coil dataframe

![image](https://user-images.githubusercontent.com/113261292/215288237-cb58190e-5bf5-499d-809f-49812ab5a4c0.png)

2. Manufacturing Lot & Suspension Coil dataframe

![image](https://user-images.githubusercontent.com/113261292/215288220-6f1243fd-2461-49e1-ba04-5ab3b49054ac.png)

According to these two dataframes, we can say that:

+ The total current manufacturing data meet the design specification for all manufacturing lots by having a total of 62.29 PSI, much less than the maximum 100 PSI required. However, if we break this down by lots, Lot1 and Lot2 with a PSI of 0.97 and 7.46, respectively, are within the maximum range established, but Lot3, with a 170 PSI, has surpassed the limit by almost double the required amount and may be one of the reasons that are causing the production troubles.

### T-Tests on Suspension Coils

For the third part of this project, we were able to create different t.tests that determined if all manufacturing lots and each lot individually are statistically different from the population mean of 1,500 pounds per square inch.

+ T.test of all manufacturing lots

![image](https://user-images.githubusercontent.com/113261292/215290045-f91adbc7-2fd9-4fc0-908f-1d725cd0a574.png)

+ T.test Lot1

![image](https://user-images.githubusercontent.com/113261292/215290065-d26fb7d3-951b-4f8b-a571-4d890e7340ee.png)

+ T.test Lot2

![image](https://user-images.githubusercontent.com/113261292/215290141-27be2d45-0494-4fc2-83c7-59515ca4f6e3.png)

+ T.test Lot3

![image](https://user-images.githubusercontent.com/113261292/215290160-363724d8-ec1c-40cb-8458-80ee2b5a16ac.png)

Based on the previous information, we can say that:

1. By calculating the total population mean and p-value for all the manufacturing lots together we can say that there is not enough evidence to support rejecting the null hypothesis, which means the mean of all the manufacturing lots is potentially similar to the population mean of 1500.

2. With both, a total population mean of 1500 and a p-value > 0.05, Lot1 and Lot2's null hypothesis cannot be rejected meaning they are statistically similar from the population mean of 1,500 pounds per square inch. However, Lot3 with a p-value < 0.05 tells us we can reject the null hypothesis of this, being the only lot with a different population mean.

## Summary 

## Study Design: MechaCar vs Competition

To finish this project, we decided to do a last statistical study that can quantify how the MechaCar performs against the competition.

1. Some metrics that we can take into consideration for future advantages can be the city, price, highway fuel efficiencies, and engine of the cars.

2. A null hypothesis about this can be that all the cars of the same brand have the same price. A alternative hypothesis, on the other hand, can be that all cars of the same brand have not the same engine or horsepower.

3. The statistical test we would use to test the hypothesis is ANOVA since it gives us more confident at the moment of analyzing and differntiate several components of the tests.

4. The data needed to run the statistical test would be the different kind of cars the company manufacturers, the different prices they have, their engine, where are they going to be commercialize, and how efficient is their fuel reserve.  
