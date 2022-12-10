---
# Documentation: https://wowchemy.com/docs/managing-content/

title: Viral Simulation
subtitle: Agency, Density, Caution
summary: Simulating viral spread with cautious agents
authors: []
tags: []
categories: []
date: 2022-11-28T21:39:58-05:00

# Optional external URL for project (replaces project detail page).
external_link: ""

banner:
  image: featured.png
  caption: Viral Simulation

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: Viral Simulation
  focal_point: Smart
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

Project 2 for Foundation of Computer Graphics was a configurable viral transmission simulation using small circles with limited agency to simulate viral spread. In addition to taking a multi-threaded approach to increase the number of individuals that could be simulated, the various visual states were pre-rendered and cached for quick blitting to the canvas. Individual agents were given a few additional parameters that influenced behavior around others when navigating to their goal points. The primary addition was a caution parameter that increased as the agent came into contact with known infected individuals. Higher caution values would cause the agent to distance themselves from others, put on a mask, and be more likely to avoid behaviors that would lead them to bumping into other individuals.

{{< vimeo 653468905 >}}
