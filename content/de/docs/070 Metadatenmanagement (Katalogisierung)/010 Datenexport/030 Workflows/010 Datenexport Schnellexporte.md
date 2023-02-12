---
title: "Datenexport Schnellexporte"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-datenexport, by-folio, cat-workflows, for-anwender]
weight: 10
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/metadata/data-export/#quick-exports) & [GBV](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio:+Datenexport+Schnellexporte)
    "
---

Schnellexporte werden in der Katalog App durchgeführt. Damit können schnell Instanzen im MARC- oder JSON-Format für ausgewählte Datensätze heruntergeladen werden. Derzeit ist nur der Export einer .csv-Datei mit UUIDs implementiert worden.

## Instanzen exportieren (MARC)

Anmerkung: Zur Zeit ist der vollständige MARC-Export über den Schnellexport noch nicht implementiert. Wenn diese Schritte befolgt werden, wird stattdessen eine .csv-Datei mit den UUIDs der ausgewählten Dateien exportiert, die im Modul Datenexport verwendet werden kann.

1.  Die App **Katalog** öffnen.
2.  In der Ansicht **Katalog** die Datensätze suchen, die exportieren werden sollen und für jeden Datensatz die Checkbox in der ersten Spalte markieren.
3.  Auf **Aktionen > Instanzen exportieren (MARC)** klicken. Abhängig vom Browser und dessen Konfigurationen wird die Datei automatisch heruntergeladen oder es wird aufgefordert, sie zu speichern. Der Export wird in der App Datenexport protokolliert.

## Instanzen exportieren (JSON)

Der Export von Instanzen in JSON ist derzeit noch nicht implementiert.
