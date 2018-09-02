# AMS540- Linear Programming

*William Murphy<br> SBID: 106796665*<br>
*Notes for chapters 1 to 3*<br>*9/1/2018*

---

## General Form (LP):
> *When the objective funtion and all constraint functions are <br> affine, the convex optimization problem is a linear program(LP). The general form of an (LP) is :*<br>
$$\begin{align*} minimize \quad c^Tx + d \\ subject \ to \ \ \ \ Gx ≼ h \\ Ax = b \end{align*}$$
> We can omit the constant, $d$ in the objective function as it has no affect on the feasible set.<br>
>  Note that we can maximize the affine function by minimizing the negation of it. e.g. *minimize* $-c^Tx - d$. The feasible set of an LP is a polyhedron, $\mathcal P$, which is just an intersection of multiple half-spaces.



### Converting an LP to Standard form
> #### 1 . If objective function is minimized, convert to maximize
>  > e.g. *minimize* $4x + y + z$ to *maximize* $-4x - y - z$
>
> #### 2 . Express the variable, $x$, as the difference of two non-negative variables.
> > e.g. We set $x = x^+ - x^-$, such that $x^+ ⪰ 0$, $x^- ⪰ 0$
> > and the following LP:
> > $$\begin{align*} minimize \qquad c^Tx + d \qquad \\ subject\ to\quad  \ \ \ \ \ Gx + s = h \ \\ Ax = b \qquad \\ s ⪰ 0 \qquad
> > \end{align*}$$
> > becomes
> > $$ \begin{align*} minimize \qquad c^Tx^+ - c^Tx^- + d \qquad \\ subject \ to\qquad  \ Gx^+ - Gx^- + s = h \ \ \\ Ax^+ - Ax^- = b \qquad\ \ \\  x^+ ⪰ 0, \ \ x^- ⪰ 0, \ \ s ⪰ 0
\end{align*}$$
