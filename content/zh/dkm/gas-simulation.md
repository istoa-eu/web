---
date: 2025-12-22
title: 气体模拟器
---
该模型允许定义一个矩形外壳以及任意数量的壁面和氩原子。该模型模拟了通过
漫反射与壁面相互作用的**理想气体**，或者同时具有壁面相互作用和
Lennard-Jones 原子间势能的**真实气体**。

在模拟过程中，包括外壳在内的所有壁面的温度设定值都可以通过鼠标进行调节。
此外还提供任意数量的覆盖矩形区域的温度探头。

![Gas Simulation](/dkm/gas-simulation.png#center)


```st
GasSimulation new
   fenceOrigin: 0@0 corner: 300@200;
   addWallFrom: 100@0 to: 80@85;
   addWallFrom: 100@200 to: 80@105;
   addMolecules: 50
```
