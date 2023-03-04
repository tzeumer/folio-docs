---
title: "📱Semesterapparate"
linkTitle: ""
date: 2023-03-04T00:00:00-00:00
tags: [app-semesterapparate, by-folio, for-anwender, cat-berechtigungen, meta-entwurf]
weight: 50
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/access/courses/courses/ ) <!-- & [GBV](https://info.gebev.de/pages/viewpage.action?pageId=839188613) -->
    "
---

{{% pageinfo %}}
Die Übersetzung "Kurs" wurde stehen gelassen, sofern es nicht um die App selber ging. Eigentlich wäre die konsequente Übersetzung immer "(Semester-)Apparate". Auch die Berechtigungen nutzen den Begriff "Kurse".
{{% /pageinfo %}}

Mit der App Semesterapparate können Semesterapparate erstellt und verwaltet werden.

Hinweis: Damit die Kurse, die in der App Semesterapparate erstellen, von Bibliotheksnutzenden gefunden werden können, muss ein externes Interface oder Discoverysystem eingerichtet sein, das mit FOLIO interagieren kann.

## Berechtigungen

Die unten aufgeführten Berechtigungen ermöglichen die Interaktion mit der App Semesterapparate und legen fest, was in der App getan werden kann und was nicht. Es können Personen in der App Personen Berechtigungen zugewiesen werden. Wenn einer Person keine dieser Berechtigungen zugewiesen ist, kann sie die App Semesterapparate und alle damit verbundenen Informationen nicht sehen.

Nachfolgend sind alle Semesterapparate-Bererchtigungen in der Reihenfolge der geringsten bis stärksten Einschränkung zu finden:

* **Semesterapparate: Alle Berechtigungen**. (Courses: All permissions)
    Mit dieser Berechtigung können Personen Kurse, Exemplare, Dozenten und verknüpfte Kurse verwalten (anzeigen, hinzufügen, bearbeiten und löschen).
* **Semesterapparate: Kurse anzeigen, hinzufügen und bearbeiten**. (Courses: Read, add, and edit courses)
    Mit dieser Berechtigung können Personen einen Kurs ansehen, hinzufügen und bearbeiten. Sie können einen Kurs jedoch nicht löschen.
* **Semesterapparate: reservierte Exemplare hinzufügen, bearbeiten und entfernen**.  (Courses: Add and edit courses’ reserved items)
    Mit dieser Berechtigung können Personen Exemplare zu einem Kurs hinzufügen und bearbeiten. Sie können keine Exemplare aus einem Kurs entfernen.
* **Semesterapparate: reservierte Exemplare hinzufügen und bearbeiten**. (Courses: Add, edit, and remove courses’ reserved items)
    Mit dieser Berechtigung können Personen Exemplare, die mit einem Kurs verbunden sind, anzeigen, hinzufügen, bearbeiten und entfernen.
* **Semesterapparate: Alles anzeigen**. (Courses: Read All)
    Mit dieser Berechtigung können Personen alle Kurse und Exemplarinformationen einsehen.
* **Einstellungen (Semesterapparate): Kann Semesterapparate-Einstellungen erstellen, bearbeiten und löschen**. (Settings (Courses): Can create, edit and delete Course Settings)
    Mit dieser Berechtigung können Personen alle Kurseinstellungen verwalten (anzeigen, hinzufügen, bearbeiten und löschen).

## Überlegungen zur Einführung

Bevor die App Semesterapparate eingesetzt wird, bitte sicherstellen, dass die folgenden Bedingungen erfüllt sind:

* App Katalog ist eingerichtet.
* [Ausleihregeln sind konfiguriert]({{< ref "docs/050 Bereitstellung (Leihverkehr)/010 Ausleihe/020 Einstellungen/" >}}).
* Personen sind importiert oder erstellt.

Wenn die App Semesterapparate zum ersten Mal konfiguriert wird, müssen zunächst die folgenden Eigenschaften in der App Einstellungen eingerichtet werden, falls benötigt:


* [Laufzeiten]({{< ref "020 Laufzeiten anzeigen, bearbeiten, loeschen" >}})
* [Kurstypen]({{< ref "030 Kurstypen anzeigen, bearbeiten, loeschen" >}})
* [Kurs Fachbereiche]({{< ref "040 Kurs Fachbereiche anzeigen, bearbeiten, loeschen" >}})
* [Bearbeitungsstatus]({{< ref "050 Bearbeitungsstatus anzeigen, bearbeiten, loeschen" >}})
* [Copyright-Status](({{< ref "060 Copyright-Status anzeigen, bearbeiten, loeschen" >}}))

Sobald die oben genannten Einstellungen vorgenommen sind, sind die folgende Tätigkeiten möglich:

* [Semesterapparate erstellen]({{< ref "020 Semesterapparate Kurs erstellen, bearbeiten, loeschen" >}}).
* [Dozenten hinzufügen]({{< ref "060 Semesterapparate Referenten erstellen, bearbeiten, loeschen" >}}).
* [Verknüpfte Kurse hinzufügen]({{< ref "030 Semesterapparate Verknuepfte Kurse erstellen, bearbeiten, loeschen" >}}).
* [Semesterapparaten reservierte Exemplare hinzufügen]({{< ref "080 Semesterapparate Reservierte Exemplare erstellen, bearbeiten, loeschen" >}}).

## Integrationen

Die Semesterapparate können optional mit diesen Anwendungen verbunden werden:

* EBSCO Discovery Service (EDS)
* VuFind

Darüber hinaus kann die App Semesterapparate über das "Learning Tools Interoperability"-Protokoll (LTI) mit einem Lernmanagementsystem verbunden werden. Für die LTI-Unterstützung ist ein separates Modul zu installieren. Weitere Informationen sind unter Semesterapparate - LTI-Konnektivität zu finden.

