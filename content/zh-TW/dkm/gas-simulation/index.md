---
date: 2025-12-22
title: 氣體模擬器
---
該模型允許定義一個矩形外殼以及任意數量的壁面和氬原子。該模型模擬了透過
漫反射與壁面相互作用的**理想氣體**，或者同時具有壁面相互作用和
Lennard-Jones 原子間勢能的**真實氣體**。

在模擬過程中，包括外殼在內的所有壁面的溫度設定值都可以透過滑鼠進行調節。
此外還提供任意數量的覆蓋矩形區域的溫度探頭。

![Gas Simulation](gas-simulation.png#center)


```st
GasSimulation new
   fenceOrigin: 0@0 corner: 300@200;
   addWallFrom: 100@0 to: 80@85;
   addWallFrom: 100@200 to: 80@105;
   addMolecules: 50
```
