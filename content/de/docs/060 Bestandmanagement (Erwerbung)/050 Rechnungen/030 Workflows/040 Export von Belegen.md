---
title: "Export von Belegen"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-rechnungen, by-folio, cat-workflows, for-anwender]
weight: 40
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/acquisitions/invoices/#exporting-vouchers) & [GBV](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio:+Export+von+Belegen)
    "
---

Folgendermaßen vorgehen, um eine Datei mit Beleginformationen im Format Komma-getrennte Werte (.csv) zu exportieren:

1.  In der Ansicht der **Suchergebnisse** auf **Aktionen > Belegexport** klicken.
2.  Auf dem Bildschirm Belegexport eine Batch-Gruppe aus dem Dropdown-Menü wählen.
3.  Alle bisher für die Batch-Gruppe ausgeführten Belegexporte werden in einer Tabelle mit den Spalten **Datum**, **Status** und **Nachricht** aufgelistet.
4.  Um einen neuen Belegexport für eine Batch-Gruppe durchzuführen, klicken Sie auf **Manuellen Export ausführen**. Es erscheint die Meldung "Alle Belege, die seit dem letzten Export für die Batch-Gruppe FOLIO erstellt wurden, werden exportiert und dieser Vorgang kann nicht rückgängig gemacht werden." Auf **Weiter** klicken, um fortzufahren oder auf **Abbrechen**.
    Wenn der Export abgeschlossen ist, wird eine neue Tabellenzeile erstellt, die eine Meldung enthält, die angibt, ob die Datei erfolgreich an den FTP-Standort hochgeladen wurde oder ob Belege für den Batch-Belegexport nicht gefunden wurden.
5.  Um eine der Belegexportdateien herunterzuladen, auf den Abwärtspfeil am Ende der Tabellenzeile klicken.

## Details zum Beleg-Export

Der Abschnitt Details zum Belegexport enthält die folgenden Felder:

-   **Batch-Gruppe**. Der Name der für die Rechnung ausgewählten Batch-Gruppe.
-   **Name der Batch-Datei**. Der Name der durch den Belegexport erzeugten Datei, ausgedrückt als Datum und Uhrzeit.
-   **Status der Batchdatei**. Der Status der Stapeldatei des Belegexports: Hochgeladen oder Fehler.

Nach dem Export von Belegen können Details zum Export angezeigt und die vollständige Belegexportdatei heruntergeladen werden, indem eine Rechnung gesucht wird, die im Exportauftrag enthalten war. Wie folgt vorgehen, um die Details des Belegexports anzuzeigen und die Datei in lokal herunterzuladen:

1.  In der Ansicht **Suchen und Filtern** die Rechnung suchen, die angezeigt werden soll und sie auswählen.
2.  In der Ansicht **Rechnungsnummer des Lieferanten** nach unten zum Abschnitt **Belegexportdetails** scrollen.
3.  Um die vollständige Belegexportdatei herunterzuladen, neben dem Namen der Batch-Datei auf das Download-Symbol mit dem Abwärtspfeil klicken. Diese Datei enthält alle Belege, die sich im Status Freigegeben befanden und zum Zeitpunkt der Auftragsausführung noch nicht exportiert worden waren.

### Beleg-Exportdatei

Die Belegexportdatei enthält die folgenden Datenelemente:

-   accountingCode
-   accountNo
-   amount
-   batchedVoucherLines/0/amount
-   batchedVoucherLines/0/fundCodes/
-   batchedVoucherLines/0/externalAccountNumber
-   enclosureNeeded
-   exchangeRate
-   folioInvoiceNo
-   invoiceCurrency
-   invoiceDate
-   invoiceTerms
-   status
-   systemCurrency
-   type
-   vendorInvoiceNo
-   vendorName
-   voucherDate
-   voucherNumber
-   vendorAddress/addressLine1
-   vendorAddress/addressLine2
-   vendorAddress/city
-   vendorAddress/stateRegion
-   vendorAddress/zipCode
-   vendorAddress/country
