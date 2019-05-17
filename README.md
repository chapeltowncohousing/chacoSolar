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

The initial spec document[1] included provision for 127 standard 1600x980mm panels as follow:

-   14 \* 6 panel installations on the 14 unshaded roofs of the terrace
-   4 \* 4 panel installations on the remaining 4 'type C' terrace roofs that will receive some shading
-   27 panels on the common house

Assuming a per panel output of 270 W, this would mean Chaco could generate 34 KWp in full sunshine. This scenario is illustrated in the figue below.

Based on architectural drawings, the south facing roofspace available was estimated. The first stage was to digitise the pdfs into simple block representations of the buildings and highlight south-facing roofs, as illustrated in the figure below.

<img src="layout-south-facing-with-scale.png" width="3311" />

This was georectified and digitised in QGIS, resulting in the following data:

![](README_files/figure-markdown_github/unnamed-chunk-6-1.png)

The total maximum area available, for the terrace, common house and the entire shed roof area, respectively, was calculated as follows:

    #> Units: [m^2]
    #> [1] 389.50328  87.03578  30.65030

[1] M&E performance specification(revA)
