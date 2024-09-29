
#  **Problem 2 \-** *Mean and Variance of Random Variables*

*Given Y* and *X* *random variables (RV)*.


X has mean and variance of $\mu_X$ and $\sigma_X^2$ , respectively.


Y is defined as:

 $$ Y=\frac{X-E\left(X\right)}{\sqrt{\mathrm{Var}\left(X\right)}}=\frac{X-\mu_X }{\sqrt{\sigma_X^2 }} $$ 
# Task 1

 *Analytically compute* $E\left(Y\right)$.


**Utilizing:**

```math
\mathit{\mathbf{a}}+\mathit{\mathbf{b}}*\mathit{\mathbf{E}}\left(\mathit{\mathbf{V}}\right)=\mathit{\mathbf{E}}\left(\mathit{\mathbf{a}}+\mathit{\mathbf{b}}*\mathit{\mathbf{V}}\right)
``` 

 $$ E\left(Y\right)=E\left(\frac{X-E\left(X\right)}{\sqrt{\mathrm{Var}\left(X\right)}}\right) $$ 


```math
E\left(Y\right)=\frac{1}{\sqrt{\mathrm{Var}\left(X\right)}}*E\left(X-E\left(X\right)\right)=\frac{1}{\sqrt{\mathrm{Var}\left(X\right)}}*\left(E\left(X\right)-E\left(X\right)\right)=\frac{1}{\sqrt{\mathrm{Var}\left(X\right)}}*0=0
```

# Task 2

 *Analytically compute* $\mathrm{Var}\left(Y\right)$.


**Utilizing:**

```math
{\mathit{\mathbf{b}}}^2 *\mathit{\mathbf{Var}}\left(\mathit{\mathbf{V}}\right)=\mathit{\mathbf{Var}}\left(\mathit{\mathbf{a}}+\mathit{\mathbf{b}}*\mathit{\mathbf{V}}\right)
```

 $$ \mathrm{Var}\left(Y\right)=\mathrm{Var}\left(\frac{X-E\left(X\right)}{\sqrt{\mathrm{Var}\left(X\right)}}\right) $$ 

```math
\mathrm{Var}\left(Y\right)={\left(\frac{1}{\sqrt{\mathrm{Var}\left(X\right)}}\right)}^2 *\mathrm{Var}\left(X\right)=\frac{1}{\mathrm{Var}\left(X\right)}*\mathrm{Var}\left(X\right)=\frac{\mathrm{Var}\left(X\right)}{\mathrm{Var}\left(X\right)}=1
```