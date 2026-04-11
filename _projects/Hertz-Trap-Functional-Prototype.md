---
layout: project
title: Hertz Trap Functional Prototype – Newton's Nightmares
description: Design Documentation and Physical Testing of the Hertz Trap SLF Zapper
image: /assets/images/HertzTrap_Functional_Prototype.png
---

[cite_start]Our team, Newton's Nightmares, has developed a functional prototype known as the Hertz Trap[cite: 1]. [cite_start]Our Hertz Trap device is designed to eliminate Spotted Lanternflies before they gain access to grapevines[cite: 63]. [cite_start] It achieves this by attracting the insects away from entering grapevines using 60Hz audio and then zapping them[cite: 63].

## Prototype Components and Assembly

[cite_start]To build the functional prototype, we sourced a variety of specific components to handle both the structural and electrical requirements[cite: 2]:

* [cite_start]**Structure:** We utilized an Upper Electrical Box and an Upper Lid sourced from RPL, alongside temporary legs from Amazon[cite: 2].
* [cite_start]**Zapper Mechanism:** The trap relies on Copper Mesh (McMaster Code: 9224T55) and a Shocker PCB from Amazon[cite: 2].
* [cite_start]**Electronics:** The system logic is managed by an Arduino Nano (McMaster Code: 1387N33), powered via a Battery Box (McMaster Code: 7712K317), and controlled with a Power Switch from Amazon[cite: 2]. * [cite_start]**Audio Attraction:** We integrated a Speaker and an Amplifier, both sourced from Amazon[cite: 2].

[cite_start]The physical assembly began with an empty upper electrical box[cite: 10]. [cite_start]We attached all the electrical components; they were temporarily taped in with the materials we had, but for the final version, they will be glued[cite: 11]. [cite_start]The top cover was then mounted with screws[cite: 12]. [cite_start]For the zapping mechanism, we applied the mesh to the middle mesh structure by weaving it through and hot gluing it[cite: 13]. [cite_start]For the final version, we will make this attachment more secure[cite: 14]. [cite_start]Finally, the temporary legs were attached to the electrical box with superglue[cite: 16].

## Design Validation Tests

To validate our geometry and material choices, we subjected the prototype to a series of physical tests.

### 1. Drop Test
[cite_start]This test evaluates the durability of the upper body of the Hertz Trap when dropped, focusing heavily on the strength of the material and the geometry of the electronics hub[cite: 18]. [cite_start]Because the major components are housed in this box, any failure to protect the electronics would compromise the entire prototype[cite: 19]. [cite_start]Our method involved dropping the trap, legs facing up, onto a grass surface[cite: 21]. [cite_start]We tested three heights: 1 ft, 2 ft, and 4 ft[cite: 22]. [cite_start]Since the legs attached are replaceable and not the final version, this test specifically focused on the stability and integrity of the upper box[cite: 22].

* [cite_start]**1 foot:** No damage was done to the box or the devices[cite: 24]. [cite_start]The prototype stayed in the same orientation as what we dropped it at, and we saw no change[cite: 25].
* [cite_start]**2 feet:** Again, there was no deformation to the device, though this time it fell over when hitting the ground[cite: 27]. [cite_start]There was still no visible damage, and all the devices were safe within the electrical box[cite: 28].
* [cite_start]**4 feet:** The box fell over, and the temporary legs we have were a bit unstable[cite: 29]. [cite_start]They moved quite a bit but didn't break off, and the electrical components were all still attached on the inside[cite: 30].

[cite_start]**Conclusion:** The upper box shows excellent durability at lower heights[cite: 32]. [cite_start]At 4 ft, the temporary legs exhibited instability, suggesting that the final legs should be reinforced to prevent potential breakage from higher drops or repeated impacts[cite: 32]. [cite_start]This directly informs the next prototype by emphasizing the need for stronger leg joints or additional corner reinforcement, which we plan to do[cite: 33].

### 2. Box Capacity and Electrical Component Fit
[cite_start]The purpose of this test is to determine if there is adequate space within the upper electrical box to house all the electronics we plan to install[cite: 35]. [cite_start]Since we do not know the exact electrical output or wiring needed to power our mesh correctly, we used estimates based on existing bug zappers and our planned sketches[cite: 36]. [cite_start]This tests our upgrade capabilities in case we need a bigger battery or another circuit board[cite: 37]. [cite_start]Good estimation and additional room can aid in the main function of our zapper, which is neutralizing SLFs[cite: 38]. [cite_start]We measured the approximate volume and dimensions of our current and planned components to visualize the available and needed space[cite: 39].

* [cite_start]**Results:** The volume of our box is 96 inches, but most of the components will be sitting in an area of 16 inches, with a 1.5-inch height[cite: 40]. [cite_start]Our components (the speaker, Arduino Nano, Zapper PCB board, and battery case) take up 10 inches area-wise and sit at various heights, all under 1.5 inches[cite: 41]. [cite_start]Therefore, we have more than enough room for everything in our upper electrical box[cite: 42].
* [cite_start]**Conclusion:** There is ample room for all current and planned electrical components[cite: 43]. [cite_start]This extra space allows for potential upgrades without redesigning the box, ensuring the next prototype can accommodate larger batteries, additional circuitry, or airflow improvements for heat management[cite: 44].

### 3. Strength and Sturdiness Tests
[cite_start]The purpose of this test is to determine the vertical loads that our zapper can withstand without breaking and/or buckling[cite: 46]. [cite_start] This is by far the most important test we can perform, as both the legs and the upper box's strength are tested[cite: 47]. [cite_start]These components need to remain static under large loads to simulate the weight imposed by farmers, machinery, and weather conditions[cite: 48]. [cite_start]This tests the geometry and materials chosen for our legs and upper electrical box, allowing us to decide on further upgrades needed[cite: 49]. 

[cite_start]We tested this by incrementally adding weights to the upper lid of the electrical box until the legs buckled, the lid broke, or the box tipped over[cite: 50]. [cite_start]Since we do not yet have our main Amazon legs, we simulated the test with temporary legs, which we expect to fail much more easily[cite: 52, 53].

* [cite_start]**Weight 1 (544g):** Stable[cite: 54].
* [cite_start]**Weight 2 (1095g):** Stable[cite: 56].
* [cite_start]**Weight 3 (1654g):** Stable[cite: 58].
* [cite_start]**Weight 4 (2195g):** The box started to tip over, with visible stress on the legs[cite: 59].

[cite_start]**Conclusion:** The prototype can support the weight of grapevine debris and small animals (typically 200-500 g) with a significant safety margin[cite: 60]. [cite_start]Because the temporary legs are weaker than the final design, it suggests the next prototype should include robust leg material and reinforced joints to handle higher loads and ensure long-term durability, which we plan on doing[cite: 61].
