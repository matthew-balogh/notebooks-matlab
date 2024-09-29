
#  **Problem Set 1 / Problem 2 \-** *Mean and Variance of Random Variables*

*Given Y* and *X* *random variables (RV)*.


X has mean and variance of $\mu_X$ and $\sigma_X^2$ , respectively.


Y is defined as:

 $$ Y=\frac{X-E\left(X\right)}{\sqrt{\textrm{Var}\left(X\right)}}=\frac{X-\mu_X }{\sqrt{\sigma_X^2 }} $$ 
# Task 1

 *Analytically compute* $E\left(Y\right)$.


**Utilizing:**


```math
a+b*E\left(V\right)=E\left(a+b*V\right)
```


```math
E\left(Y\right)=E\left(\frac{X-E\left(X\right)}{\sqrt{\textrm{Var}\left(X\right)}}\right)
```


```math
E\left(Y\right)=\frac{1}{\sqrt{\textrm{Var}\left(X\right)}}*E\left(X-E\left(X\right)\right)=\frac{1}{\sqrt{\textrm{Var}\left(X\right)}}*\left(E\left(X\right)-E\left(X\right)\right)=\frac{1}{\sqrt{\textrm{Var}\left(X\right)}}*0=0
```

# Task 2

 *Analytically compute* $\textrm{Var}\left(Y\right)$.


**Utilizing:**


```math
b^2 *\textrm{Var}\left(V\right)=\textrm{Var}\left(a+b*V\right)
```


```math
\textrm{Var}\left(Y\right)=\textrm{Var}\left(\frac{X-E\left(X\right)}{\sqrt{\textrm{Var}\left(X\right)}}\right)
```


```math
\textrm{Var}\left(Y\right)={\left(\frac{1}{\sqrt{\textrm{Var}\left(X\right)}}\right)}^2 *\textrm{Var}\left(X\right)=\frac{1}{\textrm{Var}\left(X\right)}*\textrm{Var}\left(X\right)=\frac{\textrm{Var}\left(X\right)}{\textrm{Var}\left(X\right)}=1
```

# Task 3

 *Interpret the resulting random variable* $Y$.


 $Y$ is expressed by the RV of $X$ , for which the participating statistics, that is the *Expected Value (mean)* and the *Variance* can be choosen arbitrarily.


Regardless of the values of $X$ , $Y$ has an *expected value* of 0 and a *variance* of 1. Therefore, $Y$ can be seen as a function which takes an arbitrary RV $X$ as input, and transforms it into a RV with *mean* of 0 and *variance* of 1.


This is essentially the **standardization** function, which, considering a *normal (Gaussian) distribution* for the RV's, shifts the position of the distribution to be centered around zero and squeezes or stretches it to have a *standard deviation* (and *variance*) of 1, utilizing the arbitrarily choosen statistics, $E\left(X\right)$ and $\textrm{Var}\left(X\right)$ .
