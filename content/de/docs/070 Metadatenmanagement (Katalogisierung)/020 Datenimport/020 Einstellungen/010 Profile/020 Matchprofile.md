---
title: "Matchprofile"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-datenimport, by-folio, cat-einstellungen, for-admin, meta-workflow_sammlung]
weight: 20
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/settings/settings_data_import/settings_data_import/#settings--data-import--match-profiles) & [GBV](https://info.gbv.de/display/FOLIOGBVEXTERN/Einstellungen+(Datenimport):+Matchprofile)
    "
---

{{% pageinfo %}}
Hinweis: Es sind eigentlich mehrere einzelne Workflows. Ob einzeln oder wie hier zusammengefasst besser ist, ist noch unentschieden.
{{% /pageinfo %}}

Matchprofile definieren die Übereinstimmung zwischen einem eingehenden Datensatz und einem vorhandenen Datensatz. Matchprofile können für mehrere Jobprofile verwendet werden.

Bevor ein Matchprofil erstellt wird, sollten zunächst Aktionsprofile und Feldmappingprofile erstellt werden.

## Matchprofil für Importjob erstellen

1.  In der Ansicht **Matchprofile** auf **Aktionen > Neues Matchprofil** klicken.
2.  Im Fenster **Neues Matchprofil** einen **Namen** für das Matchprofil eingeben.
3.  Optional: Eine **Beschreibung** des Matchprofils eingeben.
4.  Im Abschnitt **Details** das Format des eingehenden Datensatzes wählen und dann das Format des vorhandenen Datensatzes wählen, mit dem ein Abgleich vorgenommen werden soll.
5.  Im Abschnitt **Matchkriterien** das abzugleichende Feld aus dem eingehenden Datensatz und das entsprechende Feld aus dem vorhandenen Datensatz wählen, das abgeglichen werden soll.
6.  Auf **Als Profil speichern & schließen** klicken. Es erscheint eine Bestätigungsmeldung und der Auftrag wird erstellt.

## Matchprofil für Importjob suchen

Die Suchleiste verwenden, um nach Matchprofilen in der Tabelle Matchprofile zu suchen.

Die Tabelle Matchprofile enthält die folgenden Spalten:

* **Name**. Name des Matchprofils.
* **Match**. Die im Matchprofil enthaltene Übereinstimmung.
* **Tags**. Alle dem Matchprofil zugewiesenen Tags
* **Aktualisiert**. Datum, an dem das Matchprofil zuletzt aktualisiert wurde.
* **Aktualisiert von**. Person, die das Matchprofil zuletzt aktualisiert hat.

Es kann auf einen beliebigen Spaltennamen geklickt werden, um nach dieser Spalte zu sortieren.

## Matchprofil für Importjob ansehen

Um die Details eines Matchprofils anzuzeigen, folgendermaßen vorgehen:

* In der Ansicht **Matchprofile** das Profil suchen, das angezeigt werden soll und es auswählen. Das Fenster **Details zum Matchprofil** wird angezeigt.

## Matchprofil für Importjob bearbeiten

1.  In der Ansicht **Matchprofile** das Profil suchen, das bearbeitet werden soll und es auswählen.
2.  In der Ansicht **Details zum Matchprofil** auf **Aktionen > Bearbeiten** klicken.
3.  die gewünschten Änderungen an dem Matchprofil vornehmen.
4.  Auf **Als Profil speichern & schließen** klicken. Eine Bestätigungsmeldung wird angezeigt und das Matchprofil wird aktualisiert.

## Matchprofil für Importjob duplizieren

1.  In der Ansicht **Matchprofile** das Profil suchen, das dupliziert werden soll und es auswählen.
2.  In der Ansicht **Details zum** **Matchprofil** auf **Aktionen > Duplizieren** klicken.
3.  Im Fenster **Neues Matchprofil** die gewünschten Änderungen vornehmen.
4.  Auf **Als Profil speichern & schließen** klicken. Es wird eine Bestätigungsmeldung angezeigt und das doppelte Matchprofil wird erstellt.

## Matchprofil für Importjob löschen

1.  In der Ansicht **Matchprofile** das Profil suchen, das gelöscht werden soll und es auswählen.
2.  In der Ansicht **Details zum** **Matchprofil**  auf **Aktionen > Löschen** klicken.
3.  Im Dialog **Matchprofil löschen** auf **Löschen** klicken. Eine Bestätigungsmeldung wird angezeigt und das Matchprofil wird gelöscht.

## Matchprofil für Importjob mit Tag versehen

1.  In der Ansicht **Matchprofile** das Profil suchen, das getaggt werden soll und es auswählen.
2.  In der Ansicht **Details zum** **Matchprofil** auf **Tags** klicken.
3.  Im Feld **Tags** entweder ein Tag auswählen oder ein Tag eingeben. Das Tag wird automatisch für das Profil angewendet.

## Matchprofil für Importjob exportieren

Das Exportieren eines Matchprofils ist derzeit noch nicht vorgesehen.
