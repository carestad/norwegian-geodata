# Norwegian Geodata

## Files

### [`postal-codes.json.gz`](postal-codes.json.gz)

Postal codes from [Posten](https://www.bring.no/postnummerregister-ansi.txt) and geodata from [Kartverket](https://ws.geonorge.no/kommuneinfo/v1/) and [Geonorge](https://kartkatalog.geonorge.no/metadata/postnummeromraader/462a5297-33ef-438a-82a5-07fff5799be3). Merged into a single JSON file, keyed by postal codes, containing the following data:

- `postnummer` (postal code)
- `poststed` (city/place/town)
- `kommunenummer` (municipality number)
- `kommune` (municipality)
- `kategori` (cateogory)
- `kategoriforklaring` (category description)
- `fylke` (county)
- `fylkesnummer` (county number)
- `geojson` (is `null` for postal codes of categories `P` and `S`, and postal codes `0018` and `0045`)
- `senterpunkt` (centroid point within geojson polygon)

#### Example

```json
{
    "postnummer": "4180",
    "poststed": "KVITSØY",
    "kommunenummer": "1144",
    "kommune": "KVITSØY",
    "kategori": "G",
    "kategoriforklaring": "Gateadresser (og stedsadresser), dvs. \"grønne postkasser\"",
    "fylke": "Rogaland",
    "fylkesnummer": "11",
    "geojson": {
        "type": "Feature",
        "geometry": {
            "type": "Polygon",
            "coordinates": [
                [
                    [
                        5.16673,
                        59.034819
                    ],
                    [
                        5.247196,
                        58.979623
                    ],
                    [
                        5.258302,
                        58.949437
                    ],
                    [
                        5.38376,
                        58.964299
                    ],
                    [
                        5.445117,
                        58.982091
                    ],
                    [
                        5.445126,
                        58.982102
                    ],
                    [
                        5.459158,
                        59.000352
                    ],
                    [
                        5.47033,
                        59.014869
                    ],
                    [
                        5.480604,
                        59.028207
                    ],
                    [
                        5.502037,
                        59.056
                    ],
                    [
                        5.545404,
                        59.072444
                    ],
                    [
                        5.499034,
                        59.128275
                    ],
                    [
                        5.482225,
                        59.12611
                    ],
                    [
                        5.435297,
                        59.12005
                    ],
                    [
                        5.402631,
                        59.115821
                    ],
                    [
                        5.371035,
                        59.111722
                    ],
                    [
                        5.350053,
                        59.103859
                    ],
                    [
                        5.296386,
                        59.083715
                    ],
                    [
                        5.270778,
                        59.074087
                    ],
                    [
                        5.26215,
                        59.070837
                    ],
                    [
                        5.181827,
                        59.040527
                    ],
                    [
                        5.16673,
                        59.034819
                    ]
                ]
            ]
        },
        "properties": {
            "objtype": "Postnummerområde",
            "postnummer": "4180",
            "poststed": "KVITSØY",
            "lokalid": "475b20fe-9141-4a6f-bfc9-1fad998421de",
            "navnerom": "https://data.geonorge.no/sosi/administrativeenheter/postnummeromrader",
            "versjonid": "20180215",
            "datauttaksdato": "20240128060835",
            "oppdateringsdato": null,
            "opphav": "Posten Norge/Kartverket",
            "noyaktighet": 1500,
            "kommune": "1144",
            "malemetode": "55"
        }
    },
    "senterpunkt": {
        "type": "Point",
        "coordinates": [
            5.363976444240297,
            59.03918322511065
        ]
    }
}
```
