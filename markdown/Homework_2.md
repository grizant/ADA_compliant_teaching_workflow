# Homework 2 
STAT 757 -- Section 1001 <br>
Instructor: Colin Grudzien

## Due: 09/13/2019

## Instructions
<blockquote>
 You may work with others on these problems but you must turn in your own work.  
 You may type your solutions in any way you like (LaTeX, Markdown, Office, etc...) as long as you present your work clearly and in an organized way.<br>
 <strong>Whenever plotting:</strong>
<ul>
 <li> Include a copy of a short R script corresponding to your plot.</li>
 <li> Your plot must be clearly labeled in all axes, legends, and the plot must include a clear title.</li>
 <li> The plot must be sensible and easy to read. </li>
</ul>
</blockquote>

## Problems

### Problem 1:

#### Prove each of the following statements:
<ol>
   <li>The sum of the residuals, weighted by the corresponding predictor variable, is zero,
    $$\sum_{i=1}^n X_i \hat{\epsilon}_i = 0$$
   </li>
   <li>The sum of the residuals, weighted by the corresponding fitted value, is zero,
    $$\sum_{i=1}^n \hat{Y}_i \hat{\epsilon}_i = 0$$
   </li>
<div class="pagebreak"> </div>
   <li>The estimated regression function always passes through the point defined by the means (or the center of mass), $\left(\overline{X},\overline{Y}\right)$.
  </li>
</ol>

#### Hint: use the normal equations and the point estimates of $\hat{\beta}_0,\hat{\beta}_1$ discussed in lecture.

### Problem 2:

#### Install the library "Faraway" in the R environment.  Then proceed to analyze the following data sets in this library:

<ol>
  <li> The dataset ``teengamb`` concerns a study of teenage gambling in Britain. Make a numerical and graphical summary of the data, commenting on any 
  features that you find interesting. Limit the output you present to a quantity that a busy reader would find sufficient to get a basic understanding of the data.
  </li>
  <li> The dataset ``uswages`` is drawn as a sample from the Current Population Survey in 1988. Make a numerical and graphical summary of the data as in the previous
question.
  </li>
</ol>


