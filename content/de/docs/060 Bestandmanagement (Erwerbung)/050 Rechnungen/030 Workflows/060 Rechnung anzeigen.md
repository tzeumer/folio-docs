---
title: "Rechnung anzeigen"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-rechnungen, by-folio, cat-workflows, for-anwender]
weight: 60
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/acquisitions/invoices/#viewing-invoice-details ) & [GBV](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio:+Rechnung+anzeigen)
    "
---
Sobald nach einer Rechnung gesucht wird, werden die folgenden Ansichten in der Ansicht Rechnungen Suchergebnisse angezeigt:

* **Rechnungsnummer des Lieferanten**. Die vom Lieferanten für diese Rechnung angegebene Nummer.
* **Lieferant**. Der Code des Lieferanten.
* **Rechnungsdatum**. Das Rechnungsdatum des Lieferanten.
* **Status**. Der Status der Rechnung: Offen, Geprüft, Freigegeben, Bezahlt, Storniert.
* **Gesamtbetrag (System)**. Die kombinierten Kosten der bestellten Exemplare und Zusatzkosten für die Rechnung.

In den Suchergebnissen auf eine Rechnung klicken, um weitere Informationen anzuzeigen. Die Ansicht Rechnungsnummer des Lieferanten wird mit zusätzlichen Informationen zu der Rechnung angezeigt.

## Informationen zur Rechnung

Informationen zu den meisten Feldern im Bereich Rechnungsinformationen sind unter [Erstellen einer Rechnung > Rechnungsinformationen]({{< ref "010 Rechnung erstellen" >}}) zu finden. Sobald ein Rechnungsposten erstellt ist, werden die folgenden Felder vom System ausgefüllt und in den Bereich Informationen zur Rechnung aufgenommen:

* **Quelle**. Die Methode, mit der diese Rechnung erstellt wurde: Person, API, EDI oder MARC.
* **Gesamteinheiten**. Die Gesamteinheiten für die Rechnung, berechnet als Summe der Mengenwerte aller Rechnungsposten.
* **Zahlungsdatum**. Das Datum, an dem der Rechnungsstatus auf Bezahlt umgestellt wurde.

## Anzeigen von Rechnungsposten

Rechnungsposten verknüpfen eine Rechnung mit Bestellposten oder sind Rechnungsposten, die nicht mit einem bestehenden Auftrag verbunden sind. Jede Zeile besteht aus dem Titel, Zahlungsinformationen, Kostendetails und Zusatzkosten.

Im Abschnitt Rechnungsposten werden alle Rechnungsposten für die Bestellung aufgelistet. In der Tabellenliste der Rechnungsposten wird Folgendes angezeigt:

* **#**. Die Nummer des Bestellpostens (Bestellposten). Vom System generiert.
* **Bestellpostennummer**. Die Nummer des Bestellpostens.
* **Beschreibung**. Der bestellte Titel aus dem Bestellposten.
* **Fondscode**. Der Code des Fonds, aus dem die Zahlung für den Rechnungsposten geleistet wird.
* **Bestellstatus**. Der Status des Bestellvorgangs des Bestellpostens: Offen, Ausstehend, Geschlossen.
* **Inventarisierungsstatus**. Der Inventarisierungsstatus des Bestellpostens.
* **Zahlungsstatus**. Der Zahlungsstatus des Bestellpostens.
* **Lieferantenreferenznummer**. Eine eindeutige Kennung für die zu beschaffende Ressource, die für den Lieferanten spezifisch ist. Für die verschiedenen Ressourcen werden von den Lieferanten verschiedene Arten von Kennungen vergeben. Alle zugehörigen Lieferantenreferenznummern werden aufgelistet.
* **Anzahl**. Die bestellte Menge.
* **Zwischensumme**. Der Preis der Rechnung vor dem Hinzufügen von Zusatzkosten.
* **Zusatzkosten**. Die Zusatzkosten, die mit der Rechnung verbunden sind.
* **Gesamt**. Der Gesamtbetrag des Rechnungspostens, berechnet als **Zwischensumme** plus Zusatzkosten.
* **Lieferantencode**. Der Lieferantencode für die Lieferantenorganisation, die mit dem Bestellposten verbunden ist.

Um weitere Informationen zu einem Rechnungsposten anzuzeigen, auf die Zeile in der Liste der Rechnungsposten klicken. Es öffnet sich eine Ansicht mit Informationen zu dem Rechnungsposten. Eine Ansicht der Felder im Detailbereich der Rechnungsposten ist unter [Erstellen eines neuen Rechnungspostens]({{< ref "020 Rechnung einen Rechnungsposten hinzufuegen" >}}) zu finden.

### Andere verwandte Rechnungsposten anzeigen

Die Ansicht Rechnungsposten anzeigen enthält einen Akkordeonbereich, in dem **Weitere verknüpfte Rechnungsposten** aufgelistet sind. In dieser Tabelle sind alle Rechnungen aufgeführt, die sich auf denselben Bestellposten beziehen. Der Abschnitt Weitere verknüpfte Rechnungsposten enthält die folgenden Informationen:

* **Rechnungsnummer des Lieferanten**. Die vom Lieferanten für diese Rechnung angegebene Nummer. Auf das Symbol für die Zwischenablage neben der Rechnungsnummer des Lieferanten klicken, um den Wert in Ihre Zwischenablage zu kopieren.
* **Rechnungsposten #**. Die vom System generierte Nummer des Rechnungspostens.
* **Datum der Rechnung**. Das Rechnungsdatum des Lieferanten.
* **Lieferantenname**. Der Lieferantenname.
* **Status**. Der Status der Rechnung: Offen, Geprüft, Freigegeben, Bezahlt, Gestorniert.
* **Anzahl**. Die bestellte Menge.
* **Betrag**. Die kombinierten Kosten der bestellten Exemplare und Zusatzkosten für die Rechnung.
* **Kommentar**. Kommentare zu dem Rechnungsposten.

Auf den Wert eines Rechnungspostens mit der Nummer # klicken, um weitere Informationen anzuzeigen. Die Ansicht **Rechnungsposten anzeigen** wird mit zusätzlichen Informationen zu dem betreffenden Rechnungsposten angezeigt.

## Fondverteilung auf Rechnungsebene

Der Abschnitt Fondsverteilung auf Rechnungsebene der Rechnungsdetails wird nur angezeigt, wenn die Rechnung Zusatzkosten enthält, die nicht anteilig sind und für die eine Fondsverteilung ausgewählt wurden. Weitere Informationen sind unter Erstellen einer [Rechnung > Zusatzkosten > Hinzufügen von voreingestellten Zusatzkosten]({{< ref "020 Zusatzkosten" >}}) zu finden. Im Abschnitt Fondverteilung auf Rechnungsebene werden die folgenden Informationen angezeigt:

* **Zusatzkosten**. Beschreibung der Zusatzkosten.
* **Fonds**. Der Fonds, den der Betrag zugewiesen wurde.
* **Kostenart**. Die Kostenart innerhalb des Fonds, an den der Betrag zugewiesen ist. Dieses Feld zeigt nur dann Informationen an, wenn die ausgewählte Fonds-ID über zugehörige Kostenarten verfügt.
* **Wert**. Der Geldwert, der auf den Fonds angewendet werden soll, ausgedrückt als Prozentsatz oder Währungswert.
* **Betrag**. Der Betrag der Mittel, die für den Fonds gebunden sind.
* **Anfängliche Bindung**. Der ursprüngliche Betrag, der dem Fonds zugewiesen wurde.
* **Aktuelle Bindung**. Der aktuelle Betrag, der für den Fonds gebunden ist. Wenn eine Rechnung in den Status Freigegeben übergeht und die Checkbox Aktuelle Bindung in einer Rechnungsposition markiert ist, wird der Wert Aktuelle Bindung auf Null gesetzt.

## Zusatzkosten auf Rechnungsebene

Der Abschnitt Zusatzkosten auf Rechnungsebene in den Rechnungsdetails wird nur angezeigt, wenn die Rechnung Zusatzkosten enthält, die nicht anteilig sind. Bei Zusatzkosten mit einer Aufteilung nach Betrag, nach Zeile oder nach Menge werden die Zusatzkosten in der Rechnungsposten-Zeile angezeigt. Weitere Informationen sind unter [Erstellen einer Rechnung > Zusatzkosten > Hinzufügen einer voreingestellten Anpassung]({{< ref "020 Rechnung einen Rechnungsposten hinzufuegen" >}}) zu finden. Im Abschnitt Zusatzkosten auf Rechnungsebene sind die folgenden Informationen zu finden:

* **Beschreibung**. Eine Beschreibung der Zusatzkosten.
* **Wert**. Die Kosten der Anpassung.
* **Aufteilung**. Die Methode, nach der die Zusatzkosten anteilig verteilt werden sollen: Nach Zeile, Nach Betrag, Nach Menge, oder Nicht anteilig
* **Verhältnis zur Gesamtsumme**. Legt fest, wie die Zusatzkosten im Verhältnis zur Gesamtsumme der Rechnung angewendet werden: Zusätzlich zu, Inbegriffen in oder Getrennt von.

## Details zum Lieferanten

* **Rechnungsnummer des Lieferanten**. Die Rechnungsnummer des Lieferanten für die Rechnung. Auf das Symbol für die Zwischenablage neben der Rechnungsnummer des Lieferanten klicken, um den Wert in Ihre Zwischenablage zu kopieren.
* **Lieferantenname**. Der Name des Lieferanten.
* **Buchhaltungscode**. Der Buchhaltungscode für die Rechnung.
* **Adresse, primär**. Die primären Adressdaten des Lieferanten. Diese Adresse ist auf dem Beleg und dem Belegexport enthalten.

## Links und Dokumente
