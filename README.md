# Assessing Campaign Performance Using Chi-Square Test For Independence

## Project Overview
In this project we apply Chi-Square Test For Independence (a Hypothesis Test) to assess the performance of two types of mailers that were sent out to promote a new service! 

## Business Problem
Earlier in the year, our client, a grocery retailer, ran a campaign to promote their new "Delivery Club" - an initiative that costs a customer \\$100 per year for membership, but offers free grocery deliveries rather than the normal cost of \\$10 per delivery.

For the campaign promoting the club, customers were put randomly into three groups - the first group received a low quality, low cost mailer, the second group received a high quality, high cost mailer, and the third group were a control group, receiving no mailer at all.

The client knows that customers who were contacted, signed up for the Delivery Club at a far higher rate than the control group, but now want to understand if there is a significant difference in signup rate between the cheap mailer and the expensive mailer.  This will allow them to make more informed decisions in the future, with the overall aim of optimising campaign ROI!

## Data Analysis

### Choose the Analytical Method
As this project focuses on comparing the sign-up *rates* of two mail types, i.e. to compare the frequency on two groups of categorical data, I will use hypothesis test - the Chi-Square Test For Independence. I chose this statistical test as opposed to *Z-Test For Proportions* because 
 * The Chi-Square Test can be represented using 2x2 tables of data - making it easier to explain to stakeholders
 * The Chi-Square Test can extend out to more than 2 groups - meaning the client can have one consistent approach to measuring signficance.

### Analytical Process
I'll take the following steps for this hypothesis test and analysis.

 * Set up the null and alternative hypotheses as well as the acceptance criteria.
 * Prepare the data to get the observed *frequency*.
 * Run the Chi-square test to obtain the chi-square statistics and the p-value.
 * Calculate the critical value using Python's Scipy package.

### Intepret the Results
Based upon our observed values, we get:

* Mailer 1 (Low-quality-low-cost): **32.8%** signup rate
* Mailer 2 (High-quality-high-cost): **37.8%** signup rate

However, the Chi-Square Test gives us the following statistics:

* Chi-Square Statistic: **1.94**
* p-value: **0.16**

The Critical Value for our specified Acceptance Criteria of 0.05 is **3.84**

Based upon these statistics, we retain the null hypothesis, and conclude that there is no relationship between mailer type and signup rate.

In other words - while we saw that the higher cost Mailer 2 had a higher signup rate (37.8%) than the lower cost Mailer 1 (32.8%) it appears that this difference is not significant, at least at our Acceptance Criteria of 0.05.

### Business Impact and Application

Without running this Hypothesis Test, the client may have concluded that they should always look to go with higher cost mailers - and from what we've seen in this test, that may not be a great decision.  It would result in them spending more, but not *necessarily* gaining any extra membership sign-up and revenue as a result.

Our results here also do not say that there *definitely isn't a difference between the two mailers* - we are only advising that we should not make any rigid conclusions *at this point*.  

Running more A/B Tests like this, gathering more data, and then re-running this test may provide us, and the client more insight!

***
See the full analysis in my [Jupyter Notebook](./Data_Insights_for_New_Movie_Studio.ipynb) or review this [presentation](./Data_Insights_for_New_Movie_Studio_presentation.pdf).

For additional info, contact Ruthy Yao at [zejia.yao@gmail.com](mailto:zejia.yao@gmail.com)
