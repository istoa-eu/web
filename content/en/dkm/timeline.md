---
date: 2025-12-22
title: Timeline
---
The model allows representing a timeline with an arbitrary number of
events. Each event includes a date and a description. A timeline with
very scattered events can be compressed using the ```shrink```
message.

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
