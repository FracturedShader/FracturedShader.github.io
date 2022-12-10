---
# Documentation: https://wowchemy.com/docs/managing-content/

title: Boids
subtitle: Flocking, Flowing, Swarms
summary: Highly parallel 3D boids numbering in the thousands
authors: []
tags: []
categories: []
date: 2022-11-28T21:40:10-05:00

# Optional external URL for project (replaces project detail page).
external_link: ""

banner:
  image: boids_header.png
  caption: Endlessly Flowing Boids

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: Boids
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

Project 4 for Simulation of Biology was the classic Boids simulation as described by Craig W. Reynolds in 1987. The expected outcome was just enough 2D Boids to exhibit flocking behavior with either toroidal wrapping boundaries, or hard boundaries that deflect incoming Boids. The ability to turn particular forces on/off on demand and attract/repel the Boids from the mouse was also required. Leveraging data-oriented principles, multi-threading, frustum culling during the render phase, and OpenGL display lists to cache the OpenGL 1.0 geometry calls I was able to create an interactive 3D Boids simulation that could support thousands of Boids simultaneously. While using an Octree data structure to accelerate spatial searching was considered, it ended up not being the limiting factor for performance.

{{< vimeo 653460237 >}}
