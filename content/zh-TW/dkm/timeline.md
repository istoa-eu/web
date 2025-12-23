---
date: 2025-12-22
title: 時間軸
---
該模型允許表示包含任意數量事件的時間軸。每個事件包括日期和描述。對於事
件非常分散的時間軸，可以使用 ```shrink``` 訊息進行壓縮。

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
