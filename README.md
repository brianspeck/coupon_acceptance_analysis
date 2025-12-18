# coupon_acceptance_analysis
Exploratory data analysis of coupon acceptance behavior across different contexts and coupon types.



COUPON ACCEPTANCE ANALYSIS (PRACTICAL APPLICATION 1)

This project analyzes a coupon dataset to understand what factors influence whether a driver accepts a coupon (Y = 1) or does not accept (Y = 0). The work includes basic exploratory analysis, targeted comparisons for bar coupons, and an independent investigation across multiple coupon types.


REPOSITORY CONTENTS

* brianspeck_PA_1.ipynb: main analysis, plots, and written interpretation

* data/coupons.csv

* README.md: project overview and conclusions


DATA CLEANING / MISSING DATA

* I did not globally drop missing data.

* Missing values were removed only for the variables required in each specific analysis.

* Duplicate rows were not removed, because identical responses could represent either repeated submissions from the same driver or distinct drivers with similar characteristics.


EXPLORATORY VISUALIZATIONS

The notebook begins with simple visualizations to understand:

* Missing values by feature

* Overall coupon acceptance rate

* Coupon counts by type (and by acceptance)

* Temperature distribution


BAR COUPON QUESTIONS

For the bar coupon questions, I compare acceptance rates between specific "included groups" and "all others."

These analyses focus on relationships such as:

* Bar visit frequency ( ≤3 vs >3)

* Bar visits combined with age criteria

* Bar visits combined with passenger and occupation


INDEPENDENT INVESTIGATION

After the bar coupon investigations, I extend the workflow to additional coupons and contexts.


Investigation Part 1: Restaurant(<20)

Goal: Explore whether acceptance depends more on social context or time of day for drivers with no urgent destination.

Summary: Acceptance is highest during dinner hours regardless of social context. Outside dinner hours, acceptance drops for both social and non-social groups, suggesting time of day has a stronger influence than social context.


Investigation Part 2: Carry Out & Take Away

Goal: Explore how acceptance varies by passenger type and weather for drivers with no urgent destination.

Summary: Acceptance varies widely by weather and passenger type. Some passenger-weather combinations have small sample sizes, so conclusions should be interpreted cautiously. 


Investigation Part 3: Coffee House

Goal: Explore how acceptance varies by passenger type across time of day for drivers with no urgent destination.

Summary: Acceptance varies by time and passenger type, and some combinations have no observations.


OVERALL CONCLUSIONS

Coupon acceptance appears to depend strongly on context (time, weather, passenger, and prior behavior) rather than any single demographic factor. Bar coupon acceptance is most strongly associated with visitation frequency, while restaurant/carry out/coffee coupons show clearer relationships with situational context. 

