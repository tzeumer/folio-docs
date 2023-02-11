---
title: "MARC-Felder mit Schreibschutz"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-datenimport, by-folio, cat-einstellungen, for-admin]
weight: 20
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/settings/settings_data_import/settings_data_import/#settings--data-import--marc-field-protection) & [GBV](https://info.gbv.de/display/FOLIOGBVEXTERN/Einstellungen+(Datenimport):+MARC-Felder+mit+Schreibschutz)
    "
---

Diese Einstellung verwenden, um ein bestimmtes MARC-Feld ganz oder teilweise vor Aktualisierungen zu schützen, wenn neue Kopien von MARC-Datensätzen importiert werden.

Der Feldschutz unterscheidet sich für wiederholbare und nicht wiederholbare Felder. Wenn das Feld wiederholbar ist, wird das vorhandene Feld beibehalten und ein neues Feld mit den neuen Daten erstellt. Wenn das Feld nicht wiederholbar ist, wird das vorhandene Feld beibehalten und die aktualisierten Daten werden verworfen.

## MARC-Feldschutz hinzufügen

Das Sternchen (\*) ist der einzige verfügbare Platzhalter. Wenn er verwendet wird, steht er für alles.

1.  In der Ansicht **MARC-Felder mit Schreibschutz** auf **Neu** klicken.
2.  Das **Feld** eingeben.
3.  Ist gewünscht, dass alle Daten in diesem Feld geschützt werden, unabhängig von Indikator, Unterfeld und Daten, dann ein Sternchen (\*) in jedem Feld stehen lassen. Ansonsten die Felder ausfüllen.
4.  Auf **Speichern** klicken. Das MARC-Feld wird der Tabelle hinzugefügt.

## MARC-Feldschutz bearbeiten

1.  Klicken Sie in der Ansicht **MARC-Felder mit Schreibschutz** auf das Bleistiftsymbol in der Zeile des Feldes klicken, das bearbeitet werden soll.
2.  Die gewünschten Änderungen vornehmen.
3.  Auf **Speichern** klicken. Das MARC-Feld wird aktualisiert.

## MARC-Feldschutz löschen

1.  Klicken Sie in der Ansicht **MARC-Felder mit Schreibschutz** auf das Mülleimersymbol in der Zeile des Feldes klicken, das gelöscht werden soll.
2.  Im Dialog **MARC-Feld mit Schreibschutz löschen** auf **Löschen** klicken. Es wird eine Bestätigungsmeldung angezeigt und der MARC-Feldschutz wird gelöscht.
