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
Let's start with a normal (Gaussian) distribution, also known as a bell curve.

A normal distribution in a variate $$X$$ with mean $$\mu$$ and variance $$\sigma^2$$ is a statistic with probability density function

$$
P(x) = \frac{1}{\sigma\sqrt{2\pi}}\e^{\frac{-(x-\mu)^2}{2\sigma^2}}
$$
on the domain
$$
x\in(-\infty, \infty)
$$

Let's break it down. 