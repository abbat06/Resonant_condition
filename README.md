## Conditions on existence of resonances in Hamiltonian system

Consider an analytic Hamiltonian system 
```math
\dot{\mathbf x}=\frac{\partial H}{\partial\mathbf y}, \dot{\mathbf y}=-\frac{\partial H}{\partial\mathbf x},
```
with $n$ degrees of freedom, near its equilibrium at the origin $\mathbf x=\mathbf y=0$.

The Hamilton function $H(\mathbf x,\mathbf y)$ expands into a convergent power series 
```math
H(\mathbf x,\mathbf y) = \sum H_{\mathbf p\mathbf q}\mathbf x^{\mathbf p}\mathbf y^{\mathbf q}
```
with constant coefficients $H_{\mathbf{pq}}$, where $\mathbf p,\mathbf q\geq0$, $|\mathbf p|+|\mathbf q|\geq2$, and $|\mathbf{p}|=|p_1|+\dotsb+|p_n|$. 

Linear approximation of the Hamiltonian phase flow is provided by system 
```math
\dot{\mathbf{z}}=B\mathbf{z}\text{ with matrix }B =\mathit{J}\mathrm{Hess}\,{H}|_{\mathbf x=\mathbf y=0}, 
```
where $\mathbf z=(\mathbf x,\mathbf y)$ and $\mathrm{Hess}\,{H}$ is the Hessian of function $H(\mathbf x,\mathbf y)$. 

The eigenvalues of matrix $B$ can be reordered is a such way that $\lambda_{j+n}=-\lambda_j$, $j=1,\dotsc,n$.  Denote by vector $ \boldsymbol{\lambda} = (\lambda_1,\dotsc,\lambda_n)$ the set of **basic eigenvalues** of the linear system with Hamiltonian  $H_2$. In the Hamiltonian case the characteristic polynomial is written  in the form
```math
f(\mu)=\mu^n+a_1\mu^{n-1}+a_2\mu^{n-2}+\dotsb+a_{n-1}\mu+a_n, 
```
where $ \mu=\lambda^2$.

According to Theorem 12 in [Bruno1972]:[^1]  in the case of semi-simple eigenvalues of quadratic form $H_2$ there exists a canonical formal transformation that reduces the Hamiltonian system to its **normal form** 
```math
\dot{\mathbf u}=\frac{\partial h}{\partial\mathbf v},\quad \dot{\mathbf v}=-\frac{\partial h}{\partial\mathbf u},
```
given by the normalized Hamiltonian $ h(\mathbf u,\mathbf v)$: 
````math
h(\mathbf u,\mathbf v) =\sum_{j=1}^n\lambda_ju_jv_j+\sum_{|\mathbf p|+|\mathbf q|\geqslant2} h_{\mathbf p\mathbf q}{\mathbf u}^{\mathbf p}\mathbf v^{\mathbf q}, 
```
````

containing only the resonant terms $h_{\mathbf p\mathbf q}\mathbf u^{\mathbf p}\mathbf v^{\mathbf q}$ satisfying the **resonant equation** 
```math
\left\langle\mathbf p-\mathbf q,\boldsymbol{\lambda}\right\rangle=0.
```
Here $\left\langle\mathbf p, \boldsymbol{\lambda}\right\rangle=\sum\limits_{j=1}^n p_j\lambda_j $ is the scalar product.

The resonant equation has two kinds of solutions, which correspond to two kinds of resonant terms in the normal form:

1) *Secular terms* of the form $ h_{\mathbf{pp}}\mathbf u^{\mathbf p}\mathbf v^{\mathbf p} $, which are always present in the Hamiltonian normal form due to the special structure of the matrix $ B $ of the linearized system.
2) *Strictly resonant terms*, which correspond to nontrivial integer solutions of the equation $\left\langle \mathbf p,\boldsymbol{\lambda}\right\rangle=0$.

Following [2, Ch. I, Sec. 3]:[^2] we define **resonance multiplicity** $\mathfrak{k}$ as the number of linearly independent solutions $\mathbf p\in\mathbb Z^n $ to the equation $\left\langle \mathbf p,\boldsymbol{\lambda}\right\rangle=0$, and the *resonance order* $\mathfrak q=\min |\mathbf{p}|$ by $\mathbf{p} \in \mathbb{Z}^{n}$, $\mathbf{p} \neq 0,\langle\mathbf{p}, \boldsymbol{\lambda}\rangle=0$. If the solution to the equation $\left\langle \mathbf p,\boldsymbol{\lambda}\right\rangle=0$ contains only two eigenvalues, then such resonance is called a **two-frequency resonance**, if more than two, then it is called a  **multifrequency resonance**.

**Problem.** Obtain conditions on the coefficients $ a_j $, $ j=1,\dotsc,n $,  of the polynomial $f(\mu)$  of degrees  $n=3$ and $n=4$, under which the multifrequency resonance of multiplicity 1 of order 3 or order 4 takes place.



[^1]: A.D. Bruno Analytical form of differential equations (II) // *Trans. Moscow Math. Soc.*, 26:199--239, 1972.
[^2]: A.D. Bruno. *The Restricted 3-body Problem: Plane Periodic Orbits*. Walter de Gruyter, Berlin, 1994.
