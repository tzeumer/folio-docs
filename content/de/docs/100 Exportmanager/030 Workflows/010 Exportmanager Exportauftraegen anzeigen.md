---
title: "Exportmanager Exportaufträgen anzeigen"
linkTitle: ""
date: 2023-03-04T00:00:00-00:00
tags: [app-exportmanager, by-folio, cat-workflows, for-anwender, meta-uebersetzungsproblem]
weight: 10
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/export-manager/#viewing-export-jobs) <!-- & [GBV](https://info.gebev.de/pages/viewpage.action?pageId=845709337) -->
    "
---

{{% pageinfo %}}
Fehlende offizielle Übersetzungen. ("Budget (Bursar)", "EDIFACT-Bestellungen")
{{% /pageinfo %}}

Mit der App Exportmanager können Personen Exportprotokolle einsehen, die von den folgenden Apps oder Funktionen aus gestartet wurden:

* Massenbearbeitung
* Budget (Bursar)
* Ausleihprotokoll
* EDIFACT-Bestellungen
* eHoldings

Sobald ein Export in einem dieser Bereiche eingeleitet wird, erscheint ein Protokoll des Exports in der App Exportmanager. In der Ansicht **Suchen & Filtern** der App werden zwei Registerkarten angezeigt: **Alle** und **Organisationen**. Die Registerkarte Organisationen unterstützt den Export von EDIFACT-Bestellungen, während alle anderen unterstützten Exporte über die Registerkarte **Alle** zugänglich sind.

Die Anzeige der Spalten im Ergebnisbereich hängt von der im Bereich **Suchen & Filtern** ausgewählten Registerkarte ab.

In der Ansicht der Registerkarte **Alle** werden die folgenden Spalten angezeigt:

* **Job ID**. Die Identifikationsnummer des Exports.
* **Status**. Status des Exports: Geplant, In Bearbeitung, Erfolgreich, Fehlgeschlagen.
* **Jobtyp**. Der Typ des Exports, der zu dem entsprechenden Auftrag geführt hat. Zu den Auftragstypen gehören: Budget, Ausleihprotokoll, eHoldings, BULK\_EDIT\_IDENTIFIERS und BULK\_EDIT\_UPDATE.
* **Beschreibung**. Erscheint in den Exporten von Bursar mit einer zusammenfassenden Zählung der im Job enthaltenen Gebühren und Erstattungen.
* **Quelle**. Die Person, die den Export veranlasst hat. Der Eintrag kann 'System' für automatisierte Exporte oder 'folio' für Aufträge enthalten, die aus einer Massenbearbeitung oder einem wiederholten EDIFACT-Export resultieren.
* **Startzeit**. Datum und Uhrzeit des Beginns des Exports.
* **Endzeit.** Datum und Uhrzeit, zu der der Export beendet wurde.

Auf einen beliebigen Spaltennamen klicken, außer Beschreibung und Quelle, um nach dieser Spalte zu sortieren.

Die Ansicht der Ergebnisse auf der Registerkarte Organisationen zeigt die folgenden Spalten an:

* **Job ID**. Identifikationsnummer des Exports.
* **Status**. Status des Exports: Geplant, In Bearbeitung, Erfolgreich, Fehlgeschlagen.
* **Beschreibung**. Erscheint bei Bursar\-Exporten mit einer Übersicht über die im Auftrag enthaltenen Gebühren und Erstattungen.
* **Quelle**. Die Person, die den Export veranlasst hat. Der Eintrag kann 'System' für automatisierte Exporte oder 'folio' für Aufträge enthalten, die aus einer Massenbearbeitung oder einem wiederholten EDIFACT-Export resultieren.
* **Startzeit**. Datum und Uhrzeit des Beginns des Exports.
* **Endzeit**. Datum und Uhrzeit, zu der der Export beendet wurde.
* **Exportmethode**. Dieser Wert entspricht dem Namen der Integration in den Integrationsdetails des zugehörigen Organisationsdatensatzes.

Auf einen beliebigen Spaltennamen klicken, außer Beschreibung, Quelle und Exportmethode, um nach dieser Spalte zu sortieren.

Bei Aufträgen mit dem Status **Erfolgreich** auf die verlinkte Auftrags-ID klicken, um die Datei herunterzuladen.

Auf die Auftragszeile klicken, um zusätzliche Details zu dem Auftrag anzuzeigen, einschließlich Fehlerdetails.
