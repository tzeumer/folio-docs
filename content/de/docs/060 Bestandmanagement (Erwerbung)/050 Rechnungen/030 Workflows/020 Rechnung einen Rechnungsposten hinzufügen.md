---
title: "Rechnung einen Rechnungsposten hinzufügen"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-rechnungen, by-folio, cat-workflows, for-anwender]
weight: 20
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/acquisitions/invoices/#adding-an-invoice-line-to-an-invoice) & [GBV](https://info.gbv.de/pages/viewpage.action?pageId=851345662)
    "
---

(Nach Abschluss von [Folio: Rechnung erstellen](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio%3A+Rechnung+erstellen) üblicherweise)

## Rechnungsposten hinzufügen

1.  Im Abschnitt Rechnungsposten auf **Aktion > Hinzufügen** klicken.
2.  Im Fenster **Bestellposten auswählen** im Feld Suchen & Filtern Stichwörter eingeben, um nach dem Bestellposten (Bestellposten) zu suchen.
3.  Optional: Die Ergebnisse filtern.
4.  Auf **Suchen** klicken. Die Suchergebnisse werden in der Ansicht Suchergebnisse angezeigt.
5.  Um einen oder mehrere Bestellposten auszuwählen, die Checkboxen links neben der Bestellposten-Nummer markieren.
6.  Auf **Speichern** klicken. Die Bestellposten erscheinen in der Tabelle Rechnungsposten. Um einen Rechnungsposten anzuzeigen, auf eine Zeile in der Tabelle Rechnungsposten klicken. Weitere Informationen sind unter [Rechnungsposten anzeigen](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio%3A+Rechnung+anzeigen) zu finden. Wenn ein Bestellposten ausgewählt wird, der einen Lieferanten enthält, der nicht mit der Organisation für die Rechnung übereinstimmt, wird ein Bestätigungsdialog angezeigt. Auf Bestätigen klicken, um mit der Auswahl der Bestellposten fortzufahren oder auf Abbrechen, um einen anderen Bestellposten auszuwählen.

Wenn die ausgewählte Bestellposition den Zahlungsstatus **Vollständig bezahlt** hat, wird oben im Rechnungskopf ein rotes Banner und neben dem entsprechenden Rechnungsposten ein rotes Ausrufezeichen angezeigt, um darauf hinzuweisen, dass der ausgewählte Bestellposten bereits vollständig bezahlt ist.

## Neuen Rechnungsposten hinzufügen

Um einen Rechnungsposten zu erstellen, der nicht mit einem bestehenden Bestellposten verbunden ist, wie folgt vorgehen:

1.  Im Abschnitt Rechnungsposten auf **Aktion >** **Neue Leerzeile** klicken.
2.  Im Fenster **Lieferantenrechnungsposten erstellen** die Abschnitte Informationen zur Rechnung, Fondverteilung und Zusatzkosten ausfüllen. Weitere Informationen zu den Feldern und Aktionen, die in diesen Abschnitten verfügbar sind, sind in den Abschnittsbeschreibungen unten zu finden.
3.  Auf **Speichern & schließen** klicken. Es erscheint eine Bestätigungsmeldung und der Rechnungsposten wird in der Tabelle Rechnungsposten angezeigt.

## Einen Rechnungsposten mit einem Bestellposten verknüpfen

Wenn Rechnungen im EDIFACT-Format von Lieferanten durch Datenimport in das System geladen werden, werden Rechnungsposten auf der Grundlage der vom Lieferanten bereitgestellten Informationen erstellt. Das System ist möglicherweise nicht in der Lage, einige Rechnungsposten automatisch mit einem bestehenden Bestellposten zu verknüpfen. Um einen Rechnungsposten manuell mit einem Bestellposten zu verknüpfen, wie folgt vorgehen:

1.  In der Ansicht der Lieferantenrechnung das Akkordeon Rechnungsposten prüfen, um festzustellen, ob das System automatisch eine Verknüpfung zu einem Bestellposten erstellt hat. Eine erfolgreich verknüpfte Rechnungsposten enthält einen **Bestellposten** in der Tabellenliste Rechnungsposten. Wenn der Bestellposten leer ist, konnte das System keine Verbindung zu einer bestehenden Bestellung herstellen.
2.  Um den Rechnungsposten manuell zu verknüpfen, auf das **Verknüpfungssymbol** klicken, um eine Bestellposten-Suche aufzurufen.
3.  Das Fenster **Bestellposten auswählen** wird geöffnet. Im Feld **Suchen & Filtern** Stichwörter eingeben, um nach dem Bestellposten (Bestellposten) zu suchen.
4.  Optional: Die Ergebnisse filtern.
5.  Auf **Suchen** klicken. Die Suchergebnisse werden in der Ansicht Suchergebnisse angezeigt.
6.  Auf die eine **Bestellung** klicken, die mit dem Rechnungsposten verknüpft werden soll. Der Wert des **Bestellpostens** wird ausgefüllt und die Verknüpfung wird erstellt.

## Bestellposten-Details

### Informationen zur Rechnungposten

* **Beschreibung**. Die Beschreibung oder der Titel des Rechnungspostens. Sie kann die Ressourcen, die Dienstleistung oder die Gebühr enthalten, die in Rechnung gestellt wird.
* **Rechnungspostenummer**. Die Nummer des Rechnungspostens, der nach dem Speichern dieser neuen Rechnungszeile erstellt wird.
* **Status**. Der Status des Rechnungspostens: Offen, Geprüft, Freigegeben, Bezahlt, Gestorniert.
* **Lieferantenreferenznummern**. Auf **Lieferantenreferenznummer hinzufügen** klicken, um Lieferantenreferenznummern für den Rechnungsposten hinzuzufügen. Weitere Informationen zu Lieferantenreferenznummern sind unter [Bestellungen > Hinzufügen einer Bestellposition zu einer Bestellung > Lieferanten-Referenznummer](https://info.gbv.de/pages/viewpage.action?pageId=851017779) zu finden.
* **Lieferantenreferenztyp**. Ein Typ zur Definition der Lieferantenreferenznummer. Die eindeutige Lieferantenbestellnummer, die Interne Lieferantennummer, die Lieferantenabonnementnummer, die Lieferantenfortsetzungsnummer oder die eindeutige Lieferantentitelnummer.
* **Informationen zum Abonnement**. Informationen für diesen Rechnungsposten, z.B. welche Bände in Rechnung gestellt werden.
* **Beginn des Abonnements**. Das Datum, an dem das Abonnement beginnt.
* **Ende des Abonnements**. Das Datum, an dem das Abonnement endet.
* **Kommentar**. Eventuelle zusätzliche Kommentare zum Rechnungsposten.
* **Buchhaltungscode**. Der Buchhaltungscode für den Rechnungsposten. Wenn eine Kontonummer aus der Dropdown-Liste augewählt wird, wird der zugehörige Buchhaltungscode hier angezeigt. Anmerkung: Wenn die Checkbox **An Haushaltssystem exportieren** aktiviert ist, ist der **Buchhaltungscode** erforderlich.
* **Kundennummer**. Die Kundennummer für den Rechnungsposten. Diese Dropdown-Liste enthält die Kundennummer für den auf der Rechnung ausgewählten Lieferanten, sofern im Datensatz der Organisation des Lieferanten welche vorhanden sind. Wenn im Organisationsdatensatz des Lieferanten ein oder mehrere Lieferantenkonten vorhanden sind, wird das erste Konto in diesem Feld als Standardwert angezeigt.
* **Anzahl**. Die Anzahl der Exemplare des Rechnungsposten.
* **Zwischensumme**. Der Betrag für diesen Rechnungsposten. Anmerkung: Der Zwischensummenbetrag muss auf einen oder mehrere Fonds aufgeteilt werden und wird in der Währung angegeben, die unter [Einstellungen > Mandant > Sprache und Lokalisierung](https://info.gbv.de/display/FOLIOGBVEXTERN/Einstellungen+%28Mandant%29%3A+Sprache+und+Lokalisierung) definiert ist.
* **Bindung lösen**. Dieses Feld markieren, um den Restwert der zugehörigen Bindung(en) aus dem Fonds freizugeben, dem sie zugewiesen wurde, wenn die Rechnung in den Status **Freigegeben** übergeht. Wenn dieses Kästchen nicht markiert ist, bleibt der verbleibende Wert der damit verbundenen Bindung auch nach der **Freigabe** der Rechnung bestehen und der Zahlungsstatus der damit verbundenen Bestellposten geht erst dann auf **Vollständig bezahlt** über, wenn die Bindung freigegeben ist. Wenn der Bestellposten beispielsweise 50 € kostet, der Rechnungsbetrag aber 40 € beträgt und die Option Belastung freigeben nicht markiert ist, bleibt die Differenz von 10 € als Bindung auf dem in der Fondverteilung angegebenen Fonds bestehen.

### Fondverteilung

Der zu verteilende Restbetrag wird auf der Grundlage der oben eingegebenen Zwischensumme berechnet.

1.  Auf **Fondverteilung hinzufügen** klicken.
2.  Die Fondsinformationen in die unten beschriebenen Felder einfügen. Es können mehrere Fondsverteilungen hinzugefügt werden. Um eine Fondverteilung zu entfernen, auf das **Mülleimersymbol** neben der entsprechenden Zeile klicken.
* **Zusatzkosten**. Die Zusatzkosten, die für die Fonds für die Rechnung gelten.
* **Fonds-ID**. Der Fonds, an den der Betrag vergeben werden soll. Anmerkung: Die Verwendung von Erwerbungsteams kann die Anzeige der Fonds in dieser Liste einschränken. Wenn ein Erwerbungsteam so eingerichtet ist, dass es die Ansichtsberechtigungen einschränkt, werden in der Dropdown-Liste nur Fonds angezeigt, die demselben Erwerbungsteam wie die Person zugewiesen sind. Weitere Informationen sind unter [Einstellungen > Erwerbungsteams](https://info.gbv.de/pages/viewpage.action?pageId=849379720) zu finden.
* **Kostenart**. Die Kostenart innerhalb des Fonds, auf den der Betrag verteilt werden soll. Dieses Feld wird nur angezeigt, wenn der ausgewählten Fonds-ID Kostenarten zugeordnet sind.
* **Wert**. Der Geldwert, der auf den Fonds angewendet werden soll, ausgedrückt als Prozentsatz oder Währungswert.
* **Typ**. Auswählen, ob der **Wert** als Prozent- oder Währungswert ausgedrückt werden soll.
* **Betrag**. Der Betrag der Mittel, die dem Fonds zugewiesen werden.

### Zusatzkosten

Um voreingestellte Zusatzkosten zu verwenden, diese aus der Dropdown-Liste **Zusatzkosten voreinstellen** auswählen. Voreingestellte Zusatzkosten werden unter [Einstellungen > Rechnungen > Zusatzkosten](https://info.gbv.de/display/FOLIOGBVEXTERN/Einstellungen+%28Rechnungen%29%3A+Zusatzkosten) erstellt. Wenn neue Zusatzkosten benötigt werden, die noch nicht als Voreinstellung vorhanden sind, auf Zusatzkosten hinzufügen klicken.

* **Beschreibung**. Eine Beschreibung der Zusatzkosten.
* **Wert**. Die Kosten für die Zusatzkosten.
* **Aufteilung**. Festelgen, ob der Wert der Zusatzkosten auf mehrere Rechnungsposten verteilt ist.
* **Verhältnis zur Gesamtsumme**. Legt fest, ob die Zusatzkosten im Gesamtbetrag der Rechnung enthalten sind, zu diesem hinzukommen oder von ihm getrennt sind. Anmerkung: Zusatzkosten, die mit einem **Verhältnis zur Gesamtsumme** von **Getrennt von** erstellt werden, sind nicht in der **Gesamtsumme der Zusatzkosten** oder dem **berechneten Gesamtbetrag** der Rechnung enthalten.
* Auf **Speichern & Schließen** klicken, um den neuen Rechnungsposten zu speichern und zur Ansicht der Rechnung zurückzukehren. Der neue Rechnungsposten wird nun im Akkordeon Rechnungsposten des Rechnungsdatensatzes angezeigt.
