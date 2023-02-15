---
title: "ldpmarc"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-ldp, by-folio, for-admin]
weight: 20
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/reporting/ldpmarc/) <!-- & [GBV](https://info.gebev.de/display/FOLIOGBVEXTERN/ldpmarc) -->
    "
---

Das Tool ldpmarc ist Teil des Projekts Library Data Platform (LDP). Das ldpmarc-Tool konvertiert SRS/MARC-Datensätze von JSON in ein Tabellenformat, um sie in eine LDP-Berichtsdatenbank zu laden. SRS steht für Source Record Storage. MARC steht für Machine-Readable Cataloging (maschinenlesbare Katalogisierung), ein Standardformat zur Speicherung von Datenelementen in bibliografischen Datensätzen in Computersystemen. Sobald die MARC-Daten in die Berichtsdatenbank geladen wurden, führt ldpmarc inkrementelle Aktualisierungen der Daten durch, was Zeit beim Transferieren der Daten von der Transaktionsdatenbank zur Berichtsdatenbank spart.

Das Tool ldpmarc liest die SRS MARC-Daten aus den Datenbanktabellen public.srs\_marc und public.srs\_records. Anschließend wandelt es nur die aktuellen Versionen der Datensätze aus diesen Tabellen in tabellarische Daten um. Die umgewandelten Datensätze werden in die Tabelle public.srs\_marctab geschrieben.

Sobald die MARC-Daten transformiert sind, kann die Tabelle public.srs\_marctab in Abfragen verwendet werden, die MARC-Daten aus der Berichtsdatenbank benötigen. Die folgende Abfrage zeigt zum Beispiel den Inhalt des Feldes MARC 008, das allgemeine bibliografische Informationen über ein Exemplar einer Bibliothek erfasst.

```
SELECT
    sm.instance_hrid,
    sm.field,
    sm.content
FROM srs_marctab AS sm
WHERE (sm.field = '008')
LIMIT 10
;
```

## Installation und Konfiguration des ldpmarc Tools

Ausführliche Informationen über die Einrichtung und Konfiguration des ldpmarc-Tools sind in den unten verlinkten Anleitungen, die im [ldpmarc-Repository](https://github.com/library-data-platform/ldpmarc) verfügbar sind zu finden. Dort sind auch die neuesten Versionen und Korrekturen für das ldpmarc-Tool zu finden.

* [System requirements](https://github.com/library-data-platform/ldpmarc/tree/v1.5.3#system-requirements): Software- und Hardware-Anforderungen
* [Building](https://github.com/library-data-platform/ldpmarc/tree/v1.5.3#building-the-software): Installation / Erstellung des ldpmarc-Tools
* [Running ldpmarc](https://github.com/library-data-platform/ldpmarc/tree/v1.5.3#running-ldpmarc): Starten und Ausführen des ldpmarc Tools
* [Full vs. incremental update](https://github.com/library-data-platform/ldpmarc/tree/v1.5.3#full-vs-incremental-update): erklärt, wie ldpmarc-Updates funktionieren und wie man ein vollständiges Update erzwingt
* [Resetting ldpmarc](https://github.com/library-data-platform/ldpmarc/tree/v1.5.3#resetting-ldpmarc): wie die ldpmarc Datenbank zurückgesetzt wird
