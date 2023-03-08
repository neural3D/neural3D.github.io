---
title: "Presentation on Neural Rendering for Dynamic Scenes"
excerpt_separator: "<!--more-->"
date: 2023-03-06T13:00:00-00:00
categories:
  - Blog
tags:
  - Meeting
  - Presentation
  - Chalmers
---
During the second meeting in 2023, the new team member David Nilsson introduced the team to the state of the art in neural rendering for dynamic scenes.
<!--more-->
Neural rendering for dynamic scenes has several aspects which make it more difficult than classic neural rendering for static scenes.
In particular, the fact that the observations of the scene are usually monocular (only one observation per time step) means that the observations of the scene become ambiguous, as there are multiple explanations for why a change has occurred in the scene.
For example, an object that appears smaller between two time steps may have either shrunk or simply moved away from the camera.