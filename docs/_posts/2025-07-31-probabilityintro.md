---
title: Introduction to Probability
date: 2025-07-31
layout: single
categories: [blog]
excerpt: "Basics of probability"
math: true
---
## The Birthday Paradox ##
Consider the question, how many people must be a room such that the probability of at least two will share a birthday exceeds 50%?

You might guess about 182 because it's about half the days in a year, or 100 because it's a nice round number. However, the answer might surprise you. 

The correct answer is just 23 people. How can this be true?! The answer lies in probability theory. Let the event A be that of a group of k people not having any repeated birthdays, and let B be that of a group of k people having at least two who share a birthday, i.e. $$P(B) = 1 - P(A)$$.

<figure>
  <img src="/assets/images/Birthday_Paradox.png" alt="Birthday paradox">
  <figcaption><em> The probability function of the birthday problem P(B) for n people. Illustration by Rajkiran g, CC BY-SA 3.0 via Wikimedia Commons.
  </em></figcaption>
</figure>

To calculate the number of k persons to exceed 50% one technique we might use is to decrement the number of possible shared birthdays for $$n+1$$ people. For person 1 there is 100% chance they don't share their birthday with another person, when adding person 2, there is a $$\frac{364}{365}$$ chance they don't share their birthday with person 1, and this continues as a conditional probability until you reach >50%. 

$$P(A)= \frac{365}{365} \times \frac{364}{365} \times \cdots \times \frac{343}{365} \approx 0.493$$

$$\therefore P(B) \approx 1 - 0.493 = 0.507$$

A more concise way of representing this is the probability function $$\bar{p} = \frac{365!}{365^n(365-n)!}$$. An approximation to try (that doesn't require numerical methods) is $$n\geq \frac{1}{2} + \sqrt{\frac{1}{4} + 2\times\ln{2}\times 365}$$.

A quick refresher on combinations and permutations. The number of combinations (order doesn't matter) of n choose r is $$C(n, r)= \frac{n!}{r!(n-r)!}$$ where $$!$$ is the factorial operator (e.g. $$4! = 4\times 3\times 2\times 1 = 24$$). Similarly, the number of permutations (order does matter) is $$P(n, r) = \frac{n!}{(n-r)!}$$. For both of these formulas, $$n$$ is the number of total objects, and $$r$$ is the number of objects chosen at once. 

## Conditional Probability ##
Conditional probability is the probablity of one thing happening given that another event has already occurred. 

## Joint Probability ##
Joint probability is the probability of two or more events occurring simultaneously.