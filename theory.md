## Farkas Lemma

One and only one of the following is true

$\begin{cases} 
\exist x, Ax=b, x\geq0 \\
\exist y, A^T y \geq0, b^T y \lt0 \end{cases}$



## Farkas Lemma Variant

One and only one of the following is true

$\begin{cases} 
\exist x, Ax \leq b, \\
\exist y, A^T y = 0, b^T y \lt0, y \geq0 \end{cases}$



## weak duality

$p^*=\min\limits_{x \in R^n} c^Tx, s.t. Ax=b, x\geq0$

$d^*=\min\limits_{y \in R^m} b^Ty, s.t. A^Ty \leq 0$

$\Rightarrow p^* \geq d^*$



## strong duality

primal optimal value coincides with the dual optimal value for linear programming, if both are bounded

$p^*=\min\limits_{x \in R^n} c^Tx, s.t. Ax=b, x\geq0$

$d^*=\min\limits_{y \in R^m} b^Ty, s.t. A^Ty \leq 0$​

$\Rightarrow p^* =d^*$

### proof

It suffices to show 
$\exist \ \bar{y}, b^T\bar{y} \geq p^*, A^T\bar{y} \leq c\qquad(*)$ 
(so that combined with weak duality, $b^T\bar{y} \leq p^*$ , $\Rightarrow b^T\bar{y}=p^*=d^*$)

$\Leftrightarrow \begin{pmatrix}A^T \\-b^T\end{pmatrix} y \leq\begin{pmatrix}c \\-p^*\end{pmatrix} \qquad (1)$

Assume that $(1)$ is not feasible, by Farkas Lemma Variant, 

$\exist \ \lambda=\begin{pmatrix}\widetilde{\lambda} \\\lambda_0\end{pmatrix} \geq 0, s.t. \begin{pmatrix}A \ & -b\end{pmatrix} \begin{pmatrix}\widetilde{\lambda} \\\lambda_0\end{pmatrix}=0$

$\Rightarrow A\widetilde\lambda=b\lambda_0$











