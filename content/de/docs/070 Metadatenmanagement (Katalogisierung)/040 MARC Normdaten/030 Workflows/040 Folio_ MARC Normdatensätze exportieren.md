---
title: "Folio: MARC Normdatensätze exportieren"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-marc_normdaten, by-folio, cat-workflows, for-anwender]
weight: 40
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/metadata/inventory/marcauthority/#exporting-marc-authority-records) & [GBV](https://info.gbv.de/pages/viewpage.action?pageId=854294552)
    "
---

MARC Normdatensätze können auf die gleiche Weise exportiert werden wie Instanzdatensätze als MARC (siehe [Folio: Instanzen exportieren (MARC/JSON)](https://info.gbv.de/pages/viewpage.action?pageId=852492494)). Anmerkung: Zur Zeit ist der vollständige MARC-Export über den Schnellexport noch nicht implementiert. Werden diese Schritte ausgeführt, wird stattdessen eine .csv-Datei mit den UUIDs der ausgewählten Dateien zur Verwendung im Datenexportmodul exportiert.

1.  Die App **MARC Normdaten** öffnen.
2.  In der Ansicht **MARC-Normdatensatz** die Datensätze suchen, die exportiert werden sollen und für jeden Datensatz die **Checkbox** in der ersten Spalte aktivieren. Bitte beachten, dass die zugehörigen Referenzen in der Ergebnisliste ebenfalls markiert werden müssen; die Meldung am oberen Rand des Fensters zeigt die genaue Anzahl der ausgewählten Datensätze an.
3.  Auf **Aktionen > Ausgewählte Datensätze exportieren (CSV/MARC)** klicken. Abhängig von dem Browser und dessen Konfigurationen wird die Datei automatisch heruntergeladen oder es wird aufgefordert, sie zu speichern. Der Export wird in der App Datenexport protokolliert.

Um die exportierten Datensätze anzuzeigen, den Anweisungen unter [Folio: Exportmanager Exportaufträgen anzeigen (Entwurf)](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio%3A+Datenexport+Logs+und+Ergebnisse+anzeigen) folgen.
