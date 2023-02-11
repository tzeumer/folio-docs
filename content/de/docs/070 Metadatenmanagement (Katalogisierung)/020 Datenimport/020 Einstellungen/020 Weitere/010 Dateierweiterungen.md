---
title: "Dateierweiterungen"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-datenimport, by-folio, cat-einstellungen, for-admin]
weight: 10
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/settings/settings_data_import/settings_data_import/#settings--data-import--file-extensions) & [GBV](https://info.gbv.de/display/FOLIOGBVEXTERN/Einstellungen+(Datenimport):+Dateierweiterungen)
    "
---

Dateierweiterungen werden verwendet, um zu konfigurieren, welche Dateiformate für den Import zugelassen sind und welche blockiert sind und nicht importiert werden können. Es kann zum Beispiel gewünscht sein, dass .mrk-Dateien für den Import gesperrt werden. Wenn eine Datei eine Erweiterung hat, die nicht in der Liste enthalten ist, kann die Datei hochgeladen werden und der Import wird versucht. Wenn es Probleme mit der Dateistruktur oder den Daten gibt, schlägt der Import fehl, was im Datenimportprotokoll vermerkt wird.

## Dateierweiterung hinzufügen

1.  In der Ansicht **Dateierweiterungen** auf **Aktionen > Neue Dateierweiterung** klicken.
2.  Im Fenster **Neue Dateierweiterungsmapping** eine **Beschreibung** der Dateierweiterung eingeben.
3.  Die **Dateierweiterung** in das Feld eingeben.
4.  Optional: Wenn die Erweiterung für den Import gesperrt werden soll, **Import blockieren** wählen.
5.  Im Feld **Datentyp(en)** die Datentypen auswählen, für die die Erweiterung gilt: MARC und/oder EDIFACT.
6.  Auf **Als Dateierweiterung speichern & schließen** klicken. Eine Bestätigungsmeldung wird angezeigt und die Dateierweiterung wird hinzugefügt.

## Dateierweiterung suchen

Die Suchleiste verwenden, um nach Dateierweiterungen in der Tabelle Dateierweiterungen zu suchen.

Die Tabelle Dateierweiterungen enthält die folgenden Spalten:

-   **Dateierweiterung**. Die Dateierweiterung.
-   **Import blockieren**. Ob ein Import der Dateierweiterung erlaubt oder blockiert ist.
-   **Datentyp(en)**. Der Datentyp, der mit der Dateierweiterung verknüpft ist.

Es kann auf einen beliebigen Spaltennamen geklickt werden, um nach dieser Spalte zu sortieren.

## Dateierweiterung anzeigen

Um die Details eines Dateierweiterungsprofils anzuzeigen, wie folgt vorgehen:

-   In der Ansicht **Dateierweiterungen** die Dateierweiterung suchen, die angezeigt werden soll und sie auswählen. Das Fenster mit den Details der Dateierweiterung wird angezeigt.

## Dateierweiterung bearbeiten

1.  In der Ansicht **Dateierweiterungen** die Dateierweiterung suchen, die bearbeitet werden soll und sie auswählen.
2.  In der Ansicht mit den **Details der Dateierweiterung** auf **Aktionen > Bearbeiten** klicken.
3.  die gewünschten Änderungen an der Dateierweiterung vornehmen.
4.  Auf **Als Dateierweiterung speichern & schließen** klicken. Eine Bestätigungsmeldung wird angezeigt und die Dateierweiterung wird aktualisiert.

## Dateierweiterung löschen

1.  In der Ansicht **Dateierweiterungen** die Dateierweiterung suchen, die gelöscht werden soll und sie auswählen.
2.  In der Ansicht mit den **Details der Dateierweiterung** auf **Aktionen > Löschen** klicken.
3.  Im Dialog **Dateierweiterung löschen** auf **Löschen** klicken. Es wird eine Bestätigungsmeldung angezeigt und die Dateierweiterung wird gelöscht.
