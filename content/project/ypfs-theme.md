---
title: 'YPFS ggplot theme'
author: corey
date: '2020-04-24'
categories:
  - open data
  - R
  - YPFS
tags: []
summary: "Here's my attempt to create a visual theme for our work"
authors: []
external_link: ''
image:
  caption: ''
  focal_point: ''
  preview_only: no
url_code: 'https://github.com/runkelcorey/theme'
url_pdf: 'https://github.com/runkelcorey/theme/blob/master/examples/theme_print.pdf'
url_slides: ''
url_video: ''
slides: ''
---

This project is a bit on hold as I strike the right balance between accessibility and flexibility.
It makes use of [`showtext`](https://github.com/yixuan/showtext), which allows for the installation of custom fonts, but doesn't handle extremely high and low quality as well as [`ggplot2`](https://ggplot2.tidyverse.org/) does.

When we at YPFS spent our whole days blogging about the pandemic's toll on economies worldwide, we put out a lot of graphs, and they all looked different.
This isn't the biggest deal, but consistent style goes a long way to weave different research threads together.
And with a [typekit](https://yaleidentity.yale.edu/web) and [palette](https://toolness.github.io/accessible-color-matrix/?n=white&n=light&n=emphasis&n=Yale%20blue&n=black&v=F9F9F9&v=63AAFF&v=286DC0&v=00356B&v=222222) as beautiful as Yale's, using Excel and Calibri is something of a shame.

This repository is an evolving project to standardize the production of figures within R, an open-source statistical package. Researchers who publish with[in] the Yale School of Management will recognize its distinct use of Helvetica Neue, while affiliated with the University at large will recognize that typekit and palette of blues. However, conforming to the school's style can be a time-consuming process, likely to be ignored in favor of other work. A standard theme can plug the gap caused by tedious formatting.
