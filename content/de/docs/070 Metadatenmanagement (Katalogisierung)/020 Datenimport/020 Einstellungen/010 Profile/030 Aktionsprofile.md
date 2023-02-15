---
title: "Aktionsprofile"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-datenimport, by-folio, cat-einstellungen, for-admin, meta-workflow_sammlung]
weight: 30
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/settings/settings_data_import/settings_data_import/#settings--data-import--actions-profiles ) <!-- & [GBV](https://info.gebev.de/display/FOLIOGBVEXTERN/Einstellungen+(Datenimport):+Aktionsprofile) -->
    "
---

{{% pageinfo %}}
Hinweis: Es sind eigentlich mehrere einzelne Workflows. Ob einzeln oder wie hier zusammengefasst besser ist, ist noch unentschieden.
{{% /pageinfo %}}

Aktionsprofile definieren bestimmte Aktionen, die beim Import mit den eingehenden Datensätzen und/oder vorhandenen Datensätzen durchgeführt werden sollen.

Bevor ein Aktionsprofil erstellt wird, sollten zunächst Feldmappingprofile erstellt werden.

## Aktionsprofil für Importjob erstellen

1.  In der Ansicht **Aktionsprofil e** auf **Aktionen > Neues Aktionsprofil** klicken.
2.  Im Fenster **Neues Aktionsprofil** einen **Namen** für das Aktionsprofil eingeben.
3.  Optional: Eine **Beschreibung** des Aktionsprofil s eingeben.
4.  In der Dropdown-Liste **Aktion** eine der folgenden Optionen wählen:
    1.  **Erstellen**. Diese Option wählen, um einen neuen Datensatz zu erstellen.
    2.  **Aktualisieren**. Diese Option wählen, um einen bestehenden Datensatz zu aktualisieren.
    3.  **Ändern**. Diese Option wählen, um den eingehenden Datensatz zu ändern, bevor ein Datensatz erstellt oder aktualisiert wird. Nur für eingehende MARC-Datensätze verwenden.
5.  In der Dropdown-Liste **FOLIO-Datensatztyp** den Datensatztyp auswählen, der sich aus der gewählten Aktion ergibt.
6.  Optional: Um ein Feldmappingprofil mit dem Aktionsprofil zu verknüpfen, auf **Profil verknüpfen** klicken. Dieses Feldmappingprofil muss bereits existieren, um es zu verknüpfen. Ein Aktionsprofil kann nur mit einem Feldmappingprofil verknüpft werden. Wenn ein Aktionsprofil bearbeitet wird, werden diese Bearbeitungen in allen Feldmapping- und Jobprofilen, in denen das Aktionsprofil verwendet wird, übernommen.
    1.  Im Dialogfeld **Feldmapping-Profile auswählen** das Suchfeld verwenden, um das Feldmappingprofil zu finden, das dem Aktionsprofil hinzugefügt werden soll.
    2.  Auf das Feldmappingprofil klicken, um es auszuwählen. Das Feldmappingprofil wird zu dem Aktionsprofil hinzugefügt.
7.  Auf **Als Profil speichern & schließen** klicken. Es erscheint eine Bestätigungsmeldung und der Auftrag wird erstellt.

## Aktionsprofil für Importjob suchen

Die Suchleiste verwenden, um nach Aktionsprofil en in der Tabelle Aktionsprofil e zu suchen.

Die Tabelle Aktionsprofile enthält die folgenden Spalten:

* **Name**. Name des Aktionsprofils.
* **Aktion**. Die im Aktionsprofil enthaltene Aktion.
* **Tags**. Alle dem Aktionsprofil zugewiesenen Tags
* **Aktualisiert**. Datum, an dem das Aktionsprofil zuletzt aktualisiert wurde.
* **Aktualisiert von**. Person, die das Aktionsprofil zuletzt aktualisiert hat.

Es kann auf einen beliebigen Spaltennamen geklickt werden, um nach dieser Spalte zu sortieren.

## Aktionsprofil für Importjob ansehen

Um die Details eines Aktionsprofil s anzuzeigen, folgendermaßen vorgehen:

* In der Ansicht **Aktionsprofile** das Profil suchen, das angezeigt werden soll und es auswählen. Das Fenster **Details zum Aktionsprofil** wird angezeigt.

## Aktionsprofil für Importjob bearbeiten

1.  In der Ansicht **Aktionsprofile** das Profil suchen, das bearbeitet werden soll und es auswählen.
2.  In der Ansicht **Details zum Aktionsprofil** auf **Aktionen > Bearbeiten** klicken.
3.  die gewünschten Änderungen an dem Aktionsprofil vornehmen.
4.  Auf **Als Profil speichern & schließen** klicken. Eine Bestätigungsmeldung wird angezeigt und das Aktionsprofil wird aktualisiert.

## Aktionsprofil für Importjob duplizieren

1.  In der Ansicht **Aktionsprofile** das Profil suchen, das dupliziert werden soll und es auswählen.
2.  In der Ansicht **Details zum** **Aktionsprofil** auf **Aktionen > Duplizieren** klicken.
3.  Im Fenster **Neues Aktionsprofil** die gewünschten Änderungen vornehmen.
4.  Auf **Als Profil speichern & schließen** klicken. Es wird eine Bestätigungsmeldung angezeigt und das doppelte Aktionsprofil wird erstellt.

## Aktionsprofil für Importjob löschen

1.  In der Ansicht **Aktionsprofile** das Profil suchen, das gelöscht werden soll und es auswählen.
2.  In der Ansicht **Details zum** **Aktionsprofil**  auf **Aktionen > Löschen** klicken.
3.  Im Dialog **Aktionsprofil löschen** auf **Löschen** klicken. Eine Bestätigungsmeldung wird angezeigt und das Aktionsprofil wird gelöscht.

## Aktionsprofil für Importjob mit Tag versehen

1.  In der Ansicht **Aktionsprofile** das Profil suchen, das getaggt werden soll und es auswählen.
2.  In der Ansicht **Details zum** **Aktionsprofil** auf **Tags** klicken.
3.  Im Feld **Tags** entweder ein Tag auswählen oder ein Tag eingeben. Das Tag wird automatisch für das Profil angewendet.
