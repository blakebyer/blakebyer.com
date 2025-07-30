---
title: Introduction to Statistics for Biologists
date: 2025-07-30
layout: single
categories: [blog]
excerpt: "Let's add another tool to our toolbelt"
math: true
---

## Why learn statistics? ##
Statistics are the backbone of impactful, reproducible research. Properly done, statistics provide us with basis for cause and effect (known as causal inference). I wanted to write a few supplementary articles for myself and others to understand the basics of probability, statistics, and linear algebra to boost their research.

## Introduction ##
The simple <b>arithmetic mean</b> $$\bar{x}$$ of a set is 
$$
M = \frac{1}{n}\sum_{i=1}^{n}x_i
$$

The <b>geometric mean</b> is the $$n$$th root of the product of the elements in a set.
$$
G = (\prod_{i=1}^{n}x_i)^{\frac{1}{n}} = \sqrt[n]{x_1, x_2, ..., x_n}
$$

Finally, the <b>harmonic mean</b> is the number of values $$n$$ over the sum of the values' reciprocals.
$$
H = \frac{n}{\frac{1}{x_1} + \frac{1}{x_2} + ... + \frac{1}{x_n}} = \frac{n}{\sum_{i=1}^{n}\frac{1}{x_i}}
$$

<b>Standard deviation</b> $$\sigma$$, also abbreviated as SD, is a measure of the amount of variation of the values of a variable about its mean.
$$
\sigma = \sqrt{\frac{1}{N}\sum_{i=1}^{N}(x_i - \bar{x})^2}
$$
if values $$i$$ through $$N$$ represent the entire population. If values are selected at random, a correction is applied (Bessel's correction), such that
$$
\sigma = \sqrt{\frac{1}{N - 1}\sum_{i=1}^{N}(x_i - \bar{x})^2}
$$

<b>Variance</b> is quantifies the spread of data around a sample mean and is just $$\sigma^2$$. A higher variance means greater spread.

## Sampling Methods ##
In a <b>simple random sample</b>, every member of the population has an equal chance of being selected $$\frac{1}{N}$$.

## Normal Distribution ##
Let's start with a normal (Gaussian) distribution, also known as a bell curve.

A <b>normal distribution</b> in a variate $$X$$ with mean $$\mu$$ and variance $$\sigma^2$$ is a statistic with probability density function

$$
P(x) = \frac{1}{\sigma\sqrt{2\pi}}e^{\frac{-(x-\mu)^2}{2\sigma^2}}
$$
on the domain
$$
x\in(-\infty, \infty)
$$

Let's break it down, assuming the mean $$\mu = 0$$ and the variance $$\sigma^2 = 1$$. $$\sigma$$ alone is the standard deviation. Therefore, when $$x = 0$$, $$P(x)$$ has an absolute maximum at
$$
\frac{1}{1\sqrt{2\pi}}e^{\frac{-(0-0)^2}{2(1)^2}} = \frac{1}{1\sqrt{2\pi}}
$$.

A <b>Z-score</b> is quantified as the number of standard deviations a value falls away from the sample mean. To calculate a Z-score
$$
z = \frac{x - \mu}{\sigma}
$$
where $$\mu$$ is the mean of the population, and $$\sigma$$ is the standard deviation of the population.

A Z-score can help us describe the normal distribution in quantiles. The empirical rule (68-95-99.7 rule) of the normal distribution states that approximately 68% of the data falls within 1 SD of the mean, 95% within 2 SD, and 99.7% within 3 SD of the mean.
