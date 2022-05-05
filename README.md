# helsinkiBSS
Reproducible code, R Markdown file and data links corresponding to the city of Helsinki for the analysis of the Helsinki Bike Sharing System (BSS) in R.

# TDS (Transport Data Science)

This is a GitHub Repository made as part of the Transport Data Science module at the University of Leeds - conforming to standards of reproducible research. 

# Prerequisites

## Software

To run this project need to have up-to-date versions of R and RStudio
installed on a computer you have access to:

-   R from [cran.r-project.org](https://cran.r-project.org/)
-   RStudio from
    [rstudio.com](https://rstudio.com/products/rstudio/download/#download)
-   R packages, which can be installed by opening RStudio and typing
    `install.packages("tidyverse")` in the R console, for example.
-   To produce any maps made as part of the analysis, QGIS will be needed which is downloadable from [here](https://qgis.org/en/site/forusers/download.html).

## Data

*Bikes data*

To reproduce this project (or run the code for a different time period), download data regarding Helsinki's Bike Share System from [Helsinki's Open Data Interface](https://www.hsl.fi/en/hsl/open-data#journeys-made-by-city-bikes). For this project, data for the Month of April 2021 was used spanning to 12th May, i.e. "dev.hsl.fi/citybikes/od-trips-2021/2021-04.csv". To use a different month, simply change the data required, alternatively larger datasets to assess longer temporal trends can be downloaded via the same interface by stating the year required, i.e. "dev.hsl.fi/citybikes/od-trips-2021/2021-04.csv".

*Docking locations*

The associated docking locations of the city bikes can be downloaded in spatial format from [here](https://hri.fi/data/en/dataset/hsl-n-kaupunkipyoraasemat). As this dataset possessing geometries relating to the spatial location of each station, this file can be joined to the `bikes data` to link relative geometries to the flows.

*Demographic data*

Demographic data referring to the year 2020 was also used as part of the analysis. This data can be downloaded from [here](https://pxnet2.stat.fi/PXWeb/pxweb/en/Postinumeroalueittainen_avoin_tieto/Postinumeroalueittainen_avoin_tieto__2022/paavo_pxt_12ey.px/) at postal level. Within this project proportions of each group in each postal sector were obtained for direct comparison, this was achieved through dividing the number of a group in an area by the total number of inhabitants in that area, and multiplying by 100. The corresponding postal sector boundary files were downloaded in `.shp` format for functionality with QGIS from [here](https://hri.fi/data/en_GB/dataset/paakaupunkiseudun-postinumeroalueet/resource/0a952d7c-a038-40e3-b9fe-e910c76153f3).

If a differing geographic aggretation is required as part of the project, please refer to the [Statistics Finland](https://stat.fi/tup/tilastotietokannat/index_en.html) website and select your required aggregation and variables. There are also a host of additional datasets available from the [Helsinki Region Infoshare](https://hri.fi/fi/) which may be useful for alternate analyses.

## Running the script

The file 


## Issues and contributing

Any feedback or contributions to this repo are welcome. If you have a
question please open an issue via Github (you’ll need a GitHub account), alternativelty contact the owner at ll16e7m@leeds.ac.uk.
