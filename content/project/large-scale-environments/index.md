---
# Documentation: https://wowchemy.com/docs/managing-content/

title: Large Scale Environments
subtitle: Global Scale, VR Performance, Real Data
summary: Managing large sections of real-world data for high-speed traversal in VR
authors: []
tags: []
categories: []
date: 2022-11-28T21:40:30-05:00

# Optional external URL for project (replaces project detail page).
external_link: ""

banner:
  image: grid_header.png
  caption: Large Scale Environments

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: Large Scale Environments
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

A large project at work required the ability to go from ground level to an altitude of 20,000ft. in an instant while remaining performant enough for VR headsets. While there existed some solutions out there to manage larger worlds within Unity, none of them met the project’s requirements. I set out to create a system that treated the real-world terrain data as a nested subdivision tree. Each layer of subdivision can have multiple LODs for better performance and each cell of the layer can be comprised of an arbitrary whole number of divisions of the next greatest resolution. Since every cell is loaded asynchronously the system ensures that there is never a gap in the ground by only switching out cells when all are ready (does not apply to very first load). What makes this solution novel is that there is support for more than one effector on the structure of the grid and how each effector influences the grid can adjust dynamically over time. The system regularly calculates what shape satisfies all conditions and dynamically loads tiles of various resolutions that are stored as Unity scenes. The system also integrates an origin-shifting solution to manage areas far larger than the physics system will typically allow. The system similarly maintains a cache of recently processed tiles to accelerate hops to and from a distant area. The video below shows how the system can manage a large area (over six hundred square kilometers) with ease. Even in the editor the system can help maintain over 350fps for an area this size.

{{< vimeo 663821513 >}}
