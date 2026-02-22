---
fontsize: 11pt
geometry: margin=1in
papersize: letter
pagestyle: empty
header-includes:
  - \pagenumbering{gobble}
  - \usepackage{titlesec}
  - \titlespacing*{\section}{0pt}{0.6ex}{0.8ex}
  - \titlespacing*{\subsection}{0pt}{0.4ex}{0.6ex}
  - \setlength{\parskip}{0pt}
  - \setlength{\parindent}{0pt}
  - \renewcommand{\baselinestretch}{0.95}
  - \raggedbottom
---


# HertzTrap: Frequency-Based Spotted Lanternfly Deterrent

**Team:** Newton's Nightmares  
**Client(s):** Cornell CALS Extension / E\&J Gallo Winery / National Grape

## Problem statement

Farmers in vineyards are trying to continue growth and production of their vineyards. However, the growing population of Spotted Lanternflies (SLFs) puts significant pressure on farmers as these insects feed off grapevines, lowering yield and significantly damaging or killing the plants. The SLF is an exceptionally harmful pest because there are no natural predators and regular pest control does not work effectively. When harvesting, if more than 2 SLFs are found in a 1 kg sample of harvest, the entire section must be discarded per health code—a devastating loss for farmers already running on thin margins. Our team is aiming to take advantage of the SLF's documented attraction to 60 Hz frequencies and create a product that draws SLFs away from grapevines.

## Impact

SLF infestations prevent farms from passing health code inspections, forcing the discard of otherwise viable harvests. This directly threatens farm profitability and viability. A product that removes SLFs from grapevines before harvest can prevent yield loss, help farms meet health codes, and significantly increase both productivity and profit margins.

## Proposed direction(s)

### Concept A: HertzTrap

**What it is:** A modified electric insect trap designed to attract adult SLFs using a 60 Hz vibrational stimulus, based on published observations of SLF responsiveness to specific frequency cues.

**How it would be used:**
- Traps are installed along vineyard perimeters or near vine canopies before harvest
- Device emits 60 Hz stimulus to attract SLFs away from grape vines
- SLFs fly into an electrified grid and are neutralized before entering vineyard
- Device operates continuously during migration window

**Why it's better than the status quo:**
- Targets SLFs before they enter vineyards and have access to grapes
- Avoids pesticide application and associated labor
- Uses simple electrical components instead of a high-precision sorting system

**End-of-semester proof-of-concept:** We will develop a full CAD model with real-world dimensions and a scaled-down HertzTrap shell built to accurate proportions. The shell will include an internal slot and 60 Hz speaker, plus a PLA or ABS mesh outer layer to represent the electrically charged shock layer.

## Key risks / unknowns

- **Attraction Strength:** SLFs may not respond strongly enough to 60 Hz cues in open vineyard environments. We will test this through outdoor trials to validate effectiveness.
- **Nontarget Effects:** The trap may attract or harm beneficial insects. We will evaluate trap selectivity through observational testing.
- **Environmental Durability:** Outdoor weather and dust may reduce performance. We will evaluate possible materials, durability, and placement strategies.

## Questions

1. **What size trap would be most practical for your operations?** *Decision affected:* Sizing and the number of traps we recommend installing per acre.
2. **Will disposing of dead flies be an issue for your farms?** *Decision affected:* Whether we need to design the trap to minimize aftereffects or provide disposal guidance.
3. **Is harming non-SLF animals and pests of similar size/behavior a major environmental concern?** *Decision affected:* Whether we need to refine trap selectivity or if the current design approach is acceptable.


## References

- Wine Market Value - https://www.grandviewresearch.com/industry-analysis/us-wine-market 
- Spotted Lanternfly Information - https://cals.cornell.edu/integrated-pest-management/outreach-education/whats-bugging-you/spotted-lanternfly/spotted-lanternfly-damage
- 60 Hz Research - https://www.usda.gov/about-usda/news/blog/spotted-lanternfly-reveals-potential-weakness 


## Figure

<div style="text-align:center">
<img src="{{ '/assets/images/HertzTrap_Figure.png' | relative_url }}" alt="HertzTrap schematic" style="max-width:80%;height:auto;" />
</div>
