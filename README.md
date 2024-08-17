# Experimental-design-of-Instagram-story-feature-on-Facebook

This project focuses on Statistical hypothesis in Data science by implementing different testing techniques.
The goal is to prove if including the stories feature from instagram to face book is beneficial in terms of user growth and financial growth.

A/B test
The primary objective of this A/B test is to evaluate whether the introduction of the Stories
feature on Facebook will significantly increase the Engagement rate metric among a
selected user base.

Hypothesis
We aim to investigate the following hypotheses:
Alternative Hypothesis (H1): Introducing the Stories feature on Facebook will increase the
Engagement rate metric by an average of 1% for the selected user base.
Null Hypothesis (H0): Introducing the Stories feature on Facebook will not increase the
Engagement rate metric for the selected user base.
By examining these hypotheses, we seek to provide insights into the potential impact of
integrating Stories into the Facebook platform, informing future product development
decisions and enhancing user engagement strategies.

Metrics
Key Metric
● User engagement. According to Meta’s annual report FORM 10-K, the key metric
we use to measure user engagement is the percentage of Daily Active Users on
Monthly Active Users (DAU/MAU)
● DAU - Number of Active Users in a given date
● MAU - Number of Active Users in the last 30 days from a given date

Guardrail metrics
The guardrail metrics considered for the experiment are:
1) the number of posts per user per day on Facebook
2) the latency rate of the homepage on Facebook
3) Instagram Daily Active Users
4) Number of users posting new stories on Instagram
5) Number of stories viewed by users on Instagram

Sample Size
I calculated the sample size based on the sample size formula. 
𝑛 = (𝑍𝛼+𝑍𝛽)2×𝑝0(1−𝑝0)/𝛿2.

In our condition:
𝑝0 = 0.75 (baseline proportion of user engagement in the US region)
𝑍𝛼 = 1.645 (Z score of a one-tailed test at a significant level of 0.05)
𝑍𝛽 = 0.84 (Z score of a power of 80%)
𝛿 = 0.01 (the expected effect size of a 1% increase in engagement rate)
Given all the parameters, the estimated sample size is around 11,579 (we have 10,000
samples in the data), with a 50% split between the control and treatment groups.

Results
T-test
The t-test results show that there was a significant difference of 1.16% between the
control and treatment group’s user engagement (p<0.001, CI = [1.15%, 1.16%]). It
indicates that introducing story features on Facebook can increase user engagement by
1.16% in selected user groups.

Robustness Check
Segmentation Test
We conducted t-tests in different user segments to check the robustness of the result.
We chose three different segments: age, gender, and device. All the results show that
there was a significant difference between the control and treatment group’s user
engagement, which validates the robustness of the result.
