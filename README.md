---
title: "README"
author: "Jamaal Green"
date: "September 7, 2017"
output: html_document
---

#lehdr

**lehdr** is an R package that allows users to interface with the Longitudinal and Employer-Household Dynamics (LEHD) Origin-Destination Employment Statistics (LODES) dataset returned as dataframes. The package is currently in development and can be installed at:

```
install.packages("devtools")
library(devtools)

devtools::install_github("jamgreen/lehdr")
```

#Why lehdr?

The LODES dataset is frequently used by transportation and economic development planners, regional economists, disaster managers and other public servants in order to have a fine grained understaning of the distribution of employment. Such data is integral for regional travel demand models that help to dictate transportation policy options, regional economists and economic development planners interested in the spatial distribution of particular kinds of work use the data to weigh different industrial or workforce policy options. Finally, as a census product, the LODES data can be joined to census Decennial or American Community Survey data to help visualize the interactions between different population groups and work. In short, the LODES dataset is the only source of detailed geographic information on employment for the country and should be more widely available for researchers and analysts who work on regional development issues. 

#Future Development

Currently, **lehdr** is designed to grab the LODES flat files (origin-destination, workplace, and residential association files) and includes an option to aggregate results to the census tract level from the block level that the LODES tables come in. Next steps include linking this package with the **sf** and **tigris** packages to allow for easier mapping of LODES data. 