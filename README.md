## Linked Pasts Network

A workspace for technical matters related to linking historical research data

#### Place Interconnection Format (PGIFv2)

Work-in-progress update to the [Pelagios Gazetteer Interconnection Format (PGIF)](https://github.com/pelagios/pelagios-cookbook/wiki/Pelagios-Gazetteer-Interconnection-Format), for future use in contributing to [Peripleo](http://peripleo.pelagios.org) and [World-Historical Gazetteer](http://whgazetteer.org). The format constitutes an example of a proposed GeoJSON extension, [GeoJSON-T](https://github.com/kgeographer/geojson-t)

PGIFv2 is valid GeoJSON. A challenge remains to convert place records represented this way to a valid RDF syntax, e.g. JSON-LD or RDF/XML. Some experimentation is under way (see below), which will be informed by upcoming work on an updated JSON-LD spec (1.0 -> 1.1) in summer of 2018.

- ./pgif_v2{x}.json: _latest annotated draft for comment_

#### JSON-LD experiments

Files in the /json-ld folder are attempts to find solutions to the age-old "edge properties problem" of RDF. Discussion of this is [issue 1 in this repo](#1) [@kgeographer, @gklyne]

- json-ld/place-v{n}-example.jsonld: _sample record_

- json-ld/place-v{n}-context.jsonld: _JSON-LD context_

[latest example @ JSON-LD playground](http://tinyurl.com/yd5brj66)

*NOTE*: The JSON-LD 1.0 specification does not support lists of lists, so the GeoJSON-LD geometries will not validate as JSON-LD. The above example [_*is*_ valid GeoJSON](https://github.com/LinkedPasts/lp-network/blob/master/place-v3-example.json), however. The [JSON-LD 1.1 spec in development](https://json-ld.org/spec/latest/json-ld/) promises a workaround to this problem when completed.
