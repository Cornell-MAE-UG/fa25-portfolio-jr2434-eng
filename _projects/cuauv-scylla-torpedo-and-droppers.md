---
layout: project
title: CUAUV Scylla Torpedo and Droppers
image: /assets/images/torps_1.png
---

## Project Overview

During the development of Scylla, the Cornell University Autonomous Underwater Vehicle (CUAUV), the payload delivery system required a comprehensive mechanical overhaul to maximize competition scoring. The legacy design suffered from tight clearance issues around the primary camshaft, which introduced friction and jamming risks in the dropper deployment. Because the torpedo targets hold higher point values in competition, optimizing their launch trajectory was the primary design driver. 

While the primary torpedoes required strict, unobstructed alignment with the submarine's forward-facing camera, the secondary droppers relied on downward-facing optics for targeting. My redesign introduces a synchronized, dual-action mechanism that completely decouples these paths, providing the torpedoes with a true straight line of fire and integrating a dedicated, unobstructed downward vision system to optimize dropper deployment accuracy.

## Kinematic Restraint Mechanism

The legacy camshaft architecture utilized standard radial cams to actuate the restrainer arms, a configuration that forced the arms into an orthogonal orientation and compromised forward alignment. 

To achieve the necessary straight-ahead trajectory for the torpedoes while preserving the reliable, single-actuator axial rotation, I engineered a custom face cam at the distal end of the shaft. This novel face cam profile directly drives newly designed, monolithic restrainer arms featuring a built-in 90-degree geometric offset. This design allows the torpedoes to sit perfectly parallel to the longitudinal axis of the vehicle while maintaining a robust, bind-free mechanical release.

<!-- Add image 1: original restrainer arms. -->
<!-- Add image 2: redesigned restrainer arms and face cam. -->

## Integrated Vision System Packaging

Optimizing the internal volume around the redesigned camshaft and kinematic arms freed up crucial real estate within the payload bay. Leveraging this newly available envelope and the camera's precise focal specifications, I designed a rigid, low-vibration mounting bracket for the downward-facing camera. This ensures absolute optical alignment with the dropper release window for accurate targeting.

<!-- Add image 3: camera opening and mount. -->

## Structural Enclosure & DFM

To house the intricate mechanical linkages, I developed a modular, multi-part enclosure optimized for Design for Manufacturing (DFM) and rapid field maintenance. The system is held in a ready position until the camshaft initiates the drop sequence.

* **Base Chassis:** Acts as the foundational structural member, providing precision-aligned interfaces for the camera, droppers, and dynamic restrainer mounts. 
* **Mid-Frame:** Supports the primary camshaft and absorbs rotational loads. It features strategic cutaways to reduce weight and allow for rapid in-field servicing, while the external ribbing acts as a mechanical shield to protect the sensitive linkage arms from dynamic impacts or collisions during underwater operation.
* **Top Plate:** Bounds the mounts and provides a seamless, hydrodynamic mounting interface flush against Scylla's underbelly.

<!-- Add image 4: bottom case. -->
<!-- Add image 5: assembled case design. -->

## Deployment Kinematics

The payload system utilizes precisely timed cam profiles to execute distinct deployment sequences based on rotational degree steps. Each actuation phase rotates relative to the mechanism's position at the conclusion of the previous step.

### Primary Sequence: Torpedoes First

| Action Phase | Required Camshaft Rotation |
| :--- | ---: |
| **Fire Torpedo 1** | -67.7° |
| **Fire Torpedo 2** | -67.7° |
| **Deploy Dropper 1** | +203.1° |
| **Deploy Dropper 2** | +67.7° |
| **System Reset** | -135.4° |

### Alternate Sequence: Droppers First

| Action Phase | Required Camshaft Rotation |
| :--- | ---: |
| **Deploy Dropper 1** | +67.7° |
| **Deploy Dropper 2** | +67.7° |
| **Fire Torpedo 1** | -203.1° |
| **Fire Torpedo 2** | -67.7° |
| **System Reset** | +135.4° |

<!-- Add image 6: full submarine CAD. -->