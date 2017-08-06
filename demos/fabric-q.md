---
layout: default
title:  "Fabric?"
date:   2017-08-05 12:00:18 -0400
categories: demos canvas
src: "fabric-q.html"
---

This was kind of an accident that I stumbled upon when making the 'Fabric' simulation. I had originally collapsed each click to a point. This caused constraint distance to go to 0, which probably caused force to overflow and give `console.log(hi)`.
