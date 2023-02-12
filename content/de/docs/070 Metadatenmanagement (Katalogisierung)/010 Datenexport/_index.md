---
title: "📱Datenexport"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-datenexport, by-folio, cat-berechtigungen, for-anwender]
weight: 10
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/metadata/data-export/) & [GBV](https://info.gbv.de/pages/viewpage.action?pageId=839188634)
    "
---

Mit der App Datenexport können bibliografische Daten aus dem Source Record Storage (SRS) sowie Instanz-, Bestandsdatensätze und Exemplare, die in der App Katalog gespeichert sind, exportiert werden. Die exportierten Datensätze werden im MARC 21-Format geliefert.

Wenn die Datensätze aus der App "Katalog" exportiert werden und die zugrunde liegenden MARC-Quelldaten vorhanden sind, werden diese Daten exportiert. Wenn keine zugrunde liegenden Quelldaten vorhanden sind, wird ein vereinfachter MARC-Datensatz erstellt.

Die App Datenexport wird mit einem Standard Jobprofil geliefert, das festlegt, wie die Informationen in die generierte MARC-Datei exportiert werden. Um eigenen Jobprofile zu erstellen, können Jobprofile in der App Einstellungen konfiguriert werden. Weitere Informationen sind unter [Einstellungen > Datenexport](https://info.gbv.de/pages/viewpage.action?pageId=849379672) zu finden.

Definition von Bedingungen im Zusammenhang mit der App Datenexport:

* **Jobprofil**. Bestimmt, wie Informationen aus FOLIO in die generierte MARC-Datei exportiert werden.
* **SRS**. Source Record Storage. Eine Speicherebene in FOLIO. Wenn eine Instanz einen zugrundeliegenden MARC-Datensatz hat, wird dieser Datensatz in SRS gespeichert.

## Berechtigungen

Um die App für den Datenexport anzuzeigen und mit ihr zu interagieren, muss einer Person die folgende Berechtigung zugewiesen werden:

* **UI: Datenexportmodul ist aktiviert**. (UI: Data export module is enabled)
    Mit dieser Berechtigung kann die Person die App "Datenexport" sehen und verwenden.

Anmerkung: Dies ist die einzige Berechtigung, die für die Datenexport App verfügbar ist. Personen können den Datenexport nicht sehen und darauf zugreifen, wenn ihnen diese Berechtigung nicht zugewiesen ist. Personen kann in der App Personen die Berechtigungen zugewiesen werden.
