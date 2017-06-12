# Pandoc and reveal.js -- simple, beautiful slides
## Getting started

Clone the repository and run
```
>>> git clone https://github.com/TammoR/pandoc_to_reveal
>>> cd pandoc_to_reveal
>>> pandoc -t revealjs -s -o myslides.html pandoc_test.md -V revealjs-url=http://lab.hakim.se/reveal-js -V theme=sky --mathjax --slide-level=2 --css pandoc_test.css -V transition=cube
```

This should create myslide.html, demonstrating some standard features.
To view your presentation open the .html output file in any browser.
* including code
* including images
* formatting multiple columns
* LaTeX rendered equations
* fragmented appearance

To modify the presentation edit the corresponding `.md` file. A good markdown cheat-sheet is available [here](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet).


You can render a html file that is on github using github's rendering tool and appending the URL.
```
http://htmlpreview.github.io/?https://github.com/TammoR/pandoc_to_reveal/blob/master/pandoc_test.html
```
## Get a pdf version of your slides
Open your slides in the browser and add `?print-pdf` to the URL. E.g. using the htmlpreview tool:
```
http://htmlpreview.github.io/?https://github.com/TammoR/pandoc_to_reveal/blob/master/pandoc_test.html?print-pdf
```
Then you can use your browsers print function (might need some adjustment of margins) to create a PDF.

## Change appearance
You can change the theme and the slide transitions by adjusting the corresponding options in the pandoc command. All options are documented in the [reveal.js project page](https://github.com/hakimel/reveal.js/).

Further modifications can be made by editing the local css file (pandoc_test.css).

## Section structure
The intended section depths is defined by the ```--slide-level=2``` option.
Content should only be put under the lowest level slides (this limitation is discussed [here](https://github.com/jgm/pandoc/issues/816).
