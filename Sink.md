## Data Sink

**Großes ToDo: Besseren Namen finden**

Für den Aufbau der Events siehe Events.md (noch nicht fertig)

Die einzelnen Module können auch in einem Prozess laufen, aber jeweils als eigene Instanz ihrer Klasse.

### Data Sink Core

- Empfängt Daten über verschiedene Kanäle/Protokolle
- Authentifiziert Sensoren
- Triggert mit dem Sensor verknüpfte Events (zu diskutieren wo das ganze stattfindet, halte ich hier für sinnvoll)
- Validiert Datentypen
- Schreibt Messwerte in die Datenbank

#### Module: Virtual Sensors

- Erzeugt virtuelle Sensoren, z.B. ein Failover/Merge

### Data Sink Authenticator

- Verwaltet Rechte
- Authentifiziert Requests

### Data Sink Cron

- Triggert Cron-Events



