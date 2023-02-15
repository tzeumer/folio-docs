---
title: "Jobprofile"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-datenimport, by-folio, cat-einstellungen, for-admin, meta-workflow_sammlung]
weight: 10
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/settings/settings_data_import/settings_data_import/#settings--data-import--job-profiles) <!-- & [GBV](https://info.gebev.de/display/FOLIOGBVEXTERN/Einstellungen+(Datenimport):+Jobprofile) -->
    "
---

{{% pageinfo %}}
Hinweis: Es sind eigentlich mehrere einzelne Workflows. Ob einzeln oder wie hier zusammengefasst besser ist, ist noch unentschieden.
{{% /pageinfo %}}

Jobprofile definieren die Art des Imports auf der höchsten Ebene. Ein Jobprofil enthält alle Schritte, die für einen individuellen Datenimport erforderlich sind: Feldmappings, Aktion und Abgleich (Matchingprofile).

## Jobprofil für Importjob erstellen

1.  In der Ansicht **Jobprofile** auf **Aktionen > Neues Jobprofil** klicken.
2.  Im Fenster **Neues Jobprofil** einen **Namen** für das Jobprofil eingeben.
3.  Den **akzeptierten Datentyp** wählen: MARC oder EDIFACT. Dies ist das akzeptierte Format des importierten Datensatzes.
4.  Optional: Eine **Beschreibung** für das Jobprofil eingeben.
5.  Im Akkordeon **Übersicht** können **Matchprofile** und **Aktionsprofile** hinzugefügt oder entfernt werden. Wenn ein **Matchprofil** hinzugefügt wird, wird dieser Vorgang wiederholt, solange Übereinstimmungen gefunden oder keine Übereinstimmungen gefunden werden. Auf diese Weise können mehrere **Matchprofile** miteinander verschachtelt werden, um einen Abgleich für mehrere Datenfelder zu ermöglichen. Alle **Aktionsprofile** oder **Matchprofile**, die hinzugefügt werden sollen, müssen bereits existieren, bevor sie dem **Jobprofil** hinzugefügt werden.
6.  Auf **Als Profil speichern & schließen** klicken. Es erscheint eine Bestätigungsmeldung und der Auftrag wird erstellt.

## Jobprofil für Importjob suchen

Die Suchleiste verwenden, um nach Jobprofilen in der Tabelle Jobprofile zu suchen.

Die Tabelle Jobprofile enthält die folgenden Spalten:

* **Name**. Name des Jobprofils.
* **Tags**. Alle dem Jobprofil zugewiesenen Tags
* **Aktualisiert**. Datum, an dem das Jobprofil zuletzt aktualisiert wurde.
* **Aktualisiert von**. Person, die das Jobprofil zuletzt aktualisiert hat.

Es kann auf einen beliebigen Spaltennamen geklickt werden, um nach dieser Spalte zu sortieren.

## Jobprofil für Importjob ansehen

Um die Details eines Jobprofils anzuzeigen, folgendermaßen vorgehen:

* In der Ansicht **Jobprofile** das Profil suchen, das angezeigt werden soll und es auswählen. Das Fenster **Details zum Jobprofil** wird angezeigt.

## Jobprofil für Importjob bearbeiten

* In der Ansicht **Jobprofile** das Profil suchen, das bearbeitet werden soll und es auswählen.
* In der Ansicht **Details zum Jobprofil** auf **Aktionen > Bearbeiten** klicken.
* die gewünschten Änderungen an dem Jobprofil vornehmen.
* Auf **Als Profil speichern & schließen** klicken. Eine Bestätigungsmeldung wird angezeigt und das Jobprofil wird aktualisiert.

## Jobprofil für Importjob duplizieren

* In der Ansicht **Jobprofile** das Profil suchen, das dupliziert werden soll und es auswählen.
* In der Ansicht **Details zum Jobprofil** auf **Aktionen > Duplizieren** klicken.
* Im Fenster **Neues Jobprofil** die gewünschten Änderungen vornehmen.
* Auf **Als Profil speichern & schließen** klicken. Es wird eine Bestätigungsmeldung angezeigt und das doppelte Jobprofil wird erstellt.

## Jobprofil für Importjob löschen

* In der Ansicht **Jobprofile** das Profil suchen, das gelöscht werden soll und es auswählen.
* In der Ansicht **Details zum Jobprofil** auf **Aktionen > Löschen** klicken.
* Im Dialog **Jobprofil löschen** auf **Löschen** klicken. Eine Bestätigungsmeldung wird angezeigt und das Jobprofil wird gelöscht.

## Jobprofil für Importjob mit Tag versehen

* In der Ansicht **Jobprofile** das Profil suchen, das getaggt werden soll und es auswählen.
* In der Ansicht **Details zum Jobprofil** auf **Tags** klicken.
* Im Feld **Tags** entweder ein Tag auswählen oder ein Tag eingeben. Das Tag wird automatisch für das Profil angewendet.

## Jobprofil für Importjob exportieren

Das Exportieren eines Jobprofils ist derzeit noch nicht vorgesehen.
