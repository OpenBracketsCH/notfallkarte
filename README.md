# Notfallkarte für Feuerwehren

## Ausgangslage

Das wichtigste bei einem Feuerwehr-Einsatz ist es, sich schnell eine Übersicht zu verschaffen.Die ersten Minuten eines Einsatzes sind meist hektisch und chaotisch, eine einfache, intuitive Bedienung von Anwendungen daher essentiell. Visualisierung von Einsatzorten und taktischen Gegebenheiten wird bei komplexen Überbauungen und grossen Nachbarschaften immer wichtiger.

Es gibt bereits Apps und Anwendungen die genau dies erfüllen. Jedoch sind viele davon nicht frei verfügbar und an kostenpflichtige, respektive kostspielige Abos angebunden.

Die Lösung sind Open-Source Daten die frei zu Verfügung stehen. In OpenStreetMap lässt sich alles abbilden was man möchte und die Daten stehen allen zu Verfügung. Mit diversen Tools wie uMap und Mapbox lassen sich die Daten nach eigenen Bedürfnissen visualisieren.

## Umsetzung

Gestartet wurde das Projekt mit Hydranten mit der Intention so rasch als möglich den nächstgelegenen Hydranten anzuzeigen.
Das Projekt wurde aber sehr rasch um zusätzliche Daten erweitert, alles einsatzrelevante Daten die wichtig erschienen:

* Hydranten

  * Daten von Sichtungen.

  * Daten von Gemeinde und Kanton.

  * schwierig mit reinen Sichtungen zuverlässige Daten zu erheben.

* Schlüsselrohre

  * Schlüsselrohre ermöglichen der Feuerwehr mittels eines Passepartout diese Rohre zu öffnen und den effektiven Schlüssel für den Zugang zum Objekt zu gewährleisten.

  * Daten von effektiv bestehenden Schlüsselrohren und einer Liste aller in der Gemeinde befindlichen, zu kontrollierenden Rohre.

* Defibrillatoren

  * öffentlich zugängliche Defibrillatoren in der Gemeinde.

  * Liste der Gemeinde.

* Einsatzpläne

  * grosse oder komplexe Objekte bei denen Feuerwehreinsatzpläne bestehen.

  * Verzeichnis bestehender Einsatzpläne und Unterlagen.

* BMA Bedienstellen

  * Zugänge für die Feuerwehr um Brandmeldeanlagen und deren Bedienstellen zu erreichen.

  * lokales Wissen und Pläne.

* Evakuierungspunkte

  * Sammelpunkte für Evakuierungen von Gebäuden.

### verwendete OSM Tags

| key | tag | Beschreibung
|- |- |-
| emergency | defibrillator| Defibrillatoren
| emergency | fire_hydrant | Hydranten
| emergency | assembly_point | Evakuierungspunkte / Sammelplätze
| emergency | key_depot | Schlüsseldepot Feuerwehr
| emergency | fire_control_panel| BMA Bedienstellen
| emergency:plan| yes | Feuerwehr Einsatzplan
| emergency | siren | ZSO Sirene
| emergency | disaster_help_point | Notfalltreffpunkte (in Zukunft)
| emergency| fire_water_pond | Löschwasserbecken

**Solaranlagen mit folgenden Tags versehen:**
```
generator:method=photovoltaic
generator:output:electricity=small_installation
generator:place=roof
generator:source=solar
generator:type=solar_photovoltaic_panel
power=generator
```