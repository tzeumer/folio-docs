---
title: "Feldmappingprofile"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-datenexport, by-folio, cat-einstellungen, for-admin, meta-workflow_sammlung]
weight: 20
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/settings/settings_data_export/settings_data_export/#settings--data-export--job-profiles ) & [GBV](https://info.gbv.de/display/FOLIOGBVEXTERN/Einstellungen+(Datenexport):+Feldmappingprofile)
    "
---

Das System verfügt über ein standardmäßiges Feldmappingprofil, das mit dem Standard-Jobprofil verknüpft ist. Das Feldmappingprofil bestimmt, wie die Daten aus FOLIO-Datensätzen in der generierten MARC-Datei erscheinen.

## Feldmappingprofil für Export erstellen

1.  In der Ansicht **Feldmappingprofile** auf **Neu** klicken.
2.  Im Fenster **Neues Feldmappingprofil** einen **Namen** für das Feldmappingprofil eingeben.
3.  Ein **Ausgabeformat** aus der Dropdown-Liste wählen. MARC ist die einzige Option.
4.  So viele **FOLIO-Datensatztypen** auswählen, wie zutreffend sind, indem die Checkbox neben der jeweiligen Option aktiviert wird (es muss mindestens eine Option ausgewählt werden):
    -   Quellendatenspeicher (gesamter Datensatz)
    -   Kataloginstanz (ausgewählte Felder)
    -   Bestand
    -   Exemplar
5.  Optional: Eine **Beschreibung** für das Feldmappingprofil eingeben.
6.  Optional: Um eine Transformation hinzuzufügen, auf **Transformationen hinzufügen** klicken und diesen Schritten folgen:
    -   Im Dialogfeld **Transformationen** auswählen das Suchfeld und die Filter verwenden, um die Transformationen zu finden, die dem Feldmappingprofil hinzugefügt werden soll.
    -   Für jede Transformation, die hinzugefügt werden soll, die **Checkbox** daneben aktivieren und die Felder Feldnummer, Indikatoren und Unterfeld ausfüllen. Unterfelder müssen mit einem $ beginnen.
    -   Sobald alle Transformationen hinzugefügt wurden, auf **Speichern & schließen** klicken. Es erscheint eine Bestätigungsmeldung und die Umwandlungen werden dem Feldmappingprofil hinzugefügt.
7.  Auf **Speichern & schließen** klicken. Es wird eine Bestätigungsmeldung angezeigt und das Feldmappingprofil wird erstellt.

## Feldmappingprofil für Export suchen

Die Suchleiste verwenden, um nach Profilen zu suchen, die in der Tabelle Feldmappingprofile enthalten sind.

Die Tabelle Feldmappingprofile enthält die folgenden Spalten:

-   **Name**. Name des Jobprofils.
-   **FOLIO-Datensatztyp**. Die Arten der im Export enthaltenen Datensätze: Quellendatenspeicher (gesamter Datensatz), Kataloginstanz (ausgewählte Felder), Bestand
    und/oder Exemplar.
-   **Format**. Format des exportierten Datensatzes.
-   **Aktualisiert**. Datum, an dem das Feldmappingprofil zuletzt aktualisiert wurde.
-   **Aktualisiert von**. Person oder System, die das Feldmappingprofil zuletzt aktualisiert hat.

Es kann auf einen beliebigen Spaltennamen geklickt werden, um nach dieser Spalte zu sortieren.

## Feldmappingprofil für Export anzeigen

Um die Details eines Feldmappingprofils anzuzeigen, wie folgt vorgehen:

-   In der Ansicht **Feldmappingprofile** das Profil suchen, das angezeigt werden soll und es auswählen. Das Fenster mit den **Details des Feldmappingprofils** wird angezeigt.

## Feldmappingprofil für Export bearbeiten

Anmerkung: Solange ein Feldmappingprofil einem Jobprofil zugewiesen ist, kann es nicht bearbeitet oder gelöscht werden.

-   In der Ansicht **Feldmappingprofile** das Profil suchen, das bearbeitet werden soll und es auswählen.
-   Im Detailfenster mit den **Details des Feldmappingprofils** auf **Aktionen > Bearbeiten** klicken.
-   Die Änderungen an dem Profil vornehmen.
-   Auf **Speichern & schließen** klicken. Eine Bestätigungsmeldung wird angezeigt und das Feldmappingprofil wird aktualisiert.

## Feldmappingprofil für Export duplizieren

-   In der Ansicht **Feldmappingprofile** das Profil suchen, das dupliziert werden soll und es auswählen.
-   Im Detailfenster mit den **Details des Feldmappingprofils** auf **Aktionen > Duplizieren** klicken.
-   Im Fenster **Neues Feldmappingprofil** die gewünschten Änderungen an dem duplizierten Profil vornehmen.
-   Auf **Speichern & schließen** klicken. Eine Bestätigungsmeldung wird angezeigt und das Feldmappingprofil wird erstellt.

## Feldmappingprofil für Export löschen

Anmerkung: Solange ein Feldmappingprofil einem Jobprofil zugewiesen ist, kann es weder bearbeitet noch gelöscht werden.

-   In der Ansicht **Feldmappingprofile** das Profil suchen, das gelöscht werden soll und es auswählen.
-   Im Detailfenster mit den **Details des Feldmappingprofils** auf **Aktionen > Löschen** klicken.
-   Im Dialogfeld **Feldmappingprofil löschen** auf **Löschen** klicken. Es wird eine Bestätigungsmeldung angezeigt und das Feldmappingprofil wird gelöscht.
