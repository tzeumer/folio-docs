---
title: "📱Datenimport"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-datenimport, by-folio, cat-berechtigungen, cat-workflows, for-anwender, meta-uebersetzungsproblem]
weight: 10
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/metadata/data-import/ ) & [GBV](https://info.gbv.de/pages/viewpage.action?pageId=839188636)
    "
---

{{% pageinfo %}}
Rot: Fehlende offizielle Übersetzungen. ("Datenimport: Kann Dateien hochladen, importieren und Protokolle anzeigen.", "Datenimport: Kann Importprotokolle löschen."
{{% /pageinfo %}}

Mit der App Datenimport können einer oder mehrere Datensätze in die App Katalog importiert oder Rechnungen in die App Erwerbung geladen werden. Mit dem Datenimport können bibliografische MARC-Datensätze importiert werden, um Datensätze in der App "Katalog" und im Source Record Storage (SRS) zu erstellen und/oder zu aktualisieren.

Definition von Bedingungen im Zusammenhang mit der App Datenimport:

-   **Jobprofil**. Enthält alle Schritte, die zum Abschluss eines einzelnen Datenimportauftrags erforderlich sind.
-   **SRS**. Source Record Storage. Eine Speicherebene in FOLIO. Wenn eine Instanz einen zugrundeliegenden MARC-Datensatz hat, wird dieser Datensatz in SRS gespeichert.

## Berechtigungen

Um die App Datenimport anzeigen und mit ihr interagieren zu können, muss einer Person die folgende Berechtigung zugewiesen werden:

-   **Datenimport: Kann Dateien hochladen, importieren und Protokolle anzeigen**. (Data import: Can upload files, import, and view logs)
    Mit dieser Berechtigung kann die Person die App Datenimport sehen und verwenden. Die Person kann alle Funktionen außer dem Löschen von Protokollen ausführen.
-   **Datenimport: Kann Importprotokolle löschen**. (Data import: Can delete import logs)
    Diese Berechtigung ermöglicht es der Person, Protokolle in der Datenimport App zu löschen.

Anmerkung: Dies sind die einzigen Berechtigungen, die für die Datenimport App verfügbar sind. Wenn diese Berechtigung nicht zugewiesen sind, können Datenimport nicht angezeigt und nicht darauf zugergriffen werden. Sie können Personen in der App Benutzer Berechtigungen zugewiesen werden.
