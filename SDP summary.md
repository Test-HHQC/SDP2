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


##  The Arora-Kale framework

* complexity for the Arora-Kale framework
| ref | algorithm   |  complexity |
| --- | ---- |  ------ |
| [1] | classical  |  $\tilde{O}(nms(\frac{Rr}{\varepsilon})^4 + ns(\frac{Rr}{\varepsilon})^7)$ |
| --- | ---- |  ------ |
| [1] | QM   |  O(N)       |
| --- | ---- |  ------ |

The details are listed in the [Appendix](#details)
The complexities are listed in Table 


# My Anchored Heading {#my-anchor}

- Blah blah. I want say some things about the [Methods](#methods) section. 

[link to my anchored heading](#my-anchor)

## Methods {#methods}

This is what I did. 


An oft-requested feature was the ability to have Markdown automatically handle within-document links as easily as it handled external links. To this aim, I added the ability to interpret [Some Text][] as a cross-link, if a header named “Some Text” exists.

As an example, [Metadata][] will take you to the [section describing metadata][Metadata].

Alternatively, you can include an optional label of your choosing to help disambiguate cases where multiple headers have the same title:

### Overview [MultiMarkdownOverview] ##
This allows you to use [MultiMarkdownOverview] to refer to this section specifically, and not another section named Overview. This works with atx- or settext-style headers.

If you have already defined an anchor using the same id that is used by a header, then the defined anchor takes precedence.

In addition to headers within the document, you can provide labels for images and tables which can then be used for cross-references as well.



## Reference:
[1] [Fernando G.S.L. Brandao, Krysta Svore, Quantum Speed-ups for Semidefinite Programming](https://arxiv.org/abs/1609.05537)


##  Appendix{#details}
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

