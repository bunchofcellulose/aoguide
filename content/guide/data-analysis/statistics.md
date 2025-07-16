---
title: Statistics
weight: 3
---


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

{{< tabs items="P1,Solution,IOAA 2018" >}}
    {{< tab >}}
    An observer measured trigonometric parallaxes of stars in a star cluster. Due to random errors, the measured parallax values are distributed symmetrically around the expected value with standard deviation equal to $0.05$ mas (milliarcsec). Assume there are no systematic errors and assume all stars in the said cluster have the same luminosity. It is known that the distance of this cluster from us is $R=5$ kpc.

    He gave the data table to 4 of his students (A, B, C and D) and they estimated the distance to the cluster in the following ways:

    1.  A. Convert each parallax measurement into distance and then find the average distance $(R_{A})$
    2.  B. Take the average of all parallaxes first and then convert the average parallax into distance. $(R_{B})$
    3.  C. Convert each parallax measurement into distance and then take the median distance value. $(R_{C})$
    4.  D. Find the median value of the parallaxes and then convert the median value into distance. $(R_{D})$

    State if the following statements are true or false. In case a given mathematical relation is false, give the correct relation.

    1.  If the $i^{th}$ star gave the smallest value of parallax and the $j^{th}$ star gave the highest value of parallax, in all likelihood $R_{i}-R>R-R_{j}$
    2.  $R_{A}=R$ (i.e. there is a high chance that the distance estimated by A fairly matches the true distance)
    3.  $R_{B}=R$ (i.e. there is a high chance that the distance estimated by B fairly matches the true distance)
    4.  $R_{C}<R$ (i.e. there is a high chance that the distance estimated by C will be systematically lower than the true distance)
    5.  $R_{D}=R$ (i.e. there is a high chance that the distance estimated by D fairly matches the true distance)
    {{< /tab >}}

    {{< tab >}}
    For parallaxes, we have a Gaussian distribution with mean $\mu=0.2$ mas and standard deviation $\sigma=0.05$ mas. This means the standard deviation is 25% of the expectation value.

    1.  **True.** The relationship between parallax $(p)$ and distance $(d)$ is $d = 1/p$. This is an inverse relationship. If parallax values are symmetrically distributed, the distances will not be. Small parallaxes correspond to large distances, and large parallaxes correspond to small distances. Thus, a small error in parallax for a close star has a smaller impact on distance than the same error for a distant star.
    2.  **False.** Correct relation: $R_{A} > R$. Due to the inverse relationship $d=1/p$, converting each parallax to distance _before_ averaging tends to overestimate the true distance. Smaller parallaxes (larger distances) have a disproportionately large effect on the average.
    3.  **True.** Taking the average of parallaxes first $(p_{avg})$ and then converting to distance $(R_B = 1/p_{avg})$ tends to give a more accurate estimate of the true distance, especially when errors are symmetric around the true parallax.
    4.  **False.** Correct relation: $R_{C} = R$. Taking the median of distances $(R_C)$ is generally robust against extreme values. For a symmetrically distributed parallax, the median of distances will be a good estimator of the true distance.
    5. **True.** Finding the median value of parallaxes $(p_{median})$ and then converting it to distance $(R_D = 1/p_{median})$ should also provide a good estimate that matches the true distance, as the median is less sensitive to outliers.
    {{< /tab >}}
{{< /tabs >}}

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
