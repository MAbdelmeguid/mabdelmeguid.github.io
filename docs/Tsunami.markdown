---
layout: page
title: "Tsunamigensis"
permalink: /tsunami/
---

### Anatomy of Strike-slip Fault Tsunami Gensis
##### A. Elbanna, M. Abdelmeguid, X. Ma, F. Amlani, H.S. Bhat, C. Synolakis, A.J. Rosakis
<https://doi.org/10.31223/X57G72>

Even though a small fraction of all tsunamis studied thus far are believed to be triggered by strike-slip motion, the devastating humanitarian impact warrants further investigation into this particular mechanism for tsunamigenesis.

<video width="680" height="320" controls="controls">
  <source src="/assets/videos/Palu_Damage.mp4" type="video/mp4">
</video> 
<div style="text-align: center"><em>Example of the damage caused by an unexpected localized tsunami induced by the September 2018 Mw 7.5 Sulawesi earthquake that occurred on the Palu-Koro (P-K) strike-slip fault system (Courtesy of Prof. Synoloakis, USC).</em></div>
<p></p>

However, strike slip faults are usually under-rated for tsunami hazard, except possibly for potential tsunami generation by undersea landslides that may be triggered by the earthquake’s strong ground motion. In our recent paper we show that the omission of intrinsic hazard related to strike slip faulting may be dangerous, especially for faults traversing bays. 

Key?  **“Horizontal displacements”**. 

<div style="text-align: center"><img src="/assets/figures/gif3.gif" width="700" height="250" /></div>

#### So, what did we do?

We integrate models for earthquake rupture dynamics with models of tsunami generation and propagation. The three-dimensional time dependent vertical and horizontal ground motions from spontaneous dynamic rupture models are used to drive boundary motions in the tsunami model

In our analysis we opted for a more generic bathymetry to focus our attention on basic tsunami generation processes that would, otherwise, be obscured by more complex bathymetries. While the bay geometry is partially inspired by the geometry of the Palu Bay. We expect that our results are not per se location specific and applies to bays traversed by strike-slip faults in different geographic areas

<div style="text-align: center"><img src="/assets/figures/Fig9_1.png" width="500" height="200" /></div>
<div style="text-align: center"> <em>Bay bathymetry, with the various observation stations (OP)</em></div>
<p></p>

#### We used Pylith for the 3D rupture modeling.

![Earthquake](/assets/figures/Fig_1.png){:class="img-responsive"}
<div style="text-align: center"><em>Evolution of a supershear rupture on a right lateral strike-slip fault.</em></div>
<p></p>


On the fault plane, the rupture nucleates at depth within an overstressed region. It subsequently expands to reach the surface and propagates at supershear speeds after saturating the seismogenic zone.

<div style="text-align: center"><img src="/assets/figures/gif2.gif" width="600" height="200" /></div>
<p></p>

On the seafloor, shear shock wave fronts (Mach cones) emerge and sharpen, extending away from the fault with little attenuation, as the rupture continues to propagate. 
<div style="text-align: center"><img src="/assets/figures/gif4.gif" width="600" height="200" /></div>
<p></p>


#### We developed SWIM, within MOOSE
SWIM is an in-house implicit FE solver for the 2D nonlinear shallow water wave equation. We implement SWIM within Multiphysics Object Oriented Simulation Environment (MOOSE) from Idaho National Lab

<div style="text-align: center"><img src="/assets/figures/gif5.gif" width="600" height="200" /></div>
<p></p>
Studying the evolution of the tsunami reveals three distinct phases: (1) A dynamic instantaneous phase, (2) A co-seismic phase, and (3) A post-seismic phase.

<img src="/assets/figures/Picture11.png" width="500" height="500" />{: style="float: right"}
<p></p>


1. The instantaneous dynamic tsunami phase occurs on the scale of few seconds in which the water surface is directly and almost instantaneously drove by the coseismic motion of the sea floor, even at large distances from the fault line in the superstar case due to the shock waves.

2. The coseismic tsunami phase is initiated by the dynamic seafloor motion but propagate much slower than the dynamic one, due to the diminishing effect of time dependent sea floor motion as the rupture zips along the fault plane.


3. The post-seismic, tsunami is much slower and propagate on the scale of tens of seconds to several minutes. It is driven by gravity and is prone to reflection and refraction by the bay geometry.

<div style="text-align: center"><img src="/assets/figures/Picture12.png" width="450" height="450" /></div>
<p></p>

Strike slip faults generate vertical displacements, which are not negligible, especially in the supershear case, but they are also generally not large enough to generate a considerable tsunami. **The horizontal displacements, however, may be significant!  As the rupture propagates, it pushes and pulls the bathymetry on both sides leading to vertical rise and subsudence of the sea surface and water waves that can be substantially amplified by depth reduction.**   It is the focusing effect associated with strike slip faults and  the large horizontal displacements that can generate several meters high water waves. Furthermore, there is a fascinating reflection effect that occur at the apex of the bay and may contribute to further amplification.

<div style="text-align: center"><img src="/assets/figures/gif6.gif" width="500" height="250" /></div>
<div style="text-align: center"> <em>Role of horizontal displacement in generating surface waves.</em></div>
<p></p>

The strike-slip motion result in a lack of perfect asymmetry in which the particle velocity varies at the lateral sides of the bay. The lack of perfect antisymmetry is explained by the symmetric nature of the strike-normal seafloor horizontal displacement, whilst the other two components of seafloor displacement are antisymmetric. This is consistent with the field observations.
<div style="text-align: center"><img src="/assets/figures/Picture23.png" width="500" height="450" /></div>
<div style="text-align: center"> <em>Snapshots of the in-plane water particle velocity vectors.</em></div>
<p></p>

 __The details of rupture propagation matter.__ Supershear ruptures may be capable of generating larger tsunamis than sub-Rayleigh ruptures for the same rupture area and nucleation procedure. The scaling of the water level by average slip shows that difference in slip between supershear and sub-Rayleigh does not completely explain the difference in the changes in the water level profile as a function of time, nor the amplitude difference.

<div style="text-align: center"><img src="/assets/figures/Fig8_1.png" width="700" height="450" /></div>
<div style="text-align: center"> <em>Comparison between water level time histories corresponding to a supershear and a sub-Rayleigh ruptures traversing the same bay.</em></div>
<p></p>

Consideration of the vertical displacement only (case 2), or a flat ocean floor with constant depth (case 3), suggest that the tsunami generation potential is negligible. Accounting for the horizontal displacements with topography (case 1) lead to interesting wave patterns that may reach few meters high.
<div style="text-align: center"><img src="/assets/figures/Fig_6.png" alt="drawing" width="650" height="250" /></div>
<div style="text-align: center"><em>The effect of including the horizontal motion on a basin bathymetry for a bay traversed by a supershear rupture.</em></div>
<p></p>


### Acknowledgment

A.E. acknowledges support by the National Science Foundation (CAREER Award Number 1753249). and A.J.R. acknowledges support by the Caltech/MCE Big Ideas Fund (BIF), as well as the Caltech Terrestrial Hazard Observation and Reporting Center (THOR). This research is part of the Blue Waters sustained-petascale computing project, which is supported by the National Science Foundation (awards OCI-0725070 and ACI-1238993) the State of Illinois, and as of December, 2019, the National Geospatial-Intelligence Agency. Blue Waters is a joint effort of the University of Illinois at Urbana-Champaign and its National Center for Supercomputing Applications. H. S. B. would like to acknowledge ERC Consolidator Grant PERSISMO a#865411) for financial support. C.E.S thanks the National Science Foundation for Award Number 1906162, Field Survey of the 27 September 2018 Sulawesi Tsunami.
