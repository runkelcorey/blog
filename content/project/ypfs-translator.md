---
title: 'YPFS web scraper'
author: corey
date: '2020-04-24'
categories:
  - open data
  - YPFS
tags: []
summary: "A custom translator for YPFS' archive"
authors: []
external_link: ''
image:
  caption: ''
  focal_point: ''
  preview_only: no
url_code: 'https://github.com/runkelcorey/translators/blob/master/ypfs.js'
url_pdf: ''
url_slides: ''
url_video: ''
slides: ''
---

RAs would told me how much time it takes to enter metadata into both Zotero and [our own archive](ypfs.som.yale.edu).
Because our Zotero library captures more information than our archive, the ideal solution was to export Zotero information to our Drupal content management system.
However, YPFS gets no love from Yale's business-school IT department.
We ultimately find a lot of workarounds to aid our work, and it was no different here.

Another way to cut down on time spent entering metadata was the reverse: instead of exporting to our archive, we could export *from* our archive.
This is where Zotero comes in.
It accepts a number of different formats for bibliographic information stored on websites.
Unfortunately, our website exposes metadata in none of these [standard](https://www.zotero.org/support/dev/exposing_metadata) formats.

Again, we needed to slightly modify our idea of how to transfer data between Zotero and our archive.
In this case, we *imported* from our archive.
Zotero [allows](https://github.com/zotero/translators/) people to volunteer translators that let Zotero read metadata on specific sites.

I learned the basics of JavaScript to write [this](https://github.com/zotero/translators/pull/2358) bit of code.
This totally felt like learning a new language.
My previous experience with programming had really been limited to data science.
I was accustomed to static products like a plot or table.
Here, I contended with interactivity---in which a command is triggered by an end-user action---and inputs not yet defined (a/k/a new webpages created in the future).

The result is a plug-in that, once accepted by Zotero's administrators, will allow all users of Zotero to import directly from our archive.
Significantly, it is the only website-specific translator I've seen that accepts more than just webpage snapshots or PDFs.
This translator will accept audio, video, Word documents, images, you name it.
