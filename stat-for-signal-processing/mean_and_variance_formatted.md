
#  **Problem 2 \-** *Mean and Variance of Random Variables*

*Given Y* and *X* are *random variables*.


X has mean and variance of $\mu_X$ and $\sigma_X^2$ , respectively.


Y is defined as:

 $$ Y=\frac{X-E\left(X\right)}{\sqrt{\mathrm{Var}\left(X\right)}}=\frac{X-\mu_X }{\sqrt{\sigma_X^2 }} $$ 
# Task 1
 $$ E\left(Y\right)=E\left(\frac{X-E\left(X\right)}{\sqrt{\mathrm{Var}\left(X\right)}}\right) $$ 

```math
a+b*E\left(V\right)=E\left(a+b*V\right)
```

 $$ E\left(Y\right)=\frac{1}{\sqrt{\mathrm{Var}\left(X\right)}}*E\left(X-E\left(X\right)\right)=\frac{1}{\sqrt{\mathrm{Var}\left(X\right)}}*\left(E\left(X\right)-E\left(X\right)\right)=\frac{1}{\sqrt{\mathrm{Var}\left(X\right)}}*0=0 $$ 
# Task 2
 $$ \textrm{Var}\left(Y\right)=\textrm{Var}\left(\frac{X-E\left(X\right)}{\sqrt{\textrm{Var}\left(X\right)}}\right) $$ 

**using** $b^2 *\textrm{Var}\left(V\right)=\textrm{Var}\left(a+b*V\right)$ ,

 $$ \begin{array}{l} \textrm{Var}\left(Y\right)={\left(\frac{1}{\sqrt{\textrm{Var}\left(X\right)}}\right)}^2 *\textrm{Var}\left(X\right)\newline =\frac{1}{\textrm{Var}\left(X\right)}*\textrm{Var}\left(X\right)\newline =\frac{\textrm{Var}\left(X\right)}{\textrm{Var}\left(X\right)}\newline =1 \end{array} $$ 

### Task 5

*Based on the previous task, find a method to generate a random vector with arbitrary mean vector and arbitrary (hermitian and positive definite) covariance matrix based on a standard multivariate Gaussian random vector.*


We are dealing with a similar situation as in **Task 4**, in the sense of transforming a normal distribution into a new one with arbitrary mean and variance. Yet here, instead of a single *RV* and its corresponding *PDF* plotted on a 2\-dimensional plane, we go into additional dimensions, such as $D=n+1$ , where $n\ge 2$ denotes the number of *RV*'s.


Considering $D=2$ , we arrive at the following initial setup compared to *Task 4*:

|      |      |
| :-- | :-- |
| **Task 4** <br>  | **Task 5** <br>   |
| **single** *RV* of $X_1$ <br>  | **multiple** *RV*'s of, $X_1 \;,X_2$ <br>   |
| $\displaystyle X_1 ~N\left(0,\;1\right)$ <br>  | $\displaystyle X_1 ,X_2 ~N\left(0,\;1\right)$ <br>   |
| $\displaystyle D=\left(n+1\right)=\left(1+1\right)=2$ <br>  | $\displaystyle D=\left(n+1\right)=\left(2+1\right)=3$ <br>   |
| data points in a single dimension <br>  | data points in a two dimensional space (plane) <br>   |
| density function of RV is obtained and displayed in the second dimension <br>  | density function is obtained for both RV, with covariance considered, they form a density surface in 3D space <br>   |
|      |       |


As for the transformation:

|      |      |
| :-- | :-- |
| **Task 4** <br>  | **Task 5** <br>   |
| single mean <br>  | vector of means: $M=\left\lbrack \mu_1 ,\mu_2 \right\rbrack$ <br>   |
| single variance <br>  | variance for each RV accompanied by their covariance: <br> $\displaystyle C=\left\lbrack \begin{array}{cc} \textrm{Var}\left(X_1 \right) | \textrm{Cov}\left({\mathit{\mathbf{X}}}_1 ,{\mathit{\mathbf{X}}}_2 \right)\newline \textrm{Cov}\left({\mathit{\mathbf{X}}}_1 ,{\mathit{\mathbf{X}}}_2 \right) | \textrm{Var}\left(X_2 \right) \end{array}\right\rbrack$ <br>   |
|      |       |


With concrete values:


Given the *standard normal (Gaussian) distributions*, $X_1$ and $X_2$ ,

 $$ X_1 ,X_2 ~N\left(0,\;1\right) $$ 

Given the following arbitrary *mean vector* and *covariance matrix*,

 $ $ \begin{array}{l} M=\left\lbrack 3,2\right\rbrack \newline C=\left\lbrack \begin{array}{cc} 2 & 0\ldotp 5\newline 0\ldotp 5 & 1 \end{array}\right\rbrack 
\end{array} $ $ 

The transformation is visualized as follows:


![figure_5.png](mean_and_variance_formatted_media/figure_5.png)
