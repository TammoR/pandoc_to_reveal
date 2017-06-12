---
author: Tammo Rukat
title: Demo
date: June 12, 2017
---

# Include code

## Here is some code
```python
print("hello world")
```

# Include images

## Size can be given in curly brackets
``` ![placeholder](./calc_digit_data.png){height=100px} ```
![placeholder](./figures/calc_digit_data.png){height=200px}


# Mutiple columns are done using html
<div class="column" style="float:left; width: 50%">
col1
</div>
<div class="column" style="float:left; width: 50%">
col2
</div>


# LaTeX support

## LaTeX for maths rendering
* requires ```--mathjax``` option
* Inline with ```$x^2$```: $x^2$
* Single line with ```$$\sqrt{x}$$```: $$\sqrt{x}$$


# Fragmented appearance

## Example
<span class="fragment (appear)" data-fragment-index="1"><p>
Things can appear

<span class="fragment (appear)" data-fragment-index="2"><p>
one

<span class="fragment (appear)" data-fragment-index="3"><p>
by

<span class="fragment (appear)" data-fragment-index="4"><p>
one
