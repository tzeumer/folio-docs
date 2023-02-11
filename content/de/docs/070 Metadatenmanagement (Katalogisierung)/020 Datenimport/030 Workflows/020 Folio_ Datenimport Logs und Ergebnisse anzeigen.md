---
title: "Folio: Datenimport Logs und Ergebnisse anzeigen"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-datenimport, by-folio, cat-workflows, for-anwender]
weight: 20
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/metadata/data-import/#viewing-import-logs) & [GBV](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio:+Datenimport+Logs+und+Ergebnisse+anzeigen)
    "
---

## Importprotokolle anzeigen

Sobald ein Import abgeschlossen ist, unabhängig davon, ob er fehlerfrei oder mit Fehlern abgeschlossen wurde oder fehlgeschlagen ist, wird er in der Tabelle Logs in der Ansicht Logs angezeigt.

Die Tabelle Protokolle enthält die folgenden Spalten:

-   **Dateiname**. Name der MARC-Datei, die importiert wurde.
-   **Status**. Status des Imports: Abgeschlossen, Abgeschlossen mit Fehlern oder Fehlgeschlagen.
-   **Datensätze**. Anzahl der Datensätze im Import.
-   **Jobprofil**. Name des verwendeten Jobprofils.
-   **Lauf beendet**. Datum und Uhrzeit, zu der der Import beendet wurde.
-   **Ausgeführt von**. Person oder System, von dem der Import erstellt wurde.
-   **ID**. Identifikationsnummer des Imports.

Es kann auf einen beliebigen Spaltennamen geklickt werden, um nach dieser Spalte zu sortieren.

### Alle Protokolle anzeigen

Protokolle werden nie gelöscht. Die neun aktuellsten Protokolle werden in der Tabelle Protokolle in der Ansicht Protokolle angezeigt. Um alle Protokolle anzuzeigen, in der Ansicht **Protokolle** auf **Alle anzeigen** klicken. Das Fenster Protokolle wird angezeigt.

#### Suchen und Filtern von Protokollen

Nachdem alle Protokolle angezeigt werden, kann in der Ansicht **Suchen & Filtern** nach Dateien gesucht werden. Um nach einer Datei zu suchen, die Bedingungen in das Feld eingeben. Die Dropdown-Liste **Schlüsselwort** wählen, um in einem der folgenden Felder zu suchen:

-   **Schlüsselwort (ID, Dateiname)**. Schlüsselwortsuche über die Felder ID und Dateiname.
-   **ID**. Identifikation des Imports.
-   **Dateiname**. Name der Importdatei.

Es kann auch nach Protokollen gesucht werden, indem einer der Filter in der Ansicht **Suchen & Filtern** ausgewählt wird. Außerdem können die Filter nach einer Suche angewendet werden, um die Ergebnisse einzuschränken. Weitere Informationen sind in den folgenden Abschnitten zu finden.

##### Fehler beim Import

Um Protokolle danach zu filtern, ob sie Fehler enthalten oder nicht, eine der folgenden Optionen wählen:

-   **Nein**. Protokolle, die keine Fehler enthalten.
-   **Ja**. Protokolle mit Fehlern.

##### Datum

Folgendermaßen vorgehen, um nach Protokollen anhand des Datums zu suchen, an dem sie ausgeführt wurden:

1.  In der Ansicht **Suchen & Filtern** auf **Datum** klicken.
2.  Ein Startdatum in das Feld **Von** und ein Enddatum in das Feld **Bis** eingeben.
3.  Auf **Anwenden** klicken. Die Suchergebnisse werden in der Ansicht Protokolle angezeigt.

##### Jobprofil

Folgendermaßen vorgehen, um anhand des Jobprofils nach Protokollen zu suchen:

1.  In der **Ansicht Suchen & Filtern** auf **Jobprofil** klicken.
2.  Das gewünschte Jobprofil aus der Dropdown-Liste wählen. Die Suchergebnisse werden in der Ansicht Logs angezeigt.

##### Person

Um nach Protokollen auf der Grundlage der Person zu suchen, die den Bericht ausgeführt hat, wie folgt vorgehen:

1.  In der **Ansicht Suchen & Filtern** auf **Person** klicken.
2.  Die gewünschte Person aus der Dropdown-Liste auswäheln. Die Suchergebnisse werden in der Ansicht Protokolle angezeigt.

##### Katalog-Einzeldatensatzimporte

Einzeldatensatzimporte sind Datensätze, die aus einer externen Quelle wie OCLC geladen werden. Diese Datensätze werden über die App Katalog importiert, aber die Protokolle werden in Datenimport angezeigt.

Um Protokolle danach zu filtern, ob es sich um Einzeldatensatzimporte aus dem Katalog handelt oder nicht, in der Ansicht **Suchen & Filtern** auf **Einzeldatensatzimporte aus dem Katalog** klicken und eine der folgenden Optionen auswählen:

-   **Nein**. Alle anderen Arten von Protokollen.
-   **Ja**. Protokolle für Katalog-Einzelsatzimporte.

## Abrufen von Datenexportergebnissen

Bei allen Exporten mit dem Status Abgeschlossen oder Abgeschlossen mit Fehlern kann auf den Dateinamen in der Ansicht Protokolle geklickt werden, um die Ergebnisse des Datenexports abzurufen. Abhängig vom Browser und dessen Konfiguration wird die Datei automatisch heruntergeladen oder es wird aufgefordert, sie zu speichern.

## Fehlerbehebung bei fehlgeschlagenen Importen

Bei allen Importen mit dem Status Fehlgeschlagen oder Abgeschlossen mit Fehlern in die Zeile des Imports klicken, um das Fehlerprotokoll anzuzeigen. Für alle fehlgeschlagenen Importe  wird keine MARC-Datei erstellt.
