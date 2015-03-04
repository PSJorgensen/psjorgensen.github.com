---
layout: post
category : lessons
tagline: "Supporting tagline"
tags : [intro, beginner, jekyll, tutorial]
---
{% include JB/setup %}

EXPLORING HOW TO SET UP AN OPEN LAB BOOK
========================================

First things first
------------------

Since this is my first post attempting to use a reproducible workflow
integrated with the "rmarkdown" package and "knitr" as well as "git",
"github" and maybe "jekyll", this first part of the post covers how to
install these.

    install.packages("rmarkdown")
    library(rmarkdown);library(knitr)

### install R studio

### installing Rmarkdown package to create write the document

### setting up a github account

<http://www.github.com> - click "create account"

### downloading git for windows and setting up https connection

guide to install git for windows
<http://guides.beanstalkapp.com/version-control/git-on-windows.html>

set username and password <https://help.github.com/articles/set-up-git/>

caching your password in git
<https://help.github.com/articles/caching-your-github-password-in-git/>

### the most simple https-based github commands

cloning - fetching - merging - pulling
<https://help.github.com/articles/which-remote-url-should-i-use/>

### Jekyll and ruby installation guide

<http://jekyllrb.com/docs/installation/>

<http://jekyll-windows.juthilo.com/1-ruby-and-devkit/>

### Jekyll install fix - change https to http

<https://github.com/juthilo/run-jekyll-on-windows/issues/34>

### setting up the jekyll-bootstrap blog

<http://jekyllbootstrap.com/usage/jekyll-quick-start.html>

IMPORTANT - figure out whether you are on https or ssh with github.

### switching jekyll-bootstrap theme

<http://www.techrepublic.com/article/build-full-featured-sites-with-jekyll-bootstrap-and-github/>

See the themes here: <http://themes.jekyllbootstrap.com/>

I chose the mark-reid theme with the following lines in the git bash
prompt in the root of my github site directory

    Rake theme:install git="https://github.com/jekyllbootstrap/theme-mark-reid.git"
    > Enter "y" or "yes"

### and this is the result

<http://psjorgensen.github.io/>

### converting rmarkdown to markdown

> This approach is necessary for Github Pages since plugins are not
> supported. Using this approach, we can convert the R Mardown file to
> plain Markdown using the R script below. The converted Markdown file
> will be saved in the same directory so that Jekyll can then convert
> the resulting file. For simplicity, I place the rmarkdown.r function
> in the root directory of my site (alternatively you can place this in
> your .Rprofile file in your home directory). I then call rmd.sh (also
> located in the root directory) to first, determine the directory where
> the script is be executed from, and two, call the convertRMarkdown
> function. This function will process all R Markdown files (.rmd by
> default) in the current working directory (which can be set explicitly
> with the dir parameter or by the rmd.sh script) and convert them to
> plain markdown (with .markdown file extension by default). Once
> converted, Jekyll will the process the resulting file(s). This file
> can be downloaded here.

#### 0. starting assumptions

this
====

#### 1. first download R markdown
