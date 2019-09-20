---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Tinkertoy"
summary: "A 2D particle constraint dynamic system with distance, circle, and sine constraints."
authors: [Yunbo Zhang]
tags: []
categories: []
date: 2017-10-05

# Optional external URL for project (replaces project detail page).
external_link: ""

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
  focal_point: ""
  preview_only: true

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
# links:
# - name: Follow
#   url: https://twitter.com
#   icon_pack: fab
#   icon: twitter

url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---

## Overview
This is a course project I did from CS 4496 computer animation class. In this project, I implemented a 2D particle-based constraint dynamic system with three different constraints: distance constraint, circle constraint, and a sine constraint.

### Distance Constraint
For two points $p_1$, $p_2$, and the disired distance between them $d$, the constraint is
$C(p_1,p_2) = \frac{1}{2}(p_1-p_2)^T(p_1-p_2)-\frac{1}{2}d^2$
### Circle Constraint
For a point $p$, circle center $p_c$, and circle radius $r$, the constraint is
$C(p) = \frac{1}{2}(p-p_c)^T(p-p_c)-\frac{1}{2}r^2$
### Sine Constraint
For a point $p$, amplitude $A$, frequency $\omega$, and virtical offset $c$, the constraint is
$C(p) = p_y-Asin(\omega p_x)+c$

{{<youtube ppV7fKofleM>}}
