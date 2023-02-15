---
title: "Berichte (Library Data Platform)"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-ldp, by-folio, for-anwender, topic-fernleihe]
weight: 120
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/reporting/) <!-- & [GBV](https://info.gebev.de/pages/viewpage.action?pageId=839188642) -->
    "
---

**Anmerkung: Diese Dokumentation bezieht sich auf [LDP v1.8.2](https://github.com/library-data-platform/ldp/tree/1.8.2) und [FOLIO Analytics v1.5.0](https://github.com/folio-org/folio-analytics/tree/release-1.5), die etwa zur gleichen Zeit wie FOLIO Nolana veröffentlicht wurden.**

Die Library Data Platform (LDP) ist ein Projekt, das eine Open-Source-Plattform entwickelt, die sowohl vom [FOLIO](http://folio.org/)\- als auch vom [ReShare](https://projectreshare.org/)\-Projekt genutzt wird, um statistische und operative Analysen zu erstellen. Die LDP-Software extrahiert Daten aus den FOLIO-Modulen in eine relationale Datenbank (in der FOLIO-Gemeinschaft informell häufig als "LDP" bezeichnet) und ermöglicht so die Erstellung komplexer Berichte und Analysen unter Verwendung von FOLIO-Daten. Während einige FOLIO Apps über integrierte Berichte oder die Möglichkeit verfügen, Ergebnisse aus einem Such- und Filter-Workflow herunterzuladen, unterstützt die LDP größere und komplexere Abfragen, die Daten aus allen FOLIO Apps kombinieren.

## Datenfluss von FOLIO zur LDP

Der grundlegende Datenfluss von FOLIO zur LDP wird in der folgenden Abbildung beschrieben. Die LDP extrahiert Daten aus der von den FOLIO Apps verwendeten Datenbank. Von der LDP fließen die Daten in zwei Arten von Abfragen: abgeleitete Tabellen/"derived tables" (die die FOLIO-Daten vereinfachen und die Ergebnisse zurück in die LDP speichern) und Berichtsabfragen/"report queries" (die den spezifischen Anforderungen von Personen entsprechen). Diese Abfragen werden über das FOLIO Analytics Query Repository gemeinsam genutzt und bilden auch das Rückgrat der Ad-hoc-Abfragen.

![Die LDP-Software extrahiert Daten aus der FOLIO Datenbank und lädt sie in die LDP-Datenbank. Das FOLIO Analytics Repository speichert abgeleitete Tabellenabfragen, die der LDP-Datenbank abgeleitete Tabellen hinzufügen, und Berichtsabfragen, die Berichte für Personen erstellen. Die LDP-Datenbank kann auch verwendet werden, um Nicht-FOLIO-Daten in benutzerdefinierten Tabellen zu speichern.](/img/de/_index/_index_2023-02-10-19-19-47.png)

## Features der LDP

* Open-Source-Software und Erstellung von Abfragen
* Basiert auf vertrauenswürdigen Datenbankplattformen
* Möglichkeit, benutzerdefinierte Tabellen zu erstellen, um Nicht-FOLIO-Daten zu importieren
* Verfolgung der Historie von FOLIO-Datensätzen
* Möglichkeit der Anbindung von einer Vielzahl von Berichtsanwendungen
* Möglichkeit, App-übergreifende FOLIO-Abfragen durchzuführen
* Möglichkeit zur Abfrage von FOLIO-Daten ohne Beeinträchtigung der Leistung der Produktionsanwendung
* Möglichkeit zur Abfrage eines vereinfachten FOLIO-Datenmodells durch die Verwendung abgeleiteter Tabellen
