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

#  the test section
Also see Equation \@ref(eq:mean).

\begin{equation}
\bar{X} = \frac{\sum_{i=1}^n X_i}{n} (\#eq:mean)
\end{equation}

And see Table \@ref(tab:mtcars).

```{r mtcars, echo=FALSE}
knitr::kable(mtcars[1:5, 1:5], caption = "The mtcars data.")
```


# Semidefinite programming
## Contents
* Problem definition
* complexity

## Problem definition
The goal is to maximize the object function $$Tr(CX)$$ under the constraint $Tr(A_j X)\le b_j$ for all $j \in [m]$ with semidefinite $X$.


The improvment for the QM approach to the Arora-Kale framework is the [Gibbs sampling](#improvement).


##<a id="AKframe" \>The Arora-Kale framework

* complexity for the Arora-Kale framework

| ref | algorithm   |  complexity |
| --- | ---- |  ------ |
| [1] | classical  |  $\tilde{O}(nms(\frac{Rr}{\varepsilon})^4 + ns(\frac{Rr}{\varepsilon})^7)$ |
| [1] | QM   |  $\tilde{O}(\sqrt{mn}s^2 R^{32}/\delta^{18})$       |

The details are listed in the [Appendix](#details)
The complexities are listed in Table 


There are several frameworks to solve SDP. One of it is the [AK framework](#AKframe).


## <a id="improvement" \>Main improvement
Use the Gibbs sampling.
    
    
## test

```sequence
Alice->Bob: Hello Bob, how are you?
Note right of Bob: Bob thinks
Bob-->Alice: I am good thanks!
```

```flow
st=>start: Start
op=>operation: Your Operation
cond=>condition: Yes or No?
e=>end

st->op->cond
cond(yes)->e
cond(no)->op
```


## Reference:
[1] [Fernando G.S.L. Brandao, Krysta Svore, Quantum Speed-ups for Semidefinite Programming](https://arxiv.org/abs/1609.05537)


## <a name="details" />Appendix
$$ \Vert\vec{x}\Vert_1=\sum_{i=1}^N\vert{x_i}\vert $$

$$ evidence\_{i}=\sum\_{j}W\_{ij}x\_{j}+b\_{i} $$

$$
\operatorname{ker} f=\{g\in G:f(g)=e_{H}\}{\mbox{.}}
$$

Test a display math with equation number:
$$
  \begin{align}
    |\psi_1\rangle &= a|0\rangle + b|1\rangle \\\\
    |\psi_2\rangle &= c|0\rangle + d|1\rangle       
  \end{align}
$$

