---
layout: project
title: FSAE Air Intake Restrictor Analysis
description: Transonic flow and separation analysis of a converging-diverging Venturi restrictor.
gallery: false
image: /assets/images/restrictor-final.jpeg
---

The Air Intake Restrictor project is an engineering analysis task focused on designing and simulating a converging-diverging nozzle (Venturi tube) for Formula SAE applications. The primary goal is to limit engine power by choking airflow at a mandated 20mm throat while minimizing downstream pressure drop. My role involved modeling the geometry and conducting iterative CFD simulations to optimize fluid behavior.

## Project Overview

In competitive racing series, organizers mandate an intake restrictor to cap total engine mass flow rate. The engineering challenge is pulling air past this 20mm bottleneck with as little energy loss as possible. The project required creating a baseline CAD geometry and utilizing fluid dynamics tools to diagnose and correct flow separation, shock-induced stall, and adverse pressure gradients to maximize aerodynamic efficiency.

## Design Process

The initial baseline restrictor geometry was modeled in SolidWorks, featuring a 14° converging inlet and a highly sensitive 6° diverging diffuser. However, the first iteration lacked proper tangent fillets at the throat bottleneck. This sharp, sudden transition tripped the flow, leading to localized supersonic acceleration (Mach 1.46). A strong normal shock wave blasted the boundary layer off the wall, causing massive flow separation and destroying pressure recovery.

<figure style="text-align:center; margin-top:1rem;">
  <img src="{{ '/assets/images/bad-airflow-nofillet.jpg' | relative_url }}" alt="CFD plot showing shock-induced flow separation due to lack of fillets" style="max-width:100%;height:auto;" />
  <figcaption>Figure 1 - Initial 6° design showing shock-induced flow separation from sharp throat transitions.</figcaption>
</figure>

## Analysis and Simulation

To properly capture transonic phenomena, the internal fluid volume was extracted using Ansys SpaceClaim. Localized mesh refinement, including prism inflation layers, was applied to accurately resolve the near-wall boundary layer. A compressible 3D fluid flow simulation was configured in Ansys Fluent utilizing the k-omega SST turbulence model and Ideal Gas density settings. 

## Prototype and Testing

Virtual testing and iteration involved applying smooth tangent fillets to the throat and conducting multiple pressure boundary condition sweeps to locate the critical pressure ratio:
*   **Part-Throttle (-5000 Pa):** Resulted in perfectly attached, but entirely subsonic flow at 267 m/s.
*   **Near-Choke (-10000 Pa):** Accelerated the flow to the transonic boundary (331 m/s) with maintained symmetry.
*   **Optimized Choke (-12000 Pa):** Pushed the limits to find the exact pressure differential required for Mach 1.

<figure style="text-align:center; margin-top:1rem;">
  <img src="{{ '/assets/images/reiterated-sweep.jpg' | relative_url }}" alt="CFD plot showing optimized attached transonic flow" style="max-width:100%;height:auto;" />
  <figcaption>Figure 2 - Final 6° iteration achieving Mach 1 choke (354 m/s) with fully attached flow.</figcaption>
</figure>

## Results

The final 6° iteration successfully choked the flow at exactly Mach 1 (354 m/s) while keeping the boundary layer perfectly attached throughout the diffuser. To validate why this specific geometry is the standard, a final simulation tested a steeper 10° diverging diffuser. The 10° expansion forced aggressive supersonic acceleration (410 m/s), causing total boundary layer separation and a violent asymmetric stall driven by the Coanda effect.

<figure style="text-align:center; margin-top:1rem;">
  <img src="{{ '/assets/images/10-degree-fail.jpg' | relative_url }}" alt="CFD plot showing chaotic flow separation in a 10 degree diffuser" style="max-width:100%;height:auto;" />
  <figcaption>Figure 3 - 10° diffuser demonstrating massive flow separation and asymmetric stall.</figcaption>
</figure>

## Reflection and Next Steps

Comparing these results highlights the critical nature of diffuser geometry, proving definitively why the shallow 6° standard is necessary to maintain pressure recovery. This project provided valuable hands-on experience in diagnosing complex internal flows, tuning mesh inflation layers, and translating CFD data into actionable geometry adjustments. Future work could involve exporting these pressure profiles into Ansys Mechanical to analyze the structural stresses on potential 3D-printed restrictor prototypes.