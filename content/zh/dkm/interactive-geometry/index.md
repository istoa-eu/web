---
date: 2025-12-25
title: 交互式几何
---

通过该模型，用户可以构建交互式几何图形。得到的图形随后可以用鼠标进行变
形。通过使用脚本，我们创建了种类繁多的图形，当应用循环或递归时，其中一
些图形会变得非常复杂。

*该 DKM 将由 [Dr. Geo](http://gnu.org/s/dr-geo) 改编而来，可作为 DKM
 模块和独立应用程序共同使用。*

![交互式几何](interactiveGeometry.png#center)

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
