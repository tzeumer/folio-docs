---
title: "Haushaltsjahr, Etat, Gruppe, Fonds anzeigen"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-finanzen, by-folio, cat-workflows, by-folio, meta-gemeldet_docsfolioorg]
weight: 70
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/acquisitions/finance/#viewing-fiscal-year-ledger-group-fund-and-budget-details ) & [GBV](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio:+Haushaltsjahr,+Etat,+Gruppe,+Fonds+anzeigen)
    "
---

Die Art der Informationen, die in Ihren Suchergebnissen angezeigt werden, hängt von der Art der durchgeführten Suche ab (Haushaltsjahr, Etat, Gruppe oder Fonds). Diese können folgende Informationen umfassen:

* **Name**. Der Name des Haushaltsjahres, des Etats, der Gruppe, des Fonds oder des Budgets.
* **Code**. Ein eindeutiger Identifikator für das Haushaltsjahr, den Etat, die Gruppe, den Fond oder das Budget.
* **Beschreibung**. Der Zweck des Haushaltsjahres, des Etats, der Gruppe, des Fonds oder des Budgets.
* **Status**. Gibt an, ob der Etat, die Gruppe, der Fonds oder das Budget aktiv, inaktiv oder gesperrt ist.
* **Etat**. Das mit dem Fonds verbundene Etat.

In den Suchergebnissen auf ein beliebiges Ergebnis klicken, um es anzuzeigen. In der Ansicht Haushaltsjahr, Etat, Gruppe oder Fonds werden jeweils zusätzliche Informationen, einschließlich Finanzübersichten, angezeigt. Fonds, die über ein Budget für das Haushaltsjahr verfügen, werden in der Ansicht mit den Details zum Haushaltsjahr angezeigt. Fonds, die über ein Budget für das aktuelle Geschäftsjahr verfügen, werden in der Ansicht für das Etat oder die Gruppe angezeigt. Fonds, für die keine Budgets erstellt wurden, erscheinen nur in der Ansicht der Fondssuchergebnisse.

## Haushaltsjahr: Details anzeigen

Der Detailbereich für das Haushaltsjahr enthält eine Zusammenfassung der Finanzdaten des Haushaltsjahres sowie alle mit dem Haushaltsjahr verbundenen Etats, Gruppen und Fonds.

* Um Details zum Haushaltsjahr anzuzeigen, das gewünschte Haushaltsjahr suchen und es auswählen. Die Ansicht Haushaltsjahr-Details wird angezeigt.

### Informationen zum Haushaltsjahr

Der Abschnitt Informationen zum Haushaltsjahr enthält die folgenden Felder:

* **Datensatz zuletzt aktualisiert**. Datum und Uhrzeit, zu der der Datensatz zuletzt aktualisiert wurde. Auf Datensatz zuletzt aktualisiert klicken, um die nächsten drei Felder anzuzeigen.
    * **Quelle**. Name der Person, die den Datensatz zuletzt aktualisiert hat.
    * **Datensatz erstellt**. Datum und Uhrzeit, zu der der Datensatz erstellt wurde.
    * **Quelle**. Name der Person, die den Datensatz erstellt hat.
* **Name**. Name des Haushaltsjahres.
* **Code**. Code für das Haushaltsjahr.
* **Beginn des Zeitraums**. Datum, an dem das Haushaltsjahr beginnt.
* **Ende des Zeitraums**. Datum, an dem das Haushaltsjahr endet.
* **Erwerbungsteams**. Alle Erwerbungsteams, die dem Haushaltsjahr zugeordnet sind.
* **Beschreibung**. Beschreibung des Haushaltsjahres.

### Finanzübersicht

In diesem Abschnitt wird eine Tabelle mit zusammenfassenden Finanzinformationen für alle dem Haushaltsjahr zugeordneten Fonds-Budgets angezeigt.

**Informationen zur Finanzierung**

* **Anfängliche Zuweisung**. Der Betrag der ersten Zuweisung an ein Budget, zusammengefasst für alle Fonds-Budgets für das Haushaltsjahr.
* **Insgesamt zugewiesen**. Die Summe aller Zuweisungsbeträge über alle Fonds-Budgets für das Haushaltsjahr (anfängliche Zuweisung plus Erhöhung der Zuweisung minus Verringerung der Zuweisung)
* **Gesamtfinanzierung**. Der gesamte zugewiesene Betrag plus der Betrag der Netto-Transfers. Anmerkung: Für die Übersicht über das Haushaltsjahr wird der Netto-Transferbetrag nicht angezeigt, da das System nur Transfers zwischen Budgets innerhalb desselben Haushaltsjahres zulässt. Netto-Transferbeträge werden nur in den Übersichtstabellen Etat, Gruppe und Budget angezeigt.
* **Kassenbestand**. Der Gesamtbetrag der Fonds abzüglich des ausgegebenen Betrags.
**Finanzielle Aktivität & Überschüsse**

* **Gebunden**. Die Summe aller Transaktionsbeträge mit Bindung gegen alle Fonds-Budgets für das Haushaltsjahr.
* **Zu Bezahlung vorgesehen**. Die Summe aller Vorläufigen Zahlungstransaktionsbeträge für alle Fondsbudgets für das Haushaltsjahr.
* Ausgaben. Die Summe aller Zahlungstransaktionsbeträge abzüglich der Kredittransaktionsbeträge zu Lasten aller Fondsbudgets für das Haushaltsjahr.
* **Nicht verfügbar**. Der gesamte nicht verfügbare Betrag aller Fonds-Budgets für das Haushaltsjahr, berechnet als Summe der belasteten, zur Zahlung anstehenden und ausgegebenen Beträge.
* **Überzogene Bindung**. Der gesamte belastete Betrag abzüglich des gesamten Finanzierungsbetrags für alle Fondsbudgets für das Haushaltsjahr.
* **Überzogene Ausgaben**. Der Gesamtbetrag der Ausgaben abzüglich des Gesamtbetrags der Mittel aller Fonds-Budgets für das Haushaltsjahr.
* **Verfügbares Guthaben**. Verfügbarer Gesamtbetrag aller Fonds-Budgets für das Haushaltsjahr, berechnet als **Gesamtfinanzierung** abzüglich des **nicht verfügbaren** Betrags. Anmerkung: In dieser Version von FOLIO werden negative verfügbare Salden als 0 € angezeigt. Wenn z. B. das Feld für zulässige Ausgaben für das Budget leer ist, gibt es keine Einschränkungen, wie viel für das Budget ausgegeben werden kann. Wenn Transaktionen verarbeitet wurden, die den Gesamtfinanzierungsbetrag um 100 € übersteigen, wird der Betrag im Feld Verfügbares Guthaben als 0 € und nicht als negativ (100 €) angezeigt. Negative Saldenbeträge werden in einer zukünftigen Version des Systems angezeigt.

### Etat

In diesem Abschnitt wird eine Tabelle mit allen dem Haushaltsjahr zugeordneten Etats angezeigt. Um nach einer Spalte zu sortieren, auf den Spaltennamen klicken. Um Details zu einem Etat in der Tabelle anzuzeigen, auf eine beliebige Stelle in der Zeile des Etats klicken.

Die Tabelle der Etats enthält die folgenden Spalten:

* **Name**. Name des Etats.
* **Code**. Code für den Etat.
* **Zugewiesen**. Gesamtbetrag, der allen Fonds mit einem Budget für das Haushaltsjahr zugewiesen wurde, die mit dem Etat verbunden sind.
* **Nicht verfügbar**. Nicht verfügbarer Gesamtbetrag für alle Fonds mit einem Budget für das Haushaltsjahr, die mit dem Etat verbunden sind.
* **Verfügbar**. Verfügbarer Gesamtbetrag für alle Fonds mit einem Budget für das Haushaltsjahr, die mit dem Etat verbunden sind.

### Gruppe

In diesem Abschnitt wird eine Tabelle mit allen Gruppen angezeigt, die mit dem Haushaltsjahr verbunden sind. Die Tabelle enthält die gleichen Spalten wie die Tabelle Etat.

### Fonds

In diesem Abschnitt wird eine Tabelle mit allen Fonds angezeigt, die mit dem Haushaltsjahr verbunden sind. Die Tabelle enthält die gleichen Spalten wie die Tabelle Etat.

## Etat-Details anzeigen

Die Ansicht Etat-Informationen enthält eine Zusammenfassung der Finanzdaten des Etats sowie alle mit dem Etat verbundenen Gruppen und Fonds.

* Um die Details zu einem Etat anzuzeigen, den gewünschte Etat suchen und auswählen. Die Ansicht des Etats wird angezeigt.

### Etat-Informationen

Der Abschnitt Etat-Informationen enthält die folgenden Felder:

* **Datensatz zuletzt aktualisiert**. Datum und Uhrzeit, zu der der Datensatz zuletzt aktualisiert wurde. Auf Datensatz zuletzt aktualisiert klicken, um die nächsten drei Felder anzuzeigen.
    * **Quelle**. Name der Person, die den Datensatz zuletzt aktualisiert hat.
    * **Datensatz erstellt**. Datum und Uhrzeit, zu der der Datensatz erstellt wurde.
    * **Quelle**. Name der Person, die den Datensatz erstellt hat.
* **Bezeichnung**. Name des Etats.
* **Code**. Code für das Etat.
* **Aktuelles Haushaltsjahr**. Der Name des aktuellen Haushaltsjahres. Das System ermittelt das aktuelle Haushaltsjahr anhand des aktuellen Datums und des Beginns und Endes des Zeitraums für das Haushaltsjahr.
* **Status**. Der Status des Etats: Aktiv, Inaktiv, Gesperrt.
* **Erwerbungsteams**. Alle Erwerbungsteams, die dem Etat zugeordnet sind.
* **Beschreibung**. Beschreibung des Etats.

### Finanzübersicht

**Informationen zur Finanzierung**

* **Anfängliche Zuweisung**. Der Betrag der ersten Zuweisung an ein Budget, zusammengefasst für alle Fonds-Budgets für das Etat.
* Erhöhung der Zuweisung. Die Summe aller Zuweisungstransaktionsbeträge, ohne die anfänglichen Zuweisungen, die für alle Fonds-Budgets für das Etat vorgenommen wurden.
* **Verringerung der Zuweisung**. Die Summe aller Zuweisungstransaktionsbeträge, ohne die anfänglichen Zuweisungen, die von allen Fondsbudgets für das Etat vorgenommen wurden.
* **Insgesamt zugewiesen**. Die Summe aller Zuweisungsbeträge aus allen Fonds-Budgets für das aktuelle Haushaltsjahr, die mit dem Etat verbunden sind (anfängliche Zuweisung plus Erhöhung der Zuweisung minus Verringerung der Zuweisung).
* **Netto-Transfers**. Die Summe der Netto-Transferbeträge für alle Fonds-Budgets für das aktuelle Haushaltsjahr, die mit dem Etat verbunden sind.
* **Gesamtfinanzierung**. Der gesamte zugewiesene Betrag plus der Betrag der Netto-Transfers.
* **Kassenbestand**. Der Betrag der Gesamtfinanzierung abzüglich des Betrags für die Ausgaben.
**Finanzielle Aktivität & Überschüsse**

* **Gebunden**. Die Summe aller Beträge von Bindungstransaktionen gegen alle Fondsbudgets für den Etat während des laufenden Haushaltsjahres.
* **Zu Bezahlung vorgesehen**.  Die Summe aller Transaktionsbeträge für ausstehende Zahlungen für alle Fondsbudgets des Etats im laufenden Haushaltsjahr.
* **Ausgaben**. Die Summe aller Zahlungstransaktionsbeträge abzüglich der Kredittransaktionsbeträge für alle Fondsbudgets für das Etat im laufenden Haushaltsjahr.
* **Nicht verfügbar**. Der Gesamtbetrag, der im aktuellen Haushaltsjahr für alle Fondsbudgets des Etats nicht verfügbar ist, berechnet als Summe der belasteten, noch zu zahlenden und ausgegebenen Beträge.
* **Überzogene Bindung (fehlte; Formulierung richtig?)**. Der gesamte belastete Betrag abzüglich des gesamten Finanzierungsbetrags für alle Fondsbudgets des Etats für das Haushaltsjahr.
* **Überzogene Ausgaben (fehlte; Formulierung richtig?)**. Der Gesamtbetrag der Ausgaben abzüglich des Gesamtbetrags der Mittel aller Fonds-Budgets des Etats für das Haushaltsjahr.
* **Verfügbares Guthaben**. Verfügbarer Gesamtbetrag aller Fonds-Budgets für das Etat im laufenden Haushaltsjahr, berechnet als **Gesamtfinanzierung** abzüglich des **nicht verfügbaren** Betrags. Anmerkung: In dieser Version von FOLIO werden negative verfügbare Guthaben als 0 € angezeigt. Wenn z. B. das Feld für zulässige Ausgaben für das Budget leer ist, gibt es keine Einschränkungen, wie viel für das Budget ausgegeben werden kann. Wenn Transaktionen verarbeitet wurden, die den Betrag der Gesamtfinanzierung um 100 € übersteigen, wird der Betrag im Verfügbaren Guthaben als 0 € und nicht als negativ (100 €) angezeigt. Negative Saldenbeträge werden in einer zukünftigen Version des Systems angezeigt.

### Gruppe

In diesem Abschnitt wird eine Tabelle mit allen Gruppen angezeigt, die mit dem Etat verbunden sind. Um nach einer Spalte zu sortieren, auf den Spaltennamen klicken. Um Details zu einer Gruppe in der Tabelle anzuzeigen, auf eine beliebige Stelle in der Zeile der Gruppe klicken.

Die Tabelle Gruppe enthält die folgenden Spalten:

* **Name**. Name der Gruppe.
* **Code**. Code für die Gruppe.
* **Zugewiesen**. Zugewiesener Gesamtbetrag für alle Fonds mit einem Budget für das Haushaltsjahr, die mit der Gruppe verbunden sind.
* **Nicht verfügbar**. Gesamtbetrag, der für alle Fonds mit einem Budget für das Haushaltsjahr, die mit der Gruppe verbunden sind, nicht verfügbar ist.
* **Verfügbar**. Verfügbarer Gesamtbetrag für alle Fonds mit einem Budget für das Haushaltsjahr, die mit der Gruppe verknüpft sind.

### Fonds

In diesem Abschnitt wird eine Tabelle mit allen Fonds angezeigt, die mit dem Etat verbunden sind. Die Tabelle enthält die gleichen Spalten wie die Tabelle Gruppe.

### Fehlerprotokoll für Jahresübergänge im Haushaltsjahr

In diesem Abschnitt wird die Liste der Fehlerprotokolle für Jahresübergänge angezeigt. Klicken Sie auf den .csv-Dateinamen, um das Fehlerprotokoll herunterzuladen.

## Etats und Budgets exportieren

Wie folgt vorgehen, um eine Datei mit Budgetinformationen für Fonds, die einem Etat zugeordnet sind, im Format Komma-getrennte Werte (.csv) zu exportieren:

In der Ansicht **Suche & Filter** die Such- und Filteroptionen verwenden, um ein **Etat** auszuwählen. Auf den Etat in der Ergebnistabellenliste klicken. In der Ansicht des Etats auf **Aktionen** klicken und **Budgetinformationen exportieren (CSV)** wählen.

Im Dialogfeld **Exporteinstellungen** wird die folgende Meldung angezeigt: "Dieser Export kann einige Minuten dauern. Wenn Sie die Seite neu laden oder schließen, wird der Export nicht fertiggestellt. Sobald die Datei bereitgestellt ist, kann Ihr Browser eine Weile benötigen, um das Herunterladen zu beenden. Sie können bei Bedarf in einem anderen Browser-Tab an weiteren Rechnungen und Rechnungsposten arbeiten."

Das zu exportierende **Haushaltsjahr** aus der Dropdown-Liste auswählen.

Die zu exportierenden **Kostenarten** aus der Dropdown-Liste auswählen: Alle, Aktiv, Inaktiv, Keine.

Auf **Exportieren** klicken. Die Datei wird an heruntergeladen und enthält die folgenden Felder:

**Liste der Felder der Etat-Fonds-Budgets, die exportiert werden:**

* Name (Fund) (Name (Fonds))
* Code (Fund) (Code (Fonds))
* Status (Fund) (Status (Fonds))
* Type (Typ)
* Group (Code) (Gruppe (Code))
* Acquisition unit (Erwerbungsteams)
* Transfer from (Übertragung von)
* Transfer to (Überweisung an)
* External account number (Externe Kontonummer)
* Description (Beschreibung)
* Name (Budget) (Bezeichnung (Budget))
* Status (Budget) (Status (Haushalt))
* Allowable encumbrance (Zulässige Bindung)
* Allowable expenditure (Zulässige Ausgaben)
* Date created (Budget) (Erstellungsdatum (Haushalt))
* Initial allocation (Anfängliche Zuweisung)
* Increase (Erhöhung)
* Decrease (Verringerung)
* Total allocation (Zuweisung insgesamt)
* Transfers (Übertragungen)
* Total Funding (Gesamtfinanzierung)
* Encumbered (Budget) (Verrechnet (Haushalt))
* Awaiting payment (Budget) (In Erwartung einer Zahlung (Haushalt))
* Expended (Budget) (Verausgabt (Haushaltsplan))
* Unavailable (Nicht verfügbar)
* Over encumbered (Zu viel belastet)
* Over expended (Überzogene Ausgaben)
* Cash balance (Kassenbestand)
* Available (Verfügbar)
* Name (Exp Class) (Name (Ausgabenklasse))
* Code (Exp Class) (Code (Ausgabenklasse))
* Status (Exp Class) (Status (Ausgabenklasse))
* Encumbered (Exp Class) (Belastet (Exp Klasse))
* Awaiting payment (Exp Class) (In Erwartung einer Zahlung (Exp Class))
* Expended (Exp Class) (Ausgegeben (Ausgabenklasse))
* Percentage of total expended (Prozentsatz der Gesamtausgaben)

## Gruppendetails anzeigen

Die Ansicht Gruppendetails enthält eine Zusammenfassung der Finanzdaten der Gruppe und listet alle Fonds und Kostenarten auf, die mit der Gruppe verbunden sind.

* Um die Gruppendetails anzuzeigen, die Gruppe suchen, die angezeigt werden soll und sie auswählen. Die Ansicht Gruppendetails wird angezeigt.

### Informationen zur Gruppe

* **Datensatz zuletzt aktualisiert**. Datum und Uhrzeit, zu der der Datensatz zuletzt aktualisiert wurde. Auf **Datensatz zuletzt aktualisiert** klicken, um die nächsten drei Felder anzuzeigen.
    * **Quelle**. Name der Person, die den Datensatz zuletzt aktualisiert hat.
    * **Datensatz erstellt**. Datum und Uhrzeit, zu der der Datensatz erstellt wurde.
    * **Quelle**. Name der Person, die den Datensatz erstellt hat.
* **Name**. Name der Gruppe.
* **Code**. Code für die Gruppe.
* **Haushaltsjahr**. Name des zwölfmonatigen Zeitraums, den die Bibliothek für die Verwaltung ihrer Finanzen verwendet. Als Standard wird das aktuelle Haushaltsjahr angezeigt. Die Dropdown-Liste verwenden, um ein anderes Haushaltsjahr auszuwählen. Die Übersicht der Finanzdaten wird für das ausgewählte Haushaltsjahr angezeigt.
* **Status**. Status der Gruppe: Aktiv, Inaktiv, Gesperrt.
* **Erwerbungsteams**. Alle Erwerbungsteams, die der Gruppe zugeordnet sind.
* **Beschreibung**. Beschreibung der Gruppe.

### Finanzübersicht

**Informationen zur Finanzierung**

* **Anfängliche Zuweisung**. Der Betrag der ersten Zuweisung an ein Budget, zusammengefasst für alle Fonds-Budgets der Gruppe.
* **Erhöhung der Zuweisung**. Die Summe aller Zuweisungstransaktionsbeträge, ohne die anfänglichen Zuweisungen, die an alle Fonds-Budgets für die Gruppe vorgenommen wurden.
* **Verringerung der Zuweisung**. Die Summe aller Zuweisungstransaktionsbeträge, ohne die anfänglichen Zuweisungen, die von allen Fondsbudgets für die Gruppe vorgenommen wurden.
* **Insgesamt zugewiesen**. Die Summe aller zugewiesenen Beträge über alle Fonds-Budgets für das ausgewählte Haushaltsjahr, die mit der Gruppe verbunden sind (anfängliche Zuweisung plus Erhöhung der Zuweisung minus Verringerung der Zuweisung).
* **Netto-Transfers**. Gesamtbetrag der Netto-Transfers für alle Fonds-Budgets für das ausgewählte Haushaltsjahr, die mit der Gruppe verknüpft sind.
* **Gesamtfinanzierung**. Der gesamte zugewiesene Betrag plus der Betrag der Netto-Transfers.
* **Kassenbestand**. Der Betrag der Gesamtfinanzierung abzüglich des Betrags für die Ausgaben.
**Finanzielle Aktivität & Überschüsse**

* **Gebunden**. Die Summe der Beträge der Bindungstransaktionen gegen alle Fondsbudgets für die Gruppe während des ausgewählten Haushaltsjahres.
* **Zur Bezahlung vorgesehen**. Die Summe der Transaktionsbeträge für ausstehende Zahlungen für alle Fondsbudgets der Gruppe im ausgewählten Haushaltsjahr.
* **Ausgaben**. Die Summe der Zahlungstransaktionsbeträge abzüglich der Kredittransaktionsbeträge für alle Fondsbudgets der Gruppe im ausgewählten Haushaltsjahr.
* **Nicht verfügbar**. Gesamtbetrag, der in dem ausgewählten Haushaltsjahr für alle Fonds-Budgets der Gruppe nicht verfügbar ist, berechnet als Summe der belasteten, zur Zahlung anstehenden und ausgegebenen Beträge.
* **Überzogene Bindung (fehlte; Formulierung richtig?)**. Der gesamte belastete Betrag abzüglich des gesamten Finanzierungsbetrags für alle Fondsbudgets der Gruppe für das Haushaltsjahr.
* **Überzogene Ausgaben (fehlte; Formulierung richtig?)**. Der Gesamtbetrag der Ausgaben abzüglich des Gesamtbetrags der Mittel aller Fonds-Budgets der Gruppe für das Haushaltsjahr.
* **Verfügbares Guthaben**. Verfügbarer Gesamtbetrag aller Fondsbudgets für die Gruppe im ausgewählten Haushaltsjahr, berechnet als **Gesamtfinanzierung** abzüglich des **nicht verfügbaren** Betrags. Anmerkung: In dieser Version von FOLIO werden negative verfügbare Guthaben als Null angezeigt. Wenn z. B. das Feld für zulässige Ausgaben für das Budget leer ist, gibt es keine Beschränkungen, wie viel für das Budget ausgegeben werden kann. Wenn Transaktionen den Betrag der Gesamtfinanzierung um 100 € übersteigen, wird der Betrag im Verfügbaren Guthaben als Null und nicht als negativ (100 €) angezeigt. Negative Saldenbeträge werden in einer zukünftigen Version des Systems angezeigt.

### Fonds

In diesem Abschnitt werden alle Fonds aufgeführt, die der Gruppe zugeordnet sind. Um die Gruppe einem Fonds zuzuordnen, der der Gruppe noch nicht zugeordnet ist, wie folgt vorgehen:

1.  Im Bereich Fonds-Akkordeon auf **Zur Gruppe hinzufügen** klicken.
2.  Im Dialogfeld **Fonds auswählen** den Fond oder mehrere Fonds mithilfe des Suchfelds und/oder der Filter suchen.
3.  Auf den/die Fonds klicken, die ausgewählt werden sollen.
4.  Auf **Speichern** klicken. Die Fonds werden der Gruppe hinzugefügt.

Um einen Fonds aus der Gruppe zu entfernen, auf das **X** am Ende der Fonds-Zeile in der Akkordeon-Tabellenliste Fonds klicken.

Die Fondstabelle enthält die folgenden Spalten:

* **Name**. Name des Fonds.
* **Code**. Code für den Fonds.
* **Zugewiesen**. Zugewiesener Gesamtbetrag für alle Fonds mit einem Budget für das Haushaltsjahr, die mit der Gruppe verbunden sind.
* **Nicht verfügbar**. Nicht verfügbarer Gesamtbetrag für alle Fonds mit einem Budget für das Haushaltsjahr, die mit der Gruppe verknüpft sind.
* **Verfügbar**. Verfügbarer Gesamtbetrag für alle Fonds mit einem Budget für das Haushaltsjahr, die mit der Gruppe verknüpft sind.

### Kostenarten

In diesem Abschnitt werden alle Kostenarten aufgelistet, die mit den der Gruppe zugeordneten Fonds verbunden sind. Die Tabelle Kostenarten enthält die folgenden Spalten:

* **Kostenart**. Name der Kostenart, einer fiskalischen Einheit, die dazu dient, Transaktionen für einen bestimmten Zweck oder eine bestimmte Funktion innerhalb eines Fonds zu verfolgen.
* **Gebunden**. Gesamtbetrag, der für die Kostenart belastet ist.
* **Zur Bezahlung vorgesehen**. Gesamtbetrag, der für die Kostenart zur Zahlung ansteht.
* **Ausgaben**. Gesamtbetrag, der für die Kostenart ausgegeben wurde.
* **Prozent der Gesamtausgaben**. Gesamtbetrag, der für die Kostenart ausgegeben wurde, als Prozentsatz der Gesamtausgaben für alle Kostenarten der Fonds in der Gruppe.

## Fond-Details anzeigen

Die Ansicht Fondsdetails enthält Fondsinformationen und alle aktuellen, geplanten und früheren Budgets sowie Kostenarten, die mit einem Fonds verbunden sind. Die Budgetabschnitte in der Ansicht zeigen die insgesamt zugewiesenen, nicht verfügbaren und verfügbaren Mittel nach Fonds und Kostenart an. Um eine Liste der Transaktionen für das aktuelle Budget eines Fonds anzuzeigen, auf **Aktionen > Transaktionen für aktuelles Budget anzeigen** klicken. Weitere Informationen sind unter Anzeigen von Budgettransaktionen zu finden.

* Um Fondsdetails anzuzeigen, den [gewünschten Fond suchen]({{< ref "060 Haushaltsjahr, Etat, Gruppe, Fonds suchen" >}}) und ihn auswählen. Die Ansicht mit den Fondsdetails wird angezeigt.

### Fonds-Informationen

Der Abschnitt Fondinformationen enthält Details über den Fonds. Eine Beschreibung der einzelnen Felder in diesem Abschnitt ist unter Fondsinformationen zu finden. Zusätzlich zu den Feldern, die bei der Fondserstellung verfügbar sind, wird in der Ansicht Fondsdetails die Fondswährung angezeigt. Der Wert der Fondswährung wird unter [Einstellungen > Mandant > Sprache und Lokalisierung]({{< ref "020 Sprache und Lokalisierung" >}}) auf den Währungswert gesetzt. Anmerkung: Wenn eine Bestellung geöffnet wird, erstellt das System eine Bindungstransaktion für das aktuelle Budget für den Fonds, der im Abschnitt Fondsverteilung der Bestellung ausgewählt wurde. Wenn die Währung der Bestellzeile nicht mit der Budgetwährung übereinstimmt, wird die Bindung im Budget als umgerechneter Betrag angezeigt. Die Budgetwährung wird zum Zeitpunkt der Erstellung des Datensatzes Finanzen > Haushaltsjahr auf den Wert der Mandantenwährung gesetzt. Wenn der Wert der Mandantenwährung aktualisiert wird, basieren daher alle Budgets, die vor der Aktualisierung erstellt wurden, weiterhin auf der Mandantenwährung, die bei der Erstellung des mit dem Budget verbundenen Haushaltsjahres verwendet wurde.

### Aktuelles Budget

Dieser Abschnitt enthält eine Tabelle mit Informationen über das aktuelle Budget, sofern eines vorhanden ist. Das aktuelle Jahr basiert auf dem Zeitraum des Geschäftsjahres und dem aktuellen Datum/Uhrzeit.

### Aktuelle Kostenarten

Dieser Abschnitt enthält eine Tabelle mit Informationen zu den Kostenarten, die dem aktuellen Budget zugeordnet sind, sofern vorhanden.

### Geplantes Budget

Dieser Abschnitt enthält eine Tabelle mit Informationen über zukünftige Budgets, sofern vorhanden. Vor dem Anlegen eines geplanten Budgets muss ein neues Haushaltsjahr angelegt werden. Siehe Haushaltsjahr anlegen. Um ein neues geplantes Budget anzulegen, auf **Neu** klicken. Weitere Informationen sind unter Erstellen eines neuen Budgets zu finden.

### Vorheriges Budget

Dieser Abschnitt enthält eine Tabelle mit allen Budgets aus Haushaltsjahren vor dem aktuellen Haushaltsjahr, sofern vorhanden.

## Budgetdetails anzeigen

Das Fenster mit den Budgetdetails enthält eine Zusammenfassung des Budgets, einschließlich Informationen zur Finanzierung und zu finanziellen Aktivitäten und Überschüssen, sowie Budgetinformationen.

Folgendermaßen vorgehen, um die Budgetdetails anzuzeigen:

1.  [Den Fonds mit dem Budget suchen]({{< ref "060 Haushaltsjahr, Etat, Gruppe, Fonds suchen" >}}), das angezeigt werden soll und ihn auswählen.
2.  In der Ansicht der **Fondsdetails** in den Abschnitten **Aktuelles Budget**, **Geplantes Budget** oder **Vorheriges Budget** auf den **Namen** klicken. Das Fenster mit den Budgetdetails wird angezeigt.

### Übersicht über das Budget

Der Abschnitt Budgetübersicht enthält die folgenden Felder:

* **Datensatz zuletzt aktualisiert**. Datum und Uhrzeit, zu der der Datensatz zuletzt aktualisiert wurde. Auf Datensatz zuletzt aktualisiert klicken, um die nächsten drei Felder anzuzeigen.
    * **Quelle**. Name der Person, die den Datensatz zuletzt aktualisiert hat.
    * **Datensatz erstellt**. Datum und Uhrzeit, zu der der Datensatz erstellt wurde.
    * **Quelle**. Name der Person, die den Datensatz erstellt hat.
**Informationen zur Finanzierung**

* **Anfängliche Zuweisung**. Der Betrag der ersten Zuweisung an den Haushalt.
* **Erhöhung der Zuweisung**. Die Summe aller Transaktionsbeträge für Zuweisungen, ohne die anfänglichen Zuweisungen, die dem Budget zugewiesen wurden.
* **Verringerung der Zuweisung**. Die Summe aller Zuweisungstransaktionsbeträge, ohne die anfänglichen Zuweisungen, die vom Budget abgezogen wurden.
* **Insgesamt zugewiesen**. Die Summe aller zugewiesenen Beträge für den Haushalt (anfängliche Zuweisung plus Erhöhung der Zuweisung minus Verringerung der Zuweisung).
* **Netto-Transfers**. Der gesamte Netto-Transferbetrag für das Budget.
* **Gesamtfinanzierung**. Der gesamte zugewiesene Betrag plus der Betrag der Netto-Transfers.
* **Kassenbestand**. Der Betrag der Gesamtfinanzierung abzüglich des ausgegebenen Betrags.
**Finanzielle Aktivität & Überschüsse**

* **Gebunden**. Die Summe aller Beträge der Bindungstransaktionen gegen das Budget.
* **Zu Bezahlung vorgesehen**. Die Summe der vorläufigen Zahlungstransaktionsbeträge zu Lasten des Budgets.
* **Ausgaben**. Die Summe der Zahlungstransaktionsbeträge abzüglich der Kredittransaktionsbeträge zu Lasten des Haushalts.
* **Nicht verfügbar**. Der Gesamtbetrag, der für das Budget nicht verfügbar ist, berechnet als Summe der belasteten, zur Zahlung anstehenden und ausgegebenen Beträge.
* **Überzogene Bindung**. Der gesamte belastete Betrag abzüglich des gesamten Finanzierungsbetrags für alle Fondsbudgets für das Haushaltsjahr.
* **Überzogene Ausgaben**. Der Gesamtbetrag der Ausgaben abzüglich des Gesamtbetrags der Mittel aller Fonds-Budgets für das Haushaltsjahr.
* **Verfügbares Guthaben**. Der für das Budget verfügbare Gesamtbetrag, berechnet als **Gesamtfinanzierung** abzüglich des **nicht verfügbaren** Betrags. Anmerkung: In dieser Version von FOLIO werden negative verfügbare Salden als 0 € angezeigt. Wenn z. B. das Feld für zulässige Ausgaben für das Budget leer ist, gibt es keine Einschränkungen, wie viel für das Budget ausgegeben werden kann. Wenn Transaktionen verarbeitet wurden, die den Gesamtfinanzierungsbetrag um 100 € übersteigen, wird der Betrag im Feld Verfügbares Guthaben als 0 € und nicht als negativ (100 €) angezeigt. Negative Saldenbeträge werden in einer zukünftigen Version des Systems angezeigt.

### Budget-Informationen

Der Abschnitt Budgetinformationen enthält die folgenden Felder:

* **Name**. Name des Budgets.
* **Status**. Status des Etats: Aktiv, Gesperrt oder Inaktiv.
* **Beginn des Haushaltsjahres**. Startdatum des Haushaltsjahres.
* **Ende des Haushaltsjahres**. Enddatum des Haushaltsjahres.
* **Zulässige Ausgaben**. Zulässige Ausgaben, ausgedrückt als Prozentsatz.
* **Zulässige Bindungen**. Erlaubte Bindung, ausgedrückt als Prozentsatz.
* **Vorgänge**. Auf Vorgänge anzeigen klicken, um die Budgettransaktionen anzuzeigen. Weitere Informationen sind unter Anzeigen von Budgettransaktionen zu finden.
