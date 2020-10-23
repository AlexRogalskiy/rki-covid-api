# Robert-Koch Institut API

This is a JSON API to easily get the data from this website:

[~~https://www.rki.de/DE/Content/InfAZ/N/Neuartiges_Coronavirus/Fallzahlen.html~~](https://www.rki.de/DE/Content/InfAZ/N/Neuartiges_Coronavirus/Fallzahlen.html)

https://services7.arcgis.com/mOBPykOjAyBO2ZKk/arcgis/rest/services/Coronafälle_in_den_Bundesländern/FeatureServer/0/query?where=1%3D1&outFields=LAN_ew_GEN,LAN_ew_EWZ,Fallzahl,Aktualisierung,faelle_100000_EW,Death,cases7_bl_per_100k&returnGeometry=false&outSR=4326&f=json

## Endpoints

### `https://rki-covid-api.now.sh/api/states`

#### Data Structure

```json
{
  "lastUpdate": 1603317600000,
  "states": [
    {
      "name": "Baden-Württemberg",
      "count": 58653,
      "weekIncidence": 42,
      "casesPer100k": 343.099136209832,
      "deaths": 1927,
      "code": "BW"
    },
    {
      "name": "Bayern",
      "count": 77904,
      "weekIncidence": 39,
      "casesPer100k": 123.099136209832,
      "deaths": 2714,
      "code": "BY"
    },
    ...
    {
      "name": "Schleswig-Holstein",
      "count": 5600,
      "weekIncidence": 13,
      "casesPer100k": 121.099136209832,
      "deaths": 163,
      "code": "SH"
    },
    {
      "name": "Thüringen",
      "count": 4793,
      "weekIncidence": 18,
      "casesPer100k": 324.099136209832,
      "deaths": 198,
      "code": "TH"
    }
  ]
}
```

### `https://rki-covid-api.now.sh/api/states-map`

You receive a PNG image:

<img src="media/states-map.png" alt="states-map" width="300"/>

### `https://rki-covid-api.now.sh/api/districts-map`

You receive a PNG image:

<img src="media/districts-map.png" alt="districts-map" width="300"/>


## Project Showcase (project using this API)

[Add your project by openening an issue with your project details!](https://github.com/marlon360/rki-covid-api/issues/new)

- https://coronafallzahlen.de



## Donation

[Buy me a coffee](https://ko-fi.com/marlon360)
