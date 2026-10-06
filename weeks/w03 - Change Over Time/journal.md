---
title: w03 - Change Over Time
date: 2026-09-14
week: 1
tags:
  - image
  - prompting
  - experiment
publish: true
---

## Notes

**Assignment: Design a Timepiece - a system that communicates time or the passage of time**

##### My idea 1: "Time is a loop that leaves traces"
- Pendulum that moves leaving ghost trails that pile up (could fade after some time)
- Type of movement: Swings left to right. slows down at those left-right extremities. The speed is not constant, but in a steady rhythm, in a cycle
  
Reference image:  https://ch.pinterest.com/pin/10133167907180632/ ![[Pasted image 20261006144851.png|300]]

How I would code this (conceptually):
Cycle: in a cycle, the system would return to where it started so A -> B ->A is a full cycle. A -> B is half a cycle
- left extremity, point A = -1 and right extremity, point B is 1, The middle = 0
- the pendulum moves back and forth on its own from -1 to 1, using sin()
Need:
Pivot point
Length from the pivot to the circle/pendulum
Angle (how far it is swung)
Pendulum/circle position
Time -> frameCount
A trail -> fading in the background or a limited array of past positions

Step 1 :
I made sure to understand how to apply sin() to my concept. I used AI(claude). After explaining my concept I prompted: - explain how I can apply sin() to form an arc and follow my concept.
-Claude answer:

**(WIP)**

## Reflection


