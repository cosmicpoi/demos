---
layout: default
title:  "Fluids"
date:   2017-08-05 12:34:18 -0400
categories: demos canvas
src: "fluid.html"
---

**Controls:**

- Mouse down on a cell to increase fluid volume. 
- Mouse up to watch things happen.

This is a physics-based fluid simulation using [cellular automata](https://en.wikipedia.org/wiki/Cellular_automaton). I got this algorithm from this [Reddit post](https://www.reddit.com/r/cellular_automata/comments/6jhdfw/i_used_1dimensional_cellular_automata_to_make_a/).

I added some of my own fine-tuning, as well. Occasionally the fluid pressure will go out of whack and cause some volume to go over the walls. In order to avoid this, I added damping on each step. This pretty much ensures that the fluid will flatten out over time. I also added a small adjustment to make sure pressures are not negative for too long, as this can lead to some odd occurences.

**Note:** It is a known bug that the simulation will stop working properly if any fluid gets onto the left or right walls. This may occur if you make a really large stack of fluid close to the walls.