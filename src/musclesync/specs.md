---
title: "MuscleSync Tasks"
date: "2025-09-04"
---

# MuscleSync: Specifications for each task

This is to provide clear specifications, in writing, for each task I will perform, so we can hold my work accountable and evaluate if it meets requirements.

## Proof-of-concept protoboard

Create a prototype that:

- Reads data from force sensor in real time as user pedals on bicycle
- Has an initial calibration period that analyzes user's max output over an e.g. 10 second period and computes upper and lower thresholds customized to that user.
- After calibration, goes into feedback mode, continuously monitoring user's output and periodically notifying user via haptic motor where their current output falls relative to upper and lower thresholds:

  1. Warning buzz when muscle output falls below lower threshold (when user's output is too low)
  1. Separate warning buzz when output rises above upper threshold (when user's muscle output is too high)
  1. Optionally: an intermittent *ping, ping, ping* when user's output is in target range

- Allows testing the device while actually pedalling on a bicycle
- Ensures (via filtering, noise cancellation etc.) that vibration from the haptic motor will not disturb the reading of the muscle signal at the quadriceps with the force sensor.

- Has a muscle-output-classification algorithm that works in real time an is efficient enough to run on a small microcontroller, *with the understanding that* the classification algorithm will be crude in this initial prototype stage, and that a robust classification algorithm that consistently classifies live muscle sensor input as below, in, or above threshold is a dedicated milestone to be developed in the post-Kickstarter phase and will require a large database of measurements from many test subjects to develop; and also that accurate and sensitive reading of muscle output is conditional on buying/acquiring a force sensor designed to respond quickly to small (e.g. 0-10 newton) loads.
