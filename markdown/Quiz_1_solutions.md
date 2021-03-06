# Quiz 1


## Instructions

>  Write your name at the top right.  You are to work on this quiz alone without any help 
>  from any other resource <b>except for a single $8.5 \times 11$ inch page of handwritten notes</b>.  
>  This quiz will be ungraded but must be handed in for attendance. 


## Problems:

### Problem 1:
Assume that the following relationship is valid:
$$
Y_i = \beta_0 + \beta_1 X_i + \epsilon_i
$$
where $\mathbb{E}\left[\epsilon_i\right] = 0$ and $\mathbb{E}\left[\epsilon_i^2\right] = \sigma^2$.  Use the definition of the variance of a random variable to derive the variance of $Y_i$.
<div class="solutions">
#### Solution:
Recall, the mean of the random variable $Y_i$ is given as,
$$\mathbb{E}\left[Y_i \right] =  \mathbb{E}\left[ \beta_0 \right] + \mathbb{E}\left[\beta_1 X_i \right] + \mathbb{E}\left[\epsilon_i \right]$$
by the linearity of the expectation over sums.  Assuming that $\beta_0,\beta_1,X_i$ are all deterministic constants, then,
$$\mathbb{E}\left[Y_i \right] =   \beta_0 + \beta_1 X_i. $$
By definition of the variance, we can compute,
$$\begin{align}
\mathbb{E}\left[\left(Y_i -  \beta_0 + \beta_1 X_i\right)^2\right] &= \mathbb{E}\left[ \epsilon_i^2\right] \\
&=\sigma^2 
\end{align}$$
</div>


<div class="pagebreak"> </div>
### Problem 2:

Which of the following equations linear in the parameters $\beta_j$, or can be transformed into such an equation?  Explain.
<ol> 
  <li>$Y_i = \beta_0 + \beta_1 X_i^\frac{3}{2} +\epsilon_i$;</li>
  <li>$Y_i = \beta_0 + \beta_1 * \beta_2 * \beta_3 X_i + \epsilon_i$;</li>
  <li>$Y_i = \beta_0 X_i^{\beta_1} \epsilon_i$.</li>
</ol>

<div class="solutions">
#### Solution:

<ol>
   <li> Note that $X_i^\frac{3}{2}$ can always just be written as a change of scale; the linearity of the equation in the parameters is not affected by the nonlinearity of the predictor.</li>
   <li> The product of the three parameters $\beta_1,\beta_2,\beta_3$ in addition to the terms in the sum renders this nonlinear, without a direct transformation available.</li>
   <li> Note that if we take log of the equality, then
    $$ \log(Y_i) = \log(\beta_0) + \beta_1 \log(X_i) +  \log(\epsilon_i),$$
    Note that if $\epsilon$ is assumed to be mean zero, this may prove to be an issue, and our assumptions about $\epsilon_i$ will necessarily change with respect to such a model.</li> 
</ol>

</div>
