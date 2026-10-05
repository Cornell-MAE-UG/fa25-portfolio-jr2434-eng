---
layout: project
title: CUAUV Scylla Torpedo and Droppers
image: /assets/images/torps_1.png
---

## Project Overview

The previous torpedo and dropper design had a critical issue in the dropper system: it fit very tightly around the camshaft's main component. Because the torpedo mission is worth more in competition, the launcher was the primary design focus. The torpedoes were aligned with the submarine's forward-facing camera, while the droppers needed more accurate alignment using a downward-facing camera.

My redesign gives the torpedoes a straight line of fire aligned with the forward-facing camera and improves dropper aiming through a dedicated downward-facing camera.

## Torpedo Restraint Mechanism

The previous camshaft design used small cams to rotate the restrainer arms. This arrangement worked because the arms were oriented 90 degrees from the camshaft's length. To preserve the desired axial rotation while aiming the torpedoes straight ahead, I used a face cam at the end of the camshaft. The face cam actuates newly designed arms with a built-in 90-degree turn.

<!-- Add image 1: original restrainer arms. -->
<!-- Add image 2: redesigned restrainer arms and face cam. -->

## Camera Mount

The redesigned camshaft and restrainer arms left space for a downward-facing camera. Using the camera's specifications, I designed a mount to position it for accurate dropper aiming.

<!-- Add image 3: camera opening and mount. -->

## Enclosure Design

I designed a multi-part case to hold the restrainers in their ready position until the camshaft rotates. The bottom case provides the base for the camera, dropper, and restrainer mounts, which were all designed to interface with it.

<!-- Add image 4: bottom case. -->

The mid case supports the camshaft. Its cutaways make maintenance easier, while the surrounding structure shields the remaining sensitive arms from collisions during operation.

The top case bounds the mounts along Scylla's underbelly.

<!-- Add image 5: assembled case design. -->

## Actuation Sequences

Each step rotates from the mechanism's position at the end of the previous step.

### Torpedoes First

| Action | Camshaft rotation |
| --- | ---: |
| Torpedo 1 | -67.7 degrees |
| Torpedo 2 | -67.7 degrees |
| Dropper 1 | +203.1 degrees |
| Dropper 2 | +67.7 degrees |
| Reset | -135.4 degrees |

### Droppers First

| Action | Camshaft rotation |
| --- | ---: |
| Dropper 1 | +67.7 degrees |
| Dropper 2 | +67.7 degrees |
| Torpedo 1 | -203.1 degrees |
| Torpedo 2 | -67.7 degrees |
| Reset | +135.4 degrees |

<!-- Add image 6: full submarine CAD. -->