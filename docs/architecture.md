# Software- und Systemarchitektur

## Datenfluss

1. Sensor misst physikalische Größe.
2. ESP32 liest den Sensor.
3. Firmware prüft Messwert und Einheit.
4. ESP32 überträgt den Messwert per WLAN.
5. Home Assistant übernimmt Speicherung, Visualisierung und Automationen.

## Messwertprinzip

Sensoren sollen möglichst eine klare interne Einheit liefern:

- Temperatur: °C
- Luftfeuchtigkeit: %
- Luftdruck: hPa
- Windgeschwindigkeit: km/h
- Windrichtung: °
- Niederschlag: mm

## Ausfallsicherheit

Die Wetterstation soll auch bei einem kurzfristigen Ausfall von Home Assistant oder WLAN möglichst sinnvoll weiterarbeiten.

Geplant:

- lokale Sensorabfrage
- Wiederverbindung zum WLAN
- keine dauerhafte Abhängigkeit von Cloud-Diensten
- sinnvolle Fehlerzustände für nicht erreichbare Sensoren

## Home Assistant

Home Assistant ist die zentrale Stelle für:

- Dashboard
- Historie
- Langzeitaufzeichnung
- Automationen
- Benachrichtigungen

## Erweiterbarkeit

Neue Sensoren sollen hinzugefügt werden können, ohne die bestehende Architektur grundlegend zu verändern.
