---
date: 2025-12-22
title: 时间轴
source: 
status: "developed" # developed | project | progress | improvement
author: Hilaire Fernandes
version: "1.0"
apiVersion: "25.11"
cost: 1600
financed: 105
---
该模型允许表示包含任意数量事件的时间轴。每个事件包括日期和描述。对于事
件非常分散的时间轴，可以使用 ```shrink``` 消息进行压缩。

![Timeline](/dkm/timeline.png#center)


```st
Timeline title: 'Five Defining Moments of Alexander' ::
   addEvent: 'Tutelage by Aristotle. At age 13, he began three years of study under the most famous philosopher of the time.' on: '-343.1.1';
   addEvent: 'Accession to the Throne. His father, Philip II, was assassinated, making Alexander King of Macedon at age 20.' on: '-336.10.1';
   addEvent: 'Cutting the Gordian Knot. He symbolically became the destined ruler of Asia by violently "untying" the legendary knot.' on: '-333.5.1';
   addEvent: 'Victory at Gaugamela. His decisive military triumph over Darius III, effectively ending the Achaemenid Persian Empire.' on: '-331.10.1';
   addEvent: 'Death in Babylon. His sudden death at age 32, leaving no clear heir and causing his vast empire to fragment.' on: '-323.6.11';
   width: 2;
   color: Color yellow darker
```
