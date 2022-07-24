# elezioni22

Utilizziamo dati provenienti dal [sito della camera](http://dati.camera.it).

Principali utilizzi del sito:
1. Lista dei candidati alle elezioni 2022
2. Dati sulle precedenti legislature

# Esempio di query

```
http://dati.camera.it/sparql?default-graph-uri=&query=select%20distinct%20%2A%20where%20%7B%0A%3Fatto%20a%20ocd%3Aatto.%0A%3Fatto%20dc%3Atitle%20%3FnomeAtto.%0A%3Flegge%20a%20ocd%3Alegge%3B%20ocd%3Arif_leg%20%3Chttp%3A%2F%2Fdati.camera.it%2Focd%2Flegislatura.rdf%2Frepubblica_17%3E.%0A%3Flegge%20ocd%3AlavoriPreparatori%20%5B%3Flavoro%20%3Fatto%5D%0A%7D&format=application%2Fsparql-results%2Bjson
```

Altri esempi di SPARQL queries provengono dal sito (hackathon2014-montecitorio)[https://github.com/hackathon2014-montecitorio/sparql/wiki]

# Progetti simili

- (PalMas)[https://github.com/obujor/PalMaS]
- (Dati Camera at Wiki)[https://github.com/CristianCantoro/DatiCameraAtWikidata/blob/master/dati.py]

