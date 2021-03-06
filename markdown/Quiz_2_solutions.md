# Quiz 2


## Instructions

>  Write your name at the top right.  You are to work on this quiz alone without any help 
>  from any other resource <b>except for a single $8.5 \times 11$ inch page of handwritten notes</b>.  
>  This quiz will be ungraded but must be handed in for attendance. 


## Problems:

### Problem 1:
When asked to state the simple linear regression model, a student wrote it as follows: 
$$\mathbb{E}\left[Y_i\right] = \beta_0 + \beta_1 X_i + \epsilon_i$$ 
Do you agree?  Explain.
<div class="solutions">
#### Solution:

Note, there is a major issue in the above where the expectation of $Y_i$ should be equal to,
$$\mathbb{E}\left[Y_i\right] = \beta_0 + \beta_1 X_i.$$

There are several reasonable responses to this question, including that
$$Y_i = \beta_0 + \beta_1X_i + \epsilon_i$$
can be considered our model for simple linear regression, as it is our hypothesis for the form of the signal, with variation, in the data.

Alternatively, we could also say that the form of the regression function is given by,
$$\hat{Y} = \hat{\beta}_0 + \hat{\beta}_1 X$$
with respect to the parameters estimated by least squares.
</div>

<div class="pagebreak"></div>


### Problem 2:
What is the <b>BLUE</b>?  Explain in what sense this is an "optimal" regression solution, and under what conditions these properties hold true.
<div class="solutions">
#### Solution:
The BLUE stands for the "Best Linear Unbiased Estimate" or "Best Linear Unbiased Estimator" either is fine.  This is an optimal solution in the sense
that the least squares estimates $\hat{\beta}_0$ and $\hat{\beta}_1$ have the minimum variance among all linear, unbiased estimators.

This holds in the case that the error $\epsilon_i$ is mean zero, constant variance $\sigma^2$ for all $i$, and for each $i \neq j$, $\mathbb{E}\left[\epsilon_i \epsilon_j\right] = 0$.
</div>

<div class="pagebreak"></div>


### Problem 3:
Use the definition of the <b>unbiased, sample-based variance estimate</b> to recover the regression estimate for $\sigma^2$.
Recall, the denominator must divide by the degrees of freedom remaining after the estimation of the mean.

<div class="solutions">
#### Solution:
Recall, our estimate for the mean response at case $i$ is given by the fitted value,
$$\hat{Y}_i = \hat{\beta}_0 + \hat{\beta}_1 X_i,$$
which depends on estimating the two parameters $\hat{\beta}_0,\hat{\beta}_1$, using two degrees of freedom.

The unbiased, sample-based estimate of the variance is given by the sum of square deviations of the samples from the estimated mean, normalized
by the number of left-over degrees of freedom, i.e,
$$\begin{align}
\hat{\sigma} &= \frac{\sum_{i=1}^n \left(\hat{Y}_i - Y_i \right)^2}{n - p} 
\end{align}$$

where $p$ is the number of parameters, in this case $p=2$.  By definition we recover furthermore,
$$\begin{align}
\hat{\sigma} &= \frac{\sum_{i=1}^n \left(\hat{Y}_i - Y_i \right)^2}{n - p}\\
& = \frac{\sum_{i=1}^n \hat{\epsilon}^2}{n-p} \\
&= \frac{RSS}{n-p} 
\end{align}$$
</div>
