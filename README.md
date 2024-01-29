# Norwegian Geodata

## Files

### [`postal-codes.json.gz`](postal-codes.json.gz)

Postal codes from [Posten](https://www.bring.no/postnummerregister-ansi.txt) and geodata from [Kartverket](https://ws.geonorge.no/kommuneinfo/v1/) and [Geonorge](https://kartkatalog.geonorge.no/metadata/postnummeromraader/462a5297-33ef-438a-82a5-07fff5799be3). Merged into a single JSON file, keyed by postal codes, containing the following data:

- postal code
- city/place (poststed)
- municipality number
- municipality
- cateogory
- category description
- county (fylke)
- county number (fylkesnummer)
- geojson (is `null` for postal codes of categories `P` and `S`, and postal codes `0018` and `0045`)
