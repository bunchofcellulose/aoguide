---
title: Distributions
weight: 4
---

## Gaussian Distribution

A normal or gaussian distribution is a continuous probability distribution defined by the probability density function (PDF)

$$\tag{9.1.1} f(x) = \frac{1}{\sqrt{2 \pi \sigma^2}} e^{-\frac{(x - \mu)^2}{2 \sigma^2}}$$

where $\mu$ is the mean and $\sigma$ is the standard deviation. The variance of the distribution is given by $\sigma^2$.

## Poisson Distribution

The Poisson distribution is a discrete probability distribution that expresses the probability of a given number of events occurring in a fixed interval of time or space, given that these events occur with a known constant mean rate and independently of the time since the last event. The probability mass function (PMF) is given by

$$\tag{9.1.2} P(k, \lambda) = \frac{\lambda^k e^{-\lambda}}{k!}$$

where $k$ is the number of events, $\lambda$ is the average number of events in the interval, and $e$ is Euler's number.
The mean and variance of the Poisson distribution are both equal to $\lambda$.

## Binomial Distribution

The binomial distribution is a discrete probability distribution that gives the number of successes in a fixed number of independent Bernoulli trials, each with the same probability of success.
A Bernoulli trial is a random experiment with exactly two possible outcomes: "success" and "failure". The binomial distribution is used to model the number of successes in a sequence of $n$ independent experiments, each with a success probability of $p$.
The probability mass function (PMF) is given by

$$\tag{9.1.3} P(k, n, p) = \binom{n}{k} p^k (1 - p)^{n - k}$$

where $n$ is the number of trials, $k$ is the number of successes, and $p$ is the probability of success on each trial. The mean and variance of the binomial distribution are given by $np$ and $np(1 - p)$ respectively.
