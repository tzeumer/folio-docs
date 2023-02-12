---
title: "Feldmappingprofile"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-datenimport, by-folio, cat-einstellungen, for-admin, meta-workflow_sammlung]
weight: 40
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/settings/settings_data_import/settings_data_import/#settings--data-import--field-mapping-profiles ) & [GBV](https://info.gbv.de/display/FOLIOGBVEXTERN/Einstellungen+(Datenimport):+Feldmappingprofile)
    "
---

{{% pageinfo %}}
Hinweis: Es sind eigentlich mehrere einzelne Workflows. Ob einzeln oder wie hier zusammengefasst besser ist, ist noch unentschieden.
{{% /pageinfo %}}

Feldmapping-Profile ordnen Felder der eingehenden Datensätze in FOLIO gemäß den mit diesem Feldmapping verbundenen Aktionen zu.

## Feldmappingprofil für Importjob erstellen

1.  In der Ansicht **Feldmappingprofile** auf **Aktionen > Neues Feldmappingprofil** klicken.
2.  Im Fenster **Neues Feldmappingprofil** einen **Namen** für das Feldmappingprofil eingeben.
3.  Einen **Eingehenden Datensatztyp** aus der Dropdown-Liste wählen: MARC Bibliografisch, MARC Normdaten oder EDIFACT-Rechnung.
4.  Einen **FOLIO-Datensatztyp** aus der Dropdown-Liste wählen: Instanz, Bestände, Exemplar, Bestellung, Rechnung, MARC Bibliografische Daten, MARC Bestandsdaten oder MARC Normdaten. Abhängig von der Auswahl werden verschiedene Optionen angezeigt. Die Details des Feldmappings sind so gestaltet, dass sie den Erstellungs-/Bearbeitungsbildschirm des FOLIO-Datensatzes so weit wie möglich imitieren. Einzelne Felder können jedoch mit einem Verweis auf ein bestimmtes Feld im eingehenden Datensatz, einem Standardwert oder einer Kombination aus beidem ausgefüllt werden. Weitere Informationen sind in den folgenden Abschnitten zu finden.
5.  Optional: Geben Sie eine **Beschreibung** für das Feldmappingprofil eingeben.
6.  Optional: Um Aktionsprofile mit dem Feldmappingprofil zu verknüpfen, unter **Zugehörige Aktionsprofile** auf **Profil verknüpfen** klicken und die folgenden Schritte ausführen:
    1.  Im Dialog **Aktionsprofile auswählen** das Suchfeld verwenden, um die Aktionsprofile zu finden, die mit dem Feldmappingprofil verknüpft werden sollen.
    2.  Die **Checkboxen** neben den Aktionsprofilen aktivieren und auf **Speichern** klicken. Die Aktionsprofile werden zu dem Feldmappingprofil hinzugefügt.
7.  Auf **Als Profil speichern & schließen** klicken. Es erscheint eine Bestätigungsmeldung und der Auftrag wird erstellt.

### Instanz

Anmerkung: Inaktive Felder können nicht gemappt werden, da sie vom System oder vom MARC-Instanz-Mappingprofil der Bibliothek kontrolliert werden.

* Im Abschnitt **Feldmapping - Instanz** die entsprechenden Felder auswählen. Weitere Informationen zu den Feldern sind unter Manuelles [Erstellen eines Instanzdatensatzes in FOLIO](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio%3A+Instanzdatensatz+manuell+in+FOLIO+erstellen) zu finden.

### Bestände

Im Abschnitt **Feldmapping - Bestände** die zutreffenden Felder ausfüllen. Weitere Informationen zu den Feldern sind unter [Hinzufügen von Beständen zu einem Datensatz](https://info.gbv.de/pages/viewpage.action?pageId=852492467) zu finden.

### Exemplar

Im Abschnitt **Feldmapping - Exemplar** die zutreffenden Felder ausfüllen. Weitere Informationen zu den Feldern sind unter [Hinzufügen eines Exemplars zu einem Datensatz](https://info.gbv.de/pages/viewpage.action?pageId=852492470) zu finden.

### Rechnung

Im Abschnitt **Feldmapping - Rechnung** die zutreffenden Felder ausfüllen. Erforderliche Felder sind mit einem Sternchen (\*) gekennzeichnet. Weitere Informationen zu den Feldern sind unter [Erstellen einer Rechnung](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio%3A+Rechnung+erstellen) zu finden.

### MARC Bibliografisch

1.  Die **Feldmappings für MARC** aus der Dropdown-Liste wählen: Änderungen oder Aktualisierungen.
2.  Wird **Änderungen** ausgewählt, die folgenden Schritte ausführen:
    1.  Im Abschnitt **Feldmapping - MARC Bibliografisch - Änderungen** in der Spalte Aktion die gewünschte Änderung auswählen: Hinzufügen, Löschen, Bearbeiten oder Verschieben.
    2.  Ein MARC-**Feld** in das Feld eingeben.
    3.  Optional: Standardmäßig werden die Felder **Indikatoren** und **Unterfeld** mit dem Platzhalter Sternchen (\*) ausgefüllt, der alle Daten in diesen Feldern einschließt. Bei Bedarf können diese Felder mit spezifischen Daten belegt werden.
    4.  Eine **Unteraktion** aus der Dropdown-Liste wählen. Die Optionen für die Unteraktion variieren je nach der gewählten Aktion. Alle Felder ausfüllen, die im Zusammenhang mit der Unteraktion erscheinen.
    5.  Wurde als Aktion Hinzufügen oder Bearbeiten gewählt, die Daten in das Feld eingeben.
    6.  Um ein weiteres Feldmapping hinzuzufügen, auf das **+** klicken und die Schritte a-e wiederholen.
    7.  Um ein Feldmapping zu löschen, auf das **Mülleimersymbol** klicken.
3.  Wird **Aktualisierungen** ausgewählt, diesen Schritten folgen:
    1.  Wenn Aktualisierungen nur bestimmte Felder betreffen sollen, im Abschnitt **Feldmapping - MARC Bibliografisch - Änderungen** auf **Feld hinzufügen** klicken und die Felder Feld, In.1, In.2 und Unterfeld ausfüllen. Um ein weiteres Feld hinzuzufügen, auf das **+** klicken. Um ein Feld zu löschen, auf das **Mülleimersymbol** klicken.
    2.  Wenn ein geschütztes Feld durch das Profil aktualisiert werden soll, die Checkboxen in der Spalte **Überschreiben** für jedes Feld markieren, das aktualisiert werden solll.

## Feldmappingprofil für Importjob suchen

Die Suchleiste verwenden, um nach Feldmappingprofilen in der Tabelle Feldmappingprofile zu suchen.

Die Tabelle Feldmappingprofile enthält die folgenden Spalten:

* **Name**. Name des Feldmappingprofils.
* **FOLIO-Datensatztyp**. Die vom Feldmappingprofil betroffene Datensatzart.
* **Tags**. Alle dem Feldmappingprofil zugewiesenen Tags
* **Aktualisiert**. Datum, an dem das Feldmappingprofil zuletzt aktualisiert wurde.
* **Aktualisiert von**. Person, die das Feldmappingprofil zuletzt aktualisiert hat.

Es kann auf einen beliebigen Spaltennamen geklickt werden, um nach dieser Spalte zu sortieren.

## Feldmappingprofil für Importjob ansehen

Um die Details eines Feldmappingprofils anzuzeigen, folgendermaßen vorgehen:

* In der Ansicht **Feldmappingprofile** das Profil suchen, das angezeigt werden soll und es auswählen. Das Fenster **Details zum Feldmappingprofil** wird angezeigt.

## Feldmappingprofil für Importjob bearbeiten

1.  In der Ansicht **Feldmappingprofile** das Profil suchen, das bearbeitet werden soll und es auswählen.
2.  In der Ansicht **Details zum Feldmappingprofil** auf **Aktionen > Bearbeiten** klicken.
3.  die gewünschten Änderungen an dem Feldmappingprofil vornehmen.
4.  Auf **Als Profil speichern & schließen** klicken. Eine Bestätigungsmeldung wird angezeigt und das Feldmappingprofil wird aktualisiert.

## Feldmappingprofil für Importjob duplizieren

1.  In der Ansicht **Feldmappingprofile** das Profil suchen, das dupliziert werden soll und es auswählen.
2.  In der Ansicht **Details zum** **Feldmappingprofil** auf **Aktionen > Duplizieren** klicken.
3.  Im Fenster **Neues Feldmappingprofil** die gewünschten Änderungen vornehmen.
4.  Auf **Als Profil speichern & schließen** klicken. Es wird eine Bestätigungsmeldung angezeigt und das doppelte Feldmappingprofil wird erstellt.

## Feldmappingprofil für Importjob löschen

1.  In der Ansicht **Feldmappingprofile** das Profil suchen, das gelöscht werden soll und es auswählen.
2.  In der Ansicht **Details zum** **Feldmappingprofil**  auf **Aktionen > Löschen** klicken.
3.  Im Dialog **Feldmappingprofil löschen** auf **Löschen** klicken. Eine Bestätigungsmeldung wird angezeigt und das Feldmappingprofil wird gelöscht.

## Feldmappingprofil für Importjob mit Tag versehen

1.  In der Ansicht **Feldmappingprofile** das Profil suchen, das getaggt werden soll und es auswählen.
2.  In der Ansicht **Details zum** **Feldmappingprofil** auf **Tags** klicken.
3.  Im Feld **Tags** entweder ein Tag auswählen oder ein Tag eingeben. Das Tag wird automatisch für das Profil angewendet.

## Feldmappingprofil für Importjob exportieren

Das Exportieren eines Feldmappingprofils ist derzeit noch nicht vorgesehen.
