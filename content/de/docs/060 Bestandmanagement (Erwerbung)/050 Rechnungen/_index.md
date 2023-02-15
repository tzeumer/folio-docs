---
title: "📱Rechnungen"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-rechnungen, by-folio, cat-berechtigungen, for-anwender]
weight: 10
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/acquisitions/invoices/) <!-- & [GBV](https://info.gebev.de/pages/viewpage.action?pageId=839188624) -->
    "
---

Mit der App Rechnungen werden die Zahlung für die Ressourcen verwalten, die eine Bibliothek bestellt hat. Es kann auch nach bestehenden Rechnungen gesucht und diese bei Bedarf bearbeitet werden.

Definitionen der in der App Rechnungen verwendeten Begriffe:

* **Buchhaltungscode**. Der Code, der von der Bibliothek in einem Zahlungssystem in Bezug auf eine Organisation verwendet wird.
* **Erwerbungsteams**. Eine zusätzliche Ebene, die zu den Erwerbungsdatensätzen hinzugefügt werden kann und die die Möglichkeit einer Person einschränkt, mit diesen Datensätzen zu interagieren, wenn sie nicht diesem Team zugewiesen wurde. Es können beispielsweise Erwerbungsteams erstellt werden, um die verschiedenen Bibliotheken in dem Bibliothekssystem zu repräsentieren. Die Teams werden von der Bibliothek in der App Einstellungen definiert und festgelegt. Weitere Informationen sind unter [Einstellungen > Erwerbungsteams]({{< ref "010 Einstellungen (Erwerbungsteams)_ Erwerbungsteam erstellen, bearbeiten, loeschen" >}}) zu finden.
* **Zusatzkosten**. Kosten, die einer Rechnung zusätzlich zu den bestellten Ressourcen hinzugefügt werden. Versandkosten und Wechselkurse sind häufige Zusatzkosten.
* **Batch-Gruppe**. Gruppen, die ihre Rechnungen gemeinsam verarbeiten. Rechnungen aus der gleichen Bibliothek werden in der Regel gemeinsam verarbeitet.
* **Fonds**. Spezielle Zuweisungen von Mitteln innerhalb eines Etats.
* **Rechnungsposten**. Die einzelnen Rechnungsposten, die in jeder Rechnung bezahlt werden. Jede Zeile besteht aus einer Beschreibung der zu bezahlenden Ressourcen, den angefallenen Kosten und einer Lieferanten-Referenznummer. Rechnungen sind in erster Linie eine Summe der Informationen aus diesen Zeilen.
* **Organisationen**. Jede Institution, mit der die Bibliothek zusammenarbeitet. Eine Organisation kann, muss es aber nicht, eine Institution sein, von der Ressourcen gekauft werden.
* **Lieferant**. Jede Institution, von der die Bibliothek Ressourcen kauft.
* **Rechnungsnummer des Lieferanten**. Die vom Lieferanten für diese Rechnung angegebene Nummer.
* **Belegnummer**. Eine vom System generierte Nummer zur Identifizierung der aus FOLIO in ein externes Finanzsystem exportierten Zahlungsanforderung.

## Berechtigungen

Die unten aufgeführten Berechtigungen ermöglichen die Interaktion mit der App Rechnungen und legen fest, was innerhalb der App getan werde kann und was nicht. Es können Personen in der App Personen Berechtigungen zugewiesen werden. Wenn einer Person keine dieser Berechtigungen zugewiesen ist, kann sie die App Rechnungen und alle damit verbundenen Informationen nicht sehen.

Im Folgenden sind alle Berechtigungen für Rechnungen aufgeführt:

* **Rechnung: Rechnungen freigeben**. (Invoice: Approve invoices)
    Diese Berechtigung erlaubt es der Person, Rechnungen zu genehmigen.
* **Rechnung: Erwerbungsteams einem neuen Datensatz zuordnen**. (Invoice: Assign acquisition units to new record)
    Diese Berechtigung erlaubt es der Person, Erwerbungsteams neuen Rechnungen zuzuordnen.
* **Rechnung: Kann Rechnungen und Rechnungsposten anzeigen und bearbeiten**. (Invoice: Can view and edit invoices and invoice lines)
    Diese Berechtigung erlaubt es der Person, Rechnungen und Rechnungsposten einzusehen und zu bearbeiten.
* **Rechnung: Kann Rechnungen und Rechnungsposten anzeigen**. (Invoice: Can view invoices and invoice lines)
    Mit dieser Berechtigung kann die Person Rechnungen und Rechnungsposten einsehen.
* **Rechnung: Kann Rechnungen und Rechnungsposten anzeigen, bearbeiten und neue erstellen**. (Invoice: Can view, edit and create new invoices and invoice lines)
    Mit dieser Berechtigung kann die Person Rechnungen und Rechnungsposten anzeigen, bearbeiten und neu erstellen.
* **Rechnung: Kann Rechnungen und Rechnungsposten anzeigen, bearbeiten und löschen**. (Invoice: Can view, edit and delete invoices and invoice lines)
    Mit dieser Berechtigung kann die Person Rechnungen und Rechnungsposten anzeigen, bearbeiten und löschen.
* **Rechnung: Rechnung stornieren**. (Invoice: Cancel invoice)
    Diese Berechtigung erlaubt Personen, Rechnungen zu stornieren.
* **Rechnung: Batch-Datei aus dem Rechnungsdatensatz herunterladen**. (Invoice: Download batch file from invoice record)
    Mit dieser Berechtigung können Personen eine Batch-Datei aus einem Rechnungsdatensatz herunterladen.
* **Rechnungen: Suchergebnisse exportieren**. (Invoice: Export search results)
    Mit dieser Berechtigung können Personen eine Datei mit Rechnungsinformationen für eine Reihe von Rechnungen exportieren.
* **Rechnung: Erwerbungsteams verwalten**. (Invoice: Manage acquisition units)
    Mit dieser Berechtigung kann die Person die Zuordnung von Erwerbungsteams für eine Rechnung ändern.
* **Rechnung: Rechnungen bezahlen**. (Invoice: Pay Invoices)
    Diese Berechtigung erlaubt es der Person, Rechnungen zur Zahlung freizugeben.
* **Rechnungen: Belegexport**. (Invoice: Voucher export)
    Diese Berechtigung ermöglicht es der Person, den Belegexport aus dem Menü Aktionen der App Rechnungen auszuführen.
