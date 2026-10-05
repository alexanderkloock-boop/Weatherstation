# Wetterstation

Modulare DIY-Wetterstation für ESP32 und Home Assistant.

## Ziel

Die Wetterstation soll lokale Wetterdaten erfassen und zuverlässig an Home Assistant übertragen. Die konkrete Sensorhardware wird später festgelegt.

### Geplante Messgrößen

- Temperatur
- relative Luftfeuchtigkeit
- Luftdruck
- Windgeschwindigkeit
- Windrichtung
- Niederschlag
- optional UV-Strahlung / Helligkeit
- optional Bodenfeuchte
- optional Feinstaub / Luftqualität

## Grundsätze

- ESP32 als Controller
- möglichst lokale/offline-fähige Datenerfassung
- Home Assistant als zentrale Plattform
- Sensoren modular austauschbar
- keine unnötige Herstellerbindung
- Versorgung und Energieverbrauch von Anfang an berücksichtigen
- Messwerte mit Plausibilitätsprüfung und sinnvollen Einheiten

## Geplante Architektur

```
Sensoren
   ↓
ESP32
   ↓ WLAN
Home Assistant
   ↓
Langzeitaufzeichnung / Dashboard / Automationen
```

## Hardware

Noch nicht ausgewählt.

Die Auswahl soll unter anderem anhand von Messgenauigkeit, Verfügbarkeit, Stromverbrauch, Outdoor-Tauglichkeit und Preis erfolgen.

## Software

Geplant:

- ESPHome oder eigene ESP32-Firmware
- Home Assistant
- optional MQTT
- optional InfluxDB / Grafana

## Projektstruktur

```
/
├── README.md
├── docs/
│   ├── hardware.md
│   └── architecture.md
└── firmware/
    └── README.md
```

## Status

**Phase 1 – Planung**

Noch keine Hardware vorhanden. Als nächster Schritt werden Controller, Sensoren, Stromversorgung und Gehäuse ausgewählt.
