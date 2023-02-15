---
title: "Jahresübergang durchführen"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-finanzen, by-folio, cat-workflows, by-folio, meta-fehler_inhalt]
weight: 150
Description: "
    Quellen: [Folio](xxx) & [GBV](xxx)
    "
---

{{% pageinfo %}}
Abweichungen (GBV rot; "Jahresübergang beendet", "Startzeit." bis "Quelle.")
{{% /pageinfo %}}

Der Jahresübergang wird aus der Ansicht des Etats initiiert. Dieser Prozess schließt die Budgets des aktuellen Haushaltsjahres ab, wendet die Restbeträge aus den Budgets des aktuellen Haushaltsjahres auf der Grundlage der Fondsart auf die neuen Budgets des kommenden Haushaltsjahres an und übernimmt die Bindungen auf der Grundlage der Auftragsart (einmalig, laufend und laufendes Abonnement) auf die Budgets des neuen Haushaltsjahres. Diese Aktion wird nur auf die mit dem Etat verbundenen Fonds angewandt, so dass der Jahresübergang für jeden Etat separat ausgeführt werden muss. Es sollte ein Testlauf des Jahresübergangs durchgeführt werden, um festzustellen, ob unbezahlte Rechnungen vorhanden sind und um das Protokoll des Jahresübergangs einzusehen, bevor der eigentliche Jahresübergang durchführt wird.

Folgendermaßen vorgehen, um einen Testlauf des Jahrsübergang durchzuführen:

1.  In der Ansicht **Suchen & Filtern** auf **Etat** klicken.
2.  Bei Bedarf die [Such- und Filterwerkzeuge verwenden]({{< ref "060 Haushaltsjahr, Etat, Gruppe, Fonds suchen" >}}), um den Etat für den Jahresübergang zu finden.
3.  In der Ansicht mit den **Etatliste** den Namen des Etats klicken, das für den Jahresübergang verwendet werden soll.
4.  Die Ansicht mit den **Details des Etats** wird geöffnet. Auf das **Aktion > Jahresübergang** klicken.
5.  Im Fenster **Jahresübergang** das Formular ausfüllen, um die Einstellungen für den Jahresübergang festzulegen. Weitere Informationen zu den Feldern im Fenster Jahresübergang sind in den Beschreibungen unten zu finden.
6.  Einen **Screenshot des ausgefüllten Formulars speichern**. Das System speichert derzeit keine Kopie der für den Jahresübergang verwendeten Einstellungen. Es wird daher empfohlen, dass eine Kopie der für den Jahresübergang verwendeten Einstellungen als Referenz gespeichert wird.
7.  Auf die Schaltfläche **Jahresübergang testen** klicken, um einen Test des Jahresübergangs für dieses Etat zu initiieren.
8.  Wenn unbezahlte Rechnungen vorhanden sind, wird ein Dialogfenster angezeigt: "FOLIO hat Rechnungen gefunden, die noch nicht bezahlt oder storniert sind. Wenn dennoch mit dem Jahresübergang fortgefahren werden soll, auf Weiter klicken." Eine tabellarische Liste der Rechnungen zeigt die folgenden Informationen an:
    * **Rechnungsnummer des Lieferanten**.
    * **Lieferant**. Name des Lieferanten.
    * **Rechnungsdatum**.
    * **Status**.
9.  Auf **Abbrechen** klicken, um den Dialog zu schließen, ohne mit dem Testlauf des Jahresübergangs fortzufahren, Auf **Liste exportieren** klicken, um eine .csv-Datei mit der  Liste unbezahlter Rechnungen herunterzuladen. Oder auf **Fortfahren** klicken, um mit dem Testlauf des Jahresübergangs fortzufahren.
10.  Nachdem fortgefahren wurde, wird ein Dialogfeld angezeigt: "Bitte bestätigen, dass die erforderlichen Angaben gemacht wurden und mit dem Testlauf des Jahresübergangs fortgefahren werden soll. Dieser Vorgang kann einige Minuten in Anspruch nehmen. Ein Link zu den Ergebnissen wird an \[E-Mail Adresse der Person\] gesendet, sobald der Vorgang abgeschlossen ist."
11.  Auf **Bestätigen** klicken. Eine grüne Toast-Meldung zeigt an, dass der Jahresübergangstest erfolgreich gestartet wurde und der Fokus kehrt zur Dreispalten-Ansichten für den Etat zurück. Eine Bestätigungs-E-Mail wird an die E-Mail Adresse der Person gesendet.
12.  Um die Ergebnisse des Jahresübergangs im Protokoll zu sehen, auf **Aktionen > Jahresübergangsprotokolle** klicken.

Wie folgt vorgehen, um einen Jahresübergang für das Haushaltsjahr durchzuführen:

1.  In der Ansicht **Suchen & Filtern** auf **Etat** klicken.
2.  Bei Bedarf die [Such- und Filterwerkzeuge verwenden]({{< ref "060 Haushaltsjahr, Etat, Gruppe, Fonds suchen" >}}), um den Etat für den Jahresübergang zu finden.
3.  In der Ansicht mit den **Etatliste** den Namen des Etats klicken, das für den Jahresübergang verwendet werden soll.
4.  Die Ansicht mit den **Details des Etats** wird geöffnet. Auf das **Aktion > Jahresübergang** klicken.
5.  Im Fenster **Jahresübergang** das Formular ausfüllen, um die Einstellungen für den Jahresübergang festzulegen. Weitere Informationen zu den Feldern im Fenster Jahresübergang sind in den Beschreibungen unten zu finden.
6.  Einen **Screenshot des ausgefüllten Formulars speichern**. Das System speichert derzeit keine Kopie der für den Jahresübergang verwendeten Einstellungen. Es wird daher empfohlen, dass eine Kopie der für den Jahresübergang verwendeten Einstellungen als Referenz gespeichert wird.
7.  Auf die Schaltfläche **Jahresübergang** klicken, um den Jahresübergang für dieses Etat durchzuführen.
8.  Auf **Bestätigen** klicken. Warten, bis der Vorgang abgeschlossen ist, was durch den blauen Fortschrittsbalken angezeigt wird. Wenn der Vorgang abgeschlossen ist, erscheint die Meldung "Jahresübergang beendet".
9.  Auf **Schließen & Details zum Etat anzeigen** klicken, um zur Ansicht für den Etat zurückzukehren.

## Jahresübergangsinformationen

Wird die Aktion **Jahresübergang** gewählt, zeigt das System das aktuelle Jahr für den Etat oben links im Formular für den Jahresübergang an. Das aktuelle Jahr basiert auf dem Zeitraum des Haushaltsjahres und dem aktuellen Datum/Uhrzeit.

Wird der Jahresübergang vor oder nach dem Ende des Haushaltsjahres durchführt, müssen in der Registerkarte Haushaltsjahr die Daten sowohl des aktuellen Haushaltsjahres, als auch des kommenden Haushaltsjahres so angepasst werden, dass das aktuelle Datum in das Haushaltsjahr passt, aus und zu dem der Jahresübergang durchgeführt werden soll. Danach daran denken, die Daten des Haushaltsjahres nach Abschluss des Jahresübergangs wieder an die tatsächlichen Daten des Haushaltsjahres anzupassen. Weitere Informationen sind unter [Haushaltsjahr, Etat, Gruppe, Fonds bearbeiten]({{< ref "130 Haushaltsjahr, Etat, Gruppe, Fonds bearbeiten" >}}) zu finden.

* **Beginn des Zeitraums**. Das Datum des Beginns des Haushaltsjahres für das ausgewählte Haushaltsjahr. Weitere Informationen zum Datum des Zeitraums sind unter Erstellen eines Haushaltsjahres zu finden.
* **Ende des Zeitraums** Das Enddatum des Haushaltsjahres für das ausgewählte Haushaltsjahr. Anmerkung: Das Enddatum des Zeitraums muss größer als das aktuelle Datum sein, um einen Jahresübergang vom aktuellen Jahr auf ein neues Jahr zu ermöglichen.
* **Haushaltsjahr**. Das nächste Haushaltsjahr auswählen. Wenn das nächste Haushaltsjahr noch nicht eingerichtet wurde, auf **Neues Haushaltsjahr** klicken, um es zu erstellen. Weitere Informationen sind unter Erstellen eines Haushaltsjahres zu finden.
* **Einhalten von Budgetbeschränkungen für Bindungen**. Dieses Feld ist standardmäßig markiert. Dieses Kästchen markiert lassen, wenn gewünscht ist, dass das System alle Bindungen ablehnt, die den verfügbaren Betrag überschreiten würden. Wenn die Institution z.B. normalerweise keine Jahresübergänge vornimmt und die Beträge der anfänglichen Zuweisungen nach dem Jahresübergang manuell hinzufügt, könnte dieses Kästchen angekreuzt werden, um zuzulassen, dass Belastungen aus dem laufenden Jahr auf die Budgets des kommenden Jahres angewendet werden, die auf anfängliche Zuweisungen warten. Dieses Kontrollkästchen deaktivieren, wenn zugelasssen werden soll, dass Beträge für Bindungen aus dem Budget des laufenden Jahres ohne Einschränkungen auf das Budget des kommenden Jahres übertragen werden.
* **Einhalten von Budgetbeschränkungen für Ausgaben**. Dieses Feld ist standardmäßig aktiviert. Dieses Kontrollkästchen dekativieren, damit Ausgaben auch dann auf das neue Budget übertragen werden können, wenn nicht genügend Mittel zugewiesen sind.
* **Schließen aller aktuellen Budgets**. Diese Checkbox ist standardmäßig aktiviert und zeigt an, dass alle Budgets des aktuellen Haushaltsjahres im Rahmen dieses Jahresübergangs geschlossen werden sollen.

### Budgets übertragen

Die Informationen in diesem Abschnitt definieren das Verfahren beim Jahresübergang für Budgets nach Fondsart. Weitere Informationen zum Erstellen von Fondstypen sind unter Einstellungen > Finanzen > Fondstypen zu finden. Für jeden aufgeführten Fondstyp die entsprechenden Einstellungen für jedes der unten definierten Felder auswählen. Diese Einstellungen werden auf alle kommenden Haushaltsjahre der jeweiligen Fondsart angewendet.

* **Zuweisung**. Dieses Feld markieren, wenn gewünscht ist, dass der Betrag der anfänglichen Zuweisung für das kommende Haushaltsjahr dem Gesamtbetrag der Zuweisung für das aktuelle Haushaltsjahr entspricht.
* **Zuweisung anpassen in Prozent**. Dieses Feld markieren, wenn gewünscht ist, dass die anfängliche Zuweisung für das kommende Haushaltsjahr der um diesen Prozentsatz angepassten Gesamtzuweisung für das laufende Haushaltsjahr entspricht. Wenn die Gesamtzuweisung des aktuellen Budgets beispielsweise €1000 beträgt und zwei Prozent eingeben werden, wird der Wert der anfänglichen Zuweisung für das kommende Budget auf €1020 gesetzt.
* **Restmittel übertragen**. Dieses Feld markieren, wenn gewünscht ist, dass der verfügbare Betrag des Budgets des aktuellen Haushaltsjahres auf das Budget des kommenden Haushaltsjahres übertragen wird.
* **Restmittel hinzufügen als**. Gibt an, ob verfügbare Beträge, die übertragen werden, als Transfer oder als Zuweisung kategorisiert werden sollen.
* **Beschränkung festlegen**. Markieren Sie dieses Feld, um die Felder _Zulässige Bindungen in Prozent_ und _Zulässige Ausgaben in Prozent_ zu aktivieren.
* **Zulässige Bindungen in Prozent**. Der prozentuale Betrag, der auf den zugewiesenen Betrag des kommenden Budgets angewandt wird, um die zulässigen Bindungen für Fonds dieses Fondstyps zu berechnen. Um alle Bindungen ohne Begrenzung zuzulassen, dieses Feld leerlassen. Wenn der zugewiesene Gesamtbetrag des Budgets beispielsweise €1000 beträgt und eine zulässige Bindung in Prozent von 110 Prozent festlegt wird, erlaubt das System die Zahlung von Rechnungen bis zu €1100. In ähnlicher Weise begrenzt ein Wert von 90 Prozent die Ausgaben auf €900. Anmerkung: Es kann in dieses Feld nur dann einen Wert eingeben werden, wenn die Checkbox Beschränkungen festlegen markiert ist.
* **Zulässige Ausgaben in Prozent**. Der prozentuale Betrag, der auf den zugewiesenen Betrag des kommenden Budgets angewendet wird, um die zulässigen Ausgaben für Fonds dieses Fondstyps zu berechnen. Um alle Ausgaben ohne Begrenzung zuzulassen, dieses Feld leerlassen. Wenn der zugewiesene Gesamtbetrag des Budgets beispielsweise €1000 beträgt und Sie einen Wert für Zulässige Ausgaben in Prozent von 110 Prozent festlegen, erlaubt das System die Zahlung von Rechnungen bis zu €1100. Bei einem Wert von 90 Prozent werden die Ausgaben auf €900 begrenzt. Anmerkung: Es kann in dieses Feld nur dann einen Wert eingeben werden, wenn die Checkbox Beschränkungen festlegen markiert ist.

### Bindungen übertragen

Die Informationen in diesem Abschnitt definieren das Verhalten von Bindungen beim Jahresübergang nach Bestellungstyp: Einmalige Bindungen, Laufende Bindungen oder Bindungen durch laufende Abonnements. Eine Bestellung wird als laufendes Abonnement betrachtet, wenn der Bestellungstyp **Laufend** ist und die Checkbox **Abonnement** aktiviert ist. Weitere Informationen über die Checkbox Abonnement sind unter Bestellungen > Erstellen einer laufenden Bestellung > Informationen zur laufenden Bestellung zu finden. Für jede aufgelisteten Bestellungstyp die entsprechenden Einstellungen für jedes der unten definierten Felder wählen:

* **Jahresübergang**. Dieses Kästchen markieren, wenn gewünscht ist, dass die Bindungen für offene Aufträge dieser Auftragsart auf das Budget des kommenden Haushaltsjahres, das mit jedem Auftrag verbunden ist, übertragen werden. Wird dieses Feld markiert, werden die Felder **Basierend auf** und **Erhöhung um in %** aktiviert.
* **Basierend auf**. In der Dropdown-Liste **Ausgaben** wählen, um den Gesamtbetrag zu belasten, der im aktuellen Haushaltsjahr ausgegeben wurde. **Ursprüngliche Bindung** wählen, um den geschätzten Preis des Bestellpostens zu belasten. **Verbleibend** wählen, um den Betrag zu belasten, der noch nicht bezahlt wurde.
* **Erhöhen um in %**. Einen Wert eingeben, wenn gewünscht ist, dass der Betrag der Bindung um einen bestimmten Prozentsatz erhöht wird.

## Jahresübergangsprotokoll anzeigen

Für jeden Jahresübergang sind Protokolle und Ergebnisse verfügbar. Folgendermaßen vorgehen, um die Ergebnisse des Jahresübergangsprotokolls anzuzeigen:

1.  In der Ansicht **Suchen & Filtern** auf **Etat** klicken.
2.  Bei Bedarf die [Such- und Filterwerkzeuge verwenden]({{< ref "060 Haushaltsjahr, Etat, Gruppe, Fonds suchen" >}}), um den Etat für den Jahresübergang zu finden.
3.  In der Ansicht mit den **Etatliste** den Namen des Etats klicken, das für den Jahresübergang verwendet werden soll.
4.  Die Ansicht mit den **Details des Etats** wird geöffnet. Auf das **Aktion > Jahresübergangsprotokolle** klicken.
5.  Das Fenster **Jahresübergangsprotokolle** öffnet sich. Es enthält eine Ansicht zum Suchen und Filtern auf der linken Seite und eine tabellarische Liste der Jahresübergangsprotokolle auf der rechten Seite, in der die folgenden Informationen angezeigt werden:
    * **Startzeit**. Datum und Uhrzeit, zu der der Jahresübergang oder der Testlauf des Jahresübergangs gestartet wurde.
    * **Endzeit**. Datum und Uhrzeit, zu der der Jahresübergang oder der Testlauf des Jahresübergangs abgeschlossen wurde.
    * **Status**. Status des Jahresübergangs oder des Testlauf des Jahresübergangs: In Bearbeitung, Erfolgreich, Gescheitert.
    * **Fehler**. Wenn Fehler vorhanden sind, wird ein Dateiname im Format 'mm/dd/yyyyy-error' angezeigt. Auf den Dateinamen klicken, um eine .csv-Datei mit Fehlerinformationen herunterzuladen.
    * **Ergebnisse**. Wenn der Jahresübergang erfolgreich abgeschlossen wurde, wird ein Dateiname im Format 'mm/dd/yyyyy-result' angezeigt. Auf den Dateinamen klicken, um eine .csv-Datei mit den Ergebnisinformationen herunterzuladen. Die Liste der Felder in der Datei sind unter Ergebnisdatei des Jahresübergangsprotokolls unten zu finden.
    * **Quelle**. Der Name des Prozesses, der das Protokoll des Jahresübergangs erstellt hat: Jahresübergang oder Testlauf des Jahresübergangs.

### Ergebnisdatei des Jahresübergangsprotokolls

Die folgenden Felder sind in der herunterladbaren Ergebnisdatei des Jahresübergangs-Protokolls enthalten:

Felder bei Export nur englischsprachig; hier mit Übersetzt.

* Name (Budget) (Name (Budget))
* Status (Budget) (Status (Budget))
* Allowable encumbrance (Zulässige Bindung)
* Allowable expenditure (Zulässige Ausgaben)
* Initial allocation (Anfängliche Zuweisung)
* Increase (Erhöhung)
* Decrease (Senkung)
* Total allocation (Zuweisung insgesamt)
* Transfers (Transfers)
* Total Funding (Gesamtfinanzierung)
* Encumbered (Budget) (Verrechnet (Budget))
* Awaiting payment (Budget) (In Erwartung einer Zahlung (Budget))
* Expended (Budget) (Verausgabt (Budget))
* Unavailable (Nicht verfügbar)
* Over encumbered (Über belastet)
* Over expended (Überzogene Ausgaben)
* Cash balance (Kassenbestand)
* Available (Verfügbar)
* Name (Exp Class) (Name (Ausgabenklasse))
* Code (Exp Class) (Code (Ausgabenklasse))
* Status (Exp Class) (Status (Ausgabenklasse))
* Encumbered (Exp Class) (Belastet (Exp Class))
* Awaiting payment (Exp Class) (In Erwartung einer Zahlung (Exp Class))
* Expended (Exp Class) (Ausgegeben (Ausgabenklasse))
* Percentage of total expended (Prozentsatz der Gesamtausgaben)

### Jahresübergangsprotokolle - Liste filtern

Um die Liste der Jahresübergangsprotokolle mit Hilfe der Ansicht Suchen & Filtern zu filtern, einen der folgenden Filter anwenden:

* **Startzeit**. Datum und Uhrzeit, zu der der Jahresübergang oder der Testlauf des Jahresübergangs gestartet wurde. Ein Startdatum/eine Startzeit von und bis eingeben und auf Anwenden klicken, um die Protokollergebnisse nach einem Startdatum/Zeitbereich zu filtern.
* **Endzeit**. Datum und Uhrzeit, zu der der Jahresübergang oder der Testlauf des Jahresübergangs beendet wurde. Das Datum und die Uhrzeit von und bis eingeben und auf Anwenden klicken, um die Protokollergebnisse nach einem Enddatum/Zeitbereich zu filtern.
* **Status**. Status des Jahresübergangs oder des Testlauf des Jahresübergangs: In Bearbeitung, Erfolgreich, Gescheitert.
* **Quelle**. Der Name des Prozesses, der das Protokoll des Jahresübergangs erstellt hat: Jahresübergang oder Testlauf des Jahresübergangs.
