---
layout: default
title:  "Particles"
date:   2017-05-24 11:53:18 -0400
categories: demos canvas
src: "particles.html"
---

This is one of three demos found on the homepage of my website [alanluo.com](http://alanluo.com) as of August 2017.

I'd been messing with particle simulations for a while. After extensive tuning, this is the most responsive particle system I've made so far. It has two key features.

- It rather than the [inverse-square](https://en.wikipedia.org/wiki/Inverse-square_law) law for gravitational fields, it just uses an inverse law (no square).
- It uses velocity-dependent fluid damping in the differential equation.

This makes the simulation feel more responsive because the overall strength of the force is increased, but the fluid damping also means that particles are quickly stopped rather than going out of control as they would in a frictionless environment.
