---
title: "MuscleSync"
date: "2025-09-04"
---

# MuscleSync

For task specifications: [click here](./specs)

## Tasks I can complete

| Task | Estimated completion time |
| --------- | ------------------------- |
| Proof-of-concept protoboard | **October 1** |
| Pre-Kickstarter landing page | **1 week**, or as fast as **a few days** if given a Figma (or similar) design to implement in code. Domain name registration, hosting, and deployment included. |
| Algorithm – Real-time feedback | **3 weeks** (rough estimate; depending on specifications) |
| Algorithm – Post-measurement analysis | **3 weeks** (rough estimate; depending on specifications) |
| App development (Cloud + UX) | **4-8 weeks**, depending on scope, and choice of web app with integrated cloud vs native mobile app with separate cloud |
| Product website | **2-4 weeks**, depending on scope, unlikely to be more than **1-2 weeks** if given a design to implement in code. Domain name registration, hosting, and deployment included (free for a static site, a few EUR monthly if using a backend and database).  |
| Firmware (BLE, haptics) | **4 weeks** (rough estimate; depending on exact specifications; assuming available documentation and data sheets) |


## Payment/compensation

Assuming the Kickstarter campaign succeeds, I am available to work on the project full-time (e.g. cca 40 hours weekly, or by agreement).

I propose dividing compensation into two stages:

- **Pre-Kickstarter (protoboard + landing page):** one-time payment on the order of a few hundred EUR

- **Post-Kickstarter:** I propose two options:

  1. Either a stipend to cover a minimum wage (cca 1500 EUR bruto monthly-ish), plus equity...
  1. ...or a typical salary for an electronic engineer/programmer (by agreement with reference to [data from SiStat](https://pxweb.stat.si/SiStatData/pxweb/sl/Data/-/0711335S.PX/table/tableViewLayout2/) for e.g. `2152 Inženirji/inženirke elektronike`, `2512 Razvijalci/razvijalke programske opreme`, but e.g. 2500 - 3000 EUR bruto for reference)

Exact numbers of course subject to mutual agreement; these are as a rough reference.

Notes:

- I have a d.o.o. with which I can send formal invoices, so **there is a logistically straightforward way to pay me** (i.e. no need for *delo na črno*, no need to employ me via *pogodba o delovnem razmerju*, etc.)
- Payment does not have to be strictly a monthly salary — we can do payments on a contractual basis (e.g. XYZ EUR for completing milestone ABC)

## Specifications for each task

This is to provide clear specifications for each task I will perform, so we can hold my work accountable and evaluate if it met requirements.

### Proof-of-concept protoboard

Create a prototype that:

- Reads data live from MC sensor as user pedals on bicycle
- Processes the MC sensor signal in real time and categorizes the user's muscle output as below lower threshold (muscle output too low), in target range, or above upper threshold (muscle output too high)
- Has a feedback mode for each operating range:

  1. Intermittent *ping, ping, ping* when user's muscle output is in target range
  1. Warning buzz when muscle output falls below lower threshold (when user's muscle output is too low)
  1. Separate warning buzz when muscle output rises above upper threshold (when user's muscle output is too high)

- Has a physical form factor that allows wearing the device while pedalling a bicycle and that simultaneous supports vibration from the haptic motor without disturbing the reading of the muscle signal at the quadriceps with the MC sensor.
