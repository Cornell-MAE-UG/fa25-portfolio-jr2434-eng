---
layout: project
title: "Client Report: HertzTrap Project"
excerpt: "Final client report for the HertzTrap Spotted Lanternfly deterrent."
---

# ODP 6: Exhibit and Client Report

**Team:** T5 - Newton's Nightmares  
(James King, Junayed Ridwan, Kate Ainley-Zoll, Anya Besana, Sanithu Kethaka Parattu Mohottige)

## Problem Overview

During the pre-harvest grape season, vineyards across the Northeast face devastating losses from the Spotted Lanternfly (SLF). With no natural predators and ineffective conventional pest control, SLF populations continue to surge unchecked. These insects feed directly on grapevines, reducing yield and threatening plant health. The challenge is to intercept SLFs before they ever reach the vines, preserving crop quality and keeping farmers profitable.

## Sub-problem and Prototype Application

Our concept was to prevent SLFs from reaching the vines in the first place - rather than removing them after harvest, offering a more effective and scalable solution to protecting vineyard yield. To do this, we wanted to create a product that could passively kill the SLFs and draw them away from the vines before doing harm to the plant. We identified a critical weak point in the spotted lanternfly and exploited it by adapting the proven lure-and-kill method of UV bug traps to the USDA's discovery that these insects are uniquely drawn to 60 Hz frequencies. We called this product the Hertz Trap.

The HertzTrap is a self-contained electric insect trap that lures and eliminates SLFs before they reach the grapevines. By luring them toward this specific frequency, the trap brings them into contact with an electrified mesh that completes the circuit and neutralizes them instantly. Because it is compact and pesticide-free, it serves as a low-maintenance tool that can be easily deployed across large-scale vineyards without the need for manual insect removal.

## Prototype

The final HertzTrap prototype was built to validate the core concept at a functional scale. The enclosure houses a 60 Hz speaker at its center, surrounded by a dual-layer electrified mesh powered by a bug zapper circuit board. When SLFs are drawn toward the frequency stimulus, they make contact with the charged mesh, complete the circuit, and are eliminated. The four independently adjustable legs allow the trap to be staked and leveled at grapevine canopy height across uneven terrain. The enclosure was designed to be weatherproof and structurally rigid, withstanding up to 30 lbs of force without deformation. At just 8 lbs total, the final assembly is lightweight enough for rapid single-user deployment across large farm areas. Overall, the final prototype successfully integrates the electrical, acoustic, and structural subsystems into a compact, field-ready package.

## Testing and Results

Three key performance criteria were evaluated through physical testing of the prototype to ensure a successful product.

1. **Structural durability:** This was confirmed by applying incremental loads to the top of the enclosure; the trap withstood up to 40 lbs without deformation or failure, meeting the demands of outdoor farm use. We also dropped 5-10 lb weights from a foot high to replicate branches and falling situations.
2. **Adjustability:** This was verified by extending and locking each leg independently, confirming a maximum stable height of 3 feet suitable for placement near vine canopies. Individual legs were tested to support the trap at angles and rough areas.
3. **Portability:** This was tested by timing a single user relocating the trap across a simulated farm layout; the trap was consistently moved and reset in under 15 seconds, and at 6 lbs total weight, a single user could feasibly deploy over 100 units within a standard workday.

While these criteria confirmed the trap's physical viability, they did not address some more critical unknowns surrounding the trap's core function. In retrospect, more decision-relevant success criteria would have focused on biological performance: specifically, whether the mesh density and voltage are sufficient to reliably neutralize a Spotted Lanternfly upon contact, and whether the 60 Hz acoustic stimulus attracts SLFs at a meaningful range under field conditions. In order to simulate a branch falling onto the box, or a drop from a high height, we should have documented weights falling from a height rather than placing them directly on the box. Bench testing confirmed arc discharge across the mesh layers, providing a preliminary indication that the electrical system is functional, but controlled experiments with live insects at measured distances were not conducted. These tests - verifying kill reliability at the chosen mesh geometry and quantifying attraction range and capture rate in a vineyard environment - represent the most important next steps before the HertzTrap can be evaluated as an effective pest control solution.

## Prototype and Testing Details

The HertzTrap enclosure measures approximately 8 × 8 × 2 inches and was fabricated using 3D printing, chosen for its ability to produce a rigid, weatherproof housing at low cost with rapid iteration. The electrical system consists of a repurposed handheld bug zapper circuit board powered by two AA batteries, which steps up the input voltage to a level sufficient to arc across the mesh gap. In parallel with the trapping system, an acoustic subsystem was developed, consisting of a 57 mm diameter speaker driven by an amplifier and controlled by an Arduino Nano to generate a 60 Hz signal. The trap uses a dual-layer mesh configuration: a higher-density inner copper mesh and a lower-density outer metal mesh, with the two layers held at opposite polarities. When an insect bridges the gap between layers, it completes the circuit and is eliminated. The outer mesh has larger gaps so that the SLF can effectively bridge the two meshes. Successful arc discharge between the mesh layers was confirmed during bench testing, validating that the electrical system functions as intended at the chosen mesh spacing and density.

## Conclusion and Recommendations

The Hertz Trap offers significant scalability. Future iterations will integrate solar arrays atop the enclosure for continuous field operation, eliminating the need for manual recharging. Furthermore, optimizing mesh density specifically for Spotted Lanternfly geometry will ensure a more reliable circuit completion. These advancements aim to maximize capture rates and long-term durability in agricultural environments. The Hertz Trap is a promising solution to the continuous strain the SLFs put on the vineyard industry.

According to our clients, E&J Gallo Winery, they stated that another company they have been working with has provided a similar product, a form of "Bug Zapper" that can be placed around the vineyard and passively kills all of the SLFs. The Hertz Trap's next step in development would be to verify its efficiency, discovering its ideal frequency range and volume to attract the largest number of SLFs. Once that field experiment is concluded and the data drawn, the Hertz Trap will need to be optimized. The electrical components can be compacted into a custom circuit board, fueled by one rechargeable battery by the solar panels. Additionally, there would be a benefit for an additional low-density mesh on the outermost legs to ensure only the SLFs get in without debris accidentally activating the zap. Future iterations should also investigate selectivity, ensuring the trap does not harm beneficial insects, as well as long-term weatherproofing for extended outdoor operation.