---
date: 2025-12-22
title: Simulador de gas
---
El modelo permite definir un recinto rectangular y un número
arbitrario de paredes y átomos de argón. El modelo simula **gases
ideales** y una interacción con las paredes por reflexión difusa o
**gases reales** con tanto la interacción de las paredes como el
potencial interatómico de Lennard-Jones.

Durante la simulación, la consigna de temperatura de todas las
paredes, incluido el recinto, se ajusta con el ratón. También está
disponible un número arbitrario de sondas de temperatura que cubren
zonas rectangulares.

![Gas Simulation](/dkm/gas-simulation.png#center)


```st
GasSimulation new
   fenceOrigin: 0@0 corner: 300@200;
   addWallFrom: 100@0 to: 80@85;
   addWallFrom: 100@200 to: 80@105;
   addMolecules: 50
```
