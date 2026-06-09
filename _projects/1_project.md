---
layout: page
title: Gravitational Spacetime in Triangular Merge
description: Discrete geometry, graviton charges, and simplicial decomposition of curved spacetime
img: assets/img/12.jpg
importance: 1
category: work
related_publications: true
---

The geometry of spacetime at its most fundamental level may not be smooth — it may be discrete, structured by elementary simplicial units that collectively reproduce the continuous curvature we observe at classical scales. This project investigates how triangular (simplicial) decomposition of spacetime can serve as a geometric framework for modeling gravitational interactions, with particular attention to the role of graviton and anti-graviton charges in mediating curvature.

The central question is whether spacetime curvature can be recovered from the deficit angles of a triangulated manifold, and whether graviton charge asymmetry at simplex boundaries contributes a measurable correction to the Einstein field equations in the discrete limit.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/1.jpg" title="Simplicial decomposition of a 2D curved surface" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/3.jpg" title="Deficit angle and curvature at a vertex" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/5.jpg" title="Triangulated spacetime lattice structure" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Left: a 2D curved surface approximated by flat triangular patches. Middle: curvature localized at a vertex as a deficit angle — the Regge calculus analog of the Riemann tensor. Right: a lattice triangulation of a compact spacetime region with periodic boundary conditions.
</div>

## Theoretical Framework

In Regge calculus {% cite regge1961general %}, a smooth Riemannian manifold is approximated by a piecewise-flat simplicial complex. Curvature is not distributed continuously but is concentrated at the *hinges* — codimension-2 faces of the triangulation. For a 4-dimensional spacetime, hinges are triangles (2-simplices), and the curvature contribution at each hinge is proportional to the deficit angle:

$$\epsilon_h = 2\pi - \sum_{\sigma \supset h} \theta_{\sigma,h}$$

where the sum runs over all 4-simplices sharing the hinge $$h$$, and $$\theta_{\sigma,h}$$ is the dihedral angle of simplex $$\sigma$$ at $$h$$. The Regge action then becomes:

$$S_{\text{Regge}} = \frac{1}{8\pi G} \sum_h A_h \, \epsilon_h$$

recovering the Einstein–Hilbert action in the continuum limit. This project extends this framework by introducing graviton and anti-graviton charge densities at each simplex boundary, treating them as discrete analogs of the stress-energy source terms in the full Einstein equations.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/5.jpg" title="Graviton charge distribution across simplex faces" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Schematic of graviton charge asymmetry across a shared simplex face. Net charge imbalance at the boundary drives a deficit angle correction beyond the classical Regge term.
</div>

The triangular merge operation refers to the controlled identification of adjacent simplices along shared faces, progressively coarse-graining the triangulation while tracking how deficit angles accumulate and whether graviton charge is conserved across the merge boundary. This is analogous to a renormalization group flow on the triangulated manifold — as the lattice spacing increases, the effective geometry must remain consistent with the original fine-grained curvature distribution.

Say you are merging two 4-simplices $$\sigma_1$$ and $$\sigma_2$$ across a shared tetrahedral face $$\tau$$. The merged simplex $$\sigma_{12}$$ must satisfy:

$$A_{\sigma_{12}} \cdot \epsilon_{\sigma_{12}} = A_{\sigma_1} \cdot \epsilon_{\sigma_1} + A_{\sigma_2} \cdot \epsilon_{\sigma_2} + \Delta_\tau$$

where $$\Delta_\tau$$ is the correction term arising from the eliminated internal hinge at $$\tau$$. The hypothesis being tested is that $$\Delta_\tau$$ is not zero in the presence of graviton charge asymmetry — meaning the merge operation is not curvature-neutral, and the coarse-grained spacetime carries a residual geometric correction.

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/6.jpg" title="Merge operation across shared tetrahedral face" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/11.jpg" title="Residual curvature after coarse-graining" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Left: the triangular merge operation across a shared tetrahedral face between two 4-simplices. Right: residual curvature distribution in the coarse-grained lattice after a sequence of merge operations, showing non-trivial accumulation near high-charge-asymmetry regions.
</div>

## Current Status and Open Questions

This project has been in active development since 2019 as an independent theoretical investigation. The current phase focuses on:

- Formalizing the graviton/anti-graviton charge density as a tensor field defined on the simplicial complex
- Deriving the correction term $$\Delta_\tau$$ analytically under a symmetric charge distribution assumption
- Testing whether repeated merge operations converge to a smooth manifold consistent with the Einstein equations, or produce a residual discrete structure at macroscopic scales

The deeper motivation is to determine whether discreteness of spacetime at the Planck scale leaves an observable signature in the gravitational sector — and whether the triangular merge framework offers a computationally tractable approach to probing this question without a full quantum gravity formalism.

{% raw %}
```html
<div class="row justify-content-sm-center">
  <div class="col-sm-8 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/6.jpg" title="Merge operation across shared tetrahedral face" class="img-fluid rounded z-depth-1" %}
  </div>
  <div class="col-sm-4 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/11.jpg" title="Residual curvature after coarse-graining" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
```
{% endraw %}
