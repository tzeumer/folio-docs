---
title: "Jobprofile"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-datenexport, by-folio, cat-einstellungen, for-admin, meta-workflow_sammlung]
weight: 10
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/settings/settings_data_export/settings_data_export/#settings--data-export--job-profiles) & [GBV](https://info.gbv.de/display/FOLIOGBVEXTERN/Einstellungen+(Datenexport):+Jobprofile)
    "
---

Beim Exportieren von Daten wird jeder Export mit einem Jobprofil verknüpft. Das Jobprofil bietet eine Möglichkeit, eine bestimmte Liste von Datensatzidentifikatoren mit einem Feldmappingprofil zu verbinden. Das Feldmappingprofil bestimmt, wie die Daten aus FOLIO-Datensätzen in der generierten MARC-Datei erscheinen.

Bevor mit der Konfiguration von Jobprofilen begonnen wird, sollten zunächst die Feldmappingprofile konfiguriert werden. Weitere Informationen sind unter Einstellungen > Datenexport > Feldmappingprofile zu finden.

## Standard Jobprofil für den Export

Das System wird mit einem Standard Jobprofil ausgeliefert, das mit dem Standard Feldmappingprofil verknüpft ist ("Default holdings export job profile" und "Default instances export job profile"). Datensätze, die mit dem Standard Jobprofil exportiert werden, erzeugen eine MARC-Datei mit Informationen zu den angegebenen Datensatz-IDs.

Wenn das Standard-Jobprofil verwendet wird, werden vereinfachte bibliografische MARC-Datensätze für Instanzen ohne zugrunde liegende MARC-Datensätze erzeugt. Für Instanzen mit zugrunde liegenden MARC-Datensätzen, die in SRS gespeichert sind, werden diese Datensätze beim Export verwendet.

## Jobprofil für den Export erstellen

1.  In der Ansicht **Jobprofile** auf **Neu** klicken.
2.  Einen **Namen** für das Jobprofil eingeben.
3.  Ein **Feldmappingprofil** aus der Dropdown-Liste wählen. Feldmappingprofile werden in den Einstellungen erstellt. Weitere Informationen sind unter [Einstellungen > Datenexport > Feldmappingprofile]({{< ref "020 Feldmappingprofile" >}}) zu finden.
4.  Optional: Eine **Beschreibung** für das Jobprofil eingeben.
5.  Auf **Speichern & schließen** klicken. Eine Bestätigungsmeldung wird angezeigt und das Jobprofil wird erstellt.

## Jobprofil für den Export suchen

Die Suchleiste verwenden, um nach Profilen in der Tabelle Jobprofile zu suchen.

Die Tabelle Jobprofile enthält die folgenden Spalten:

* **Name**. Name des Jobprofils.
* **Aktualisiert**. Datum, an dem das Jobprofil zuletzt aktualisiert wurde.
* **Aktualisiert von**. Person, die das Jobprofil zuletzt aktualisiert hat.

Es kann auf einen beliebigen Spaltennamen geklickt werden, um nach dieser Spalte zu sortieren.

## Jobprofil für den Export anzeigen

Um die Details eines Jobprofils anzuzeigen, wie folgt vorgehen:

* In der Ansicht **Jobprofile** das Profil suchen, das angezeigt werden soll und es auswählen. Das Fenster mit den **Details des Jobprofils für den Export** wird angezeigt.

## Jobprofil für den Export bearbeiten

Anmerkung: Sobald ein Jobprofil für einen Datenexportauftrag verwendet wurde, kann es nicht mehr bearbeitet oder gelöscht werden.

1.  In der Ansicht **Jobprofile** das Profil suchen, das bearbeitet werden soll und es auswählen.
2.  Im Fenster mit den **Details des Jobprofils für den Export** auf **Aktionen > Bearbeiten** klicken.

## Jobprofil für den Export duplizieren

1.  In der Ansicht **Jobprofile** das Profil suchen, das dupliziert werden soll und es auswählen.
2.  Im Fenster mit den **Details des Jobprofils für den Export** auf **Aktionen > Duplizieren** klicken.

## Jobprofil für den Export löschen

Anmerkung: Sobald ein Jobprofil für einen Datenexportauftrag verwendet wurde, kann es nicht mehr bearbeitet oder gelöscht werden.

1.  In der Ansicht **Jobprofile** das Profil suchen, das gelöscht werden soll und es auswählen.
2.  Im Fenster mit den **Details des Jobprofils für den Export** auf **Aktionen > Löschen** klicken.
3.  Im Dialog **Jobprofil löschen** auf **Löschen** klicken. Es wird eine Bestätigungsmeldung angezeigt und das Jobprofil wird gelöscht.
