# Guidelines: Markdown

This document contains guidelines to write "good" markdown.

## Markdowns

Markdown is not yet standardised.
It has also lots of different implementations.
Unfortunately, there are a lot of small imcompatibilities between the different implementation.
Here are some flavors of markdown:

* [Markdown](https://daringfireball.net/projects/markdown/)
* [Pandoc's Markdown](https://pandoc.org)
* [Commonmark](https://commonmark.org)
* [Github Flavored Markdown](https://github.github.com/gfm/)
* [R Markdown](https://rmarkdown.rstudio.com)

Markdown was originally created by John Gruber in 2004.
Originally, It was a text-to-HTML conversion tool for web writers.
It is generally a subset of all the different markdown flavors.

Pandoc is a universal document converter.
It can notably create ebook, présentation and PDF from a markdown text file.
It has a very rich markdown syntax.
Pandoc's markdown is ideal to express text documents.

Commonmark aims to standardise the markdown syntax.
It is a specification that try to cover all the corner cases.

Github Flavored Markdown or GFM is a superset of Commonmark.
It is used by the Github website.

R Markdown is used with the R programming language.
It is notably useful to create notebooks.

## Wide application

We can see that markdown has a wide range of applications.
It is no more limited to a simple conversion tool from text to HTML.

Markdown can be written everywhere: from email to forum posts, but the aim of these guidelines is for stand-alone documents.

## Pandoc

The following guidelines focus on Pandoc's markdown syntax.
The use of Pandoc allows to write a single markdown text file and convert it into multiple file format.

This will allow to notably create:

* a stand-alone PDF
* an ebook
* a slide presentation
* a web page

# G: General

## Use UTF-8 file encoding

### Reason

Core Guidelines

### Remark

* Check your text editor.

## Use the `.md` file extension

### Reason

Short and familiar.

# Use `%` for commenting (non-md)

A comment must start on column 1.

### Reason

Markdown syntax do not provide a way for commenting.
The `%` is a good choice because it is not used by Gruber's markdown.
It is also familiar for LaTeX users.

Having comments starting on column 1 avoid the confusion between the start of a comment and the percent symbol.
It makes also a file easy to parse to remove comments.

Pandoc use the `%` symbol in its syntax, but this functionnality is easily replaceable by another syntax.

### Remark

* Comments must start on column 1.
* Use a space after `%`.

### Example

```
% This is a comment
```

## Use a YAML block to store metadata (Pandoc)

### Reason

The YAML block can store more information and without ambiguity compare to the `%` block.
Also, the `%` symbol can be used for commenting.

### Remark

* Follow the YAML specification.
* Do not use `%` for the metadata block

### Example

```
---
title: Awesome Title
author: John Smith
date: March 2020
...
```

### Example, bad

```
---
title: Awesome Title
author: John Smith
date: March 2020
---
```

```
% Awesome Title
% John Smith
% March 2020
```
