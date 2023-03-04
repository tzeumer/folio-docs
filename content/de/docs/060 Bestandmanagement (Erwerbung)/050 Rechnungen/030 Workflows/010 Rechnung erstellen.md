---
title: "Rechnung erstellen"
linkTitle: ""
date: 2023-03-04T00:00:00-00:00
tags: [app-rechnungen, by-folio, cat-workflows, for-anwender, meta-gemeldet_docsfolioorg]
weight: 10
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/acquisitions/invoices/#creating-an-invoice) & [GBV](https://docs.folio.org/docs/acquisitions/invoices/#creating-an-invoice)
    "
---

Rechnungen enthalten eine Liste der fälligen Zahlungen für Ressourcen, die von der Bibliothek bei Lieferanten bestellt wurden.

1.  In der Ansicht **Rechnungen** auf **Neu** klicken.
2.  Im Fenster **Rechnung erstellen** die Abschnitte Informationen zur Rechnung, Zusatzkosten, Informationen zum Lieferanten, Erweiterte Informationen und Links & Dokumente ausfüllen. Weitere Informationen zu den Feldern und Aktionen, die in diesen Abschnitten verfügbar sind, sind in den Abschnittsbeschreibungen unten zu finden.
3.  Sobald alle gewünschten Informationen zur Rechnung eingegeben wurden, auf **Speichern & schließen** klicken. Anmerkung: Wenn die Person eine Rechnungsnummer für einen Lieferanten eingegeben hat, die mit einer bereits vorhandenen Rechnungsnummer mit demselben Rechnungsdatum übereinstimmt, erscheint ein Popup-Fenster mit der Meldung "Dies scheint eine doppelte Rechnungsnummer zu sein." Auf **Absenden** klicken, um mit der Erstellung der Rechnung fortzufahren, oder auf **Abbrechen**, um zur Ansicht Rechnung erstellen zurückzukehren.
4.  Die Rechnung wird gespeichert und der Ansicht Rechnungen hinzugefügt.

## Informationen zur Rechnung

Dieser Abschnitt enthält die Kopfdaten der Rechnung. Rechnungsdatum, Status und Batch-Gruppe sind die einzigen Pflichtfelder in diesem Abschnitt.

* **Rechnungsdatum (erforderlich)**. Das Rechnungsdatum des Lieferanten.
* **Status (erforderlich).** Der Status der Rechnung. Der Standardstatus für eine neue Rechnung ist "Offen". "Überprüft" ist ebenfalls in der Dropdown-Liste verfügbar.
* **Zahlung fällig**. Das Datum, an dem die Zahlung der Rechnung fällig ist.
* **Bedingungen**. Die zusätzlichen Bedingungen, die mit der Rechnung verbunden sind, wie z.B. Geschäfts- oder Vertragsbedingungen.
* **Freigabedatum**. Das Datum, an dem eine Person die Rechnung zur Weiterleitung freigegeben hat. Dieses Datum wird vom System generiert, nachdem die Rechnung erstellt und genehmigt wurde.
* **Freigegeben durch**. Die Person, die die Rechnung freigegeben hat. Der Name der Person wird angezeigt, nachdem die Rechnung erstellt und genehmigt wurde.
* **Erwerbungsteams**. Die der Rechnung zugewiesenen Erwerbungsteams. Weitere Informationen sind unter [Einstellungen > Erwerbungsteams]({{< ref "010 Einstellungen (Erwerbungsteams)_ Erwerbungsteam erstellen, bearbeiten, loeschen" >}}) zu finden.
* **Rechnungsadresse**. In der Dropdown-Liste Rechnungsadresse die Rechnungsadresse für die Rechnung auswählen. Sobald eine Adresse ausgewählt wurde, erscheint die Rechnungsadresse unter Adresse. Adressen werden in der App Einstellungen konfiguriert. Weitere Informationen sind unter [Einstellungen > Mandant > Adressen]({{< ref "010 Adressen" >}}) zu finden.
* **Batch-Gruppe (erforderlich)**. Die Batch-Gruppe, mit der der Rechnungsbeleg für den Belegexport gruppiert werden soll. Rechnungen aus der gleichen Bibliothek werden in der Regel gemeinsam verarbeitet. Weitere Informationen zum Export von Stapelbelegen sind unter [Exportieren von Belegen]({{< ref "040 Export von Belegen" >}}) zu finden.
* **Zwischensumme**. Die Zwischensumme der Rechnung, die sich aus der Summe der Zwischensummenwerte aller Rechnungsposten ergibt. Das System generiert diesen Betrag, nachdem die Rechnung erstellt wurde.
* **Gesamtzusatzkosten**. Die gesamten Zusatzkosten der Rechnung, berechnet als Summe aller Zusatzkosten im Rechnungskopf und in allen Rechnungsposten. Das System generiert diesen Betrag, nachdem die Rechnung erstellt wurde.
* **Berechneter Gesamtbetrag**. Der Gesamtbetrag der Rechnung, berechnet als Summe des Wertes der Zwischensumme und des Wertes der Gesamtzusatzkosten. Das System generiert diesen Betrag, nachdem die Rechnung erstellt wurde.
* **Gesamtsumme fixieren**. Dieses Feld markieren, um anzugeben, dass ein Gesamtbetrag eingegeben wird. Dieses Feld unmarkiert lassen, wenn gewünscht ist, dass das System den Gesamtbetrag auf der Grundlage der Beträge der Rechnungsposten berechnet.
* **Gesamtsumme fixieren\***. Die Gesamtausgaben für die Rechnung. Dieses Feld kann nur bearbeitet werden, wenn die Checkbox Gesamtsumme fixieren markiert ist. Wenn ein Gesamtsumme eingeben wird, müssen alle Rechnungsposten und Korrekturwerte dieser Gesamtsumme entsprechen, bevor eine Person die Rechnung genehmigen kann.
* **Bemerkung**. Alle zusätzlichen Kommentare, die für die Rechnung relevant sind.

## Zusatzkosten

Zusatzkosten sind optional und definieren die Kosten, die einer Rechnung über die bestellten Exemplare hinaus anhaften. Versandkosten und Wechselkurse sind zwei gängige Zusatzkosten. Es können entweder eine oder mehrere voreingestellte Zusatzkosten aus dem Dropdown-Menü ausgewählt oder eine neue erstellt werden.

Wie voreingestellte Zusatzkosten erstellt werden, ist unter [Einstellungen > Rechnungen > Zusatzkosten]({{< ref "020 Zusatzkosten" >}}) beschrieben.

### Voreingestellten Zusatzkosten auswählen

Voreingestellte Zusatzkosten aus der Dropdown-Liste wählen und auf **Zusatzkosten hinzufügen** klicken.

* **Beschreibung (erforderlich)**. Beschreibt die Zusatzkosten.
* **Wert (erforderlich)**. Der Betrag der Zusatzkosten.
* **Typ**. Eine Währung oder einen Prozentsatz wählen. Anmerkung: Diese Auswahl bezieht sich auf den Betrag, der unter Wert eingegeben wurde.
* **Aufteilen (erforderlich)**. Die Methode wählen, nach der die Zusatzkosten anteilig verteilt werden sollen: **Nach Zeile**, **Nach Betrag**, **Nach Anzahl** oder **Nicht aufgeteilt**, **Nach Zeile** verteilt die Anpassung gleichmäßig auf alle Posten, unabhängig von der Menge in jeder Zeile; **Nach Betrag** verteilt die Anpassung proportional auf alle Posten, basierend auf dem Betrag jeder Zeile; **Nach Anzahl** verteilt die Anpassung basierend auf der Anzahl. Wenn es zum Beispiel zwei Rechnungsposten gibt und der erste eine Menge von "1" und der zweite eine Menge von "2" hat, wird bei einer Anpassung nach Menge von @€3,00 €1,00 auf Zeile eins und €2,00 auf Zeile zwei angewandt. Bei der Option **Nicht aufgeteilt** wird die Anpassung auf Rechnungsebene und nicht auf jede einzelne Zeile angewendet. Wenn diese Option gewählt wird, wird eine Schaltfläche "Fondverteilung hinzufügen" angezeigt. Klicken Sie auf "Fondverteilung hinzufügen", um den Fonds festzulegen, auf den diese Anpassung angewendet werden soll.
* **Verhältnis zur Gesamtsumme (erforderlich)**. Legt fest, wie diese Anpassung im Verhältnis zur Rechnungssumme angewendet werden soll. Eine Option wählen: Zusätzlich zu, Enthalten in oder Getrennt von. Anmerkung: Zusatzkosten, die mit dem Wert **Verhältnis zur Gesamtsumme** von **Getrennt von** erstellt werden, sind nicht im **Gesamtbetrag der Zusatzkosten** oder im **berechneten Gesamtbetrag** der Rechnung enthalten.
* **An Haushaltssystem exportieren**. Markieren Sie diese Checkbox, um die Anpassungsdetails im Belegexport an Ihr externes Zahlungssystem für diese Rechnung zu senden.

### Zusatzkosten erstellen

Wenn neue Zusatzkosten erstellt werden, die nicht als voreingestellte Zusatzkosten existieren, auf **Zusatzkosten hinzufügen** klicken. Die Details der Zusatzkosten in die Felder eingeben, die oben unter Auswahl einer voreingestellten Zusatzkosten beschrieben wurden.

## Informationen zum Lieferanten

Der Abschnitt Informationen zum Lieferanten ist obligatorisch.

1.  Die **Rechnungsnummer des Lieferanten** eingeben, die vom Lieferanten geliefert wurde.
2.  Um den Lieferanten auszuwählen, **Organisationssuche** klicken. Im Dialogfeld **Organisation auswählen** den Organisationsdatensatz für den Lieferanten mithilfe des Suchfelds und/oder der Filter suchen. Auf die Organisation klicken, um sie auszuwählen. Anmerkung: Die für die Zahlung einer Rechnung ausgewählte Organisation muss ein Lieferant sein. Das System lässt die Auswahl einer Organisation zu, die kein Lieferant ist, aber eine Rechnung, die mit einer Organisation verbunden ist, die kein Lieferant ist, kann nicht freigegeben werden. Weitere Informationen sind unter [Bestandsmanagement (Erwerbung) > Organisationen > Anlegen eines Lieferanten]]({{< ref "020 Organisation als Lieferanten anlegen" >}}) zu finden.
3.  Der **Buchhaltungscode** des Lieferanten aus der Übersicht seines Organisationsdatensatzes wird automatisch angezeigt, sobald der Lieferanten ausgewählt ist und die Rechnung gespeichert wird. Wenn der Lieferant mehrere Konten mit unterschiedlichen Buchhaltungscodes hat, dann den entsprechenden Buchhaltungscode aus der Dropdown-Liste wählen. Weitere Informationen über die  Buchhaltungscodes von Organisationen sind unter [Organisationen > Erstellen einer Organisation]({{< ref "020 Organisation als Lieferanten anlegen" >}}) zu finden.

## Erweiterte Informationen

1.  Eine **Zahlungsart** aus dem Dropdown-Menü wählen: Bargeld, Kreditkarte, EFT, Einlagenkonto, Scheck, Banküberweisung, Interne Transfer oder Weitere.
2.  Wenn nach bestehenden Abonnements gesucht werden soll, die Checkbox **Abonnementüberschneidung prüfen** markieren. Anmerkung: Die Systemlogik ist derzeit nicht implementiert, so dass das System nicht auf sich überschneidende Abonnements prüft.
3.  Wenn ein Beleg an ein externes Finanzsystem gesendet werden soll, auf die Checkbox **An Haushaltssystem exportieren** klicken. Die Einstellung des Kontrollkästchens **An Haushaltssystem exportieren** im Datensatz Organisation des Lieferanten bestimmt die Standardeinstellung dieses Kontrollkästchens auf den Rechnungen für diesen Lieferanten. Anmerkung: Wenn diese Checkbox aktiviert ist, ist der **Buchhaltungscode** im vorangegangenen Abschnitt Informationen zum Lieferanten ein Pflichtfeld.
4.  Wenn einem externen Buchhaltungssystem mitgeteilt werden soll, dass für diese Rechnung eine Anlage erforderlich ist, auf die Checkbox **Anlage benötigt** klicken. Wenn die Checkbox An Haushaltssystem exportieren aktiviert ist und ein Beleg für diese Rechnung erstellt wird, enthält die Exportbelegdatei im Datenelement **Anlage erforderlich** den Wert "wahr".
5.  Eine **Währung** aus der Dropdown-Liste wählen. Der Standardwert ist in den Mandant-Einstellungen als Primärwährung hinterlegt. Weitere Informationen sind unter [Einstellungen > Mandant > Sprache und Lokalisierung]({{< ref "020 Sprache und Lokalisierung" >}}) zu finden. Wenn eine andere Währung als die Standardwährung gewählt wird, zeigt das System den aktuellen Wechselkurs an.
6. Wenn ein Wechselkurswert eingegeben werden soll, der den Wert des aktuellen Wechselkurses überschreibt, die Checkbox **Festgelegten Wechselkurs anwenden** aktivieren und den Kurs in das Feld **Wechselkurs festlegen** eingeben.

## Links und Dokumente

In diesem Bereich können Dokumente an einen Rechnungsdatensatz anhängt werden, z. B. digitalisierte physische Rechnungen oder E-Mails von Lieferanten. Dateien können entweder direkt hochgeladen oder URL-Links zu Dateien hinzugefügt werden, die in einem externen Dateiverwaltungssystem gespeichert sind. Dokumente können auch an eine Rechnung angehängt werden, z.B. Bilder von physischen Rechnungen oder E-Mails von einem Lieferanten.

### Link hinzufügen

1.  Auf **Link hinzufügen** klicken.
2.  Einen **Linknamen** eingeben, um den Dateilink zu identifizieren.
3.  Optional: Eine **externe URL** für eine aktive Website eingeben.

Wenn ein Link gelöscht werden soll, auf das **Löschsymbol** klicken.

### Dokument hinzufügen

Es gibt zwei Möglichkeiten, ein Dokument hinzuzufügen:

* Eine Datei per Drag & Drop in das vorgesehene Feld ziehen oder
* Auf **oder Datei auswählen** klicken, um ein Dokument aus den lokalen Dateien hinzuzufügen.

Wenn ein Dokument gelöscht werden soll, auf das **Löschsymbol** klicken.

## Rechnung speichern und schließen

Dies ist das Ende des Bildschirms Neue Rechnung erstellen. Auf **Speichern & schließen** klicken, um die Rechnung zu speichern.

Es müssen neue **Rechnungsposten hinzugefügt oder erstellt** werden, bevor die Rechnung genehmigt oder bezahlt werden kann.

* Um einen bestehenden Bestellposten für eine offene Bestellung mit der Rechnung zu verknüpfen, den Schritten zum [Hinzufügen eines Rechnungspostens zu einer Rechnung]({{< ref "020 Rechnung einen Rechnungsposten hinzufuegen" >}}) folgen. Die Informationen aus dem Bestellposten werden in die Felder der Rechnungsposten übernommen, z.B. das Startdatum des Abonnements, das Enddatum des Abonnements und die Anzahl. Die Kontonummer und der Buchhaltungscode werden aus dem Kontobereich des Lieferanten im Organisationsdatensatz abgeleitet. Unter [Organisationen > Konten]({{< ref "020 Organisation als Lieferanten anlegen" >}}) sind weitere Informationen zu Lieferantenkonten zu finden.
* Um einen neuen Rechnungsposten zu erstellen, der nicht mit einer Bestellung verknüpft ist, den Schritten zum [Erstellen eines neuen Rechnungspostens](https://info.gbv.de/pages/viewpage.action?pageId=851345662) folgen.
