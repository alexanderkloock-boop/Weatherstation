# Hardwareplanung

## Controller

### Favorit: ESP32

Anforderungen:

- WLAN
- ausreichend GPIOs
- I2C
- SPI
- geringer Stromverbrauch
- gute ESPHome-Unterstützung

Die konkrete ESP32-Variante wird nach Auswahl der Sensoren festgelegt.

## Sensoren

| Messgröße | Auswahl | Status |
|---|---|---|
| Temperatur | offen | ⏳ |
| Luftfeuchte | offen | ⏳ |
| Luftdruck | offen | ⏳ |
| Windgeschwindigkeit | offen | ⏳ |
| Windrichtung | offen | ⏳ |
| Niederschlag | offen | ⏳ |
| UV | optional | ⏳ |
| Helligkeit | optional | ⏳ |
| Bodenfeuchte | optional | ⏳ |

## Outdoor-Anforderungen

Bei allen Außenkomponenten sind zu berücksichtigen:

- Schutz gegen Regen und Spritzwasser
- UV-Beständigkeit
- Kondensation
- Temperaturbereich
- Korrosion
- Wartbarkeit
- Montagehöhe und Messort

## Energieversorgung

Noch offen:

- Netzteil
- 5-V-/12-V-Versorgung
- Solar + Akku
- Kombination aus Solar und Netzversorgung

Bei einer autarken Variante müssen insbesondere WLAN-Laufzeit und Messintervalle berücksichtigt werden.
