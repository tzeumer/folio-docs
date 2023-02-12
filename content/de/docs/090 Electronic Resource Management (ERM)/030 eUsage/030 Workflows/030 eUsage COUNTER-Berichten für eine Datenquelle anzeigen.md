---
title: "eUsage COUNTER-Berichten für eine Datenquelle anzeigen"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-e_usage, by-folio, cat-workflows, for-anwender]
weight: 30
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/erm/eusage/#viewing-stored-counter-reports-for-a-usage-data-provider) & [GBV](https://info.gbv.de/pages/viewpage.action?pageId=847904776)
    "
---

1.  Den Datenquellen-Anbieter suchen, für den die gespeicherten Berichte angezeigt werden sollen und ihn auswählen.
2.  In der Ansicht **Datenquellen-Details** auf **COUNTER-Berichte** klicken.
3.  Wenn Berichte gespeichert sind, werden sie für jedes Jahr in einer eigenen Tabelle angezeigt. Auf das Jahr klicken, das angezeigt werden soll oder auf **Alle Jahre ausklappen** klicken.

Die Tabelle **COUNTER-Berichte** zeigt eine Zeile für jeden Berichtstyp und eine Spalte für jeden Monat an. Wenn ein Bericht gespeichert ist oder versucht wurde, ihn abzurufen, wird in der entsprechenden Zelle der Tabelle eine Schaltfläche Bericht angezeigt. Die Schaltflächen zeigen den Status des Berichts mit einem Symbol an:

-   **Grün/Häkchen**. Ein gültiger Bericht ist für den Monat verfügbar.
-   **Orange/Ausrufezeichen**. Der Bericht wurde abzurufen versucht, ist aber fehlgeschlagen. Der Harvester versucht es beim nächsten Abruf erneut.
-   **Rot/Kreuz**. Der Bericht hat  die in den Einstellungen festgelegte maximale Anzahl von Abrufversuchen erreicht. Um einen weiteren Abrufversuch zu unternehmen, muss der Bericht gelöscht werden. Weitere Informationen sind unter Festlegen der maximalen Anzahl von Ernteversuchen und Löschen von Berichten zu finden.

In der Tabelle COUNTER-Berichte auf eine Schaltfläche Bericht klicken. Das Dialogfeld Berichtsinfo wird mit zusätzlichen Informationen über den Bericht angezeigt:

-   **Datenquelle**. Der Name der Datenquelle für die Nutzungsdaten.
-   **Typ**. Der Berichtstyp.
-   **Datum**. Der Zeitraum für den Bericht, immer ein Monat.
-   **Informationen**. Wenn der Bericht nicht korrekt abgerufen werden konnte, wird hier die vom SUSHI-Dienst bereitgestellte Fehlermeldung angezeigt.
-   **Fehlversuche**. Anzahl der versuchten Abrufe, die auch die Anzahl der maximalen Versuche ist.
-   **Manuelle Änderungen**. Wenn der Bericht manuell geändert wurde, erscheint diese Überschrift zusammen mit dem Grund, warum der Bericht manuell bearbeitet wurde.
-   **Aktionen**. Mögliche Aktionen, weitere Informationen sind unter Löschen von Berichten und Herunterladen von Berichten zu finden.
