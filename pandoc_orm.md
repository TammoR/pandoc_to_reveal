---
author: Tammo Rukat
title: OrMachine -- pandoc demo
date: June 12, 2017
---

# Motivation

## Single Cell Gene Expression
![](./mouse_data.png)


# Boolean Matrix Factorisation

## Intuition for Boolean Matrix Factorisation
<div class="column" style="float:left; width: 50%">
$$ $$
<span class="fragment (appear)" data-fragment-index="1"><p>
![](./figures/calc_digit_data.png)
</div>
<div class="column" style="float:left; width: 50%">
<span class="fragment (appear)" data-fragment-index="2"><p>
![](./figures/calc_digit_factor.png)
</div>
<div class="column" style="float:left; width: 100%">
<span class="fragment (appear)" data-fragment-index="3"><p>
![](./figures/calc_example.png)
</div>

## Probabilistic Generative Model
$$p(\underbrace{x_{nd}}_{\substack{\text{obser-} \\ \text{vation}}}|\overbrace{\mathbf{u}_d}^{\text{codes}},\underbrace{\mathbf{z}_n}_{\substack{\text{latent}\\ \text{rprsnt.}}},\overbrace{\lambda}^{\substack{\text{disper-}\\ \text{sion}}})= \begin{cases} \big(1+\exp[-\lambda]\big)^{-1};\;&\text{if}\;\color{darkgreen}{x_{nd}=\min(1,\mathbf{z}_n^T\mathbf{u}_d)}\;\; \\ \big(1+\exp[\lambda]\big)^{-1};\;&\text{else} \end{cases} \\ = \sigma_{\substack{\text{logistic} \\ \text{sigmoid}}}\left[\lambda \underbrace{\tilde{x}_{nd}}_{\tilde{x} = 2x-1} \left(1-2\color{brown}{\prod\limits_{l}(1-z_{nl}u_{ld})}\right) \right]$$
