---
title: "Software by INBO: packages for environmentalists and ecologists!"
date: 2019-03-25
csl: ../inbo.csl
bibliography: ../reproducible_research.bib
categories: ["development", "r", "statistics", "databases"]
tags: ["open science", "packages", "r", "python"]
output: 
    md_document:
        preserve_yaml: true
weight: 1
---

At the Research Institute for Nature and Forest (INBO), we are eager to
sustain, promote and develop open-source software that is relevant to
biodiversity researchers! This page lists **R and Python packages**
which INBO developed or made a significant contribution to. Several of
these packages continue being developed.

Please, feel invited to **try out** packages! If you encounter a problem
or if you have a suggestion, we encourage you to post an issue on the
package's code repository. You can also directly contribute improvements
with a pull request.

The package hyperlinks below refer to the package's **documentation
website**, if available. When there is no documentation website, often
one or more **vignettes** are available within the package, describing
the package's purpose and demonstrating its use.

The following table gives a **quick overview**:

<table>
<thead>
<tr class="header">
<th>Research stage</th>
<th>Related INBO packages</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>Study design</td>
<td><a href="https://github.com/ThierryO/grts">grts</a></td>
</tr>
<tr class="even">
<td>Retrieve data: environmental</td>
<td><a href="https://ropensci.github.io/wateRinfo/">wateRinfo</a>, <a href="https://pydov.readthedocs.io/">pydov</a></td>
</tr>
<tr class="odd">
<td>Retrieve data: biological</td>
<td><a href="https://github.com/inbo/pyinaturalist">pyinaturalist</a>, <a href="https://inbo.github.io/uvabits/">uvabits</a>, <a href="https://inbo.github.io/etn/">etn</a></td>
</tr>
<tr class="even">
<td>Store data</td>
<td><a href="https://inbo.github.io/git2rdata/">git2rdata</a></td>
</tr>
<tr class="odd">
<td>Validate data</td>
<td><a href="https://inbo.github.io/pywhip/">pywhip</a></td>
</tr>
<tr class="even">
<td>Analyze data: graphs</td>
<td><a href="https://github.com/inbo/inboggvegan">inboggvegan</a></td>
</tr>
<tr class="odd">
<td>Analyze data: models</td>
<td><a href="https://inlatools.netlify.com/">inlatools</a>, <a href="https://github.com/inbo/multimput">multimput</a>, <a href="https://inbo.github.io/niche_vlaanderen/">niche_vlaanderen</a></td>
</tr>
<tr class="even">
<td>Analyze data: indices</td>
<td><a href="https://github.com/inbo/LSVI">LSVI</a></td>
</tr>
<tr class="odd">
<td>Publish</td>
<td><a href="https://inbomd.netlify.com/articles/introduction.html">INBOmd</a>, <a href="https://inbo.github.io/INBOtheme/">INBOtheme</a></td>
</tr>
<tr class="even">
<td>Miscellaneous (mixed content)</td>
<td><a href="https://inbo.github.io/inborutils/">inborutils</a></td>
</tr>
</tbody>
</table>

Study design
------------

-   **R package [grts](https://github.com/ThierryO/grts)**: draw a
    sample from a sampling frame with the Generalized Random
    Tessellation Stratified (GRTS) sampling strategy.

Retrieve data
-------------

### Environmental data

-   **R package [wateRinfo](https://ropensci.github.io/wateRinfo/)**:
    facilitates access to [waterinfo.be](https://www.waterinfo.be/), a
    website managed by the [Flanders Environment Agency
    (VMM)](https://en.vmm.be/) and [Flanders Hydraulics
    Research](https://www.waterbouwkundiglaboratorium.be/). The website
    provides access to real-time water and weather related environmental
    variables for Flanders (Belgium), such as rainfall, air pressure,
    discharge, and water level. The package provides functions to search
    for stations and variables, and download time series.
-   **Python package [pydov](https://pydov.readthedocs.io/)**: to query
    and download data from [Databank Ondergrond Vlaanderen
    (DOV)](https://www.dov.vlaanderen.be/). DOV aggregates data about
    soil, subsoil and groundwater of Flanders and makes them publicly
    available. Interactive and human-readable extraction and querying of
    the data is provided by a web application, whereas the focus of this
    package is to support machine-based extraction and conversion of the
    data.

### Biological data

-   **Python package
    [pyinaturalist](https://github.com/inbo/pyinaturalist)**: Python
    client for the iNaturalist APIs.
-   **R package [uvabits](https://inbo.github.io/uvabits/)**: provides
    an R interface to the [UvA-BiTS database](http://www.uva-bits.nl/),
    which stores bird movement data collected with UvA-BiTS GPS
    trackers. The package provides functionality to download data and
    metadata, calculate some metrics, and load the data into a
    query-optimized SQLite database for local analysis. It also allows
    to download the data in a format that can easily be uploaded to
    [Movebank](https://www.movebank.org/), a free online database for
    animal tracking data.
-   **R package [etn](https://inbo.github.io/etn/)**: provides
    functionality to access and process data from the [European Tracking
    Network (ETN)](http://www.lifewatch.be/etn/) database hosted by the
    Flanders Marine Institute (VLIZ) as part of the Flemish contribution
    to LifeWatch.

Store data
----------

-   **R package [git2rdata](https://inbo.github.io/git2rdata/)**: an R
    package for writing and reading dataframes as plain text files.
    Important information is stored in a metadata file, which allows to
    maintain the classes of variables. `git2rdata` is ideal for storing
    R dataframes as plain text files under version control, as it
    strives to minimize row based diffs between two consecutive commits.
    The package is intended to facilitate a reproducible and traceable
    workflow.

Validate data
-------------

-   **Python package [pywhip](https://inbo.github.io/pywhip/)**: a
    package to validate data against [whip
    specifications](https://github.com/inbo/whip), a human and
    machine-readable syntax to express specifications for data.

Analyze data
------------

### Make graphs

-   **R package [inboggvegan](https://github.com/inbo/inboggvegan)**:
    provides R functions for multivariate plots. More specifically,
    extended biplot and screeplot functionality is offered for the
    `vegan` package.

### Fit models and make model predictions

-   **R package [inlatools](https://inlatools.netlify.com/)**: provides
    a set of functions which can be useful to diagnose [INLA
    models](http://www.r-inla.org/): calculating Pearson residuals,
    simulation based checks for over- or underdispersion, simulation
    based checks for the distribution, visualising the effect of the
    variance or precision on random effects (random intercept, first
    order random walk, second order random walk). The functions can be
    useful to choose sensible priors and diagnose the fitted model.
-   **R package [multimput](https://github.com/inbo/multimput)**: an R
    package that assists with analysing datasets with missing values
    using multiple imputation.
-   **Python package
    [niche\_vlaanderen](https://inbo.github.io/niche_vlaanderen/)**:
    Python package to run the NICHE Vlaanderen model. Based on
    calculated abiotic properties of the location, NICHE Vlaanderen
    determines whether certain vegetation types can develop. An
    additional flooding module allows the user to test whether the
    predicted vegetations are compatible with a particular flooding
    regime. The package is a redevelopment of an existing ArcGIS plugin
    in Python, without external non-open source dependencies.

### Calculate indices

-   **R package [LSVI](https://github.com/inbo/LSVI)**: bundles a number
    of functions to support researchers in determining the local
    conservation status ('LSVI') of Natura 2000 habitats in Flanders.
    Several functions retrieve the criteria and/or associated species
    lists for determining the LSVI. A specific function allows to
    calculate the LSVI. The package is written in Dutch.

Publish your workflow and discuss your results
----------------------------------------------

-   **R package
    [INBOmd](https://inbomd.netlify.com/articles/introduction.html)**:
    provides several styles for `rmarkdown` files and several templates
    to generate reports, presentations and posters. The styles are based
    on the corporate identity of INBO and the Flemish government. All
    templates are based on `bookdown`, which is an extension of
    `rmarkdown`. `bookdown` is taylored towards writing books and
    technical documentation.
-   **R package [INBOtheme](https://inbo.github.io/INBOtheme/)**:
    contains `ggplot2` themes for INBO, the Flemish government and
    Elsevier journals. The documentation website includes a set of
    example figures for each available theme.

Last but *not least*: miscellaneous!
------------------------------------

-   **R package [inborutils](https://inbo.github.io/inborutils/)**:
    provides a collection of useful R utilities and snippets that we
    consider recyclable for multiple projects. The functions are either
    out of scope or just not mature enough to include as extensions to
    existing packages.