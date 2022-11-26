Data exploration
================

# Cycling volumes

<https://opendata.vlci.valencia.es/en/dataset/intensitat-dels-punts-de-mesura-de-bicicletes-espires-electromagnetiques>

Cycling traffic counts in Valencia city.

``` r
library("rjson")

json_file <- "https://geoportal.valencia.es/apps/OpenData/Trafico/tra_espiras_bici_p.json"
json_data <- fromJSON(paste(readLines(json_file), collapse=""))
```

    ## Warning in readLines(json_file): incomplete final line found on 'https://
    ## geoportal.valencia.es/apps/OpenData/Trafico/tra_espiras_bici_p.json'
