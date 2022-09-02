# MechaCar_Statistical_Analysis
## Project Overview 

### Purpose - 
The purpose of this project is to perform a multiple linear regression analysis to identify which variables in the dataset predict the mpg of MechaCar prototypes. We also collect summary statistics on the pounds per square inch (PSI) of the suspension coils from the manufacturing lots, run t-tests to determine if the manufacturing lots are statistically different from the mean population, design a statistical study to compare vehicle performance of the MechaCar vehicles against vehicles from other manufacturers. For each statistical analysis, you’ll write a summary interpretation of the findings.

### Resources 
Data - MechaCar_mpg.csv
Suspension_Coil.csv

Software - R version 4.2.1 , Tidyvere, dplyr - package.

### Results 
### Deliverable 1 Linear Regression to Predict MPG.
A multiple linear regression was performed using all the six variables. Analyses may be drawn by answering the following questions.

1. Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?

![image](/Images/Deliverable%201.png)

From multiple linear regression model we see that Vehicle length, spoliler angle & ground clearance show positive correlation, while AWD shows a negative correlation with the dependent variable mpg.The p-values for vehicle length and ground clearence are lower than the significant value of 0.05 indicating that their contribution to the variance in the mpg value is not randomly generated.

2. Is the slope of the linear model considered to be zero? Why or why not?
    The linear model shows dependency on two known independent variables, the vehicle length and ground clearance, therefore the slope of the line is non-zero. A linear model with a slope zero suggests no dependency on the independent varibles, and that's not the case here.
    The p-values for vehicle length, and ground clearance allows us to reject the null hypothesis that the coefficient is zero (which is what we observe), and they influence mpg.

3. Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?
    The linear model has a R-squared value of around 71%. Therefore the model is explaining 71% of the observed variance. Three variables , vehicle weight, spoiler angle, and AWD do not add significant value to the linear regression model in explaining the variance. We know this because their p-values are higher than the accepted significant value of 0.05, and they also have very low correlation coefficients.
    However, vehicle length, and ground clearance ought to be given weightage while re-creating the regression model.
    Notice too that the p-value of the intercept is significant implying that there are other considerations which contribute towards the observed variance, which is not taken into account here. All of this gives the lower adjusted R-squared of 68%.   
    

### Deliverable 2 Summary Statistics on Suspension Coils
## Total Summary 

![image](/Images/Deliverable%202.png)

## Lot Summary 

![image](/Images/lot%20summary.png)

Lot1 and Lot2 PSI values are not statistically different from population mean. Their respective p-values are greater than the significance level. However, for Lot3 is 0.04 which is lesser than the significance level and it is infered that that Lot3 mean suspension coul PSI is statistically different from the population mean.


### Deliverable 3 - ### T-Tests on Suspension Coils

![image](/Images/Deliverable%203A.png)

### T-Test comparing PSI accross manufacturing lot 1 with the population mean of 1,500 pounds per square inch.
![image](/Images/Deliverable%203B.png)

### T-Test comparing PSI accross manufacturing lot 2 with the population mean of 1,500 pounds per square inch.
![image](/Images/Deliverable%203C.png)

### T-Test comparing PSI accross manufacturing lot 3 with the population mean of 1,500 pounds per square inch.
![image](/Images/Deliverable%203D.png)

According to each of the one-sample t-tests, Lot 1 and Lot 2 PSI values are not statistically different from the population mean. However the p-value of Lot 3 is 0.041 which is below the significance level, which means there is evidence that the Lot 3 mean suspension coil PSI is statistically different from the population mean.


### Deliverable 4: Design a Study Comparing the MechaCar to the Competition.
To do analysis on MechaCar against one of its competitions, we can consider following -
Horse Power or Cost or Fuel Efficiency or Safety.

Possible Hypothesis 
1. Null Hypothesis - There is no statistical difference between MechaCar horsepower and the horsepower of all other comparable vehicles. 
2. Alternative Hypotheseis - There is a statistical difference between MechaCar horsepower and the horsepower of all other comparable vehicles.

We collect sample data for different models of the MechaCar and the comparable vehicles and perform t-test on the randomly collected samples.
 
