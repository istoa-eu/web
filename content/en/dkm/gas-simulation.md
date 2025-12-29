---
date: 2025-12-22
title: Gas Simulator
---
The model allows defining a rectangular enclosure and an arbitrary
number of walls and argon atoms. The model simulates **ideal gases**
and an interaction with the walls by diffuse reflection or **real
gases** with both the wall interaction and the Lennard-Jones
inter-atomic potential.

During the simulation, the temperature setpoint of all walls,
including the enclosure, is adjusted with the mouse. An arbitrary
number of temperature probes covering rectangular areas is also
available.

![Gas Simulation](gas-simulation.png#center)


```st
GasSimulation new
   fenceOrigin: 0@0 corner: 300@200;
   addWallFrom: 100@0 to: 80@85;
   addWallFrom: 100@200 to: 80@105;
   addMolecules: 50
