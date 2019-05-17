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

Based on the knowledge that the panels will be slightly larger: 1650x991mm. Given that the roof has an elevation of 35 degrees, such panels would have a horizontal footprint of 1619x991mm. In the original scenario, they would cover 204 m<sup>2</sup>, less than half of the total available space under optimistic assumptions.

The assumption about panel size, plus use of digitising tools in QGIS, allows the panel location to envisioned. The figure below shows two ways of aligning the panels: stacked as portrait or landscape. The portrait way is a squeeze: the roof is just over 3.3 m long in the horizontal access; two panels stacked in portrait formation are just over 3.2 m, leaving only a few cm clearance, which may be insufficient.

<img src="closeup3.png" alt="Portrait and landscape stacking. The two panels on the bottom left show the impact of the panels being at 35 degrees in each alignment: relatively minor." width="743" />
<p class="caption">
Portrait and landscape stacking. The two panels on the bottom left show the impact of the panels being at 35 degrees in each alignment: relatively minor.
</p>

The landscape stacking style leaves more room all round and 3 panels every ~2m.

The straight sections of the east and west wings are 41 m, leaving room for 20 sets of three on each, 120 panels in total. The south facing roofs on the curve are around 6.7 m at the smallest point, suggesting that there is enough room for 9 panels each (36 in total). These calculations suggest there is enough room for 156 panels on the terrace, not accounting for the complicating factors of shaded panels (see the darker red areas in the figure above) or the slightly larger roof space on 4 of the houses.

The south facing roof on the common house is ~17.5 m long and just over 5 m wide. Assuming three panels could fit in portrait formation, this would allow 3 \* 17 = 51 panels on the common house roof.

**Overall, simplistic calculations based on optimistic assumptions about stacking and shading suggest that Chaco could have room for 207 panels (56 KWp assuming no shading of 270 W modules).** This calculation ignores many things, including complicating factors around the interfaces between roofs of different heights in the terrace, assumes that panels are packed tight on the common house roof and that panels go on the curved roof. So far it ignores the shed, which could fit 12 (4x3) extra panels, and could be a place to extend the PV capacity of Chaco in the future, perhaps linked to EV charging.

It may not be possible or desirable to put that many panels on. However, it is a useful exercise to encourage more accurate and well-informed assessments of Chaco's solar PV potential and an optimal design for a PV installation.

[1] M&E performance specification(revA)
