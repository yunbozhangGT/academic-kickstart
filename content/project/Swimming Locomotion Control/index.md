---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Swimming Locomotion Control"
summary: "In this project, we investigated several optimization methods to find controlers that can drive simulated creatures to swim"
authors: [Yunbo Zhang, advised by Wenhao Yu and Greg Turk]
tags: []
categories: []
date: 2019-08-13

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

url_code: "https://github.com/DragonMyth/WaterCreatureSimulation"

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""

---
## Overview
In this project, I aimed to search for good locomotion controllers for creatures simulated as articulated rigid bodys swimming in a virtual fluid environment. Specifically, we investigated how CMA-ES and Reinforcement Learning could be used to find those controllers.

## CMA-ES
We used Covariance Matrix Adaptation (CMA-ES) to find a set of parameters that can actuate a creature to swim. For each degrees-of-freedom (DOF) in the articulated creature, we formulate its time depent target position as a sinusoidal function: $$q_{targ}=Asin(\omega t+\phi)$$
During simulation, torques for each DOF is computed from a stable PD controller to track a desired target configuration.
We then use CMA-ES to find the best set of parameters $\{ A_0,\phi_0,A_1,\phi_1,\dots,A_n,\phi_n \}$ that would make the longest distance traveled for a creature in some time period.

Using this formulation, we can get the following result of a swimming controller for an articulated flatworm.
### Flatworm
{{<youtube MjmL-VVzExU>}}

## Deep Reinforcement Learning
To get an even more robust controller that could be not only time dependent but also state dependent, we used some deep reinforcment learning algorithm to find good controllers. Specifically, we used Proximal Policy Optimization algorithm for our policy search. We build neural net policies that take input of all the DoFs of a articulated creature and out put the torque need to be generated for each DOF. 

Here are some fun results.
### Flatworm
{{<youtube nivNgAl7S-s>}}
### Turtle With Symmetric Strokes
{{<youtube wlbJOAsBesc>}}
### Turtle With Asymmetric Strokes
{{<youtube tLUJ7ZdVoTw>}}
### Humanoid
{{<youtube 8O4RJNbtLBI>}}
