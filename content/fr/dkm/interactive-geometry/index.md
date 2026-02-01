---
date: 2025-12-25
title: Géométrie interactive
---
Avec ce modèle, l'utilisateur construit des figures géométriques
interactives. Les figures obtenues se déforment ensuite à la souris.
En utilisant des scripts, nous créons une très grande variété de
figure, dont certaines très complexes lorsque des boucles ou la
récursivité sont mises en oeuvre.

![Géométrie Interactive](interactiveGeometry.png#center)


```st
| canvas r f u |

canvas := DrGeoSketch new axesOn scale: 500.
r := canvas float: 2 at: 0 @ -0.1 from: 0 to: 4 name: 'r' showValue: true.
f := [ :x | r value * x * (1 - x) ].
canvas ray: 0@0 to: 1@1.
canvas plot: f from: 0 to: 1.
u := canvas pointOnLine: (canvas segment: 0@0 to: 1@0) hide at: 0.2.

100 timesRepeat: [ | v |
	v := canvas	" v sequence term "
		point: [ :previous | previous point x @ (f value: previous point x) ] 
		parent: u.
	canvas segment: u to: v.
	u := canvas	" u is a point on the Ray (0,0) (1,1) " 
		point: [:previous | previous point y @ previous point y ]
		parent: v.
	v hide. u hide.
	canvas segment: u to: v.
	v := u]
```
