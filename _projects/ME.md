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

Flame speed is sensitive to strain rate and curvature of the flame surface.
Slot stabilized flame have curvature and strain rate variation along the flame surface.
Hence we study the variation of the flame speed with this two parameters for steady unperturbed slot stabilized flame.

Local quenching of reactions on the flame surface is of serious concern in lean combustion devices which is directly related to net heat release rate and performance of the system.
Steady flammability limit based extinction criterion has found to be more restrictive and demands unnecessary high equivalence ratio {% cite SANKARAN200277 %}.
{% cite SANKARAN200277 %} have suggested the concept of dynamic flammability limit, so as to include effect of flow time scale(strain rate) and equivalence
ratio perturbation on flammability limit.

{% cite BANSAL2007404 %} have extended the concept of dynamic flammability limit. They
have studied counter-flow premixed flame configuration subjected to various strain rates and has successfully incorporated various time scales in combustion to make extinction criteria more generalized.
They also have proposed a Dynamic Flammability Limit Extension (DFLE) as a function of non-dimensional frequency (η).
{% cite BANSAL2007404 %} work is mainly focused on counter flow configuration.
Here, we study applicability of this extinction criteron to 2D slot stabilized flame.

### Case setup

The fluid domain configuration is shown in the following figure with initial condition for various flow variables.
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

The no-slip boundary condition is applied at the wall and non-reflecting boundary condition is applied at the outlet.
The computational domain is decomposed onto multiblock structured grid with 2.4 million grid points and 965 blocks.

### Steady state
The steady state solution is obtain for equivalance ration of $\phi=0.6$.
Some of the flow varibales at steady state are shown in the following figures.

<div class="row justify-content-center">
    <div class="col-sm-5 mt-3 mt-md-0">
            {% include figure.liquid loading="eager" path="assets/img/projects/ME/SS_TV.png" title="SS_TV.png" class="img-fluid rounded z-depth-1"%}
    </div>
</div>
<div class="caption">
    Velocity field overlapped over themperature field.
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

Analyzed the flame speed $S_L$, flame curvature $C$, and strain rate $\kappa$ at 350 K contour for steady state i.e. without equivalence ratio perturbation.
<div class="row">
    <div class="col-sm-6 mt-3 mt-md-0">
            {% include figure.liquid loading="eager" path="assets/img/projects/ME/Markstein.png" title="Markstein.png" class="img-fluid rounded z-depth-1" %}
    </div>  
    <div class="col-sm-6 mt-3 mt-md-0">
            {% include figure.liquid loading="eager" path="assets/img/projects/ME/Markstein_comp.png" title="Markstein_comp.png" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
   Sensitivity of flame speed to strain rate is the Markstein length $L_u$ is showed in the left plot and $L_u$ is marked in the right plot which close to linearly extrapolated Markstein length.
</div>

Further we found the Markstein's length is in close agreement with the experimental study by {% cite VAREA2012577 %} as shown in the above figure.

### Perturbed Cases

We study the behaviour of the flmae under the equivalence ratio perturbation
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
   Deviation of equivalance ratio $\phi$ from dynamic flammability limit $\phi_t$ i.e. ($\phi-\phi_t$), temperature(K), hear release rate contours and velocity vector field for different phase angles at inlet (a) $0^{\circ}$, (b) $90^{\circ}$, (c) $180^{\circ}$, (d) $270^{\circ}$ ($\bar{\phi}=0.6$, $\epsilon=0.4$, $f=60Hz$)
</div>

In analysis for perturbed case, each case is plotted with normalized minimum equivalence ratio extension below steady flammability limit and normalized frequency, to locate case either in flammable or non-flammable region.
Case with ϵ = 0.05 lie in flammable region where ϵ = 0.2 and 0.4 lies in non-flammable region. But, no extinction is found out in any of the cases.
In order to understand this flame behaviour, combined effect of strain rate and curvature on flammability limit needs to be considered which can be taken as future work.

<p>&copy; {{ site.time | date: '%Y' }} {{ page.author}}. All rights reserved.</p>

<p style="font-size: 32px;">
    <a href="/assets/pdf/ME_thesis.pdf">ME Thesis </a><br>
    <a href="/assets/pdf/ME_thesis.pdf" target="_blank" rel="noopener noreferrer">
                <!-- <i class="fa-solid fa-file-pdf" style="font-size: 64px;"></i> -->
                <img src="/assets/img/projects/ME/ME_cover_page.png" alt="Italian Trulli" style="width:250px;height:350px;border-radius: 8px">
    </a>
</p>
<br><br>
  