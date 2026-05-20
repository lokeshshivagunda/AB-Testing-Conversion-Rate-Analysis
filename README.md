# AB-Testing-Conversion-Rate-Analysis
A/B testing Project related to Landing page using python, statistics and hypothesis testing.

One of the most interesting analytics projects I worked on was an A/B testing analysis for a landing page redesign.
The goal was to determine whether the new page improved user conversion rates compared to the old version.
The dataset included user IDs, timestamps, page version (control vs treatment), and conversion status.
The control group saw the old landing page, while the treatment group saw the redesigned version.
Before analysis, I performed data cleaning and found around 3,800 duplicate users. Since A/B testing assumes independent observations, I removed duplicates using pandas to avoid biased results.
After cleaning, I created balanced sample groups from the control and treatment data, and I used a random seed function so the sampling stayed consistent every time the analysis was run.
I then framed the statistical hypotheses:

Null hypothesis: no difference in conversion rates

Alternative hypothesis: the new page improves conversions

Since conversion is binary data and the sample size was large, I used a Two-Proportion Z-test.
The control group conversion rate was about 11.44%, while the treatment group was around 12.18%, showing a small lift of 0.74%. However, the p-value was 0.252, 
which was greater than the 0.05 significance level.
So, we failed to reject the null hypothesis, meaning there wasn’t enough statistical evidence to conclude that the new landing page significantly improved conversions.
Based on this, I recommended not rolling out the redesign globally yet and suggested running a larger experiment or power analysis if stakeholders wanted to investigate smaller effects further.
This project helped me strengthen my skills in data cleaning, hypothesis testing, statistical interpretation, and communicating insights to stakeholders.”

