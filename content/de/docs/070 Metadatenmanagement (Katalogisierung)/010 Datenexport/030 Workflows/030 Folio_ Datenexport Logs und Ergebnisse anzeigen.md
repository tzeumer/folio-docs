---
title: "Folio: Datenexport Logs und Ergebnisse anzeigen"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-datenexport, by-folio, cat-workflows, for-anwender]
weight: 30
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/metadata/data-export/#viewing-export-logs) & [GBV](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio:+Datenexport+Logs+und+Ergebnisse+anzeigen)
    "
---

Sobald ein Export abgeschlossen ist, unabhängig davon, ob er fehlerfrei oder mit Fehlern abgeschlossen wurde oder fehlgeschlagen ist, wird er in der Tabelle Protokolle in der Ansicht Protokolle angezeigt.

Die Tabelle Protokolle enthält die folgenden Spalten:

-   **Dateiname**. Name der MARC-Datei, die erstellt wurde.
-   **Status**. Status des Exports: Abgeschlossen, Abgeschlossen mit Fehlern oder Fehlgeschlagen.
-   **Gesamt**. Anzahl der Datensätze im Export.
-   **Fehlgeschlagen**. Anzahl der Datensätze, die fehlgeschlagen sind.
-   **Jobprofil**. Name des verwendeten Jobprofils.
-   **Lauf beendet**. Datum und Uhrzeit, zu der der Export beendet wurde.
-   **Ausgeführt von**. Person oder System, von dem der Export erstellt wurde.
-   **ID**. Identifikationsnummer des Exports.

Es kann auf einen beliebigen Spaltennamen geklickt werden, um nach dieser Spalte zu sortieren.

## Alle Protokolle anzeigen

Protokolle werden nie gelöscht. Die fünfundzwanzig aktuellsten Protokolle werden in der Tabelle Protokolle in der Ansicht Protokolle angezeigt. Um alle Protokolle anzuzeigen, in der Ansicht Protokolle auf **Alle anzeigen** klicken. Das Fenster Protokolle wird angezeigt.

## Abrufen von Datenexport-Ergebnissen

Bei allen Exporten mit dem Status Abgeschlossen oder Abgeschlossen mit Fehlern kann auf den Dateinamen in der Ansicht Protokolle geklickt werden, um die Ergebnisse des Datenexports abzurufen. Je nach Browser und dessen Konfigurationen wird die Datei automatisch heruntergeladen oder es wird aufgefordert, sie zu speichern.

## Fehlerbehebung bei fehlgeschlagenen Exporten

Bei allen Exporten mit dem Status Fehlgeschlagen oder Abgeschlossen mit Fehlern in die Zeile des Exports klicken, um das Fehlerprotokoll anzuzeigen. Für alle fehlgeschlagenen Exporte wird keine MARC-Datei erstellt.
