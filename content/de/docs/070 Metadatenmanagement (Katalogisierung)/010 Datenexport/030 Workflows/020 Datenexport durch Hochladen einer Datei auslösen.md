---
title: "Datenexport durch Hochladen einer Datei auslösen"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-datenexport, by-folio, cat-workflows, for-anwender]
weight: 10
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/metadata/data-export/#triggering-an-export-by-uploading-a-file ) & [GBV](https://info.gbv.de/pages/viewpage.action?pageId=846266412)
    "
---

Die App Datenexport akzeptiert zwei Arten von Daten und Dateitypen, die Datensätze für den Export identifizieren: eine CSV-Datei mit Instanz-UUIDs und eine CQL-Abfrage im CQL-Format. Das Auslösen eines Exports erzeugt eine .mrc-Datei.

Die App Datenexport wird mit einem Standard-Jobprofil geliefert, das festlegt, wie die Informationen in die generierte MARC-Datei exportiert werden. Um eigene Jobprofile zu erstellen, können Jobprofile in der App Einstellungen konfiguriert werden. Weitere Informationen sind unter [Einstellungen > Datenexport](https://info.gbv.de/pages/viewpage.action?pageId=849379672) zu finden.

## Instanz-UUIDs hochladen

Der Datenexport kann ausgelöst werden, indem die Liste der Datensatzidentifikatoren (Instances UUIDs) in einer .csv-Datei bereitstellt wird. Die Liste kann durch [Speichern der UUIDs der Datensätze](https://info.gbv.de/pages/viewpage.action?pageId=852492485) erstellt werden, die die Suchkriterien im Katalog erfüllen.

1.  In der Ansicht **Jobs** die Datei per **Drag & Drop** in das Feld ziehen oder auf **oder Datei auswählen** klicken, um die Datei auf dem Computer zu suchen.
2.  Im Fenster **Jobprofil zum Ausführen des Exports auswählen** das Jobprofil auswählen, das ausgeführt werden soll.
3.  Im Dialog **Job wirklich ausführen?** die Option **Ausführen** wählen. Das Fenster schließt sich und der Auftrag wird in der Ansicht Jobs unter dem Abschnitt Laufend angezeigt.

## CQL-Abfrage hochladen

Anmerkung: Die hochgeladene Datei, muss eine CQL-Datei sein.

1.  In der Ansicht **Jobs** die Datei per **Drag & Drop** in das Feld ziehen oder auf **oder Datei auswählen** klicken, um die Datei auf dem Computer zu suchen.
2.  Im Fenster **Jobprofil zum Ausführen des Exports auswählen** das Jobprofil auswählen, das ausgeführt werden soll.
3.  Im Dialog **Job wirklich ausführen?** die Option **Ausführen** wählen. Das Fenster schließt sich und der Auftrag wird in der Ansicht Jobs unter dem Abschnitt Laufend angezeigt.
