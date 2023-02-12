---
title: "Beleg anzeigen"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-rechnungen, by-folio, cat-workflows, for-anwender]
weight: 100
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/acquisitions/invoices/#viewing-a-voucher) & [GBV](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio:+Beleg+anzeigen)
    "
---

Sobald eine Rechnung freigegeben ist, wird ein Beleg erstellt und dem Rechnungsdatensatz hinzugefügt. Um einen Beleg anzuzeigen, wie folgt vorgehen:

-   [Die Rechnung suchen](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio%3A+Rechnung+suchen), die bearbeitet werden soll und sie auswählen.
-   In der Ansicht **Rechnungsnummer des Lieferanten** nach unten zum Abschnitt **Beleginformatione**n scrollen. In diesem Bereich werden die wichtigsten Informationen über den Beleg angezeigt.
-   Um alle Beleginformationen in einem Vollbildfenster anzuzeigen, auf **Beleg anzeigen** klicken.

## Beleginformationen

-   **Status**. Der Status des Rechnungsbelegs: Erwartet Zahlung oder Bezahlt.
-   **Belegnummer**. Die vom System zugewiesene Nummer für diesen Beleg.
-   **Belegdatum**. Datum, an dem die Rechnung freigegeben wurde und der Beleg erstellt wurde.
-   **Gesamt**. Gesamtbetrag aller Belegzeilen.
-   **Wechselkurs**. Wechselkurs, der für die Erstellung des Vorgangs verwendet wurde.
-   **Auszahlungsnummer**. Die Kennung aus einem externen System, die einer Zahlung entspricht.
-   **Kundennummer**. Die Nummer des Organisationskontos des Lieferanten für die in der Rechnung angegebene Zahlungsart. Dieser Wert wird nur ausgefüllt, wenn der Organisationsdatensatz des Lieferanten im Abschnitt Konten eine Kundennummer für die Zahlungsart enthält, die für diese Rechnung verwendet wird.
-   **Buchhaltungscode**. Buchhaltungscode des Lieferanten zur Identifizierung der Lieferantenorganisation in einem externen Buchhaltungssystem.
-   **Anlage benötigt**. Falls wahr und die Zahlungsart "Scheck" ist, zeigt dies einem externen Buchhaltungssystem an, dass eine Beilage zu dieser Rechnung erforderlich ist. Wenn die Checkbox An Haushaltssystem exportieren auf wahr gesetzt ist und ein Beleg für diese Rechnung erstellt wird, enthält die Exportbelegdatei im Datenelement Anlage erforderlich den Wert wahr.
-   **Lieferant**. Lieferantname.
-   **Adresse 1**. Adresse des Lieferanten 1. Dies ist die Hauptadresse des Lieferanten aus der App Organisation. Weitere Informationen sind unter [Organisationen> Hinzufügen einer Adresse](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio%3A+Organisation+als+Lieferanten+anlegen) zu finden.
-   **Adresse 2**. Adresse des Lieferanten 2.
-   **Stadt**. Stadt des Lieferanten.
-   **Bundesland/Provinz/Region**. Code des Bundeslandes, der Provinz oder der Region des Lieferanten.
-   **Postleitzahl**. Postleitzahl des Lieferanten.
-   **Land**. Land des Lieferanten.

## Belegposten

Die Belegposten werden nach externen Kostenstellen gruppiert. Wenn eine Rechnung beispielsweise mehrere Rechnungsposten enthält, die dieselbe externe Kostenstelle des Fonds aufweisen, wird nur ein Beleg erstellt, der den Gesamtbetrag für diese Rechnungsposten enthält.

-   **Externe Kostenstelle**. Die externe Kostenstelle des Fonds.
-   **Gesamt**. Der Gesamtbetrag für alle Belegposten, der unten in der Tabelle der Belegzeilen angezeigt wird.

Die Tabelle der Belegposten enthält diese Informationen für jede Belegzeile:

-   **Zeilennummer**.
-   **Gruppe**.
-   **Fondscode**.
-   **Externe Kostenstelle**.
-   **Betrag**.
