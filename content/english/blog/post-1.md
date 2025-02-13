---
title: "Tint Is Not Tufte: Brief Intro"
meta_title: ""
description: "this is meta description"
date: 2022-11-01T05:00:00Z
image: "/images/image-placeholder.png"
categories: ["Application", "Data"]
author: "John Doe"
tags: ["nextjs", "tailwind"]
draft: false
---

### Dirk Eddelbuettel and Jonathan Gilligan

{{< grid >}}
  {{< col cols="8" isMarkdown="true" >}}
   ###  An Introduction to tint
   tint (Eddelbuettel and Gilligan, 2019) updates the look and feel of ‘Tufte’ documents for R. It combines the (html and pdf parts of the) excellent tufte package
  (Xie and Allaire, 2018) with the Roboto Condensed font use and color scheme
  proposed by envisioned css plus minor style changes such as removal of italicsÐbut remains otherwise true to the tufte package for R. Later additions are a
  book style and well as generalisation of the font handling allowing for Lato and
  Garamond fonts along with extended color selection.

  The package name follows an old tradition and is recursive: tint is not tufte.
  Full documentation is available in the longer PDF vignette, its Lato and
  Garamond variants (see below) as well as the longer HTML vignette. As these
  render to about two megabytes each, we no longer include them by default in
  the package as it swells the size of the installed package unnecessarily
  {{< /col >}}

  {{< col cols="4" >}}
   {{< image src="images/nuevo laredo.png" >}}
  {{< /col >}}
{{< /grid >}}

### Margin Examples


```R
ggplot (mtcars, aes(wt, mpg)) +
geom_point (size-3, aes(colour-factor (cyl))) + theme (legend position="none")
```