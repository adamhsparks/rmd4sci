# HTML, PDF, and Word (and more!)

One of the really great, powerful things about rmarkdown is that we can convert it to many different output types. The top three that you might be most likely to use are HTML, PDF, and Microsoft Word. There are others, but in this section, we are going to briefly discuss how to render to these output formats, and some things that you might want to do for each of them.

## Overview

## Questions

* How do I convert to HTML, PDF, or Word?
* How do I set options specific to each of these?
* How can I include a screenshot of an interactive graphic in PDF or Word?

## Objectives

## How do I convert to HTML, PDF, or Word?

Here are three ways to do this:

1. You can control this in the "knit" button


```r
knitr::include_graphics("figs/rstudio-knit-button")
```

You might notice that depending on the option you select, this changes things in the YAML - which is another way to control which output you have:

2. You can change the YAML option

```YAML

```

And if we remember from the previous lesson, the information in the YAML is passed into the `render` function:

3. You can call the `render` function.



### A note on workflow with rmarkdown: HTML first, PDF/word later

It can be easy to get caught up with how your document looks. I highly recommend avoiding compiling to PDF or word until _you really need to_. [This is also recommended by the author of rmarkdown and knitr, Yihui Xie](). Because HTML doesn't have page breaks, this means that you can spend time working on generating content, and not trying to get figures to line up correctly. 

## Your Turn {.exercise}

1. Generate three reports, one as HTML, one as PDF, and one as microsoft word. Remember, if you are having PDF problems, see the installation chapter note on installing $\LaTeX$ with the R package, `tinytex`.

## Templates

## Controlling the outputs

Depending on the output type, HTML, PDF, or word, you can actually control how the document looks

### Options for HTML

Some common options for HTML include:

- Adding tab sets
- floating table of contents

### Options for PDF

- Adding page breaks
- injecting LaTeX into your rmarkdown document

### Options for Word

- templates using .doct files

## How do I set options specific to each output

Sometimes you might want to have specific output changes to 

## How can I include a screenshot of an interactive graphic in PDF or Word?

You might wish to include a screenshot of an interactive graphic you had in your HTML document. To do this, you will need the webshot package, and will need the following code in your rmarkdown document.

I recommend using the `webshot` package.

