---
# Documentation: https://wowchemy.com/docs/managing-content/

title: Ribbon Curves
subtitle: Dynamic, Symmetric, Curve Bridging
summary: Bridging two curves in three dimensions using a ribbon-like approach
authors: []
tags: []
categories: []
date: 2022-11-28T21:16:53-05:00

# Optional external URL for project (replaces project detail page).
external_link: ""

banner:
  image: ribbon_header.png
  caption: Bridging 3D Curves

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: Ribbon Curves
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

Project 3 for Foundation of Computer Graphics was to use two curves in 3D space to create a pipe with a bonus aspect for coming up with a symmetric solution for the pipe or being able to show an osculating ball that would roll along one curve while not ever being pierced by the other. In addition to performance improvements from using OpenGL display lists, I came up with what may be an original solution to the problem by way of what I call the wrapping paper or ribbon method for continuously mapping one curve onto the other. The process starts with discretized versions of the curves and the two points from each curve that are closest to one another across all points. The process then marches along the curves point by point creating triangles by selecting the shorter of the next two edge candidates. This results in a ribbon between the curves that is then used for finding a more stable mid-point mapping between the curves than other solutions that only consider the absolute closest point of the other curve regardless of context. This also produces a symmetric solution that does not depend on which curve is the basis for solving the problem.

{{< vimeo 653471933 >}}

