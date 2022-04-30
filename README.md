# MechaCar_Statistical_Analysis
to review the production data for insights that may help the manufacturing team

## Linear Regression to Predict MPG
> Deliverable 1
**Result**
<img width="757" alt="Screen Shot 2022-04-08 at 16 18 35" src="https://user-images.githubusercontent.com/95068439/162524298-91e0e066-59bb-4a61-9942-698d1bf476e7.png">

<img width="776" alt="Screen Shot 2022-04-08 at 16 18 58" src="https://user-images.githubusercontent.com/95068439/162524421-9ff93bdd-e6d8-49a6-a20e-340a0faaf7bd.png">

Slope of the Linear Model: 
mpg = (6.267)vehicle_length + (0.0012)vehicle_weight + (0.0688)spoiler_angle + (3.546)ground_clearance + (-3.411)AWD + (-104.0)

**Statistics Summary:** 
1. The *vehicle_length* and *ground_clearance* are statistically likely to provide non-random amounts of variance to the model. They a significant impact on miles per gallon on the MechaCar prototype. On the other hand, *vehicle weight, spoiler_angle, and AWD(All Wheel Drive)* have p-values that inidicate a random amount of variance with the datase. 
2. The p-value for this model analysis is 5.35e-11 which is much smaller than the assumed significance level of .05%. This indicates that there is sufficient evidence to **reject the null hypothesis**, which further indicates that the slope of this linear model is not zero. 
3. This linear model produce an r-squared value of 0.7149, which indicates that roughly about 71.49% of all mpg predictions will be determied by this model. Statistically, this regression model does pedict the mpg of MechaCar prototypes effectively. 

## Summary Statistics on Suspension Coils
> Deliverable 2
**Result**
* Total Summary

<img width="1440" alt="Total_Summary" src="https://user-images.githubusercontent.com/95068439/162530216-b13ce5de-74b0-4d78-9611-4e006444114c.png">

* Lot Summary

<img width="1440" alt="Lot_Summary" src="https://user-images.githubusercontent.com/95068439/162530256-fb0ebf0a-1da5-4b88-809c-70648d2cfca5.png">

**Statistics Summary:**
1. When looking at the entire population at the `total summary` of the production lot, the variance of the coils is 62.29 PSI which is well within the 100 PSI variance requirement
2. From the `lot summary`, we can see that Lot 1 and Lot 2 are well within the 100 PSI variance requirement with their variance being approximately 0.98 and 7.47. Meanwhile, Lot 3 indicates a much larger variance in performance and consisteny with a variance of approximately 170.29 PSI. This means that Lot 3 Variance is the one that causes the variance at the full lot seemed disproportionate. 

## T-Tests on Suspension Coils
> Deliverable 3
**Result**

<img width="764" alt="t-test_main" src="https://user-images.githubusercontent.com/95068439/162546919-78bdeabe-a728-4af7-b74b-df5b9ef9f0b3.png">

* As we can see, the Sample Mean is 1498.78. With a p-value of approximately 0.06, it is higher than the level of significance which is 0.05 so that means that there is not enough evidence to reject the null hypothesis. 

<img width="426" alt="t-test_Lot1" src="https://user-images.githubusercontent.com/95068439/162547125-29232770-2c1c-4f99-ac0f-9d795497e992.png">

* In the sample of Lot 1, the sample mean is 1500 similar to the one above this. By having a p-value of 1, we fail to reject the null hypothesis as there is no statistical difference between the observed sample mean and the presumed population mean

<img width="410" alt="t-test_Lot2" src="https://user-images.githubusercontent.com/95068439/162547963-fb70e65e-d4ea-495b-b179-e0e8bb4ca7eb.png">

* In the sample of Lot 2, the Sample Mean is 1500.2. By having a p-value of approximately 0.61, then we fail to reject the null hypothesis as the sample mean is also similar to the population mean. 

<img width="404" alt="t-test_Lot3" src="https://user-images.githubusercontent.com/95068439/162548053-5e60ac39-3d4f-4856-a0d7-effe5b764df3.png">

* In the sample of Lot 3, the sample mean is 1496.14. By having a p-value of approximately 0.04, it is lower than the level of significance of 0.05 which means that we can reject the null hypothesis. This indicates that something odd is in Lot 3 therefore we need to inspect the production cycle of Lot 3 for any system failure and the suspension coils from this lot need to be inspected to remove those not meeting quality criteria. 

## Study Design: MechaCar vs Competition

The statistical study would involve collecting data on MechaCar and its comparable models across several different manufacturers over the last 3 years.
> What are the competitions' comparable models,

> Which cars will MechaCar be competing with head-to-head? which cars will be included in the study?

> Which factors will look at the study to determine the relevant to selling price?

**Metrics**
Collecting data for comparable models across all major manufacturers for past 3 years for the following metrics:

* Safety Feature Rating: Independent Variable
* Current Price (Selling): Dependent Variable
* Drive Package : Independent Variable
* Engine (Electric, Hybrid, Gasoline / Conventional): Independent Variable
* Resale Value: Independent Variable
* Average Annual Cost of ownership (Maintenance): Independent Variable
* MPG (Gasoline Efficiency): Independent Variable

**Hypothesis: Null and Alternative**
After determining which factors are key for the MechaCar's genre:
* Null Hypothesis (H0): MechaCar is priced correctly based on its performance of key factors for its genre.
* Alternative Hypothesis (HA): MechaCar is NOT priced correctly based on performance of key factors for its genre.


**Statistical Tests**

A multiple linear regression would be used to determine the factors that have the highest correlation/predictability with the list selling price (dependent variable); or which combination has the greatest impact on price

> LinkedIn: https://www.linkedin.com/in/wilson-alexei/

> Email: wils.alexei@gmail.com
