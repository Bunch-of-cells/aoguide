---
title: Data Analysis
weight: 9
---

## Drawing Graphs

Drawing graphs is one of the most important aspects of data analysis. Questions in astronomy olympiads generally only ask to draw scatter plot graphs, with just a few exceptions. A good graph should be easy to read and interpret, and should clearly convey the information being presented. The key points to remember when drawing graphs are

- Use a sharp pencil to draw graphs. Do not use pen on the graph paper.
- Mark and label the axes clearly with the units of measurement.
- Each tick on the axes need not be labeled. However, it should be easily deducible what value that tick represents.
- Use a suitable scale for the axes. The scale should be chosen so that the data is clearly visible and easy to interpret. State the scale used at the top of the graph.
- The origin of your graph does not have to be at (0, 0). It can be at any point on the graph, as long as it is clearly marked and labeled.
- All the given data points should be marked inside the green port
ion of the graph paper, so choose the scale accordingly. The data points should be marked on the green grid lines, and not inside the white boxes. Mark the data points on a graph by placing a small dot at the coordinates of the point and then drawing a small circle around the point to make it easily visible.
- The graph should cover at least 80% of the area of the graph paper.
- Every graph should have a title that clearly states which variables appear on the plot. Also, write your name and the date on the plot as well for convenient reference.
- The marked data points should be clearly visible and distinguishable from the background. If multiple data sets are plotted on the same graph, use different symbols for each. Legend should be provided for each symbol.
- If possible, turn the relation to be plotted into a linear form. For example, if the graph of $y$ vs $x$ follows the relation $y = bx^m$, plot $log(y)$ vs $log(x)$ or $y$ vs $x^m$ instead of $y$ vs $x$.
- The data points should be connected with a simple smooth curve or line. If a linear fit is used, write the equation of the line on the graph. The curve/line will not necessarily pass through all the points, but should pass as close as possible to each point, with about half the points on each side of the curve/line; this curve is intended to guide the eye along the data points and to indicate the trend of the data. Do not connect the data points by straight-line segments in a dot-to-dot fashion. The curve now indicates the average trend of the data, and any predicted values should be read from this curve rather than reverting back to the original data points.

### Choosing an appropriate scale

The scale of a graph is the ratio of the distance on the graph to the actual value. For example, if 1 cm on the graph represents 10 m/s of the actual value, then the scale is 1 cm = 10 m/s.

When choosing a scale for your graph, consider the range of your data and the level of detail you want to convey. Ideally, the scale should be of the form 1 cm = $2^m \cdot 5^n$ (units), which makes it very easy to read the coordinates of the data points. Other choices (e.g. 1 cm = 3 units) make both plotting and reading very hard.

Scales should be made no finer than the smallest increment on the measuring instrument from which data were obtained. For example, data from a meter stick (which has 1 mm graduations) should be plotted on a scale no finer than 1 cm = 1 mm. A scale finer than this would provide no additional plotting accuracy, since the data from the meter stick are only accurate to about 0.5 mm. Frequently the scale must be considerably coarser than this limit, in order to fit the entire plot onto a single sheet of graph paper.

### Drawing a linear fit

Place a transparent ruler or drafting triangle on your graph and adjust its position so that the edge is as close as possible to all the data points. The best adjustment will bring about one-half of the data points beneath the ruler, evenly distributed along the line. Draw a line along the ruler edge that extends to the nearest coordinate axis at one end and somewhat beyond the last data point at the other end. The degree to which the data are consistent with the equation is shown by how close the data points are to the fitted line. The construction of this straight line performs a smoothing of the raw experimental data, and thus may be a more reliable indication of the outcome of the experiment than any one pair of data points. Measurements taken from the graph should therefore be made on the fitted line and not on the data points themselves. Do not 'force' the fitted line to pass through some point (like the origin) of the graph, even if the original function passes through that point.

The slope of a straight line is computed by dividing the 'rise' by the 'run' of the line, as shown. For the 'run', choose two convenient scale locations along the horizontal axis near the ends of the line, and draw light vertical lines to intersect the plotted line. Read off the positions of these intersections along the vertical axis and subtract to obtain the 'rise'. Always report the calculated slope on the graph itself. You may find it helpful to label 'rise' and 'run' and intersection points as shown in the example, at least until your graphing technique is well developed. When you are asked to determine the intercept with the y-axis, label the intercept where the plotted line intersects the vertical axis (assuming that the vertical axis is located at the '0' position along the horizontal scale).

The uncertainty in the slope and intercept can be estimated by drawing two more straight lines with the maximum and minimum slope that still allows the lines to pass through most of the data points. The corresponding range of slopes and intercept values can then be used as a reasonable estimate of the uncertainty in these values.

## Significant Figures

Significant figures, are digits that carry both reliability and necessity in conveying a particular quantity.

To avoid conveying a misleading level of precision, numbers are often rounded. For instance, it would create false precision to present a measurement as 12.34525 kg when the measuring instrument only provides accuracy to the nearest gram (0.001 kg). In this case, the significant figures are the first five digits (1, 2, 3, 4, and 5) from the leftmost digit, and the number should be rounded to these significant figures, resulting in 12.345 kg as the accurate value.

### Rules to identify significant figures in a number

- Non-zero digits within the given measurement or reporting resolution are significant.
- Zeros between two significant non-zero digits are significant (significant trapped zeros).
- Zeros to the left of the first non-zero digit (leading zeros) are not significant.
- Zeros to the right of the last non-zero digit (trailing zeros) in a number with the decimal point are significant if they are within the measurement or reporting resolution.
- Trailing zeros in an integer may or may not be significant, depending on the measurement or reporting resolution.
- An exact number has an infinite number of significant figures. (If the number of apples in a bag is 4 (exact number), then this number is 4.0000... (with infinite trailing zeros to the right of the decimal point). As a result, 4 does not impact the number of significant figures or digits in the result of calculations with it.)
- A mathematical or physical constant has significant figures to its known digits.

### Rounding to significant figures

To round a number to n significant figures:

- If the n + 1 digit is greater than 5 or is 5 followed by other non-zero digits, add 1 to the n digit. For example, if we want to round 1.2459 to 3 significant figures, then this step results in 1.25.
- If the n + 1 digit is 5 not followed by other digits or followed by only zeros, then rounding requires a tie-breaking rule. For example, to round 1.25 to 2 significant figures, i. Round half away from zero rounds up to 1.3; or ii. Round half to even, which rounds to the nearest even number. With this method, 1.25 is rounded down to 1.2. If this method applies to 1.35, then it is rounded up to 1.4. This is the method preferred by many scientific disciplines, because, for example, it avoids skewing the average value of a long list of values upwards
- For an integer in rounding, replace the digits after the n digit with zeros. For example, if 1254 is rounded to 2 significant figures, then 5 and 4 are replaced to 0 so that it will be 1300. For a number with the decimal point in rounding, remove the digits after the n digit. For example, if 14.895 is rounded to 3 significant figures, then the digits after 8 are removed so that it will be 14.9.

### Significant figures in writing uncertainty

It is recommended for a measurement result to include the measurement uncertainty such as $x_\text{best} \pm \sigma_x$, where $x_\text{best}$ and $\sigma_x$ are the best estimate and uncertainty in the measurement respectively. $x_\text{best}$ can be the average of measured values and $\sigma_x$ can be the standard deviation or a multiple of the measurement deviation. The rules to write $x_\text{best} \pm \sigma_x$ are:

- $\sigma_x$ should usually be quoted to only one or two significant figures, as more precision is unlikely to be reliable or meaningful.
- The digit positions of the last significant figures in $x_\text{best}$ and $\sigma_x$ are the same, otherwise the consistency is lost. For example, "1.79 ± 0.067" is incorrect, as it does not make sense to have more accurate uncertainty than the best estimate.

### Implied uncertainty

Uncertainty may be implied by the last significant figure if it is not explicitly expressed. The implied uncertainty is $\pm$ the half of the minimum scale at the last significant figure position. For example, if the mass of an object is reported as 3.78 kg without mentioning uncertainty, then $\pm$ 0.005 kg measurement uncertainty may be implied. If the mass of an object is estimated as 3.78 ± 0.07 kg, so the actual mass is probably somewhere in the range 3.71 to 3.85 kg, and it is desired to report it with a single number, then 3.8 kg is the best number to report since its implied uncertainty ± 0.05 kg gives a mass range of 3.75 to 3.85 kg, which is close to the measurement range. If the uncertainty is a bit larger, i.e. 3.78 ± 0.09 kg, then 3.8 kg is still the best single number to quote, since if "4 kg" was reported then a lot of information would be lost.

### Arithmetic with significant figures

When performing arithmetic operations with numbers that have significant figures, the result should be rounded to the appropriate number of significant figures based on the operation performed.

- For quantities created from measured quantities via multiplication and division, the calculated result should have as many significant figures as the least number of significant figures among the measured quantities used in the calculation.
- For quantities created from measured quantities via addition and subtraction, the last significant figure position (e.g., hundreds, tens, ones, tenths, hundredths, and so forth) in the calculated result should be the same as the leftmost or largest digit position among the last significant figures of the measured quantities in the calculation.
- The base-10 logarithm of a normalized number (i.e., $a \times 10^b$ with $1 \leq a < 10$ and $b$ as an integer), is rounded such that its decimal part (called mantissa) has as many significant figures as the significant figures in the normalized number. When taking the antilogarithm of a normalized number, the result is rounded to have as many significant figures as the significant figures in the decimal part of the number to be antiloged.

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

The difference between true value of the quantity being measured and the measured value is called error. Since we do not know the true value, we can never know the error, only estimate it. There are two types of errors - systematic errors and random errors. Random errors are caused by unpredictable fluctuations in the measurement process, while systematic errors are caused by a consistent bias in the measurement process. Systematic errors can be reduced by calibration and careful experimental design, while random errors can be reduced by taking multiple measurements and averaging them.

A precise measurement is one that is consistent and reproducible, while an accurate measurement is one that is close to the true value. A measurement can be precise but not accurate, or accurate but not precise. Ideally, we want measurements that are both precise and accurate.

We use the term "uncertainty" to refer to the range of values within which we expect the true value to lie. The uncertainty in a measurement is often expressed as a percentage of the measured value, or as a range of values.

Statistical analysis is the process of collecting, analyzing, interpreting, presenting, and organizing data. It involves using statistical methods to summarize and describe the data, as well as to make inferences and predictions based on the data. It allows us to estimate random errors and uncertainties in measurements, and to determine the significance of the results. However, statistical analysis cannot tell us about systematic errors, which are often more difficult to detect and correct.

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
