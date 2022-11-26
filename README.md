Data exploration
================
Eugeni Vidal-Tortosa
2022-11-26

Potential title: “Cycling growth in Valencia: a quantitative analysis 5
years after the implementation of the ‘Cycling Ring’ (and other measures
to promote sustainable transport)”.

# Some context

<https://energy-cities.eu/best-practice/a-new-cycling-ring-to-transform-mobility-in-valencia/>

# Data

<https://opendata.vlci.valencia.es/en/dataset/intensitat-dels-punts-de-mesura-de-bicicletes-espires-electromagnetiques>

Cycling traffic counts in Valencia city.

``` r
library("rjson")

json_file <- "https://geoportal.valencia.es/apps/OpenData/Trafico/tra_espiras_bici_p.json"
json_data <- fromJSON(paste(readLines(json_file), collapse=""))
```

    ## Warning in readLines(json_file): incomplete final line found on 'https://
    ## geoportal.valencia.es/apps/OpenData/Trafico/tra_espiras_bici_p.json'

# Next steps…
