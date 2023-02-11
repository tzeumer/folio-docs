---
title: "Folio: Bestellposten zu einer Bestellung hinzufügen"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [by-folio, for-anwender, cat-workflows, app-bestellungen, nmeta-uebersetzungsproblem]
weight: 10
Description: "
    Quellen: [Folio](xxx) & [GBV](xxx)
    "
---

Diesen Schritten folgen, um einen Bestellposten zu einer Bestellung hinzuzufügen. Ein Bestellposten kann auch über die App Katalog hinzugefügt werden, indem nach einer Instanz gesucht und auf Katalog > Aktionen > Neue Bestellung geklickt wird.

1.  [Nach der Bestellung suchen](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio%3A+Bestellungen+suchen+und+exportieren), zu der der Bestellposten hinzugefügt werden soll und sie auswählen.
2.  In der Ansicht **Bestellung** im Bereich **Bestellposten** auf **Aktion > Bestellposten hinzufügen** klicken.
3.  Im Fenster **Bestellposten hinzufügen** die Felder in den Abschnitten Exemplardetails, Details zum Bestellposten, Lieferant, Kostendetails und Fondsverteilung ausfüllen. Weitere Informationen zu den Feldern und Aktionen, die in diesen Abschnitten verfügbar sind, sind in den Abschnittsbeschreibungen unten zu finden.
4.  **Weitere erstellen**\-Checkbox: Wenn der Grenzwert für [Einstellungen > Bestellungen > Bestellposten](https://info.gbv.de/display/FOLIOGBVEXTERN/Einstellungen+%28Bestellungen%29%3A+Bestellposten-Limit) größer als eins ist, auf diese Checkbox am unteren Rand des Fensters klicken, damit das Fenster Bestellposten hinzufügen auch nach dem Speichern des aktuellen Bestellpostens geöffnet bleibt.
5.  Ggf. auf **Speichern**, **Speichern & Schließen** oder **Speichern & Öffnen der Bestellung** klicken. Wenn anhand der Werte für Titel und Produkt-ID mögliche Duplikate gefunden werden, wird ein Modal mit einer Liste möglicher doppelter Bestellungen angezeigt. Fortsetzen oder Stornieren wählen. Diese Dublettenprüfung kann in den Einstellungen deaktiviert werden. Weitere Informationen über die Prüfung auf Duplikate und die Möglichkeit, Bestellungen gleichzeitig zu speichern und zu öffnen, sind unter [Einstellungen > Bestellungen > Bestellung öffnen](https://info.gbv.de/pages/viewpage.action?pageId=851345579) zu finden.
6.  Sobald der Bestellposten erstellt ist, können Anmerkungen hinzugefügt werden. Weitere Informationen sind unter [Hinzufügen einer Anmerkung zu einem Bestellposten](https://info.gbv.de/pages/viewpage.action?pageId=851017789) zu finden. Wenn es sich bei dem Bestellposten um ein Paket handelt, können Pakettitel hinzugefügt werden. Siehe Hinzufügen von Pakettiteln zu einem Bestellposten.

## Exemplardetails

-   **Paket**. Wird ein Paket hinzugefügt, die Checkbox Paket markieren. Wenn dieses Feld markiert ist, wird der Titel zum Paketnamen. Das Feld Inventarisierung wird automatisch auf "Unabhängige Bestell- und Inventariesierungmenge" gesetzt, sobald die Checkbox Paket markiert wird. Weitere Informationen über die Inventarisierung sind im Abschnitt Details zum Bestellposten weiter unten zu finden.
-   **Titel/Paketname**. Titel des Exemplars. Wenn das Exemplar bereits in der App Katalog vorhanden ist, kann das Exemplar über die Titelsuche mit dem Katalog-Datensatz verknüpft werden. Dadurch werden alle zutreffenden Felder automatisch ausgefüllt. Um eine Verknüpfung mit einem Katalog herzustellen, auf **Titelsuche** klicken. Im Dialog **Instanz auswählen** und den Titel mit Hilfe des Suchfeldes und/oder der Filter suchen. Auf den Titel klicken, um ihn auszuwählen. Der Titel wird im Feld Titel angezeigt und die entsprechenden Felder für das Exemplar werden ausgefüllt.
-   **Inventarisierungsnotiz**. Eine beliebige Notiz für die Inventarisierung des Exemplars eingeben. Die Anmerkungen werden in der App Inventarisierung für diesen Bestellposten angezeigt.
-   **Inventarisierungsnotiz bestätigen**. Dieses Feld markieren, damit die Notiz zur Inventarisierung in der App Inventarisierung angezeigt wird, wenn die Person auf den Titel klickt, um ihn zu inventarisieren. Siehe Inventarisierung > Empfangen.
-   **Abonnement von**. Wenn es sich bei dem Exemplar um ein Abonnement handelt, auswählen wann das Abonnement beginnt. Das Datum wird in der App Rechnungen angezeigt, wenn dieser Bestellposten zu einer Rechnung hinzugefügt wird.
-   **Abonnement bis**. Wenn es sich bei dem Exemplar um ein Abonnement handelt, auswählen wann das Abonnement endet. Das Datum wird in der Rechnungen App angezeigt, wenn dieser Bestellposten zu einer Rechnung hinzugefügt wird.
-   **Abonnementintervall**. Wenn es sich bei dem Exemplar um ein Abonnement handelt, eingeben oder auswählen, wie viele Tage das Abonnement läuft.
-   **Erscheinungsdatum**. Das Datum der Veröffentlichung des Exemplars.
-   **Verlag**. Der Verlag des Exemplars.
-   **Ausgabe**. Die Ausgabe des Exemplars.
-   **Verknüpftes Paket**. Um ein Paket mit einem Bestellposten zu verknüpfen, auf **Suche nach Paketbestellposten** klicken. Im Dialog Bestellposten auswählen das Paket mit Hilfe des Suchfeldes und/oder der Filter finden. Auf das Paket klicken, um es auszuwählen. Das Paket erscheint im Feld Verknüpftes Paket.
-   **Mitwirkende**. Die Mitwirkenden des Titels.
-   **Produktidentifikatoren**. Der Identifikator des Exemplars, z.B. eine ISBN.
-   **Interne Notiz**. Alle internen Notizen zu dem Exemplar eingeben.

### Mitwirkenden hinzufügen

1.  Auf **Mitwirkende(n) hinzufügen** klicken,
2.  **Mitwirkende(n)** in das Feld eingeben.
3.  Den **Typen Mitwirkender** aus der Dropdown-Liste wählen: Firmenname, Besprechungsname oder Persönlicher Name. Der Mitwirkende wird gespeichert, sobald der Bestellposten gespeichert ist.

### Mitwirkenden löschen

1.  Mitwirkende(n) suchen, der gelöscht werden soll.
2.  Auf das **Mülleimersymbol** klicken. Der Mitwirkende wird entfernt und gelöscht, sobald der Bestellposten gespeichert ist.

### Produkt-ID und eines Produkt-ID-Typ hinzufügen

1.  Auf **Produkt-ID und Produkt-ID-Typ hinzufügen** hinzufügen klicken.
2.  die Produkt-ID in das Feld eingeben.
3.  Optional: Einen Qualifier in das Feld eingeben.
4.  Den Produkt-ID-Typ aus der Dropdown-Liste wählen. Der Produktidentifikator wird gespeichert, sobald der Bestellposten gespeichert ist.

### Produkt-ID und eines Produkt-ID-Typ löschen

1.  Die Produkt-ID suchen, die gelöscht werden soll.
2.  Auf das **Mülleimersymbol** klicken. Die Produkt-ID wird entfernt und gelöscht, sobald der Bestellposten gespeichert ist.

## Details zum Bestellposten

-   **Erwerbungsart**. Die Methode, die für den Erwerb des Exemplars verwendet werden soll wählen: Genehmigungsplan, Bedarfsgesteuerte Beschaffung (DDA), Depot, Evidenzbasierte Beschaffung (EBA), Tausch, Kostenlos, Geschenk, Interner Transfer, Mitgliedschaft, Sonstige, Kauf, Kauf beim Lieferanten, Technisch.
-   **Automatischer Export**. Diese Checkbox markieren, um die Bestellung in den automatischen EDI-Bestellungsexport einzubeziehen, der beim Öffnen einer Bestellung ausgelöst wird, wenn EDI für den zugehörigen Lieferanten eingerichtet ist. Die im Abschnitt Lieferant der Bestellung ausgewählte Kontonummer bestimmt, welche EDI-Konfiguration für den Export angewendet wird. Die Checkbox leerlassen, um den automatischen Export des Bestellpostens beim Öffnen zu verhindern. Weitere Informationen über die Anbindung von Lieferantenorganisationen sind unter [Organisationen (Lieferant) > EDI-Verbindung hinzufügen](https://info.gbv.de/pages/viewpage.action?pageId=842793035) zu finden.
-   **Bestellungsformat**. Das Format des Exemplars wählen, das bestellt wird: Elektronische Ressource, Physische Ressource, P/E-Mix oder Sonstige. Das Bestellformat bestimmt, welche Felder im Abschnitt **Kostendetails** erforderlich sind und ob die Abschnitte **Details zu physischen Ressourcen** oder **Details zu elektronischen Ressourcen** angezeigt werden.
-   **Inventarisierungsdatum**. Das Inventarisierungsdatum des Exemplars.
-   **In­ven­ta­ri­sie­rungs­sta­tus**. Den Inventarisierungsstatus des Exemplars wählen: Ausstehend oder Inventarisierung nicht erforderlich. Bei Bestellungen mit dem Typ Laufend wird der Empfangsstatus automatisch auf Laufend gesetzt, wenn die Bestellung gespeichert wird. Wenn keine Auswahl getroffen wird, wird die Bestellung mit dem Eingangsstatus Ausstehend angelegt. Wenn die Bestellung geöffnet wird, wird der Inventarisierungstatus automatisch auf **Inventarisierung erwartet** gesetzt. Sobald eine Bestellung geöffnet ist, kann der Status der Inventarisierung auf **Storniert**, **Vollständig inventarisiert**, **Teilweise inventarisiert** oder **Inventarisierung nicht erforderlich** geändert werden. Das System schließt Bestellungen, die sowohl den Zahlungs- als auch den Quittungsstatus "Zahlung nicht erforderlich" oder "Inventarisierung nicht erforderlich" haben, automatisch ab, indem es durch Aktionen in der App Inventarisierung und in der App Rechnungen "Vollständig bezahlt" und "Vollständig erhalten" erreicht. Es ist ratsam, die Bedürfnisse der Bibliothek zu berücksichtigen, wenn festgelegt wird, wie dieses Feld gesetzt werden soll. Zum Beispiel kann für einmalige Bestellungen von E-Ressourcen die Option "Inventarisierung nicht erforderlich" gewünscht sein, damit die Bestellung automatisch geschlossen wird, sobald die Zahlung der Rechnung abgeschlossen ist. Andernfalls, wenn die Bibliothek keine E-Ressourcen bezieht, kann eine einmalige E-Ressourcen-Bestellung auch nach Abschluss der Zahlung offen bleiben, was sich auf die erwarteten Ergebnisse beim Jahresübergang auswirken könnte.
-   **Zahlungsstatus**. Den Zahlungsstatus des Exemplars wählen: Zahlung nicht erforderlich oder Ausstehend. Bei Bestellungen mit dem Typ **Laufend** wird der Zahlungsstatus automatisch auf **Laufend** gesetzt, wenn die Bestellung gespeichert wird. Wenn keine Auswahl getroffen wird, wird die Bestellung mit dem Zahlungsstatus **Ausstehend** angelegt. Wenn die Bestellung geöffnet wird, wird der Zahlungsstatus automatisch auf **Zur Bezahlung vorgesehen** gesetzt. Sobald eine Bestellung geöffnet ist, kannn der Zahlungsstatus in **Storniert**, **Teilweise bezahlt**, **Vollständig bezahlt** oder **Zahlung nicht erforderlich** geändert werden. Der Zahlungsstatus wird automatisch auf **Teilweise bezahlt** gesetzt, wenn ein verbundener Rechnungsposten, bei dem die Checkbox **Bindung freigeben** nicht markiert/leer ist, auf den Status **Freigegeben** gesetzt wird. Das System schließt Bestellungen, die sowohl den Status "Zahlung nicht erforderlich" als auch den Status "Inventarisierung nicht erforderlich" haben, automatisch ab, indem es durch Aktionen in der App Inventarisierung und der App Rechnungen die Status "Vollständig bezahlt" und "Vollständig erhalten" erreicht.
-   **Spender(in)**. Spender(in) des Exemplars.
-   **Fachreferat**. Die Person, die das Exemplar ausgewählt hat.
-   **Bestandsanfrage für**. Die Person, die das Exemplar angefordert hat.
-   **Stornierungsbeschränkung**. Wenn für das Exemplar eine Stornierungsbeschränkung besteht, die Checkbox Stornierungsbeschränkung markieren.
-   **Eilt**. Wenn das Exemplar in Eile bearbeitet werden muss, markieren Sie die Checkbox Eilig.
-   **Sammlung**. Wenn das Exemplar Teil einer Sammlung ist, die Checkbox Sammlung markieren.
-   **Inventarisierungsworkflow**. Einen Wert aus der Dropdown-Liste wählen, um das Verhalten in der App Inventarisierung zu steuern. **Synchronisierte Bestell- und Eingangsmenge** wählen, um die Bestellmenge und die Anzahl der zu empfangenden Exemplare synchron zu halten. Wenn die Bestellung geöffnet wird, generiert das System in der App Inventarisierung Exemplarzahlen auf der Grundlage des Mengenwerts in den Bestellposten. Wenn die Menge in der Bestellung aktualisiert wird, wird die Anzahl der zu empfangenden Exemplare aktualisiert, und bei Aktualisierungen in der App Inventarisierung wird die Bestellung aktualisiert. **Unabhängige Bestell- und Eingangsmenge**, wenn eine unvorhersehbare Menge von Inventarisierungsexemplaren erstellt werden muss, z.B. für eine laufende Bestellung.
    Anmerkung: In früheren Systemversionen war dieses Feld eine Checkbox mit der Bezeichnung "Stücke für die Inventarisierung manuell hinzufügen".
-   **Stornierungsbeschreibung**. Eine Anmerkung zur Stornierung.
-   **Beschreibung des Bestellpostens**. Eine Beschreibung der Bestellpostens.
-   Tags. In das Feld alle Tags eingeben oder auswählen, die Bestellposten zugewiesen werden sollen.

## Lieferant

-   **Lieferantenreferenznummer**. Eine Lieferantenreferenznummer, mit der ein Lieferant die Bestellung oder das Exemplar identifiziert, das bestellt wurde. Bei migrierten offenen Bestellungen kann es z.B. hilfreich sein, hier die ursprüngliche Bestellnummer zu speichern, um sie mit Lieferantenrechnungen abzugleichen.
-   **Lieferantenreferenztyp**. Die Art der Referenznummer, die im vorherigen Feld eingegeben wurde wählen: Die eindeutige Lieferantenbestellnummer, die Interne Lieferantennummer, die Lieferantenabonnementnummer, die Lieferantenfortsetzungsnummer oder die eindeutige Lieferantentitelnummer.
-   **Kundennummer**. Die Kundennummer beim Lieferanten. Wenn im Datensatz der Organisation ein oder mehrere Lieferantenkonten für den im Abschnitt Bestellung der Bestellung ausgewählten Lieferanten vorhanden sind, wird das erste Konto in diesem Feld als Standardwert angezeigt. Wenn eine andere Kundennummer für diesen Lieferanten verwendet werden soll, die Kundennummer aus der Dropdown-Liste auswählen, falls zutreffend. Anmerkung: In der Liste wird der Kontoname mit der Kundennummer in Klammern angezeigt.
-   **Anweisungen an den Lieferanten**. Die Anweisungen eingeben, die bei der Eröffnung der Bestellung an den Lieferanten gesendet werden sollen.

## Kostendetails

Dieser Abschnitt enthält Informationen zu Kosten, Menge, Währung und Rabatt der Bestellposten. Abhängig vom Bestellformat, das im Abschnitt Details zum Bestellposten ausgewählt wurde, sind nur bestimmte Felder bearbeitbar. Einige Felder sind je nach Bestellungsformat erforderlich.

Anmerkung: Wenn die Checkbox Paket für die Bestellposten-Zeile aktiviert ist, ist die Feldbezeichnungen Stückpreis und Menge anstelle der Feldbezeichnungen Preis physische Ressource oder Preis elektronische Ressource oder Menge zu sehen.

-   **Preis physische Ressource**. Der Preis des physischen Exemplars. Erforderlich, wenn das Bestellformat (siehe Details zum Bestellposten) Physisch, KGV-Mix oder Sonstige ist.
-   **Physische Menge**. Die Anzahl der Exemplare, die bestellt werden. Erforderlich, wenn das Format der Bestellung (siehe Details zum Bestellposten) Physisch, P/E-Mix oder Sonstige ist.
-   **Zusatzkosten**. Alle zusätzlichen Kosten für das Exemplar.
-   **Währung**. Die Währung des Exemplars aus der Dropdown-Liste auswählen. Der Standardwert ist in den Mandant-Einstellungen als Hauptwährung hinterlegt. Weitere Informationen sind unter [Einstellungen > Mandant > Sprache und Lokalisierung](https://info.gbv.de/display/FOLIOGBVEXTERN/Einstellungen+%28Mandant%29%3A+Sprache+und+Lokalisierung) zu finden. Anmerkung: Wenn eine Bestellung geöffnet wird, erstellt das System einen Bindungsvorgang für das aktuelle Budget des Fonds, der im Abschnitt Fondsverteilung der Bestellung ausgewählt wurde. Wenn die Währung des Bestellpostens nicht mit der Budgetwährung übereinstimmt, wird die Bindung im Budget als umgerechneter Betrag angezeigt. Die Budgetwährung wird zum Zeitpunkt der Erstellung des Datensatzes Finanzen > Geschäftsjahr auf den Wert der Mandantenwährung gesetzt. Wenn also der Wert der Mandantenwährung aktualisiert wird, basieren alle Budgets, die vor der Aktualisierung erstellt wurden, weiterhin auf der Mandantenwährung, die bei der Erstellung des mit dem Budget verknüpften Haushaltsjahres verwendet wurde.
-   **Aktueller Wechselkurs**. Dieser Wert wird angezeigt, nachdem der Bestellposten gespeichert wurde. Das System ruft den aktuellen Wechselkurs automatisch über die Java Money API ab, die Währungen unter Verwendung der Europäischen Zentralbank (EZB) als Quelle abruft und umrechnet.
-   **Festgelegten Wechselkurs anwenden**. Dieses Feld markieren, wenn eine Wechselkurswert eingeben werden soll, der anstelle des aktuellen Kurses für die Bestellung verwendet werden soll.
-   **Wechselkurs festlegen**. Der Wechselkurswert, der für diese Bestellung anstelle des aktuellen Kurses verwendet werden soll. Dieses Feld ist gesperrt, was durch das Schlosssymbol neben der Feldbeschriftung angezeigt wird. Es sei denn, die Checkbox Eingestellten Wechselkurs verwenden ist aktiviert.
-   **Preis elektronische Ressource**. Der Preis für das elektronische Exemplar. Erforderlich, wenn das Format der Bestellung (siehe Details zum Bestellposten) Physisch oder P/E-Mix ist.
-   **Anzahl elektronisch**. Die Anzahl der elektronischen Exemplare, die bestellt werden. Erforderlich, wenn das Format der Bestellung (siehe Details zum Bestellposten) Elektronisch oder P/E-Mix ist.
-   **Rabatt**. Der Rabatt in Prozent oder der Preis.
-   **Typ**. Hier **%** oder **€** wählen, um die Art des Rabatts anzugeben.
-   **Schätzpreis**. Der berechnete Preis auf der Grundlage der eingegebenen Werte. Schätzpreis = Listeneinzelpreis(e) x Bestellmengen + Zusatzkosten - Rabatt.

## Fondsverteilung

Wenn Mittel bestimmter Fonds belastet werden sollen, in diesem Abschnitt die Fondverteilung eingeben. Es können Mittel für mehr als einen Fonds belastet werden. Die Bindung(en) gilt (gelten) für das Budget des aktuellen Haushaltsjahres für den (die) ausgewählten Fonds.

### **Fonds-Verteilung h****inzufügen**

1.  Auf **Fondsaufteilung hinzufügen** klicken.
2.  Die **Fonds-ID** aus der Dropdown-Liste wählen. Nur aktive Fonds werden in der Liste angezeigt. Anmerkung: Die Verwendung von Erwerbungsteams kann die Anzeige der Fonds in dieser Liste einschränken. Wenn ein Erwerbungsteam so eingerichtet ist, dass es die Anzeigeberechtigungen einschränkt, werden in der Dropdown-Liste nur Fonds angezeigt, die demselben Erwerbungsteam wie der Person zugewiesen sind. Weitere Informationen sind unter Siehe [Einstellungen > Erwerbungsteams](https://info.gbv.de/pages/viewpage.action?pageId=849379720) zu finden.
3.  Die **Kostenart** aus der Liste auswählen.
4.  Den **Wert** des Fonds eingeben, der vergeben werden soll.
5.  Hier **%** oder **€** wählen, um anzugeben, ob der Wert ein Prozentsatz oder ein Preis ist. Die Fondsaufteilung wird gespeichert, sobald der Bestellposten gespeichert wird.

### **Fonds-Verteilung löschen**

1.  Den Fonds suchen, der gelöscht werden soll.
2.  Auf das **Mülleimersymbol** neben dem Fonds klicken. Die Fondsaufteilung wird entfernt und ist gelöscht, sobald der Bestellposten gespeichert ist.

## Standort

Der Standort bestimmt den tatsächlichen Standort des Exemplars nach Erhalt. Wenn mehrere Exemplare bestellt werden, können verschiedenen Standorten zugewiesen werden.

### Standort hinzufügen

Dieses Feld ist erforderlich, wenn der Wert des Feldes **Im Katalog erstellen** Bestände enthält. Es kann aus einem bestehenden Bestand für diese Titelinstanz ausgewählt oder einen neuer Standort für diese Titelinstanz hinzugefügt werden. Weitere Informationen über das Feld **Im Katalog erstellen** sind unter [E-Ressourcen Details > Im Katalog erstellen](https://info.gbv.de/pages/viewpage.action?pageId=851345662) zu finden.

Um einen Standort hinzuzufügen, folgendermaßen vorgehen:

1.  Auf **Standort hinzufügen** klicken.
2.  Wenn das Feld **Im Katalog erstellen** für diesen Bestellposten Bestände enthält und diese Titelinstanz bereits über Bestände verfügt, enthält die Dropdown-Liste **Bestände auswählen** die Liste der vorhandenen Bestände. Einen **Namen (Code)** aus der Dropdown-Liste wählen.
3.  Wenn diese Titelinstanz noch nicht über Bestände verfügt oder eine neuer Standort angelegt werden muss, auf **Neue Bestände für Standort anlegen** klicken.
4.  In das Feld eine **Anzahl physisch** eingeben.
5.  In das Feld eine **Anzahl elektronisch** eingeben.
6.  Den Vorgang nach Bedarf wiederholen. Der Standort wird gespeichert und alle neuen Bestände werden angelegt, sobald der Bestellposten gespeichert ist.

### Standort löschen

1.  Den Standort suchen, der gelöscht werden soll.
2.  auf das **Mülleimersymbol** neben dem Standort klicken. Der Standort wird entfernt und gelöscht, sobald der Bestellposten gespeichert ist.

## Ressourcendetails

### Details zur physischen Ressource

Dieser Abschnitt erscheint nur, wenn unter Bestellformat die Option Physische Ressource oder P/E-Mix auswählt ist.

-   **Materiallieferant**. Der Lieferant des Exemplars. Das Feld ist standardmäßig mit dem Namen des Lieferanten vorbelegt, der mit dem für die Bestellung ausgewählten Lieferantencode verbunden ist. Weitere Informationen sind unter [Bestellung](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio%3A+Bestellung+anlegen) zu finden. Um den Lieferanten zu ändern, auf **Organisationssuche** klicken. Im Dialogfeld **Organisation auswählen** den Lieferanten mithilfe des Suchfelds und/oder der Filter suchen. Auf den Lieferanten klicken, um ihn auszuwählen. Der Lieferant wird dem Feld Materiallieferant hinzugefügt.
-   **Eingang fällig**. Das Datum, an dem der Eingang der Ressource fällig ist, oder das Datum, bis zu dem die Ressource eingegangen sein sollte.
-   **Erwartetes Eingangsdatum**. Das Datum, an dem die Ressource voraussichtlich eintreffen wird. Dieses Datum kann vor oder nach dem Fälligkeitsdatum des Eingangs liegen.
-   **Im Katalog erstellen**. Wählen Sie die Arten von Datensätzen aus, die in der App Im Katalog erstellt werden sollen, sobald die Bestellung geöffnet wird: **Instanz, Bestände, Exemplare**; **Instanz**; **Instanz, Bestand**; **Nichts**. Informationen zur Konfiguration der Standardeinstellung für dieses Feld sind unter [Einstellungen > Bestellungen > Katalog-Interaktionen](https://info.gbv.de/display/FOLIOGBVEXTERN/Einstellungen+%28Bestellungen%29%3A+Katalog-Interaktionen) zu finden.
-   **Materialart**. Die Art der Ressource. Wenn ein Exemplar für die Bestellung erstellt wird, erscheint dieser Wert für die Materialart auf dem Exemplardatensatz in der App Katalog. Anmerkung: Wenn die Materialart des Exemplars in der App Katalog bearbeitet wird, wird der Wert für die Materialart im Exemplardatensatz nicht aktualisiert.
-   **Band**. Eine Nummer zur Identifizierung des spezifischen Bandes, das innerhalb einer Serie, eines Sets oder einer Sammlung bestellt wird. Derzeit wird diese Information nur in der Bestellung gespeichert.

#### Band hinzufügen

Um ein Band hinzuzufügen, auf **Band hinzufügen** klicken und die Bandnummer eingeben. Der Band wird gespeichert, sobald der Bestellposten gespeichert ist.

#### Band löschen

Um ein Band zu löschen, den zu löschenden Band suchen und auf das **Mülleimersymbol** klicken. Das Band wird entfernt und gelöscht, sobald der Bestellposten gespeichert ist.

### Details zu elektronischen Ressourcen

Dieser Abschnitt erscheint nur, wenn unter Bestellformat die Option Elektronische Ressource oder P/E-Mix auswählt ist.

1.  **Zugangsanbieter**. Der Anbieter der elektronischen Ressource. Der Standardwert ist auf den Lieferanten gesetzt. Um den Zugangsanbieter zu ändern, auf **Organisationssuche** klicken, um eine andere Organisation auszuwählen. Im Dialogfeld **Organisation auswählen** die Organisation mit Hilfe des Suchfeldes und/oder der Filter suchen. Auf die Organisation klicken, um sie als Zugangsanbieter hinzuzufügen.
2.  **Aktivierungsstatus**. Wenn die E-Ressource aktiviert ist, die Checkbox Aktivierungsstatus markieren.
3.  **Aktivierung fällig**. Das Datum, an dem die Aktivierung fällig ist. Anmerkung: Wenn im Feld Erwartetes Aktivierungsintervall im Abschnitt Lieferanteninformationen des Lieferantendatensatzes ein Intervall angegeben ist, wird das Fälligkeitsdatum der Aktivierung auf der Grundlage der Anzahl der Tage ausgefüllt, die als Intervall angeben wurden. Wenn zum Beispiel das Intervall auf 365 Tage eingestellt wurde, wird das Feld Aktivierung fällig mit dem Datum gefüllt, das ein Jahr nach dem Datum der Erstellung des Bestellpostens liegt.
4.  **Im Katalog erstellen**. Die Arten von Datensätzen auswählen, die in der App Katalog erstellt werden sollen, sobald die Bestellung geöffnet wird. Informationen zur Konfiguration der Standardeinstellung für dieses Feld auf der Grundlage des Bestellformats sind unter [Einstellungen > Bestellungen > Katalog-Interaktionen](https://info.gbv.de/display/FOLIOGBVEXTERN/Einstellungen+%28Bestellungen%29%3A+Katalog-Interaktionen) zu finden.
5.  **Materialarten**. Die Art der Ressource.
6.  **Testzugang**. Wenn die E-Ressource Teil eines Testzugangs ist, diese Checkbox markieren.
7.  **Erwartete Aktivierung**. Das Datum, an dem die Aktivierung der E-Ressource erwartet wird.
8.  **Personenlimit**. Die Anzahl der Personen, die die E-Ressource auf einmal nutzen können.
9.  **URL**. Ein Link zu der E-Ressource.

### Sonstige Details zur Ressource

Dieser Abschnitt wird nur angezeigt, wenn unter Bestellformat Sonstige ausgewählt ist.

-   **Materiallieferant**. Der Lieferant des Exemplars. Das Feld ist standardmäßig mit dem Namen des Lieferanten vorbelegt, der mit dem für die Bestellung ausgewählten Lieferantencode verbunden ist. Weitere Informationen sind unter [Bestellung](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio%3A+Bestellung+anlegen) zu finden. Um den Lieferanten zu ändern, auf **Organisationssuche** klicken. Im Dialogfeld **Organisation auswählen** den Lieferanten mithilfe des Suchfelds und/oder der Filter suchen. Auf den Lieferanten klicken, um ihn auszuwählen. Der Lieferant wird dem Feld Materiallieferant hinzugefügt.
-   **Eingang fällig**. Das Datum, an dem der Eingang fällig ist.
-   **Erwartetes Eingangsdatum**. Das Datum, an dem das Exemplar voraussichtlich eintreffen wird.
-   **Im Katalog erstellen**. Die Arten von Datensätzen auswählen, die in der App Katalog erstellt werden sollen, sobald die Bestellung geöffnet wird. Informationen zur Konfiguration der Standardeinstellung für dieses Feld auf der Grundlage des Bestellformats sind unter [Einstellungen > Bestellungen > Katalog-Interaktionen](https://info.gbv.de/display/FOLIOGBVEXTERN/Einstellungen+%28Bestellungen%29%3A+Katalog-Interaktionen) zu finden.
-   **Materialart**. Die Art der Ressource.
