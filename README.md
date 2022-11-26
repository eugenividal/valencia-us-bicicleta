Data exploration
================
Eugeni Vidal-Tortosa
2022-11-26

# Potential title

Cycling growth in Valencia: a quantitative analysis after seven years of
investment in cycling infrastructure (and other sustainable transport
measures).

<!-- Alternative title: 'From Grand Prix (2013) to European Green Capital (2024)' -->

# Some context

Valencia has gone from being one of the most car-oriented Spanish cities
(it hosted the Grand Prix in 2013!), to becoming a benchmark in cycling
in the Mediterranean area in less than 10 years. The fundamental reason,
the change of government in 2015 that promoted a set of courageous
policies for social and environmental transformation. For this and for
another environmental achievements, it has just been nominated European
Green Capital 2024.

<https://energy-cities.eu/best-practice/a-new-cycling-ring-to-transform-mobility-in-valencia/>

<https://environment.ec.europa.eu/news/valencia-elsinore-and-velenje-win-2024-european-green-city-awards-2022-10-28_en>

Main measurements:

- Cycling Ring

- Bikesharing: <https://www.valenbisi.es/en/home>

- Traffic Calming Measures

# Questions

- Growth estimation.

- Health benefits? How many deaths avoided? Emissions and road safety
  improvements.

- Any kind of prediction?

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

- Valenbici?

# Next steps

Get more data!
