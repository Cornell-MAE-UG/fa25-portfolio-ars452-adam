---
layout: project 
title: MAE 2250 SLF Removal Apparatus
description: Pre-Harvesting Apparatus
technologies: [CAD, Vertical Bandsaw, Drill, Saw, 3D Printing]
image:
---

# {{ page.title }}

<div class="journal-intro">
  <img src="{{ "/assets/images/2250drawing.png" | relative_url }}" class="side-image" alt="Design Sketch">

  ## Client Pitch
  **Team:** The Entomophiles
  **Client(s):** Cornell CALS Extension/E&J Gallo Winery/National Grape  
   
  ## Problem statement
  Spotted lanternflies (SLF) infest grapevines, contaminating harvests. We aim to remove ~90% before harvest. Because grapes are fragile and SLF adhere strongly, removal requires substantial but carefully controlled force.

  ## Impact
  This product will allow grape farmers to solve the issue of SLF within harvested crops, allowing for more loads to be accepted alongside large-scale removal operations.  
</div>

---

## Proposed direction(s): Pre-Harvest Processing

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
![Design Sketch]({{ "/assets/images/2250drawing.png" | relative_url }}){: .setup-image style="width: 500px"}

### Component List
![Component List]({{ "/assets/images/2250list.png" | relative_url }}){: .setup-image style="width: 500px"}


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
