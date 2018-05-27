## Events

### Funktionsweise:

Es gibt bestimmte Punkte ("Events"), die im Laufe der Datenverarbeitung aufgerufen werden. Für jedes Event und jede Mögliche "Variable", mit der das Event aufgerufen wird (i.d.r. Sensor-ID) gibt es eine Liste, die nacheinander durchlaufen wird. Alle Aktionen in dieser Liste werden nacheinander ausgeführt.

Module/Plugins können sich in diese Events "einhängen", sie können aber auch extern (also vom Nutzer konfigurierte Hooks) sein. Module sollten auch wieder eigene Events definieren können.

### Beispiele für mögliche Events

- onDataIn(SensorId) (Daten wurden empfangen, sind aber noch nicht verarbeitet)
- onDataSaved(SensorId) (Datenverarbeitung abgeschlossen)
- onDataError(SensorId) (Datenverarbeitung mit Fehler abgebrochen)
- periodically(period) (Event für periodische Checks)

### Mögliche Nutzer

z.B. können virtuelle Sensoren sich an onDataError dranhängen, um bei einem neuen Input den Wert für virtuelle Sensoren zu aktualisieren.