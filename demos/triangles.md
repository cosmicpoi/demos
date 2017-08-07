---
layout: default
title:  "Triangle Flowers"
date:   2017-08-04 11:03:00 -0400
categories: demos canvas
src: "triangles.html"
---

**Controls:**

- Click to make a flower.
- Hold to make it bigger.
- Let go to watch it.

This is one of three demos found on the homepage of my website [alanluo.com](http://alanluo.com) as of August 2017.

This one was a lot of fun. It makes flowers! What else do you need to know?

Anyway, the way it works is that each triangle has three function attributes, corresponding to the derivative of height, rotation, and side length. I pre-constructed a bunch of these derivative functions so that the resulting path would be periodic. Each click then spawns a ring of identical triangles with a random set of functions, giving a lot of variety.