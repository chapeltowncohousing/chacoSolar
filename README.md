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

This was georectified and digitised in QGIS, resulting in the following data, which has been made available as open data:

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

The assumption about panel size, plus use of digitising tools in QGIS, allows the panel location to envisioned:

[1] M&E performance specification(revA)
