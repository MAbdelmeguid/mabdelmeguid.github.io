---
layout: page
title: "Tsunami-gensis"
permalink: /tsunami/
---

### Anatomy of Strike-slip Fault Tsunami-gensis

Strike slip faults are usually under-rated for tsunami hazard (except with landslides). We show this omission may be dangerous, especially for faults traversing bays. Key? "Horizontal displacements". So, what did we do? 

We integrate models for earthquake rupture dynamics with models of tsunami generation and propagation. The three dimensional time dependent vertical and horizontal ground motions from spontaneous dynamic rupture models are used to drive boundary motions in the tsunami model

To neutralize the effects of complex fault geometry or complex bathymetry we simulated a planar fault in a bay with a bath tub like geometry

#### We used Pylith for the 3D rupture modeling.
![Earthquake](/assets/figures/Fig_1.png){:class="img-responsive"}

On the fault plane, the rupture nucleates at depth within an overstressed region. It subsequently expands to reach the surface and propagates at supershear speeds after saturating the seismogenic zone.

<video width="680" height="320" controls="controls">
  <source src="/assets/videos/FaultAmp2-1.mp4" type="video/mp4">
</video> 

On the seafloor, shear shock wave fronts (Mach cones) emerge and sharpen, extending away from the fault with little attenuation, as the rupture continues to propagate. 
<video width="680" height="320" controls="controls">
  <source src="/assets/videos/FaultAmp4.mp4" type="video/mp4">
</video>  

#### We developed SWIM, within MOOSE
an in-house implicit FE solver for the 2D nonlinear shallow water wave equation.

<video width="680" height="220" controls="controls">
  <source src="/assets/videos/Media1.mp4" type="video/mp4">
</video> 

Studying the evolution of the tsunami reveals three distinct phases: (1) A dynamic instantaneous phase, (2) A co-seismic phase, and (3) A post-seismic phase.

1. The instantaneous dynamic tsunami phase occurs on the scale of few seconds in which the water surface is directly and almost instateneously drove by the coseismic motion of the sea floor, even at large distances from the fault line in the superstar case due to the shock waves.

2. The coseismic tsunami phase is initiated by the dynamic seafloor motion but propagate much slower than the dynamic one, due to the diminishing effect of time dependent sea floor motion as the rupture zips along the fault plane.

3. The post-seismic, tsunami is much slower and propagate on the scale of tens of seconds to several minutes. It is driven by gravity and is prone to reflection and refraction by the bay geometry.



<img src="/assets/figures/Fig_7.png" alt="drawing" width="400" height="420" />{: style="float: right"}

Strike slip faults generate vertical displacements, which are not negligible, especially in the supershear case, but they are also generally not large enough to generate a considerable tsunami. The horizontal displacements, however, may be significant! As the rupture propagates, it pushes and pulls the bathymetry on both sides leading to vertical rise and subsudence of the sea surface and water waves that can be substantially amplified by depth reduction. It is the focusing effect associated with strike slip faults and  the large horizontal displacements that can generate several meters high water waves. Furthermore, there is a fascinating reflection effect that occur at the apex of the bay and may contribute to further amplification.



 __The details of rupture propagation matter.__ Supershear ruptures may be capable of generating larger tsunamis than sub-Rayleigh ruptures for the same rupture area and nucleation procedure.

<div style="text-align: center"><img src="/assets/figures/Fig8.png" width="500" height="500" /></div>



Consideration of the vertical displacement only, or a flat ocean floor with constant depth, suggest that the tsunami generation potential is negligible. Accounting for the horizontal displacements with topography lead to interesting wave patterns that may reach few meters high.
<div style="text-align: center"><img src="/assets/figures/Fig_6.png" alt="drawing" width="650" height="250" /></div>
