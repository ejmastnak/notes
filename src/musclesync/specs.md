---
title: "MuscleSync Tasks"
date: "2025-09-04"
---

# MuscleSync: Specifications for each task

This is to provide clear specifications, in writing, for each task I will perform, so we can hold my work accountable and evaluate if it meets requirements.

## Proof-of-concept protoboard

Create a prototype that:

- Reads data from MC sensor as user pedals on bicycle
- Has a feedback mode for each operating range:

  1. Intermittent *ping, ping, ping* when user's muscle output is in target range
  1. Warning buzz when muscle output falls below lower threshold (when user's muscle output is too low)
  1. Separate warning buzz when muscle output rises above upper threshold (when user's muscle output is too high)

- Has a physical form factor that allows wearing the device while pedalling a bicycle and that simultaneous supports vibration from the haptic motor without disturbing the reading of the muscle signal at the quadriceps with the MC sensor.

- Responds to MC sensor signal in real time, categorizes the user's muscle output as below lower threshold (muscle output too low), in target range, or above upper threshold (muscle output too high), and gives corresponding feedback via haptic driver;
  *with the understanding that* the classification algorithm will be crude in this initial prototype stage, and that a robust classification algorithm that consistently classifies live muscle sensor input as below, in, or above threshold is a dedicated milestone to be developed in the post-Kickstarter phase and will require a large database of measurements from many test subjects to develop.
