# Getting started with pandoc to create beautiful reveal.js presentations

Clone the repository and run
```
>>> git clone https://github.com/TammoR/pandoc_to_reveal
>>> cd pandoc_to_reveal
>>> pandoc -t revealjs -s -o myslides.html pandoc_test.md -V revealjs-url=http://lab.hakim.se/reveal-js -V theme=sky --mathjax --slide-level=2 --css pandoc_test.css
```

This should create myslide.html, demonstrating some standard features
* including code
* including images
* formatting multiple columns
* including LaTeX rendered equations

To modify the presentation edit the corresponding `.md` file. A good markdown cheat-sheet is available [here](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet).

You can render the html using githubs hmlpreview tool
```
http://htmlpreview.github.io/?https://github.com/TammoR/pandoc_to_reveal/blob/master/pandoc_test.html
```
# Get a pdf version of your slides
Open your slides in the browser and add `?print-pdf` to the URL. E.g. using the htmlpreview tool:
```
http://htmlpreview.github.io/?https://github.com/TammoR/pandoc_to_reveal/blob/master/pandoc_test.html?print-pdf
```
Then you can use your browsers print function (might need some adjustment of margins) to create a PDF.

# Content of the markdown file
```
---
author: Tammo Rukat
title: Demo
date: June 12, 2017
---

# Include code

## Here is some code
```python
print("hello world")

# Include images

## Size can be given in curly brackets
``` ![placeholder](./calc_digit_data.png){height=100px} ```
![placeholder](./calc_digit_data.png){height=200px}


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
```
