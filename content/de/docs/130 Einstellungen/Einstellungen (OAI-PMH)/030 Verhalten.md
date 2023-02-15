---
title: "Verhalten"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-einstellungen, by-folio, cat-einstellungen, for-admin]
weight: 30
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/settings/settings_oaipmh/settings_oaipmh/#settings--oai-pmh--behavior) <!-- & [GBV](https://info.gebev.de/display/FOLIOGBVEXTERN/Einstellungen+(OAI-PMH):+Verhalten) -->
    "
---

## Unterstützung für gelöschte Datensätze

Eine von:

* **Nein** \- Gibt an, dass keine Informationen über gelöschte Datensätze angezeigt werden.
* **Persistent** \- Datensätze mit MARC Leader 05 gleich 'd', 's' oder 'x' werden in OAI-PMH ListRecords-Antworten als gelöscht aufgeführt.
* **Transient** \- Gleiches Verhalten wie Persistent, aber ohne Garantie, dass gelöschte Datensätze auf unbestimmte Zeit in FOLIO aufbewahrt werden.

Siehe [https://issues.folio.org/browse/MODOAIPMH-108](https://issues.folio.org/browse/MODOAIPMH-108) für weitere Einzelheiten zur Implementierung.

Der Einstellwert erscheint im XML-Element `deletedRecord` der Identify-Antwort.

## Unterdrückte Datensätze werden verarbeitet

Eine von:

* **Übertragung von unterdrückten Datensätzen mit Discovery-Flag-Wert** - Hinzufügen eines MARC-Unterfelds $t = 1 zum 999-Feld (für Instanzen), 852-Feld (für Exemplare) oder 952-Feld (für Artikel) von FOLIO.
* **Überspringe unterdrückte Datensätze mit Discovery-Flag-Wert** - Instanzen, die mit 'Von Discovery unterdrücken' markiert sind, werden in die OAI-PMH-Antwort aufgenommen.

## Verarbeitung von OAI-PMH-Fehlern

Eine von:

* **Mit HTTP-Status 200 verknüpfen** - Fehlermeldungen werden mit einem HTTP 200 Antwortcode zurückgegeben.
* **Mit HTTP-Fehlerstatus  verknüpfen**\- Fehlermeldungen werden mit einem entsprechenden HTTP-Fehlercode zurückgegeben.
