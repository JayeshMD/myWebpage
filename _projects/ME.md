---
layout: page
title: Study of 2D slot stabilized flame for unperturbed and perturbed equivalence ratio
description: ME Thesis
img: assets/img/projects/ME/20_Ph_0.png
importance: 0
category: work
author: Jayesh M. Dhadphale
related_publications: true
#giscus_comments: true
---

Flame speed is sensitive to both the strain rate and the curvature of the flame surface.
Slot-stabilized flames have curvature and strain rate variation along the flame surface.
Hence, we investigate the variation of the flame speed with these two parameters for a steady, unperturbed slot-stabilized flame.

Local quenching of reactions on the flame surface is a significant concern in lean combustion devices, directly related to the net heat release rate and the overall performance of the system.
A steady flammability limit-based extinction criterion is more restrictive and demands an unnecessarily high equivalence ratio {% cite SANKARAN200277 %}.
{% cite SANKARAN200277 %} have suggested the concept of dynamic flammability limit, to include the effect of flow time scale(strain rate) and equivalence
ratio perturbation on flammability limit.

{% cite BANSAL2007404 %} have extended the concept of dynamic flammability limit.
They have studied counterflow premixed flame configuration subjected to various strain rates and have successfully incorporated various time scales in combustion to make extinction criteria more generalized.
They also have proposed a Dynamic Flammability Limit Extension (DFLE) as a function of non-dimensional frequency ($\eta$).
{% cite BANSAL2007404 %}'s work is mainly focused on counterflow configuration.
Here, we study the applicability of this extinction criterion to a 2D slot-stabilized flame.

### Case setup

The fluid domain configuration is illustrated in the following figure, along with the initial conditions for various flow variables.
<div class="row">
    <div class="col-sm-5 mt-3 mt-md-0">
            {% include figure.liquid loading="eager" path="assets/img/projects/ME/Schematic.png" title="Schematic" class="img-fluid rounded z-depth-1"%}
    </div>
    <div class="col-sm-7 mt-3 mt-md-0">
        <div class="row">
            <div class="col-sm-4 mt-3 mt-md-0">
                    {% include figure.liquid loading="eager" path="assets/img/projects/ME/Initial_CH4.png" title="Initial_CH4.png" class="img-fluid rounded z-depth-1" %}
            </div>
            <div class="col-sm-4 mt-3 mt-md-0">
                    {% include figure.liquid loading="eager" path="assets/img/projects/ME/Initial_O2.png" title="Initial_O2.png" class="img-fluid rounded z-depth-1" %}
             </div>
        </div>    
        <div class="row">
            <div class="col-sm-4 mt-3 mt-md-0">
                    {% include figure.liquid loading="eager" path="assets/img/projects/ME/Initial_T.png.png" title="Initial_T.png" class="img-fluid rounded z-depth-1" %}
            </div>
            <div class="col-sm-4 mt-3 mt-md-0">
                    {% include figure.liquid loading="eager" path="assets/img/projects/ME/Initial_u.png" title="Initial_u.png" class="img-fluid rounded z-depth-1" %}
             </div>
        </div>    
    </div>
</div>

The no-slip boundary condition is applied at the wall, and the non-reflecting boundary condition is applied at the outlet.
The computational domain is decomposed onto a multiblock structured grid with 2.4 million grid points and 965 blocks.

### Steady state
The steady-state solution is obtained for an equivalence ratio of $\phi=0.6$.
Some of the steady-state flow variables are illustrated in the following figures.

<div class="row justify-content-center">
    <div class="col-sm-5 mt-3 mt-md-0">
            {% include figure.liquid loading="eager" path="assets/img/projects/ME/SS_TV.png" title="SS_TV.png" class="img-fluid rounded z-depth-1"%}
    </div>
</div>
<div class="caption">
    The velocity field is overlaid on the temperature field.
</div>

<div class="row">
    <div class="col-sm-6 mt-3 mt-md-0">
            {% include figure.liquid loading="eager" path="assets/img/projects/ME/SS_SL_C.png" title="Initial_T.png" class="img-fluid rounded z-depth-1" %}
    </div>  
    <div class="col-sm-5 mt-3 mt-md-0">
            {% include figure.liquid loading="eager" path="assets/img/projects/ME/SS_SL_K_Mod.png.png" title="Initial_CH4.png" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
   Flame speed $S_L$ as a function of curvature $C$ and strain rate $\kappa$ over the flame.
</div>

Analyzed the flame speed $S_L$, flame curvature $C$, and strain rate $\kappa$ at 350 K contour for steady state, i.e., without equivalence ratio perturbation.
<div class="row">
    <div class="col-sm-6 mt-3 mt-md-0">
            {% include figure.liquid loading="eager" path="assets/img/projects/ME/Markstein.png" title="Markstein.png" class="img-fluid rounded z-depth-1" %}
    </div>  
    <div class="col-sm-6 mt-3 mt-md-0">
            {% include figure.liquid loading="eager" path="assets/img/projects/ME/Markstein_comp.png" title="Markstein_comp.png" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
   The sensitivity of flame speed to strain rate, i.e., the Markstein length $L_u$, is shown in the left figure.
    In the right figure, $L_u$ is marked with a red asterisk and is close to the linearly extrapolated Markstein length.
</div>

Furthermore, we found that Markstein's length is in close agreement with the experimental study by {% cite VAREA2012577 %}, as shown in the above figure.

### Perturbed Cases

We study the behaviour of the flame under the equivalence ratio perturbation
and with three normalized perturbation amplitudes ϵ = 0.05, 0.2, 0.4.

<div class="row justify-content-center">
    <div class="col-sm-7 mt-3 mt-md-0">
        <div class="row">
            <div class="col-sm-6 mt-0 mt-md-0">
                <div class="caption" style="text-align:left"> (a)  </div>
                {% include figure.liquid loading="eager" path="assets/img/projects/ME/40_Ph_0.png" title="40_Ph_0.png" class="img-fluid rounded z-depth-1" %}        
            </div>
            <div class="col-sm-6 mt-0 mt-md-0">
                <div class="caption" style="text-align:left"> (b)  </div>
                {% include figure.liquid loading="eager" path="assets/img/projects/ME/40_Ph_90.png" title="40_Ph_90.pngg" class="img-fluid rounded z-depth-1" %}
             </div>
        </div>    
        <div class="row">
            <div class="col-sm-6 mt-3 mt-md-0">
                    <div class="caption" style="text-align:left"> (c)  </div>
                    {% include figure.liquid loading="eager" path="assets/img/projects/ME/40_Ph_180.png" title="40_Ph_180.png" class="img-fluid rounded z-depth-1" %}
            </div>
            <div class="col-sm-6 mt-3 mt-md-0">
                <div class="caption" style="text-align:left"> (d)  </div>
                    {% include figure.liquid loading="eager" path="assets/img/projects/ME/40_Ph_270.png" title="40_Ph_270.png" class="img-fluid rounded z-depth-1" %}
             </div>
        </div>    
    </div>
</div>
<div class="caption">
   Deviation of equivalance ratio $\phi$ from dynamic flammability limit $\phi_t$ i.e. ($\phi-\phi_t$), temperature(K), hear release rate contours and velocity vector field for different phase angles at inlet (a) $0^{\circ}$, (b) $90^{\circ}$, (c) $180^{\circ}$, (d) $270^{\circ}$ ($\bar{\phi}=0.6$, $\epsilon=0.4$, $f=60Hz$).
</div>

In the analysis for the perturbed case, each case is plotted with the normalized minimum equivalence ratio extension below the steady flammability limit and the normalized frequency to locate the case in either the flammable or non-flammable region.
The case with ϵ = 0.05 lies in the flammable region, where ϵ = 0.2 and 0.4 lie in the non-flammable region. But no extinction is found in any of the cases.
To understand this flame behavior, the combined effect of strain rate and curvature on the flammability limit needs to be considered, which can be explored as future work.

<p>&copy; {{ site.time | date: '%Y' }} {{ page.author}}. All rights reserved.</p>

<p style="font-size: 32px;">
    <a href="/assets/pdf/ME_thesis.pdf">ME Thesis </a><br>
    <a href="/assets/pdf/ME_thesis.pdf" target="_blank" rel="noopener noreferrer">
                <!-- <i class="fa-solid fa-file-pdf" style="font-size: 64px;"></i> -->
                <img src="/assets/img/projects/ME/ME_cover_page.png" alt="Italian Trulli" style="width:250px;height:350px;border-radius: 8px">
    </a>
</p>
<br><br>
  