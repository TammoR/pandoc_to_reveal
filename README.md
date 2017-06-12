# Getting started with pandoc to create beautiful reveal.js presentations

Clone the repository and run
```
>>> pandoc -t revealjs -s -o myslides.html pandoc_test.md -V revealjs-url=http://lab.hakim.se/reveal-js -V theme=sky --mathjax --slide-level=2 --css pandoc_test.css
```
This should create myslide.html, demonstrating some standard features
* including code
* including images
* formatting multiple columns
* including LaTeX rendered equations
