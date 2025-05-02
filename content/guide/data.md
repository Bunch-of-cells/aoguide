---
title: Data Analysis
weight: 9
---

## Types of Distributions

### Gaussian Distribution

A normal or gaussian distribution is a continuous probability distribution defined by the probability density function (PDF)

$$\tag{9.1.1} f(x) = \frac{1}{\sqrt{2 \pi \sigma^2}} e^{-\frac{(x - \mu)^2}{2 \sigma^2}}$$

where $\mu$ is the mean and $\sigma$ is the standard deviation. The variance of the distribution is given by $\sigma^2$.

### Poisson Distribution

The Poisson distribution is a discrete probability distribution that expresses the probability of a given number of events occurring in a fixed interval of time or space, given that these events occur with a known constant mean rate and independently of the time since the last event. The probability mass function (PMF) is given by

$$\tag{9.1.2} P(k, \lambda) = \frac{\lambda^k e^{-\lambda}}{k!}$$

where $k$ is the number of events, $\lambda$ is the average number of events in the interval, and $e$ is Euler's number.
The mean and variance of the Poisson distribution are both equal to $\lambda$.

### Binomial Distribution

The binomial distribution is a discrete probability distribution that gives the number of successes in a fixed number of independent Bernoulli trials, each with the same probability of success.
A Bernoulli trial is a random experiment with exactly two possible outcomes: "success" and "failure". The binomial distribution is used to model the number of successes in a sequence of $n$ independent experiments, each with a success probability of $p$.
The probability mass function (PMF) is given by

$$\tag{9.1.3} P(k, n, p) = \binom{n}{k} p^k (1 - p)^{n - k}$$

where $n$ is the number of trials, $k$ is the number of successes, and $p$ is the probability of success on each trial. The mean and variance of the binomial distribution are given by $np$ and $np(1 - p)$ respectively.

## Statistical Analysis

The mean or expected value of a random variable $X$ taken from a distribution $P(X)$ is given by

$$\tag{9.1.4} \mu = E[X] = \int_{-\infty}^{\infty} x P(x) dx$$

The mean is the average value of the random variable.

The expected value of a function $f(X)$ of a random variable $X$ is given by

$$\tag{9.1.5} E[f(X)] = \int_{-\infty}^{\infty} f(x) P(x) dx$$

The median is the value that separates the higher half from the lower half of the data set. It is the middle value when the data set is ordered from least to greatest. The median is less sensitive to outliers than the mean.

The mode is the value that appears most frequently in a data set. A data set may have one mode, more than one mode, or no mode at all.

The variance of a random variable $X$, represented by $\text{Var}(X)$ or $\sigma^2$ is the expected value of the squared deviation from the mean, and is given by

$$\tag{9.1.6} \sigma^2 = E[(X - \mu)^2] = E[X^2] - E[X]^2$$

The standard deviation $\sigma$ is the square root of the variance, and is a measure of the amount of variation or dispersion in a set of values.

If $a$ is a scalar constant, then

- $\text{Var}(X + a) = \text{Var}(X)$
- $\text{Var}(aX) = a^2 \, \text{Var}(X)$
- $\text{Var}(X + Y) = \text{Var}(X) + \text{Var}(Y) + 2 \, \text{Cov}(X, Y)$

$\text{Cov}(X, Y)$ or $\sigma_{XY}$ is the covariance of $X$ and $Y$, which is a measure of how much two random variables change together, or the joint variability of the variables. If $X$ and $Y$ are independent, then $\text{Cov}(X, Y) = 0$.

$$\tag{9.1.7} \sigma_{XY} = E[(X - \mu_X) \, (Y - \mu_Y)] = E[XY] - E[X]\, E[Y] $$

The weighted mean is similar to normal mean, but each element $x_i$ is weighted with some weight $w_i$. The weighted mean is given by

$$\tag{9.1.8} \bar{x} = \frac{\sum w_i x_i}{\sum w_i}$$

If $x_i$ is taken from a distribution of variance $\sigma_i^2$, the corresponding weight is $w_i = 1/ \sigma_i^2$. This gives the standard error of the weighted mean as

$$\tag{9.1.9} \sigma_{\bar{x}}^2 = \frac{1}{\sum w_i} = \frac{1}{\sum \frac{1}{\sigma_i^2}}$$

We also get that

$$\tag{9.1.10} \bar{x} = \sigma_{\bar{x}}^2 \, \sum \frac{x_i}{\sigma_i^2} $$

If all the weights are equal, then the weighted mean is same as the ordinary mean

$$\tag{9.1.11} \bar{x} = \frac{1}{n} \sum x_i$$

Hence we get that the standard error of the mean is given by

$$\tag{9.1.12} \sigma_{\bar{x}} = \frac{1}{\sqrt{n}} \, \sigma$$

where $n$ is the number of samples.

## Propagation of Uncertainty

Suppose the random uncorrelated variables $A$ and $B$ have standard deviations $\sigma_A$ and $\sigma_B$ respectively. The standard deviation of a few common functions are given below

Function | Standard Deviation / Variance |
--------|----------------|
$f = aA$ | $\sigma_f = $ \|$a$\|$ \, \sigma_A$ |
$f = A + B$ | $\sigma_f^2 = \sigma_A^2 + \sigma_B^2$ |
$f = A \cdot B$ | $\sigma_f^2 \approx f^2 \left[ \left(\frac{\sigma_A}{A}\right)^2 + \left(\frac{\sigma_B}{B}\right)^2 \right] = (B \sigma_A)^2 + (A \sigma_B)^2$ |
$f = \frac{1}{A}$ | $\sigma_f \approx \frac{\sigma_A}{A^2} $ |
$f = A^a$ | $\sigma_f \approx $ \|$f a \, \frac{1}{A}$\| $\sigma_A = $ \|$a A^{a-1}$\| $\sigma_A$ |
$f = \ln A$ | $\sigma_f \approx $ \|$\frac{1}{A}$\| $\sigma_A$ |
$f = e^A$ | $\sigma_f \approx e^A \, \sigma_A$ |

For any non linear combinations of independend variables $x_i$, we get that for any function $f(x_1, x_2, x_3, \ldots)$,

$$\tag{9.1.13} \sigma_f^2 \approx \sum_i \left( \frac{\partial f}{\partial x_i} \sigma_{x_i} \right)^2$$

when the relative uncertainties $\sigma_{x_i} / x_i$ are small. If the relative uncertainties are not small, one has to find the minimum, maximum and mean values of the function separately. Unicertainity due to significant figures should also be taken into account. For $f = A \cdot B$, the uncertainity has a maximum value of

$$\tag{9.1.14} |\frac{\sigma_f}{f}| \le |\frac{\sigma_A}{A}| + |\frac{\sigma_B}{B}|$$

when accounted for covariance between $A$ and $B$.

## Linear Regression

A linear regression is a model that estimates the linear relationship between a dependent variable $y$ and one or more independent variables $x_i$.

Consider the linear model

$$\tag{9.1.15} y = \alpha + \beta x$$

The relation may not hold exactly; the deviations are called errors.

$$\tag{9.1.16} y_i = \alpha + \beta x_i + \epsilon_i$$

where $\epsilon_i$ is the error term. The errors are assumed to be independent and identically distributed (i.i.d.) with mean 0 and variance $\sigma^2$. The least squares method is used to estimate the parameters $\alpha$ and $\beta$ by minimizing the sum of squared errors. We define the following quantities

$$
\begin{aligned}
SS_{xx} &= {\small\sum} (x_i - \bar{x})^2 &=& \: {\small\sum} x_i^2 - \frac{1}{n} ({\small\sum} x_i)^2 \\
SS_{yy} &= {\small\sum} (y_i - \bar{y})^2 &=& \: {\small\sum} y_i^2 - \frac{1}{n} ({\small\sum} y_i)^2 \\
SS_{xy} &= {\small\sum} (x_i - \bar{x})(y_i - \bar{y}) &=& \: {\small\sum} x_i y_i - \frac{1}{n} ({\small\sum} x_i)({\small\sum} y_i) \\
\end{aligned}
$$

The least squares estimates of the parameters $\hat{\alpha}$ and $\hat{\beta}$ are given by

$$\tag{9.1.17} \hat{\alpha} = \bar{y} - \hat{\beta} \bar{x}$$
$$\tag{9.1.18} \hat{\beta} = \frac{SS_{xy}}{SS_{xx}}$$

We have that ${\small\sum} \epsilon_i = {\small\sum} x_i \epsilon_i = 0$. The linear relationship is

$$\tag{9.1.19} \hat{y} = \hat{\alpha} + \hat{\beta} x$$

The standard deviations of the estimates $\hat{\alpha}$ and $\hat{\beta}$ are given by

$$\tag{9.1.20} \sigma_{\hat{\alpha}}^2 = \sigma_{\hat{\beta}}^2 \, {\small\sum} x_i^2$$
$$\tag{9.1.21} \sigma_{\hat{\beta}}^2 = \frac{SS_{xx} SS_{yy} - SS_{xy}^2}{(n - 2) SS_{xx}^2}$$
