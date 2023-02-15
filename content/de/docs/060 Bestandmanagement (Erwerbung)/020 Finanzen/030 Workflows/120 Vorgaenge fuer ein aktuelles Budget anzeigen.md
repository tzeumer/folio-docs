---
title: "Vorgänge für ein aktuelles Budget anzeigen"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-finanzen, by-folio, cat-workflows, by-folio]
weight: 120
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/acquisitions/finance/#viewing-transactions-for-a-current-budget) & [GBV](https://info.gbv.de/pages/viewpage.action?pageId=850002057)
    "
---

Es gibt zwei Methoden, um eine Liste aller Vorgänge für ein Budget anzuzeigen:

* Von einem Fonds aus: [Den Fonds suchen]({{< ref "060 Haushaltsjahr, Etat, Gruppe, Fonds suchen" >}}), für den Vorgänge angezeigt werden sollen und ihn auswählen, um die Ansicht der Fondsdetails zu öffnen. Auf **Aktionen > Vorgänge für das aktuelle Budget anzeigen** klicken.
* Von einem Budget aus: [Das Budget suchen]({{< ref "060 Haushaltsjahr, Etat, Gruppe, Fonds suchen" >}}), für das Vorgänge angezeigt werden sollen und es auswählen. Im Fenster **Budgetdetails** unter Vorgänge auf **Vorgänge anzeigen** klicken. Das Fenster Vorgänge öffnet sich und zeigt alle Vorgänge an.

## Budgetvorgänge suchen

Um nach Budgetvorgängen zu suchen, wie folgt vorgehen:

1.  Um Budgetvorgänge nach Betrag zu suchen, im Fenster **Vorgänge** in der Ansicht **Suche & Filter** einen numerischen Wert in das Suchfeld eingeben und auf **Suche** klicken. Eine Liste der Vorgänge erscheint, die den eingegebenen Betrag enthalten.
2.  Um die Ergebnisse nach Typ, Quelle, Tags oder Kostenart zu filtern, sind Informationen zu den Filtern weiter unten zu finden. Die Ergebnisse werden in der Ansicht Vorgänge angezeigt.

### Typ

Um Vorgänge nach Typ zu filtern, eine der folgenden Möglichkeiten wählen:

* **Zuweisung**. Filtert Vorgänge nach der Art der Zuweisung.
* **Gutschrift**. Filtert Vorgänge nach der Art des Kredits.
* **Bindung**. Filtert Vorgänge nach der Art der Bindung.
* **Zahlung**. Filtert Vorgänge nach der Art der Zahlung.
* **Ausstehende Zahlung**. Filtern Sie Vorgänge nach der Art der ausstehenden Zahlung.
* **Übertrag beim Jahresübergang**. Filtert Vorgänge nach der Art des Jahresübergangs.
* **Transfer/Übertrag**. Filtert Vorgänge nach der Art des Transfers.

### Quelle

Um Vorgänge nach Quelle zu filtern, eine der folgenden Möglichkeiten wählen:

* **Haushaltsjahr**. Vorgänge, die während des Jahresübergangs des Haushaltsjahres generiert wurden. Zum Beispiel automatische Zuweisungen während des Jahresübergangs, wie in [Einstellungen für den Jahresübergang]({{< ref "150 Jahresuebergang durchfuehren" >}})g definiert.
* **Rechnung**. Vorgänge, die durch die Rechnungsstellung generiert werden, insbesondere Vorgangsarten wie Gutschrift und Ausstehende Zahlung.
* **Bestellposten**. Vorgänge, die aus einem Bestellposten generiert werden, insbesondere Bindungs-Vorgangsarten.
* **Personen**. Vorgänge, die von einer Person über das Aktionsmenü des Fonds erstellt wurden, insbesondere die Transaktionsarten Zugewiesen und Transferieren.

### Bestellpostennummer der Quelle

Folgendermaßen vorgehen, um Vorgänge nach der Bestellpostennummer der Quelle zu filtern:

1.  In der Ansicht **Suche & Filter** auf **Bestellpostennummer der Quelle** klicken.
2.  Mit der Eingabe des Bestellpostens beginnen und aus der Dropdown-Liste auswählen. Das Ergebnis wird in der Ansicht Vorgänge angezeigt.

### Rechnungsnummer der Quelle

Folgendermaßen vorgehen, um Vorgänge nach der Rechnungsnummer zu filtern:

1.  In der Ansicht **Suche & Filter** auf **Rechnungsnummer der Quelle** klicken.
2.  Mit der Eingabe der Rechnungsnummer beginnen und aus der Dropdown-Liste wählen. Das Ergebnis wird in der Ansicht Vorgänge angezeigt.

### Tags

Um nach Vorgängen zu filtern, die mit bestimmten Tags versehen sind, wie folgt vorgehen:

1.  In der Ansicht **Suche & Filter** auf **Tags** klicken.
2.  Die Tags aus der Dropdown-Liste auswählen. Die Ergebnisse werden in der Ansicht Vorgänge angezeigt.

### Kostenart

Um Vorgänge nach Kostenart zu filtern, wie folgt vorgehen:

1.  In der Ansicht **Suche & Filter** auf **Kostenart** klicken.
2.  Eine Kostenart aus der Dropdown-Liste wählen. Die Ergebnisse werden in der Ansicht Vorgänge angezeigt.

Nach der Suche erscheinen die folgenden Spalten in der Tabelle der Suchergebnisse im Bereich Vorgänge. Auf den Spaltennamen klicken, um nach dieser Spalte zu sortieren.

* **Vorgangsdatum**. Datum des Vorgangs.
* **Typ**. Art des Vorgangs: Zuweisung, Gutschrift, Bindung, Zahlung, Ausstehende Zahlung oder Transfer.
* **Betrag**. Betrag für die Transaktion. Negative Werte stehen in Klammern.
* **Von**. Fondscode des Fonds, aus dem ein Transfer in den Haushalt vorgenommen wurde.
* **Zu/auf**. Fondscode des Fonds, an den ein Transfer aus dem Haushalt vorgenommen wurde.
* **Quelle**. Haushaltsjahr, Rechnung, Bestellposten oder Person.
* **Tags**. Alle mit der Transaktion verbundenen Markierungen.

## Budgetvorgänge anzeigen

Um zusätzliche Informationen zu einer Transaktion anzuzeigen, auf die Transaktionszeile in der Tabelle klicken, um eine detaillierte Ansicht zu öffnen. Jeder Vorgangstyp zeigt eine andere Gruppe von Feldern an, die für diesen Typ relevant sind. Im Folgenden sind Informationen zu den Feldern zu finden, die für jeden Typ angezeigt werden.

### Zuweisungsvorgänge anzeigen

* **Datensatz zuletzt aktualisiert**. Datum und Uhrzeit, zu der der Datensatz zuletzt aktualisiert wurde. Auf **Datensatz zuletzt aktualisiert** klicken, um die nächsten drei Felder anzuzeigen.
    * **Quelle**. Name der Person, die den Datensatz zuletzt aktualisiert hat.
    * **Datensatz erstellt**. Datum und Uhrzeit, zu der der Datensatz erstellt wurde.
    * **Quelle**. Name der Person, die den Datensatz erstellt hat.
* **Vorgangsdatum**. Datum des Vorgangs.
* **Haushaltsjahr**. Das Haushaltsjahr für das Budget.
* **Betrag**. Betrag der Transaktion. Negative Werte stehen in Klammern.
* **Quelle**. Haushaltsjahr oder Person.
* **Typ**. Art des Vorgangs: Zuweisung.
* **Von**. Fondsname und Fondscode, aus dem die Zuweisung in dieses Budget erfolgt ist, falls zutreffend. Weitere Informationen sind unter [Budget Mittel zuweisen]({{< ref "090 Budget Mittel zuweisen" >}}) zu finden.
* **Zu/auf**. Fondsname und Fondscode dieses Budgets, in das die Zuweisung erfolgt ist.
* **Kostenart**. Dieses Feld bleibt bei Vorgängen für Zuweisungen leer, da Kostenarten für Zuweisungen vom System nicht unterstützt werden.
* **Tags**. Alle mit dem Vorgang verbundenen Tags.
* **Beschreibung**. Eine Beschreibung, die von der Person bei der Zuweisung von Mitteln zu einem Budget eingegeben wird.

### Gutschriftvorgänge anzeigen

Die Ansicht für Gutschriftenvorgänge enthält viele der gleichen Felder wie die Ansicht für die Zuweisung. Einige Felder werden bei Gutschriftenvorgängen anders ausgefüllt:

* **Quelle**. Rechnungsnummer oder Kennung, die diesen Gutschriftenvorgang erzeugt hat. Auf die Rechnungskennung klicken, um die Rechnungsansicht der App Rechnungen für diese Rechnung zu öffnen.
* **Typ**. Art des Vorgangs: Gutschrift.
* **Von**. Dieses Feld ist bei Gutschriftenvorgängen leer.
* **Zu/auf**. Fondsname und Fondscode dieses Budgets, auf das die Gutschrift erfolgt ist.
* **Beschreibung**. Dieses Feld ist bei Gutschriftenvorgängen leer.

### Bindungsvorgänge anzeigen

Wenn ein Auftrag geöffnet wird, der einen Bestellposten mit einer Fondsaufteilung enthält, wird ein Bindungsvorgang gegen das Budget des aktuellen Haushaltsjahres für den Fonds erstellt. Die Ansicht für Bindungsvorgänge enthält viele der gleichen Felder wie die Ansicht für Zuweisungen. Einige Felder werden für Bindungsvorgänge anders ausgefüllt:

* **Quelle**. Die Nummer des Bestellpostens, der diesen Bindungsvorgang erzeugt hat. Auf die Bestellpostennummer klicken, um die Bestellpostenansicht der App Bestellungen für diese Bestellposition zu öffnen.
* **Typ**. Art des Vorgangs: Bindung.
* **Von**. Fondsname und -code für dieses Budget, auf das diese Bindung angewendet wurde.
* **Zu/auf**. Dieses Feld ist bei Bindungsvorgängen leer.
* **Kostenart**. Die diesem Bindungsvorgang zugewiesene Kostenart.
* **Anfängliche Bindung**. Der Betrag, der anfänglich durch die zugehörige Bestellposition belastet wurde; der Schätzpreis.
* **Zur Zahlung vorgesehen**. Der Betrag, der auf die Zahlung wartet.
* **Ausgaben**. Der aufgewendete Betrag. Dieser Betrag wird ausgefüllt, nachdem eine Rechnung für den zugehörigen Bestellposten bezahlt wurde.
* **Status**. Der Status dieser Bindung: Nicht freigegeben oder Freigegeben. Die Bindung kann manuell durch die Person oder automatisch durch das System nach Zahlung einer Rechnung freigegeben werden.
* **Beschreibung**. Dieses Feld ist bei Bindungsvorgängen leer.

#### Bindungen manuelle freigeben

Wenn eine Bestellung freigegeben werden muss, ist diese Aktion über die Vorgangsdetails des belasteten Budgets verfügbar. Dies kann erforderlich sein, um Forderungen im Zusammenhang mit laufenden Aufträgen zu verwalten. Um eine Bindung freizugeben, muss die Person über [die Berechtigung]({{< ref "080 Person Rechte zuweisen" >}}) Finanzen: Manuelle Freigabe der Bindung zugewiesen sein.

Um eine Bindung freizugeben, folgendermaßen vorgehen:

1.  Die Vorgangsliste für das belastete Budget suchen. Weitere Informationen sind unter am Anfang dieser Seite zu finden.
2.  Den Bindungsvorgang aus der Ergebnisliste auswählen.
3.  In der Ansicht für die Details der Bindung auf **Bindung freigeben** klicken.
4.  Im Bestätigungsfenster auf **Bestätigen** klicken, um die Meldung "Sind Sie sicher, dass Sie diese Bindung auflösen möchten? Der verbleibende Betrag wird dem Budget wieder gutgeschrieben." zu erhalten. Ein eventuell verbleibender Betrag wird dem Budget wieder hinzugefügt.
5.  Die Bindung wird freigegeben. Der Betrag wird dem Budget wieder hinzugefügt und der Statuswert in der Ansicht für die Bindung ändert sich von Nicht freigegeben in Freigegeben.

### Zahlungsvorgänge anzeigen

Wenn eine Rechnung bezahlt wird, wird der Wert des bestehenden Datensatzes **Ausstehende Zahlung** vom Typ Ausstehende Zahlung auf den Typ **Zahlung** aktualisiert. Die Ansicht für die Zahlungsvorgänge enthält viele der gleichen Felder wie die Ansicht für die Zuweisungen. Einige Felder werden bei Zahlungsvorgängen anders ausgefüllt:

* **Quelle**. Rechnungsnummer oder Kennung, die diesen Gutschriftenvorgang erzeugt hat. Auf die Rechnungskennung klicken, um die Rechnungsdetailsansicht der App Rechnungen für diese Rechnung zu öffnen.
* **Typ**. Art des Vorgangs: Zahlung.
* **Von**. Fondsname und -code für das Budget, dem diese Zahlung zugewiesen wurde.
* **Zu/auf**. Bei Zahlungsvorgängen bleibt dieses Feld leer.
* **Beschreibung**. Dieses Feld ist bei Zahlungsvorgängen leer.

### Ausstehende Zahlung - Vorgänge anzeigen

Wenn eine Rechnung freigegeben wird, wird ein Vorgangsdatensatz der Art **Ausstehende Zahlung** für das Budget des aktuellen Haushaltsjahres des Fonds erstellt. Der ursprüngliche Datensatz des Bindungsvorgangs für einen zugehörigen Bestellposten bleibt in der Vorgangsliste für das Budget bestehen. Der Betragswert des Bindungsvorgangs wird aktualisiert, wenn eine Rechnung freigegeben wird, da die Genehmigung der Rechnung den Betrag der ausstehenden Zahlung der Bindung freigibt. Sobald eine Rechnung bezahlt ist, wird der Wert der Transaktionsart von **Ausstehende Zahlung** in **Zahlung** geändert. Die Ansicht der ausstehenden Zahlungsvorgänge enthält dieselben Felder wie die Ansicht der Zahlungsvorgänge.

### Jahresübergangs-Transfervorgängen anzeigen

Der Prozess des Jahresübergangs erstellt Transfervorgänge, wenn die [Einstellungen für den Jahresübergang]({{< ref "150 Jahresuebergang durchfuehren" >}}) so definiert sind, dass Transfers in neue Haushaltsjahrbudgets durchgeführt werden.

### Transfervorgängen anzeigen

Wenn Mittel zwischen zwei Fonds transferiert werden, wird eine Transfervorgang erstellt. Die Ansicht für die Transfers enthält viele der gleichen Felder wie die Ansicht für die Zuweisung. Einige Felder werden bei Transfer Vorgängen anders ausgefüllt:

* **Quelle**. Bei Transfervorgängen auf Person eingestellt.
* **Typ**. Art des Vorgangs: Transfer.
* **Von**. Fondsname und Fondscode, aus dem der Transfer in dieses Budget erfolgt ist.
* **Auf/zu**. Fondsname und Fondscode dieses Budgets, in das die Zuweisung erfolgt ist.
* **Beschreibung**. Eine Beschreibung, die von der Person während des Transfers hinzugefügt wurde.
