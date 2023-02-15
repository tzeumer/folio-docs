---
title: "Bestellungsdetails anzeigen"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [by-folio, for-anwender, cat-workflows, app-bestellungen]
weight: 30
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/acquisitions/orders/#viewing-order-details ) & [GBV](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio:+Bestellungsdetails+anzeigen)
    "
---

Sobald nach einer Bestellung gesucht wurde, werden in der Ansicht Bestellungen die folgenden Informationen angezeigt:

* **Bestellnummer**. Die Bestellungsnummer.
* **Lieferantencode**. Der Lieferantencode.
* **Status**. Der Status der Bestellung: Ausstehend, Offen, Geschlossen.
* **Bestellungstyp**. Die Art der Bestellung: Einmalig, Laufend.
* **Zuletzt aktualisiert**. Das Datum, an dem die Bestellung zuletzt aktualisiert wurde.
* **Erwerbungsteams**. Die Erwerbungsteams, die der Bestellung zugewiesen sind.
* **Zugewiesen an**. Die Person, der die Bestellung zugewiesen ist.

Um die Spalten, die in der Ergebnisliste erscheinen, anzupassen, wie folgt vorgehen:

1.  In der Ansicht **Bestellung** die Schaltfläche **Aktionen** wählen.
2.  Die angezeigten Spalten sind alle standardmäßig unter **Spalten anzeigen** in der Aktionen-Liste angezeigt ausgewählt.
3.  Die Markierung aller Spalten aufheben, die aus der Ansicht Bestellungen entfernt werden sollen.
4.  Die Auswahl bleibt erhalten, bis sich von FOLIO abgemeldet wird.

In den Suchergebnissen auf eine Bestellung klicken, um sie anzuzeigen. Die Ansicht Bestellungsdetails wird mit zusätzlichen Informationen zu der Bestellung angezeigt:

## Bestellung

Weitere Informationen zu den Feldern, die in diesem Abschnitt der Bestellung angezeigt werden, sind unter Erstellen einer Bestellung > Bestellung zu finden.

* **Bestellnummer**. Die Bestellnummer für die Bestellung. Bitte beachten, dass bei der Anzeige der Bestellung die Werte für Präfix und Suffix innerhalb der Bestellnummer und nicht als separate Felder angezeigt werden.
* **Lieferant**. Der Lieferant, der mit dieser Bestellung verbunden ist.
* **Bestellungstyp**. Die Art der Bestellung: Einmalig oder Laufend.
* **Erwerbungsteams**. Die der Bestellung zugeordneten Erwerbungsteams.
* **Freigabedatum**. Das Datum, an dem der Status der Bestellung von Offen auf Freigegeben geändert wurde.
* **Zugewiesen an**. Die Person, die dieser Bestellung zugewiesen ist, falls zutreffend.
* **Rechnungsadresse**. Die für die Bestellung gewählte Rechnungsadresse.
* **Lieferadresse**. Die Lieferadresse, die für die Bestellung ausgewählt wurde.
* **Manuell**. Wenn die Checkbox Manuell markiert ist, ist die Bestellung von der automatischen Verarbeitung ausgeschlossen. Diese Option kann z.B. gewählt werden, wenn EDI eingerichtet ist, die Bestellung aber auf der Website des Lieferanten aufgegeben wurde und nicht gewünscht ist, dass sie erneut an ihn übermittelt wird.
* **Erneut belasten**. Eine vollständige Beschreibung dieses Feldes ist unter [Bestellung anlegen]({{< ref "010 Bestellung anlegen" >}}) zu finden.
* **Erstellt von**. Name der Person, die die Bestellung erstellt hat.
* **Erstellt am**. Das Datum und die Uhrzeit, zu der die Bestellung erstellt wurde.
* **Öffnungsdatum**. Das Datum und die Uhrzeit, zu der die Bestellung geöffnet wurde.

## Informationen zur laufenden Bestellung

Dieser Abschnitt wird nur für Bestellungen mit dem Typ Laufend angezeigt. Wenn die Checkbox Abonnement für diese Bestellung markiert ist, werden die folgenden Informationen angezeigt. Beschreibungen zu den einzelnen Feldern sind unter [Folio: Bestellung anlegen]({{< ref "010 Bestellung anlegen" >}}) zu finden. Nachfolgend ist die Beschreibungen für Felder zu finden, die nicht unter Erstellen einer Bestellung beschrieben sind.

* **Abonnement**.
* **Verlängerungsintervall**.
* **Verlängerungsdatum**.
* **Wiedervorlage-Zeitraum**.
* **Manuelle Verlängerung**.
* **Bemerkungen**.

Wenn die Checkbox für das Abonnement nicht markiert ist, werden die folgenden Informationen angezeigt:

* **Abonnement.**
* **Wiedervorlage.**
* **Anmerkungen.**

## Zusammenfassung der Bestellung

In diesem Abschnitt werden Preis- und Statusinformationen für die Bestellung angezeigt.

* **Einheiten insgesamt**. Bestellte Gesamtmenge für alle Bestellposten.
* **Freigegeben**. Zeigt an, ob die Bestellung freigegeben wurde.
* **Workflow-Status**. Der Status der Bestellung: Ausstehend, Offen, Geschlossen.
* **Geschätzter Gesamtpreis**. Die Summe der geschätzten Preisbeträge aller Bestellposten.
* **Bindungen gesamt**. Die Summe aller belasteten Beträge der Bestellposten.
* **Gesamtausgaben**. Der gesamte ausgegebene Betrag für alle Bestellposten. Wenn eine Rechnungsposten erstellt wird, wird er mit einem Bestellposten verknüpft. Der Gesamtbetrag der Rechnungsposten wird abgezogen, sobald die Rechnung freigegeben ist.

## Bestellposten

In diesem Abschnitt werden Informationen zu den Bestellposten für diese Bestellung angezeigt. Die Tabellenliste Bestellposten enthält die folgenden Spalten. Auf die Zeile einer Bestellposition klicken, um die Ansicht für die Details des Bestellpostens zu öffnen.

* **Bestellpostennummer**. Nummer des Bestellpostens.
* **Titel oder Paketname**. Titel oder Paketname des in der Bestellposten-Zeile bestellten Exemplars.
* **Produkt-ID**. Produkt-ID des Exemplars, das in der Bestellposten-Zeile bestellt wurde. Anmerkung: Alle zugehörigen Produkt-IDs werden hier aufgeführt.
* **Lieferanten-Referenznummer**. Die Referenznummer des Lieferanten für diesen Bestellposten.
* **Fondscode**. Der Fondscode der Fondsverteilung für den Bestellposten. Anmerkung: Wenn dem Bestellposten mehr als ein Fondscode zugeordnet ist, wird jeder Code hier aufgeführt.
* **Schätzpreis**. Der berechnete Preis auf der Grundlage der von Ihnen eingegebenen Werte. Schätzpreis = Listeneinzelpreis(e) x Bestellmengen + Zusatzkosten - Rabatt.

## Zugehörige Rechnungen

In diesem Abschnitt werden Informationen zu Rechnungen angezeigt, die mit dieser Bestellung über einen Bestellposten mit einem Rechnungsposten verknüpft sind. Die Rechnungstabellenliste zeigt die folgenden Spalten an. Um die Liste nach Rechnungsdatum zu sortieren, auf die Spaltenüberschrift klicken.

* **Rechnung #**. Die vom Lieferanten bereitgestellte Kennung für die Rechnung, die mit diesem Bestellposten verknüpft ist.
* **Rechnungsdatum**. Das Rechnungsdatum des Lieferanten. Auf den Spaltennamen klicken, um die Liste der zugehörigen Rechnungen nach Rechnungsdatum zu sortieren.
* **Lieferant**. Der Name des Lieferanten, der mit der zugehörigen Rechnung verbunden ist.
* **Rechnungsnummer des Lieferanten**.
* **Status**. Der Status der Rechnung: Offen, Überprüft, Freigegeben, Bezahlt oder Storniert.
* **Verausgabter Betrag**. Der gesamte ausgegebene Betrag der Rechnung.

## Details zum Export

In diesem Abschnitt werden Informationen zu den Bestellexporten an Lieferanten angezeigt, die mit dieser Bestellung in Verbindung stehen. Die

* **Job-ID**. Die Identifikationsnummer des Exports.
* **Exportdatum**. Datum, an dem der Exportauftrag ausgeführt wurde.
* **Dateiname**. Name der Exportdatei.
* **Exportmethode**. Der **Name der EDI-Verbindung** in den Integrationsdetails des zugehörigen Lieferantendatensatzes.

Im [Workflows Exportmanager]({{< ref "100 Exportmanager" >}}) sind weitere Informationen zum Anzeigen von Exportaufträgen zu finden.
