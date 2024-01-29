# Norwegian Geodata

## Files

### [`postal-codes.json`](postal-codes.json)

Postal codes from [Posten](https://www.bring.no/postnummerregister-ansi.txt) and geodata from [Kartverket](https://ws.geonorge.no/kommuneinfo/v1/). Merged into a single JSON file, keyed by postal codes, containing the following data:

- postal code
- city/place (poststed)
- municipality number
- municipality
- cateogory
- category description
- county (fylke)
- county number (fylkesnummer)
- geojson (might be `null` for some postal codes)
