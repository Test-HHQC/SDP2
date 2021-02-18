<head>
    <script src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>
    <script type="text/x-mathjax-config">
        MathJax.Hub.Config({
            tex2jax: {
            skipTags: ['script', 'noscript', 'style', 'textarea', 'pre'],
            inlineMath: [['$','$']]
            }
        });
    </script>
</head>

# Semidefinite programming
Special types of optimization problems.

# Problem definition
The goal is to maximize the object function

\begin{equation}
   Tr(CX)
\label{eq1}
\end{equation}

under the constraint $Tr(A_j X)\le b_j$ for all $j \in [m]$ with semidefinite $X$.

There are several frameworks to solve SDP. One of it is the [AK framework](#AKframe).

# Frameworks to solve SDP
## <a id="AKframe" />The Arora-Kale framework
For probelme definition, please see Equation \eqref{eq1}.
* complexity for the Arora-Kale framework

| ref | types | algorithm   |  complexity |
| --- | ---- | ----  |  ------ |
| [1] | classical  | Arora-Kale |  $\tilde{O}(nms(\frac{Rr}{\varepsilon})^4 + ns(\frac{Rr}{\varepsilon})^7)$ |
| [2] | QM   |   Fernando & Krysta |  $\tilde{O}(\sqrt{mn}s^2 R^{32}/\delta^{18})$       |


The improvment for the QM approach to the Arora-Kale framework is the [Gibbs sampling](#improvement).
The details are listed in the [Appendix](#details)


## <a id="improvement" />Main improvement
The quantized version of Arora- Kale approach used the Gibbs Sampler from Ref. [3] to achieve the quantum advantage.

    
## Reference:
[1]  S. Arora and S. Kale. A combinatorial, primal-dual approach to semidefinite programs. Proceedings of the thirty-ninth annual ACM symposium on Theory of computing. ACM, 2007.\
[2] [arxiv:1609.05537, Fernando G.S.L. Brandao, Krysta Svore, Quantum Speed-ups for Semidefinite Programming](https://arxiv.org/abs/1609.05537) \
[3] D. Poulin and P. Wocjan. Sampling from the thermal quantum Gibbs state and evaluating
partition functions with a quantum computer. Phys. Rev. Lett. 103, 220502 (2009).


## <a name="details" />Appendix
$$ \Vert\vec{x}\Vert_1=\sum_{i=1}^N\vert{x_i}\vert $$

$\bar{X} = \frac{\sum_{i=1}^n X_i}{n}$

$$ evidence\_{i}=\sum_j W_{ij}x_{j}+b_{i} $$

$$
\operatorname{ker} f=\{g\in G:f(g)=e_{H}\}
$$

Test a display math with equation number:
$$
  \begin{align}
    |\psi_1\rangle &= a|0\rangle + b|1\rangle \\\\
    |\psi_2\rangle &= c|0\rangle + d|1\rangle       
  \end{align}
$$


