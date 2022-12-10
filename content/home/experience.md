---
# An instance of the Experience widget.
# Documentation: https://wowchemy.com/docs/page-builder/
widget: experience

# This file represents a page section.
headless: true

# Order that this section appears on the page.
weight: 60

title: Experience
subtitle:

# Date format for experience
#   Refer to https://wowchemy.com/docs/customization/#date-format
date_format: Jan 2006

# Experiences.
#   Add/remove as many `experience` items below as you like.
#   Required fields are `title`, `company`, and `date_start`.
#   Leave `date_end` empty if it's your current employer.
#   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
experience:
  - title: Research Scientist
    company: Georgia Tech Research Institute
    company_url: 'https://gtri.gatech.edu/'
    company_logo: ''
    location: Atlanta, GA
    date_start: '2016-08-01'
    date_end: ''
    description: Projects fall into a few main categories at GTRI. C\# WPF applications, multi-threaded C++ with OpenGL, and XR/VR with Unity. The most notable project being a VR one that takes place over massive areas of land both on the ground and in the air. 

  - title: VP of Engineering
    company: Invision3D
    company_url: ''
    company_logo: ''
    location: Atlanta, GA
    date_start: '2018-02-01'
    date_end: '2018-11-01'
    description: WebGL oriented company providing visualization and product customization services.

  - title: Contract Game Architect/Programmer and VFX Developer
    company: Luxurious Animals
    company_url: ''
    company_logo: ''
    location: Atlanta, GA
    date_start: '2016-03-01'
    date_end: '2018-06-01'
    description: The primary project that I have been contracted to work on is a WebGL game called Feisty Galaxies. The project was inherited from a previous developer, and much has changed since then. The collision detection system was revamped to work on a plane-sweep model, many shaders and particle effects have been introduced, and a post-processing manager had to be built since the example one available with Three.js and an alternative called Wagner did not provide the features needed for being able to adequately manage the effects. 

  - title: Software Engineer
    company: GPA LEARN
    company_url: ''
    company_logo: ''
    location: Atlanta, GA
    date_start: '2013-08-01'
    date_end: '2016-08-01'
    description: Central duties revolved around building the core of the web-based learning systems. Primarily JavaScript based, this layer provides a functional framework for Content Developers to build out lessons using custom widgets. 

  - title: Contract Tools Developer
    company: VIMtrek
    company_url: ''
    company_logo: ''
    location: Atlanta, GA
    date_start: '2015-05-01'
    date_end: '2015-12-01'
    description: Initially work was done primarily in Unity, and encompassed a variety of different topics including the creation of shaders, UI work, and a decent amount of 3D math. Later the work shifted more towards the development of tools, ultimately culminating in a batch tool written in C++ that would load the custom VIMTrek format and optimize the models within using the Atangeo Balancer SDK, as configured by YAML files in this case, before writing them back out to the custom format. The endeavor required providing a suitable wrapper to the C# DLL without the use of COM. While multi-threading was initially explored, it was deemed unnecessary due to the nature of the machines it would be running on. 

  - title: Freelance Gameplay Programmer & TD
    company: Kaneva
    company_url: ''
    company_logo: ''
    location: Atlanta, GA
    date_start: '2011-06-01'
    date_end: '2014-04-01'
    description: My work here involved the creation of several game templates and assets which would be used as the framework for user games. I also developed an animation framework to assist in UI animation, and augmented the world building mode to allow the camera to be detached from the avatar and flown about the space freely making it easier to build at larger scales. As part of that process I also implemented the ability to record camera movement and play it back to other users whenever the creator desired. This allowed for players to create cinematic sequences, which was previously not possible.

design:
  columns: '2'
---
