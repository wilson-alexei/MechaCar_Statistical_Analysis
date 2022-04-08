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
