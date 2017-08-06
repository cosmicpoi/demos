---
layout: default
title:  "Fabric?"
date:   2017-08-05 12:00:18 -0400
categories: demos canvas
src: "fabric-q.html"
---

This was kind of an accident that I stumbled upon when making the 'Fabric' simulation. I had originally collapsed each click to a point. This caused constraint distance to go to 0, which probably caused force to overflow and give `NaN`. Once one point has `NaN`, every other point with a force calculated from that point also becomes `NaN`, and so on until every point disappears. The static ones remain because they do not calculate forces. It's cool, so I kept it.
