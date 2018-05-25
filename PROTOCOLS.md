## Protocoll wishlist freifunk-IoT

#### Aggregation (Sensor -> Data Sink)

- MQTT
- HTTP(S)-GET (data in GET-parameter)
- HTTP(S)-POST
- Carbon (https://graphite.readthedocs.io/en/latest/feeding-carbon.html)
- UDP (Carbon-Like)

#### Distribution (Data Access -> Other Services)

(active: Triggered by Data Access component,  passive: Request from externally)

- Mail (active, alert)

- Mail-Report (active, periodically)

- HTTP(S)-Hook (active, alert)

- HTTP(S)-Hook (active, periodically+report)

- HTTP(S)-REST (passive, live+historical+report, JSON)

- CSV (historical+report)

- HTTP(S) Charts (jpeg/gif/png to embed)

  