---
title: "Maximum Likelihood Estimation"
date: 2025-05-01
---


Maximum Likelihood Estimation (MLE) is a method used to estimate the parameters of a statistical model. 
The core idea is to find the parameter values that are most likely to have generated the observed data, based on the data’s distribution.

These estimated values can be used for further statistical inference, such as prediction, hypothesis testing, and confidence interval estimation.

# Explanation
Below is an explanation using the Bernoulli distribution as an example:

Assume we have a sequence of discrete random variables X, where each variable takes the value 1 with probability p and 0 with probability 1−p:

![image](https://github.com/user-attachments/assets/a166cbcc-f373-4fea-85f6-e3be43ae99d9)

First, we write the probability mass function (pmf) for the data (used for discrete distributions):

![image](https://github.com/user-attachments/assets/155df668-e8b9-4d9c-8b19-8c78077aac6c)

Since we want to estimate the most reasonable parameter based on the entire dataset, we consider the joint probability mass function (joint pmf) of the sample:

If the data are independent and identically distributed (i.i.d.), then the joint pmf is the product of the individual pmfs:

![image](https://github.com/user-attachments/assets/4aa6d001-45d3-441d-bb60-8e3feeb7fddf)

This joint pmf is the likelihood function L(p)L(p)L(p). To simplify multiplication and reduce numerical error, we usually convert it into its logarithmic form: the log-likelihood function.

![image](https://github.com/user-attachments/assets/42195856-61db-4aed-b644-9f3015ed04cd)

To find the maximum likelihood estimate p.hat​, we take the derivative of the log-likelihood function and set it equal to zero:

![image](https://github.com/user-attachments/assets/77af0f51-9ad5-4ac0-9446-7a4446836a9f)

# Conclusion
In the case of a Bernoulli distribution, the MLE is simply the sample mean X.bar— that is, the proportion of observed 1s. This result is both intuitive and statistically sound.

# References
[MLE wiki page](https://en.wikipedia.org/wiki/Maximum_likelihood_estimation?source=post_page-----b37b0453af0e---------------------------------------)
[pmf wiki page](https://en.wikipedia.org/wiki/Probability_mass_function?source=post_page-----b37b0453af0e---------------------------------------)
[Bernoulli distribution wiki page](https://en.wikipedia.org/wiki/Bernoulli_distribution?source=post_page-----b37b0453af0e---------------------------------------)
