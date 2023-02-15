---
title: "LDLite"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-ldp, by-folio, for-anwender]
weight: 50
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/reporting/ldlite/) <!-- & [GBV](https://info.gebev.de/display/FOLIOGBVEXTERN/LDLite) -->
    "
---

LDLite ist ein Tool, das Teil des Library Data Platform-Projekts ist. Es bietet grundlegende LDP-Datenberichtsfunktionen, ohne dass der LDP-Berichtsdatenbankserver installiert sein muss. Es kann auch verwendet werden, um eine LDP-Datenbank mit zusätzlichen oder Echtzeit-FOLIO-Daten zu ergänzen.

Mit LDLite können Personen FOLIO direkt abfragen. Sobald eine Verbindung zu Okapi-basierten Diensten besteht, kann die LDLite Software einige Funktionen der vollständigen Library Data Platform-Software bereitstellen, wie z.B. die JSON-Transformation. Die transformierten Daten können in einer eingebetteten Datenbank als einfache Datei auf dem Computer der Personen oder in einer gemeinsam genutzten Datenbank wie der LDP-Datenbank gespeichert werden. Personen müssen Python installiert haben, um LDLite zu installieren.

LDLite kann auch dazu verwendet werden, Berichte zu MARC-Daten zu erstellen, die aus Source Record Storage (SRS) abgerufen wurden. Diese Funktion befindet sich noch im Versuchsstadium und wird zur Zeit nicht offiziell unterstützt. Eine Anleitung für die Einrichtung des Zugriffs auf MARC-Daten von LDLite aus ist [auf GitHub zu finden](https://github.com/library-data-platform/ldlite/blob/main/srs.md).

Weitere Informationen über LDLite und Zugriff auf die Codebasis sind im [GitHub-Repository zu finden](https://github.com/library-data-platform/ldlite).
