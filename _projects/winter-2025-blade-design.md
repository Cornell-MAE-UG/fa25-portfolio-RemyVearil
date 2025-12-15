---
layout: project
title: Wind Turbine Blade Design
description: A modeling project for MAE 4272 (Fluids & Heat Transfer Lab). 
technologies: [MATLAB, BEM]
image: /assets/images/blade-design.png
---

## Project Overview
This project focused on the aerodynamic and structural design of a small-scale wind turbine blade optimized for operation in the Big Blue wind tunnel. The objective was to maximize power output at an ideal wind speed of 5.36 m/s, selected using a Weibull wind distribution, while satisfying strict experimental constraints including a 6-inch blade radius, fixed hub interface, constant-speed operation assumptions, and manufacturability via 3D printing. Blade Element Momentum (BEM) theory was used to generate a theoretically optimal blade geometry, enabling direct comparison between modeled and experimental performance.

## Design Process
Our team developed a MATLAB-based BEM model to determine the optimal spanwise chord and twist distributions using a NACA 4412 airfoil, selected for its high lift-to-drag ratio at low Reynolds numbers. The blade was designed to operate at a tip speed ratio of 7, producing a predicted power output of approximately 3.1 W at the design wind speed. Structural feasibility was assessed using beam-bending calculations derived from spanwise aerodynamic loads, which predicted a large safety factor prior to testing. A key design oversight—misinterpreting the 6-inch constraint to include the hub—ultimately resulted in a blade that was thinner and more flexible than intended, significantly impacting performance.

## Testing Summary
Experimental testing was conducted in the Big Blue wind tunnel using a torque-controlled magnetic particle brake, where brake torque was increased monotonically and the turbine was allowed to settle at its natural equilibrium RPM. Power was computed from measured torque and rotational speed across multiple wind speeds near the design point. The blade struggled to self-start due to insufficient low-speed torque and excessive flexibility, requiring manual spin-up at higher tunnel speeds. During testing, one blade failed catastrophically at the hub interface, limiting data collection to a small number of steady-state points. Measured power output peaked near 0.08 W, far below BEM predictions, highlighting the sensitivity of small-scale turbines to geometry, stiffness, and startup torque assumptions.

## My Contribution
I led the development of the Blade Element Momentum (BEM) MATLAB code used for blade geometry optimization, including the calculation of optimal spanwise chord and twist distributions, operating tip speed ratio, and predicted power and torque output. I also contributed to structural stress estimation, experimental planning, and post-test analysis, connecting discrepancies between modeled and experimental results to design assumptions and manufacturing constraints. This work emphasized the importance of integrating aerodynamic theory, structural feasibility, and experimental realities in small-scale wind turbine design.
