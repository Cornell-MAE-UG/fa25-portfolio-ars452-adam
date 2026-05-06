---
layout: project 
title: MAE 2250 SLF Removal Apparatus
description: Pre-Harvesting Apparatus (GUARD)
technologies: [CAD, Vertical Bandsaw, Drill, Saw, 3D Printing]
image: assets/images/GUARD.png

---

## Table of Contents
- [Client Pitch](#client-pitch)
- [Functional Prototype](#functional-prototype)
- [Client Report](#client-report)

---

## Introduction

Spotted lanternflies (SLF) infest grapevines, contaminating harvests and damaging vineyards that are critical to local economies in regions such as New York. Within this broader challenge, this work targets the specific, high-impact sub-problem of removal of SLF immediately prior to harvest, when insects attached to vines are likely to be collected with grape clusters and directly contaminate the product. This focus enables large short-term gains without requiring full population control.
At harvest, grapes are extremely delicate and easily damaged or dislodged, while SLF exhibit strong adhesion to surfaces, requiring substantial but carefully controlled force for removal. With chemical and biological methods still uncertain in their effectiveness and ability to scale, a kinetic alternative is necessary in the meanwhile. Our proposed solution integrates directly with existing harvesting equipment, avoids disruption to workflows or costly vineyard-wide deployment, scales easily, and targets the SLF population most immediately affecting yield. 


---

## Client Pitch

  **Team:** The Entomophiles
  
  **Clients:** Cornell CALS Extension/E&J Gallo Winery/National Grape  

---
   
  **Problem Statement:**
  Spotted lanternflies (SLF) infest grapevines, contaminating harvests. We aim to remove ~90% before harvest. Because grapes are fragile and SLF adhere strongly, removal requires substantial but carefully controlled force.
  
---

  **Impact:**
  This product will allow grape farmers to solve the issue of SLF within harvested crops, allowing for more loads to be accepted alongside large-scale removal operations.  

---

## Proposed direction: Pre-Harvest Processing

**What it is:** An apparatus that is mounted to the front of a harvester and removes the SLF before the harvesting begins. We will use water or air, and either flood or direct the fluid towards SLF.
 

**How it would be used:**

- Device mounts to the harvester and connects to water, air, and/or power.
- Apparatus dislodges SLF from vines immediately prior to harvest.
 

**Why it’s better than the status quo:**

- Addresses problem in short term regarding yield
- More adaptable to existing infrastructure  


**End-of-semester proof-of-concept:** A battery-powered miniature prototype will use air and/or water (directed or undirected) to remove simulated SLF (miniature suction cups) from a simulated or real grape vine, supplied by a water tank.

---

## Key risks/unknowns

- SLF removal may dislodge grapes or damage vines, reducing yield and future harvests; this can be tested using simulated SLF on real vines with fruit.
- Fluid use may oversaturate soil or contaminate crops; non-water chemicals could affect grape quality or food safety. We would use soil-safe fluids and minimize volume.

---

## Questions for the client

1. **How much water / air pressure is necessary to wash off SLF?** *Decision affected:* Determination of optimal force to apply. 
   

2. **What are the dimensions and physical limitations of the harvester?** *Decision affected:* Determination of apparatus size, fluid output, system complexity.


3. **Is a stable water supply available, and can the harvester power a compressor?** *Decision affected:* If not, air requires onboard compression and water requires onboard storage, increasing weight.


## Functional Prototype

### Design Sketch
<img src="../../assets/images/GUARD-Sketch.png" width=500px>

### Functionality Sketch
<img src="../../assets/images/Harvester pic.png" width=500px>

### Component List
![Component List]({{ "/assets/images/Bill of Materials.png" | relative_url }}){: .setup-image style="width: 500px"}


### Assembly Instructions

1. Assemble main frame  
   a. Fit metal rods into printed corner joints tightly. Orient 4 shorter rods vertically for balanced structure.  

2. Assemble pipe structure  
   a. Connect four T-connectors(horizontally) in a straight line with 1¾” pieces in between each connector and 1¾” pieces at the ends as well. Place an end cap on one end.  
   b. On each T- connector, connect the foot-long pvc pipes, with drilled holes alternating in offset. Place end caps at the end of each pipe.  
   c. Hose - Used 1” schedule 40 PVC to connect threaded barbed hose connectors to the ¾” PVC. We plan on using the other side of the hose to connect to our reservoir with a valve in the future. The hose was attached between these barbed connectors  
   d. Attach pipe structure to frame with zip-ties (temporary). Where necessary, tie two zip-ties together for increased length.  

---

### Design Test

Poured water into the hose of the prototype several times. Placed structure above two bins to collect water.  

- Visually inspected for unintended water leakages.  
- Part it’s testing: Testing security of connections, whether significant design changes are necessary for the parts conducting water.  
- Results: Noticed small dripping leakage at threaded connection between PVC pipe and barbed hose connector 
- Conclusion: Tapping the PVC pipe at the connection could reduce leakage.  

- Placed absorbent cloth in the bin under the prototype.  
- Part it’s testing: Whether the “checkerboard” distribution of holes and pipes is sufficient to ensure good saturation of the area within the frame.  
- Results: Cloth was fully soaked.  
- Conclusion: Good saturation is achieved. However, it may be a future consideration to implement nozzles or other to further improve saturated area and reduce damage to plants caused by a direct dripping flow.  

- Measured 1000mL of water, poured into the hose at a steady rate. Time to fully drain was recorded.  
- Part it’s testing: Hose and piping carrying water, and whether there are significant blockages.  
- Results: Expended 1000mL in 58.07 sec. 
- Conclusion: Water flows well. Existing connections and methods of processing piping are good in this regard.  

---

### Success Criteria

- 16 mL/sec water flow rate- expends the small scale jug in about 4 minutes. Sufficient water flow is important to knock SLF off, but excessive flow is harmful (can wash away grapes).  
- Goal achieved: Expends 1000mL in 58.07 sec, which is a flow rate of 17.2 mL/sec. Therefore, we know water flows efficiently through the piping. However, we believe that with improved nozzles, we can retain full saturation with less flow, thus increasing efficiency with respect to the amount of water consumed.  

- Minimal frame deflection when only supported from one end. A sturdy, stable structure is necessary for repeated use.  
- Goal achieved: Frame is sturdy and stands stable on the edges of a plastic bin.  

- Open center for grape vines to pass through, and water saturates at least 75% of the surface area directly below the frame (0.75 square feet) within 30 seconds. Water should be spread around evenly within the frame such that no areas potentially containing SLF are missed.  
- Goal achieved: Placed absorbent cloth in bin under the prototype to test the surface area that the water reaches; cloth was fully soaked.  

### Client Report


**1 Introduction**

Spotted lanternflies (SLF) infest grapevines, contaminating harvests and damaging vineyards that are critical to local economies in regions such as New York [1]. Within this broader challenge, this work targets the specific, high-impact sub-problem of removal of SLF immediately prior to harvest, when insects attached to vines are likely to be collected with grape clusters and directly contaminate the product. This focus enables large short-term gains without requiring full population control. At harvest, grapes are extremely delicate and easily damaged or dislodged, while SLF exhibit strong adhesion to surfaces [2], requiring substantial but carefully controlled force for removal. With chemical and biological methods still uncertain and difficult to scale, a kinetic alternative is necessary. The proposed solution Grapevine Unit for Arthropod Removal and Defense (GUARD) integrates directly with existing harvesting equipment, avoids disruption to workflows or costly vineyard-wide deployment, scales easily, and targets the SLF population most immediately affecting yield.


**2 Final Prototype and Application**

A front-mounted harvester spray attachment was built to wash spotted lanternflies (SLF) off grape vines immediately before harvest. Water is stored in a refillable tank mounted above the system, then flows through a controllable valve into a PVC pipe network. The pipes have evenly spaced holes arranged in a staggered (checkerboard) pattern to spread water uniformly while minimizing usage. The spray system is supported by a lightweight aluminum frame with rigid 3D-printed joints. Our device is designed to attach to the front of the harvester, extending above the vines below. Water showers onto the vines, penetrating the vines’ verdure and saturating any SLF that may be feasting on the plant. The water serves to encourage them to jump off the plant, or adsorb onto their wings such that they will fall to the ground. In its current form, our device requires a reliable water source, likely the already established irrigation system on the vineyards or a refillable water tank, and an attachment point to the front of the harvester. The controllable valve means that our device can accommodate the needs of different vineyards or grape plants without wasting resources or causing unnecessary damage. Its minimal design lends itself to infrequent and inexpensive maintenance. Our device is also singular in function, meaning that it does not require an extensive infrastructure of similar devices to perform optimally. As far as the client is concerned, this is an attachment for harvesters to immediately increase yield of harvests by removing SLF from the vines directly before harvester takes them.


**3 Conclusions and Recommendations**

Qualitatively, we believe are results are overall inconclusive. Due to time and resource limitations we were unable to implement a positive pressure system which is necessary to ”spray” water out of nozzles. Using gravity alone simply redirects the flow of water. Although our saturation test was successful, it only measured the saturation at the ground, and therefore is not the best representation of the plant saturation. The recommendation for further work is to implement directional nozzles in a positive pressure system to spray water more efficiently. It would also be beneficial to supplement the system with high pressure air blasts directed at the SLF, to knock off those that do not fall off from the water.


**4 Testing and Results**

1. <u>Objective:<u> Evaluate integrity and efficacy of water-carrying components.
- Success Criteria: Achieve steady flow rate of 17 mL/s with less than 5% water volume
lost to leakage.
- Observations: GUARD expended 1000mL in 58.1 sec (17 mL/s). Minimal dripping
leakages.
- Conclusions: Water flows well. Existing connections and methods of processing piping
are satisfactory in this regard. When fully implemented, expect to sustain fluid flow
during normal harvesting operations.

2. <u>Objective:<u> Evaluate whether “checkerboard” hole and pipe distribution enables full area
saturation.
- Success Criteria: Achieve saturation of 95% area within cage.
- Observations: Cloth was fully soaked within seconds after beginning operation.
- Conclusions: 100% area saturation was achieved. It may be a future consideration to
implement nozzles or other to further improve saturated area and reduce damage to
plants caused by a direct dripping flow. Final implementation may use more advanced
methods for ensuring fluid coverage of target area.

3. Objective: Evaluate structural integrity of cage.
- Success Criteria: less than 2 mm of deflection with only supported from one end
- Observations: The frame deflected 0.6 mm.
- Conclusions: The metal frame deflects within acceptable tolerances and is stable. Expect
to be able to scale up for final implementation while remaining relatively lightweight and
rigid.


**5 Rough Calculations for Scale**

For a typical harvester with an opening width of less than 1 m [3], we can presume that with a similar layout with a similar depth would have a flow rate of 3.3 times the current system, giving us a flow rate of 56.1 mL/s. With a 60 gallon tank, this would provide a runtime of 1.12 hours. If one was able to improve the flow rate efficiency by 9 times, this system would have a runtime of approximately 10 hours. This flow rate efficiency increase is feasible with much improved nozzle technology compared to the current “waterfall” approach. Therefore, we believe that our testing results show feasibility for continuous operations during harvesting if improved upon and designed at full scale.


**6 Prototype and Testing Details**

Our model has two main parts, the frame and the pipe structure, with the goal of keeping a straightforward and lightweight design. Our frame was built from 1⁄2” diameter steel rods cut into eight 12” pieces and four 11”pieces. We used 3D printed corner joints to connect the rods into a cubic structure with the 11” rods on the vertical. There were four 12” bars for the top of the cube, two 12” bars that were connected with another kind of joint 2” below the top of the cube and on opposite sides, and two on the bottom on the sides where the offset bars weren’t. The PVC pipe for the main pipe structure was 3⁄4 pipe size. We used two 4” pieces of scrap 1” schedule 40 PVC for the hose fittings. We cut four 13” pieces and five 7/4” pieces out of the 3⁄4 pipe size PVC. On each
13” piece we had two rows of holes. The rows were separated by a 1⁄2” and one row had holes drilled at every odd inch (1”, 3”, . . . , 11”) and the other row had holes on every even inch (2”, 4”, . . . , 10”). We then joined the 4 T-connectors in series using the 7/4” PVC pieces including both ends. We placed end caps on one end of the T-connector series and at all of the 13” pieces. We connected the 13” PVC pipes at the T-connectors, with the holes facing down. We then used a threaded 4” piece of 1” schedule 40 PVC to connect a threaded barbed hose connector to the 3⁄4 PVC at the end of the T-connector series. We used 3” of clear PVC soft tubing (1⁄2” inner diameter, 5 8 ” outer diameter) to connect the pipe structure to the gallon jug. We connected the jug to the valve with a machined metal nut. The valve was connected to another threaded 4” piece of 1” schedule 40 PVC and then another barbed hose fitting to connect with the clear tubing. We then secured the pipe structure to the top of the frame with 3D printed clips. We attached two sheets of clear PETG sheets to the sides that were parallel to the length of the PVC pipes with zip ties.

**6.1 Test Methodology Details**

Flow Rate Test: We filled a jug with 1000mL of water. Then, we opened the valve to a fixed position to ensure steady flow and recorded the time to fully drain. We made a visual inspection for any unintended water leakages. Surface Area Test: For our surface area coverage test, we placed an absorbent cloth under the system and timed and visually checked how long it took for the cloth to be saturated everywhere. Deflection Test: We held it securely from one end and placed 6 kg on the other end to test deflection. We fixed a meter stick to the original height to ensure we properly measured deflection.

