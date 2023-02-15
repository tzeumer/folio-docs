---
title: "Bestellposten anzeigen"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [by-folio, for-anwender, cat-workflows, app-bestellungen, meta-gemeldet_docsfolioorg]
weight: 240
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/acquisitions/orders/#viewing-order-line-details) & [GBV](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio:+Bestellposten+anzeigen)
    "
---

Sobald nach einem Bestellposten gesucht wird, werden die folgenden Informationen in der Ansicht Bestellposten Ergebnisse angezeigt:

* **Bestellpostennummer**. Nummer des Bestellpostens.
* **Aktualisierungsdatum**. Das Datum, an dem die Bestellposten zuletzt aktualisiert wurden.
* **Titel oder Paketname**. Der Titel oder der Paketname des Exemplars.
* **Produkt-ID**. Die Produkt-ID des Exemplars.
* **Lieferanten-Referenznummer**. Die Lieferanten-Referenznummer für diesen Bestellposten.
* **Fondscode**. Der Fondscode, der für den Kauf des Exemplars verwendet wird.
* **Bestellungsstatus**. Der Status der Bestellung: Ausstehend, Offen, Geschlossen.

In den Suchergebnissen auf einen Bestellposten klicken, um ihn anzuzeigen. Die Ansicht **Details zum Bestellposten** wird mit zusätzlichen Informationen zu dem Bestellposten angezeigt:

## Exemplardetails

Weitere Informationen zu den Feldern, die in diesem Bereich der Bestellposten angezeigt werden, sind unter [Hinzufügen eines Bestellpostens zu einer Bestellung > Exemplardetails]({{< ref "190 Bestellposten zu einer Bestellung hinzufuegen" >}}) zu finden finden.

## Bestellposten

Weitere Informationen zu den Feldern, die in diesem Bereich der Bestellposten angezeigt werden, sind unter Hinzufügen eines [Bestellpostens zu einer Bestellung > Details zur Bestellposition]({{< ref "190 Bestellposten zu einer Bestellung hinzufuegen" >}}) zu finden.

## Lieferant

Weitere Informationen zu den Feldern, die in diesem Abschnitt der Bestellposten angezeigt werden, sind unter [Hinzufügen eines Bestellpostens zu einer Bestellung > Lieferant]({{< ref "190 Bestellposten zu einer Bestellung hinzufuegen" >}}) zu finden.

## Kostendetails

Weitere Informationen zu den Feldern, die in diesem Abschnitt der Bestellposten angezeigt werden, sind unter [Hinzufügen eines Bestellpostens zu einer Bestellung > Kostendetails]({{< ref "190 Bestellposten zu einer Bestellung hinzufuegen" >}}) zu finden.

## Fondsverteilung

* **Fonds**. Der Fonds, an den Sie den Betrag ausschütten
* **Kostenart**. Die Kostenart innerhalb des Fonds, an den der Betrag ausgeschüttet wird. Dieses Feld zeigt nur dann Informationen an, wenn die ausgewählte Fonds-ID mit Kostenarten verbunden ist.
* **Wert**. Der Geldwert, der auf den Fonds angewendet werden soll, ausgedrückt als Prozentsatz oder Währungswert.
* **Betrag**. Der Betrag der Mittel, die für den Fonds gebunden sind.
* **Anfängliche Bindung**. Der ursprüngliche Betrag, der dem Fonds zugewiesen wurde.
* **Aktuelle Bindung**. Der aktuelle Betrag, der für den Fonds gebunden ist. Wenn eine Rechnung in den Status **Freigegeben** übergeht und die Checkbox **Aktuelle Bindung** auf einer Rechnungszeile markiert ist, wird der Wert Aktuelle Bindung auf €0 gesetzt. Auf den Wert klicken, um einen Link zur Detailansicht der Fondsbudget-Transaktion für die Bindung zu erhalten.

## Standort

In diesem Abschnitt werden Informationen angezeigt, wenn die Einstellung **Im Katalog erstellen** der Bestellposten **Instanz, Bestand** oder **Instanz, Bestand, Exemplar** ist. Weitere Informationen sind unter [Hinzufügen eines Standorts]({{< ref "docs/130 Einstellungen/Einstellungen (Mandant)/020 Standort einrichten/040 Standorte" >}}) zu finden.

* **Bestand**. Name und Code des Standortes für diesen Bestellposten.
* **Anzahl physisch**. Für diesen Standort bestellte Menge für diesen Bestellposten.
* **Anzahl elektronisch**. Für diesen Standort bestellte Menge für diesen Bestellposten.

## Details zur elektronischen Ressource

In diesem Abschnitt werden Informationen angezeigt, wenn die Bestellung einen Bestellposten mit dem Bestellformat Elektronisch oder P/E-Mix enthält. Weitere Informationen zu den Feldern, die in diesem Abschnitt der Bestellposten angezeigt werden, sind unter [Hinzufügen eines Bestellpostens zu einer Bestellung > Details zu E-Ressourcen]({{< ref "190 Bestellposten zu einer Bestellung hinzufuegen" >}}) zu finden.

## Details zur physischen Ressource

In diesem Abschnitt werden Informationen angezeigt, wenn die Bestellung einen Bestellposten mit einem Bestellformat von Physisch, KGV-Mix oder Sonstige enthält. Weitere Informationen zu den Feldern, die in diesem Abschnitt des Bestellposten angezeigt werden, sind unter [Hinzufügen eines Bestellpostens zu einer Bestellung > Details zu physischen Ressourcen]({{< ref "190 Bestellposten zu einer Bestellung hinzufuegen" >}}) zu finden.

## Anmerkungen

In diesem Abschnitt werden Anmerkungen zu der Bestellung angezeigt. Weitere Informationen zum Erstellen von Anmerkungen sind unter [Hinzufügen einer Anmerkung zu einer Bestellpostenzeile]({{< ref "210 Bestellposten eine Anmerkung hinzufuegen" >}}) zu finden.

* **Datum**. Zuletzt aktualisiertes Datum der Anmerkung. Auf die Spaltenbezeichnung Datum klicken, um die Anmerkungen in auf- oder absteigender Reihenfolge zu sortieren.
* **Titel und Details**. Der Titel und die Details der Anmerkung. Auf **Bearbeiten** klicken, um die Anmerkung zu bearbeiten. Auf **Speichern & Schließen** klicken, um die Änderungen zu speichern und auf **X** klicken, um das Fenster Notizen zu schließen.
* **Typ**. Der Typ der Anmerkung. Weitere Informationen zu den Notiztypen sind unter [Einstellungen > Notizen]({{< ref "010 Allgemein [Notiztypen anlegen, erstellen, loeschen]" >}}) zu finden.

## Verknüpfte Rechnungsposten

In diesem Abschnitt werden Informationen über Rechnungen und Rechnungsposten angezeigt, die mit diesem Bestellposten verknüpft sind. Die Rechnungstabellenliste zeigt die folgenden Spalten an:

* **Rechnungsposten Nr..** Die Rechnungsnummer der Rechnung, deren Rechnungsposten mit diesem Bestellposten verknüpft ist. Auf die Rechnungsnummer klicken, um die Ansicht der App Rechnungen für die Rechnung zu öffnen. Anmerkung: Der Link bezieht sich auf die allgemeine Rechnung, nicht auf den speziellen Rechnungsposten, der mit diesem Bestellposten verknüpft ist.
* **Rechnungsdatum**. Das Rechnungsdatum des Lieferanten.
* **Lieferantenname**. Der Name des Lieferanten, der mit der entsprechenden Rechnung verknüpft ist.
* **Rechnungsnummer des Lieferanten**. Die vom Lieferanten bereitgestellte Kennung für die Rechnung, die mit diesem Bestellposten verbunden ist.
* **Status**. Der Status der Rechnung: Offen, Geprüft, Freigegeben, Bezahlt oder Storniert.
* **Anzahl**. Die in Rechnung gestellte Menge. Anmerkung: Die angezeigte Menge stammt aus dem Rechnungsposten, der sich auf diese Bestellung bezieht, nicht aus der allgemeinen Rechnung.
* **Betrag**. Der Gesamtbetrag des Rechnungspostens, berechnet als Zwischensumme plus Anpassungen.
* **Kommentar**. Der Kommentar zum Rechnungsposten.

## Zugehörige Vereinbarungen

Wenn der Bestellposten mit einer Vereinbarungskomponente in der App eManagement verknüpft wurde, wird in der Ansicht Details zum Bestellposten ein Abschnitt Verknüpfte Vereinbarung angezeigt, der Informationen über die verknüpfte Vereinbarungskomponente enthält. Weitere Informationen sind unter [Vereinbarungen > Hinzufügen eines Bestellpostens zu einer Vereinbarungskomponente]({{< ref "040 Vereinbarungskomponente hinzufuegen" >}}) zu finden.

## Verknüpfte Instanz (Linked instance) - fehlt in Originaldoku

* Title
* Mitwirkende
* Verlage
