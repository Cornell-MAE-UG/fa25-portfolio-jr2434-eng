---
layout: project
title: Hertz Trap Functional Prototype – Newton's Nightmares
description: Design Documentation and Physical Testing of the Hertz Trap SLF Zapper
image: /assets/images/HertzTrap_Functional_Prototype.png
---

Our team, Newton's Nightmares, has developed a functional prototype known as the Hertz Trap. Our Hertz Trap device is designed to eliminate Spotted Lanternflies before they gain access to grapevines.  It achieves this by attracting the insects away from entering grapevines using 60Hz audio and then zapping them.

## Prototype Components and Assembly

To build the functional prototype, we sourced a variety of specific components to handle both the structural and electrical requirements:

* **Structure:** We utilized an Upper Electrical Box and an Upper Lid sourced from RPL, alongside temporary legs from Amazon.
* **Zapper Mechanism:** The trap relies on Copper Mesh (McMaster Code: 9224T55) and a Shocker PCB from Amazon.
* **Electronics:** The system logic is managed by an Arduino Nano (McMaster Code: 1387N33), powered via a Battery Box (McMaster Code: 7712K317), and controlled with a Power Switch from Amazon. * **Audio Attraction:** We integrated a Speaker and an Amplifier, both sourced from Amazon.

The physical assembly began with an empty upper electrical box. We attached all the electrical components; they were temporarily taped in with the materials we had, but for the final version, they will be glued. The top cover was then mounted with screws. For the zapping mechanism, we applied the mesh to the middle mesh structure by weaving it through and hot gluing it. For the final version, we will make this attachment more secure. Finally, the temporary legs were attached to the electrical box with superglue.

## Design Validation Tests

To validate our geometry and material choices, we subjected the prototype to a series of physical tests.

### 1. Drop Test
This test evaluates the durability of the upper body of the Hertz Trap when dropped, focusing heavily on the strength of the material and the geometry of the electronics hub. Because the major components are housed in this box, any failure to protect the electronics would compromise the entire prototype. Our method involved dropping the trap, legs facing up, onto a grass surface. We tested three heights: 1 ft, 2 ft, and 4 ft. Since the legs attached are replaceable and not the final version, this test specifically focused on the stability and integrity of the upper box.

* **1 foot:** No damage was done to the box or the devices. The prototype stayed in the same orientation as what we dropped it at, and we saw no change.
* **2 feet:** Again, there was no deformation to the device, though this time it fell over when hitting the ground. There was still no visible damage, and all the devices were safe within the electrical box.
* **4 feet:** The box fell over, and the temporary legs we have were a bit unstable. They moved quite a bit but didn't break off, and the electrical components were all still attached on the inside.

**Conclusion:** The upper box shows excellent durability at lower heights. At 4 ft, the temporary legs exhibited instability, suggesting that the final legs should be reinforced to prevent potential breakage from higher drops or repeated impacts. This directly informs the next prototype by emphasizing the need for stronger leg joints or additional corner reinforcement, which we plan to do.

### 2. Box Capacity and Electrical Component Fit
The purpose of this test is to determine if there is adequate space within the upper electrical box to house all the electronics we plan to install. Since we do not know the exact electrical output or wiring needed to power our mesh correctly, we used estimates based on existing bug zappers and our planned sketches. This tests our upgrade capabilities in case we need a bigger battery or another circuit board. Good estimation and additional room can aid in the main function of our zapper, which is neutralizing SLFs. We measured the approximate volume and dimensions of our current and planned components to visualize the available and needed space.

* **Results:** The volume of our box is 96 inches, but most of the components will be sitting in an area of 16 inches, with a 1.5-inch height. Our components (the speaker, Arduino Nano, Zapper PCB board, and battery case) take up 10 inches area-wise and sit at various heights, all under 1.5 inches. Therefore, we have more than enough room for everything in our upper electrical box.
* **Conclusion:** There is ample room for all current and planned electrical components. This extra space allows for potential upgrades without redesigning the box, ensuring the next prototype can accommodate larger batteries, additional circuitry, or airflow improvements for heat management.

### 3. Strength and Sturdiness Tests
The purpose of this test is to determine the vertical loads that our zapper can withstand without breaking and/or buckling.  This is by far the most important test we can perform, as both the legs and the upper box's strength are tested. These components need to remain static under large loads to simulate the weight imposed by farmers, machinery, and weather conditions. This tests the geometry and materials chosen for our legs and upper electrical box, allowing us to decide on further upgrades needed. 

We tested this by incrementally adding weights to the upper lid of the electrical box until the legs buckled, the lid broke, or the box tipped over. Since we do not yet have our main Amazon legs, we simulated the test with temporary legs, which we expect to fail much more easily[cite: 52, 53].

* **Weight 1 (544g):** Stable.
* **Weight 2 (1095g):** Stable.
* **Weight 3 (1654g):** Stable.
* **Weight 4 (2195g):** The box started to tip over, with visible stress on the legs.

**Conclusion:** The prototype can support the weight of grapevine debris and small animals (typically 200-500 g) with a significant safety margin. Because the temporary legs are weaker than the final design, it suggests the next prototype should include robust leg material and reinforced joints to handle higher loads and ensure long-term durability, which we plan on doing.

