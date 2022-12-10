---
# Documentation: https://wowchemy.com/docs/managing-content/

title: Mass Spring Simulation
subtitle: Rolling, Swimming, Interactivity
summary: Simulating an aquatic creature with a mass-spring body and basic fluid dynamics
authors: []
tags: []
categories: []
date: 2022-11-28T21:40:20-05:00

# Optional external URL for project (replaces project detail page).
external_link: ""

banner:
  image: eel_header.png
  caption: Mass Spring Eel

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: Mass Spring Eel
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

The final project for Simulation of Biology was to create a mass-spring simulation with two simple creatures. The expectation was to create a top-down 2D system with creatures using just a few springs and point masses to move. For the project, I opted instead to create a 3D simulation with simple fluid dynamics for an eel and a Coulomb friction-based collision system with internal pressure forces for the blob. The project uses muscle contractions and physics interactions with the environment to move both the creatures. I also made it possible to control the creatures directly using the W/A/S/D keys on the keyboard. Both creatures are dynamically configurable in terms of resolution as well. The blob in the video below is comprised of 728 points and 2904 springs, all of which undergo a small amount of contraction/expansion to drive motion. The eel in the video below consists of 308 points and 1420 total springs with 49 springs along the lateral lines of the body acting as actuated muscles.

{{< vimeo 653452249 >}}
