---
layout: default
title:  "Fabric"
date:   2017-08-05 12:34:18 -0400
categories: demos canvas
src: "fabric.html"
---

**Controls:**

- Click and release.

This is a physics-based fabric simulation using HTML5 Canvas. There is no physics library; the entire engine is hard-coded.

The way it works is that every joint has a position, velocity, and acceleration. These are integrated via addition:

```
points[i].x+=points[i].vx;
points[i].y+=points[i].vy;

points[i].vx+=points[i].ax;
points[i].vy+=points[i].ay;
```

The top row of points are ignored in these calculations, making them static. Each line represents a constraint. Constraints follow [Hooke's Law.](https://en.wikipedia.org/wiki/Hooke%27s_law) The fabric properties simply emerge from this basic system.