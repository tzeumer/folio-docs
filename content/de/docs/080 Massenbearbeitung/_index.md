---
title: "📱Massenbearbeitung"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-massenbearbeitung, by-folio, cat-berechtigungen, for-anwender]
weight: 80
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/bulk-edit/ ) & [GBV](https://info.gbv.de/pages/viewpage.action?pageId=845709320)
    "
---

## Einführung

Mit der App Massenbearbeitung können Änderungen an vielen verschiedenen Datensätzen auf einmal vorgenommen werden.

In Nolana werden Massenbearbeitungen für drei Datensatztypen unterstützt

-   **Personen**: Es können Personendatensätze über das CSV-Verfahren von FOLIO bearbeitet werden, bei dem ein Abzug des Personendatensatzes heruntergeladen, in der Datei Änderungen an den Datensätzen vorgenommen und die Datei dann zurück in die App Massenbearbeitung hochgeladen wird, wo die Änderungen übernommen werden. Es kann auch das In-App-Verfahren von FOLIO verwendet werden, bei dem eine Liste von Identifikatoren hochgeladen wird, um die Personen zu finden, die gewünschten Feldänderungen in der App einzurichten und dann den Massenbearbeitungsauftrag ausführen, um die Änderungen anzuwenden.
-   **Exemplare im Katalog**: Über das In-App-Verfahren von FOLIO können Exemplardatensätze in der App Katalog bearbeitet werden. Dazu wird eine Liste von Identifikatoren hochgeladen, um die Exemplare zu finden, die gewünschten Feldänderungen in der App einzurichten und dann den Massenbearbeitungsauftrag auszuführen, um die Änderungen anzuwenden.
-   **Katalog-Bestände**: Über das In-App-Verfahren von FOLIO können Bestandsdatensätze in der App Katalog bearbeitet werden. Dazu wird eine Liste von Identifikatoren hochgeladen, um die Exemplare zu finden, die gewünschten Feldänderungen in der App eingerichtet und dann den Massenbearbeitungsauftrag ausgeführt, um die Änderungen anzuwenden.

Andere Arten von Datensätzen werden in zukünftigen Versionen hinzugefügt.

## Berechtigungen

Die unten aufgeführten Berechtigungen ermöglichen Ihnen die Interaktion mit der App Bulk Edit und legen fest, was Sie in der App tun können und was nicht. Sie können Personen in der App Benutzer Berechtigungen zuweisen. Wenn einer Person keine dieser Berechtigungen zugewiesen ist, kann sie die App Bulk Edit und alle damit verbundenen Informationen nicht sehen.

-   **Massenbearbeitung: (CSV) Löschen**. (Bulk Edit: (CSV) Delete)
    Mit dieser Berechtigung kann die Person mehrere Personendatensätze in der Massenbearbeitung mit dem CSV-Verfahren löschen.
-   **Massenbearbeitung: (CSV) Bearbeiten**. (Bulk Edit: (CSV) Edit)
    Diese Berechtigung erlaubt es der Person, ein Feld in mehreren Personendatensätzen in der Massenbearbeitung mit dem CSV-Verfahren zu bearbeiten.

-   **Massenbearbeitung: (CSV) Anzeigen**. (Bulk Edit: (CSV) View)
    Mit dieser Berechtigung kann der Person in der Massenbearbeitung mit dem CSV-Verfahren eine Liste der identifizierten Personendatensätze anzeigen.

-   **Massenbearbeitung: In-App - Löschen**. (Bulk Edit: In App - Delete)
    Diese Berechtigung erlaubt es der Personen, mehrere Katalogdaten in der App Massenbearbeitung zu löschen.

-   **Massenbearbeitung: In-App - Bearbeiten**. (Bulk Edit: In App - Edit)
    Diese Berechtigung erlaubt es der Personen, ein Feld in mehreren Katalogdaten in der App Massenbearbeitung zu bearbeiten.

-   **Massenbearbeitung: In-App - Anzeigen**. (Bulk Edit: In App - View)
    Diese Berechtigung ermöglicht es Personen, eine Liste von Katalogdaten in der App Massenbearbeitung anzuzeigen.

Je nachdem, wie die Bibliothek Massenbearbeitungsaufträge ausführt, benötigen Personen möglicherweise auch Berechtigungen in anderen Modulen, wie Export Manager, Katalog, Personen und Einstellungen.

## Arten von Massenbearbeitungen: CSV und In-App

Die App Massenbearbeitung unterstützt zwei Methoden zur Bearbeitung von Datensätzen: CSV und In-App.

### CSV-Verfahren

Das CSV-Verfahren in der App Massenbearbeitung verwendet eine .csv-Datei, um Datensätze anzuzeigen, die einem ausgewählten **Datensatzidentifikator** entsprechen. Änderungen werden an dem entsprechenden Datensatz vorgenommen, in der .csv-Datei gespeichert und durch Hochladen der bearbeiteten .csv-Datei in der App Massenbearbeitung bestätigt.

Anmerkung: Wenn Microsoft Excel verwendet wird, kann es bei der Verarbeitung von CSV-Dateien zu unerwarteten Datenänderungen kommen, insbesondere bei Datums- und Zeitfeldern. Es wird empfohlen, die CSV-Daten in einem Texteditor zu überprüfen, um sicherzustellen, dass mit dem CSV-Verfahren keine unerwarteten Änderungen an den Datensätzen vorgenommen werden.

### In-App-Verfahren

Das In-App-Verfahren in der App Massenbearbeitung ermöglicht es dem Personen, im Browserfenster nach mehreren Datensätzen zu suchen und diese zu ändern.
