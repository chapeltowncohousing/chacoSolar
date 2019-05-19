Chaco PV overview document
================

<!-- README.md is generated from README.Rmd. Please edit that file -->
Introduction
============

Sustainability is one of Chaco's core values. With ample south-facing roofspace it makes sense to put up solar panels. It's much more economical to install PV at build time rather than retrofitting panels, so it makes sense to plan a PV installation into Chaco's design at the earliest possible stage.

The south-facing roof-space available to Chaco is illustrated below:

<img src="sitemap-aerial.png" width="942" />

How much PV is possible?
========================

Based on architectural drawings, the south facing roofspace available was estimated. The first stage was to digitise the pdfs into simple block representations of the buildings and highlight south-facing roofs, as illustrated in the figure below.

This was georectified and digitised in QGIS, resulting in the following data, which has been made available as open data, and can be view in an interactive map [here](http://rpubs.com/RobinLovelace/497201):

![](README_files/figure-markdown_github/unnamed-chunk-4-1.png)

The total maximum area available, for the terrace, common house, the shed (the least certain of the roofs for panels) and the total roof area, respectively, was calculated as follows:

    #> Units: [m^2]
    #> [1] 390  87  31
    #> 507.1894 [m^2]

Of course, these values cannot be achieved in practice: the entire 390 m<sup>2</sup> of space available on the terrace roof, for example, cannot be entirely overtaken by panels!

The initial spec document[1] included provision for 127 1600x980mm panels as follow:

-   14 \* 6 panel installations on the 14 unshaded roofs of the terrace
-   4 \* 4 panel installations on the remaining 4 'type C' terrace roofs that will receive some shading
-   27 panels on the common house

Assuming a per panel output of 270 W, this would mean Chaco could generate 34 KWp in full sunshine.

We assume the panels will be slightly larger: 1650x991mm (Manni et al. 2017). Given that the roof has an elevation of 35 degrees, such panels would have a horizontal footprint of 1619x991mm. In the original scenario, they would cover 204 m<sup>2</sup>, less than half of the total available space under optimistic assumptions.

The assumption about panel size, plus use of digitising tools in QGIS, allows the panel location to envisioned. The figure below shows two ways of aligning the panels: stacked as portrait or landscape. The portrait way is a squeeze: the roof is just over 3.3 m long in the horizontal access; two panels stacked in portrait formation are just over 3.2 m, leaving only a few cm clearance, which may be insufficient.

<img src="closeup3.png" alt="Portrait and landscape stacking. The two panels on the bottom left show the impact of the panels being at 35 degrees in each alignment: relatively minor." width="743" />
<p class="caption">
Portrait and landscape stacking. The two panels on the bottom left show the impact of the panels being at 35 degrees in each alignment: relatively minor.
</p>

The landscape stacking style leaves more room all round and 3 panels every ~2m.

The straight sections of the east and west wings are 41 m, leaving room for 24 sets of three on each, 120 panels in total. The south facing roofs on the curve are around 6.7 m at the smallest point, suggesting that there is enough room for 9 panels each (36 in total, as there are 4 curved roof sections). These calculations suggest there is enough room for 156 panels on the terrace, not accounting for the complicating factors of shaded panels (see the darker red areas in the figure above) or the slightly larger roof space on 4 of the houses.

The south facing roof on the common house is ~17.5 m long and just over 5 m wide. It may be possible to fit three panels in portrait formation on the common house roof, allowing 3 \* 16 = 48 panels on the common house roof. However, 30 panels in 2 by 15 formation would leave more room, and we will assume this number (30 panels) will be installed on the common house roof henceforth.

As a sanity check, a rough sketch respresenting this many panels on Chaco is provided below.

<img src="panels-draw.png" width="1188" />

Note that in the sketch the panels are packed tightly from the bottom to the top of the roof across the terrace. The 60 East wing panels are also packed tightly in the along the width of the roof. This is not realistic, especially in the shaded section. The West wing shows panels arranged in groups of 12. This is also not realistic. PV installers should design better, and much more accurate panel layout plans.

**Overall, simplistic calculations based on optimistic assumptions about stacking and shading suggest that Chaco could have room for 186 panels (50 KWp assuming no shading of 270 W modules).** This calculation ignores many things, including complicating factors around the interfaces between roofs of different heights in the terrace, assumes that panels are packed tight on the terrace house roof and that panels go on the curved roof. So far it ignores the shed, which could fit around 12 (4x3) extra panels, and could be a place to extend the PV capacity of Chaco in the future, perhaps linked to EV charging. But larger changes may include the distance needed between panels and whether or not to put any panels on the curved roofs or shaded sections, which could remove around 60 panels, reducing the installed capacity by a third (to 34 kWp).

If only 2 panels could fit per unit of horizontal roofspace, this would also substantally reduce the installed capacity to 130 panels (to 35 kWp, assuming panels go on the curved and shaded roof sections).

Other considerations not covered here may increase or decrease Chaco's the capacity of PV that installed in Chaco; this document is not definitive. However, it should be useful, forming a basis for more accurate and well-informed assessments of Chaco's solar PV potential and an optimal design for a PV installation.

Other considerations
====================

In addition to the installed capacity of PV, there are other considerations to account for in the design of a PV system installation for Chaco.

Aggregation of power
--------------------

For economies of scale and electricity purchase, electricity will be supplied by a private wire into a central control board. It makes sense for the PV power to supply this central supply, rather than individual houses.

Inverters
---------

Few large inverters are cheaper and more effective than many small ones for a given power rating. This raises the question: how many inverters should be supplied. One scenario would involve 3 inverters, accounting for the 3 main areas of power generation outlined above:

-   One ~20kW inverter for the west wing
-   One ~20kW inverter for the east wing
-   One ~10kW inverter for the common house

It may also make sense to install separate inverters for curved sections. Inverter configuration will be an important factor in overall performance.

Inverter location must also be decided. Options could include placement in attic space, under the stairs and in dedicated storage units outside the thermal envelope.

Financing
---------

One option explored is to finance the PV installation via Leeds Community Energy (LCE), a community benefit company. This could involve LCE owning the panels and leasing them to Chaco until the investment is paid back.

References
==========

Manni, Mattia, Raffaele Tecce, Gianluca Cavalaglio, Valentina Coccia, Andrea Nicolini, and Alessandro Petrozzi. 2017. “Architectural and Energy Refurbishment of the Headquarter of the University of Teramo.” *Energy Procedia*, ATI 2017 - 72nd Conference of the Italian Thermal Machines Engineering Association, 126 (September): 565–72. doi:[10.1016/j.egypro.2017.08.290](https://doi.org/10.1016/j.egypro.2017.08.290).

[1] M&E performance specification(revA)
