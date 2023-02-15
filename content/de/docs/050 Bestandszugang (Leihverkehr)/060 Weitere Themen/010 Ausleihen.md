---
title: "Ausleihen"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [by-folio, for-anwender, topic-sip2, app-ausleihe]
weight: 10
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/access/additional-topics/loans/loans/) & [GBV](https://info.gbv.de/display/FOLIOGBVEXTERN/Ausleihen)
    "
---

{{% pageinfo %}}
Siehe auch: [Folio: Rückgabe Vor-Ort Nutzung erfassen]({{< ref "060 Rueckgabe Vor-Ort Nutzung erfassen" >}})
{{% /pageinfo %}}

Bibliotheksmitarbeitende verwalten die Ausleihen von Personen in FOLIO über drei primäre Apps - Rückgabe, Ausleihe und Personen. Außerdem können die Mitarbeitenden Informationen über Ausleihen in den Apps Ausleihprotokoll und Katalog einsehen.

Die Bedingungen einer Ausleihe - wer ausleihen darf, wie lange das Exemplar ausgeliehen werden kann, ob es verlängert werden kann, welche Benachrichtigungen die Personen erhalten und ob Gebühren anfallen, wenn das Exemplar verspätet zurückgegeben wird - werden durch die Ausleihregeln bestimmt, die bei der Ausleihe, Verlängerung oder Änderung des Fälligkeitsdatums angewendet werden.

## Datenstruktur von Ausleihen

In FOLIO umfasst ein Ausleihobjekt spezifische Informationen, die den Leihverkehr und die Berichterstattung unterstützen.

* **userId**. Die UUID der Person, die das Exemplar ausgeliehen hat. Wenn die Ausleihe geschlossen und anonymisiert wird, wird die userId aus dem Ausleihdatensatz entfernt.
* **proxyUserId**. Wenn das Exemplar von einer Person im Namen eines anderen Person über die Bevollmächtigten-Funktion von FOLIO ausgeliehen wurde, wird die UUID der Bevollmächtigten Person gespeichert.
* **itemId**. Dies ist die Katalog-UUID des Exemplars, das ausgeliehen wurde.
* **itemEffectiveLocationIdAtCheckOut**. Dies ist der Tatsächliche Standort des Exemplars, als es ausgeliehen wurde.
* **Status**. Dies ist der Status der Ausleihe - normalerweise **offen** oder **geschlossen**.
* **loanDate**. Dies ist das Datum/die Uhrzeit, zu dem/der das Exemplar ausgeliehen wurde.
* **dueDate** : Dies ist das Datum/die Uhrzeit, zu der das Exemplar zurückgegeben werden muss. Dieses Datum kann sich ändern, wenn das Exemplar erfolgreich verlängert wurde oder wenn eine Person in FOLIO das Fälligkeitsdatum der Ausleihe ändert.
* **returnDate** : Wenn das Exemplar zurückgegeben wurde, ist dies das Datum/die Uhrzeit der Rückgabe. Die Rückgabe des Exemplars kann den Ausleihstatus auf geschlossen ändern oder auch nicht - dies hängt davon ab, ob eine Forderung erhoben wurde.
* **systemReturnDate** : Wenn die Rückgabe rückdatiert wurde, ist das Rückgabedatum das rückdatierte Datum/die rückdatierte Uhrzeit und das systemReturnDate ist das tatsächliche Datum/die tatsächliche Uhrzeit, zu der das Exemplar in der App Rückgabe zurückgegeben wurde.
* **action** : Dies ist die letzte Aktion, die für eine Ausleihe durchgeführt wurde - Werte umfassen declaredLost, renewed, renewedThroughOverride, checkedin, checkedout, checkedOutThroughOverride, recallrequested, holdrequested, claimedReturned, markedMissing, closedLoan.itemAgedToLost, dueDateChanged, checkedInReturnedByPatron, checkedInFoundByLibrary
* **itemStatus**: Dies ist der letzte Exemplar-Status in Bezug auf diese Ausleihe. Dies kann, muss aber nicht der aktuelle Status des Exemplars im Katalog sein. Wurde eine Ausleihe beispielsweise wieder zurückgebucht und in den Transport zurück an ihren Standort gebracht, lautet das Feld itemStatus **In Transit (in Transport)**, aber das Exemplar im Katalog kann **ausgeliehen** sein, wenn das Exemplar inzwischen an eine andere Person ausgeliehen worden ist.
* **renewalCount**: Dies ist die Anzahl, wie oft die Ausleihe verlängert wurde.
* **loanPolicyId**: Dies ist die UUID für die entsprechende Ausleihrichtlinie.
* **checkoutServicePointId** : Dies ist die UUID der Servicestelle, an der die FOLIO Person angemeldet war, als das Exemplar an die Person ausgeliehen wurde.
* **checkinServicePointId** : wenn das Exemplar zurückgegeben wurde, ist dies die UUID der Servicestelle, an der die Person, die das Exemplar zurückgegeben hat, angemeldet war.
* **patronGroupIdAtCheckout**: Dies ist die UUID der Personengruppe zum Zeitpunkt des Checkouts.
* **dueDateChangedByRecall**: Dies ist ein wahr/falsch-Wert, der angibt, ob das Fälligkeitsdatum des Exemplars durch einen Rückruf für eine andere Person geändert wurde.
* **declaredLostDate**: Wenn die Ausleihe als verloren erklärt wurde, wird das Datum dieser Änderung in diesem Attribut gespeichert.
* **claimedReturnedDate**: Wenn die Ausleihe als angeblich zurückgegeben markiert wurde, wird das Datum, an dem sie als angeblich zurückgegeben markiert wurde, in diesem Attribut gespeichert.
* **overdueFinePolicyId**: Dies ist die UUID für die zugehörige Forderungsrichtlinie, die bei der Erstellung der Ausleihe vergeben wird. Sie wird nicht aktualisiert, wenn die Ausleihe verlängert wird.
* **lostItemPolicyId**: Dies ist die UUID für die zugehörige Richtlinie für verlorene Exemplare, die bei der Erstellung der Ausleihe vergeben wird. Sie wird nicht aktualisiert, wenn die Ausleihe verlängert wird.
* **agedToLostDelayedBilling**: FOLIO erklärt ein Exemplar für verloren und stellt der Person dann die Forderung in einem getrennten Prozessen. Diese Attribute auf dem Ausleihobjekt unterstützen diesen Prozess.

## Was betrachtet FOLIO als Kurzausleihe? Was wird als langfristige Ausleihe betrachtet?

FOLIO behandelt Ausleihvorgänge unterschiedlich, je nachdem, ob es sich um eine Kurzausleihe oder eine Langzeitausleihe handelt. Die Unterscheidung hängt von dem Zeitintervall der Ausleihe ab.

* Wenn ein Exemplar für Minuten oder Stunden ausgeliehen wird, handelt es sich um eine Kurzausleihe.
* Wenn ein Exemplar für Tage, Wochen oder Monate ausgeliehen wird, handelt es sich um eine Langzeitausleihe.

Zu den Unterschieden zwischen den beiden Arten von Ausleihen gehören:

* Der Zeitpunkt der Fälligkeit einer Ausleihe.
    Bei einer Kurzausleihe richtet sich die Fälligkeit nach dem Ausleihdatum/der Uhrzeit und der Ausleihrichtlinie; bei einer Langzeitausleihe richtet sich die Fälligkeit nach der Ausleihrichtlinie und dem Ausleihdatum, aber die Fälligkeit ist immer um 23:59 Uhr.
    * Ein Beispiel: Nehmen wir an, eine Person leiht ein Exemplar an einer Servicestelle aus, die an sieben Tagen in der Woche von 9 bis 22 Uhr geöffnet ist. Wenn sie das Exemplar am 1. April um 11 Uhr ausleiht und die Ausleihrichtlinie besagt, dass sie es 48 Stunden lang ausleihen kann, wird es am 3. April um 11 Uhr fällig. Wenn die Ausleihrichtlinie jedoch besagt, dass das Exemplar 2 Tage lang ausgeliehen werden kann, wäre es stattdessen am 3. April um 23:59 Uhr fällig, obwohl die Servicestelle geschlossen ist.
* Wie die Benachrichtigungen zugestellt werden.
    Benachrichtigungen für Kurzausleihen werden immer in Echtzeit zugestellt. Die meisten Benachrichtigungen für  langfristige Ausleihe werden ebenfalls in Echtzeit zugestellt, **mit Ausnahme** der Benachrichtigungen, die durch **Fälligkeitsdatum/-zeit** der Ausleihe ausgelöst werden. Diese Benachrichtigungen müssen die Token für **mehrere Exemplare** verwenden und werden über Nacht (ab 23:59 Uhr) verarbeitet.

## Wenn eine Ausleihe verlängert oder das Fälligkeitsdatum einer Ausleihe geändert wird, welche Ausleihrichtlinie gilt dann und welche Richtlinien werden angewendet?

Wenn eine Person oder ein FOLIO-Benutzer die Verlängerung einer Ausleihe beantragt oder ein FOLIO-Benutzer das Fälligkeitsdatum einer Ausleihe ändert, prüft FOLIO die Datei mit den Ausleihrichtlinie und kann je nach Fund mehrere Dinge tun (nicht unbedingt in der unten aufgeführten Reihenfolge).

* FOLIO prüft, ob die Person für eine Verlängerung gesperrt ist (entweder manuell oder automatisch). Wenn sienicht gesperrt ist, kann der Prozess fortgesetzt werden.
* FOLIO prüft den Datensatz der Person, um sicherzustellen, dass sie nicht inaktiv oder abgelaufen ist. Wenn er nicht inaktiv oder abgelaufen ist, kann der Vorgang fortgesetzt werden.
* FOLIO ermittelt die Ausleihrichtlinie, die für die Ausleihe gilt, und bestimmt anhand dieser Richtlinie, ob oder wie die Ausleihe geändert werden kann. Wenn sich die Datei mit den Leihverkehrsregeln und die Exemplarinformationen nicht geändert haben, ruft FOLIO die gleiche Leihrichtlinie ab, die bei der letzten Erstellung oder Aktualisierung der Ausleihe verwendet wurde, und wendet sie an.
* Bestandsanfragerichtlinien werden nicht aktualisiert, da Bestandsanfragerichtlinien nicht in der Ausleihe gespeichert sind. Da Bestandsanfragen nur vor der Ausleihe gelten, gibt es keinen Grund, eine Referenz im Ausleihdatensatz zu speichern.
* FOLIO wird die zugehörigen Richtlinien für überfällige und verlorene Exemplare **nicht** aktualisieren, da dies dazu führen könnte, dass die Person mit höheren Beträgen haftet, als sie bei der Ausleihe des Exemplars erwartet hatte.
* FOLIO **aktualisiert** die Zeitpläne für Benachrichtigungen. Die UUID der Ausleihrichtlinie wird nicht in der Ausleihe gespeichert. Stattdessen liest FOLIO die geltenden Benachrichtigungsregeln aus der Ausleihrichtlinie, entfernt die vorherigen Benachrichtigungen und erstellt dann die entsprechenden Benachrichtigungen, die zu den neuen Kalenderdaten ausgeführt werden.
* FOLIO **erstellt** einen Eintrag im Ausleihprotokoll, um zu zeigen, dass das Exemplar verlängert wurde oder dass sich das Fälligkeitsdatum geändert hat.

## Beispiel: Eine Studentin wird zur Doktorandin

Nehmen wir an, Sofia Cruz ist Studentin an der Main University.

Die Universität Main verfügt über eine Ausleihrichtlinie, die unterschiedliche Regeln für Personengruppen enthält. Die Universität Main erlaubt Studierenden im Grundstudium (undergrad) die Ausleihe von Büchern für 28 Tage mit unbegrenzter Verlängerungsmöglichkeit und Studierenden im Hauptstudium (grad-student) die Ausleihe von Büchern für 90 Tage mit unbegrenzter Verlängerungsmöglichkeit. Zwei Ausleihregeln in FOLIO machen dies möglich:

g undergrad: l 28-day-loan r hold-only n standard-notice o standard-overdue i standard-lost
g grad-student: l 90-day-loan r allow-all n standard-notice o standard-overdue i standard-lost

Sofias FOLIO-Konto hat die Personengruppe \`undergrad', so dass die erste Zeile in dieser Regel gilt. Sie können Bücher für eine Ausleihe von 28 Tagen mit unbegrenzten Verlängerung ausleihen.

Nehmen wir an, Sofia leiht sich im Februar mehrere Bücher aus und benutzt sie weiter, so dass sich ihre Ausleihen weiter verlängern. Im Sommer beginnt sie ein Studium an der Main University, und die Personengruppe in ihrem FOLIO-Datensatz ändert sich von undergrad' zu grad-student'.

Wenn Sofia das nächste Mal ihre Bücher erneuert, gilt die zweite Zeile der Ausleihrichtlinie:

g grad-student: l 90-day-loan r allow-all n standard-notice o standard-overdue i standard-lost

So geht FOLIO bei der Erneuerung von Exemplaren von Sofia vor:

* FOLIO prüft dieAusleihrichtlinie und stellt fest, dass es die Zeile mit den Ausleihregeln verwenden soll, die mit g grad-student beginnt ...
* FOLIO aktualisiert die UUID der Ausleihrichtlinie, die in Sofias Ausleihen gespeichert ist, auf die UUID für die Richtlinie 90-Tage-Ausleihe und gibt Sofia die neue, 90-tägige rollierende Ausleihfrist.
* Im Ausleihdatensatz ist keine Bestandsanfragerichtlinie gespeichert, so dass sich dort nichts ändert.
* Die ID der Überfälligkeitsrichtlinie und die ID der Richtlinie für verlorene Exemplare **werden** im Ausleihdatensatz gespeichert, aber sie werden **nicht** aktualisiert, wenn die Ausleihe verlängert oder das Fälligkeitsdatum geändert wird. Das liegt daran, dass eine neue Richtlinie für überfällige oder verlorene Exemplare dazu führen könnte, dass die Person mit höheren Beträgen haftet, als sie bei der Ausleihe des Exemplars erwartet hatte.
* FOLIO liest die Benachrichtigungsrichtlinie aus der Ausleihrichtlinie ein. FOLIO erstellt dann die geplanten Benachrichtigungen in der Benachrichtigungsdatenbank entsprechend der Richtlinie und löscht zuvor geplante Benachrichtigungen, die nun nicht mehr verschickt werden müssen.

## Was geschieht mit den Ausleih-Regeln und -Richtlinien, wenn Exemplarinformationen geändert werden, nachdem ein Exemplar ausgeliehen wurde (z.B. wenn die Ausleihart für ein Exemplar geändert wird, das ausgeliehen ist)?

Werden Informationen zu einem Exemplar geädnert, das gerade ausgeliehen ist, ändert sich nichts am Exemplardatensatz. Die Ausleihe kann sich ändern, wenn das Exemplar verlängert oder das Fälligkeitsdatum der Ausleihe geändert wird, und die Änderung der Exemplarinformationen bedeutet, dass eine andere Leihverkehrsregel gilt. Siehe "Wenn eine Ausleihe verlängert oder das Fälligkeitsdatum einer Ausleihe geändert wird, welche Ausleihrichtlinie gilt dann und welche Richtlinien werden angewendet?"

## Was geschieht in FOLIO, wenn ein Exemplar zurückgegeben wird?

Wenn ein Exemplar in FOLIO eingecheckt wird, laufen die folgenden Schritte ab (nicht unbedingt in dieser Reihenfolge.)

* FOLIO prüft den Status des Exemplars.
* Wenn ein Exemplar den Status **Verfügbar** hat, zählt FOLIO es als Vor-Ort Nutzung.
* Wenn ein Exemplar den Status **In Transport** hat, prüft FOLIO die angemeldete Servicestelle, um festzustellen, ob sie die primäre Servicestelle für den tatsächlichen Standort des Exemplars ist. Wenn die angemeldete Servicestelle nicht übereinstimmt, bleibt der Status des Exemplars auf In Transport. Wenn die angemeldete Servicestelle übereinstimmt, ändert FOLIO den Status des Exemplars auf **Verfügbar**
* FOLIO prüft die Ausleihrichtlinie, die Überfälligkeitsrichtlinie und die Richtlinie für verlorene Exemplare, um festzustellen, ob Maßnahmen ergriffen werden müssen.
* Wenn das Exemplar als überfällig eingestuft, aber nicht zurückgerufen wurde, berechnet FOLIO die Forderungen auf der Grundlage der zugehörigen Richtlinien und bucht sie auf das Konto der Person, wenn die Forderung größer als Null ist.
* Wenn das Exemplar zurückgerufen wurde und überfällig ist, berechnet FOLIO die Forderungen für den Rückruf auf der Grundlage der zugehörigen Richtlinie und belastet das Konto der Person, wenn die Forderung größer als Null ist.
* Wenn der Status eines Exemplars als **für verloren erklärt** wird oder als **Verloren erklärt** gilt, zeigt FOLIO eine Warnmeldung an, und das Personal muss die Option wählen, die Rückgabe fortzusetzen. Wenn die Rückgabe fortgesetzt wird, verweist FOLIO auf die Richtlinie für verlorene Exemplare, um festzustellen, ob für die Person Forderungen anfallen, und schreibt diese dem Konto der Person zu.
* Wenn die Ausleihrichtlinie vorsieht, dass Forderungsbescheide verschickt werden müssen, werden diese Bescheide erstellt und verschickt.
* Wenn ein Exemplar den Status **Ausgeliehen**, **Verloren erklärt** oder **für verloren erklärt** hat: Wenn ein Exemplar verloren erklärt wurde oder für verloren erlklärt gilt, zeigt FOLIO eine Warnmeldung an und die Mitarbeitenden müssen in der Abfrage auswählen, ob sie die Rückgabe fortsetzen möchten.

## Wie wird die Vor-Ort Nutzung in den FOLIO Daten erfasst?

FOLIO verfolgt kein explizites Datenattribut für die Vor-Ort Nutzung eines Exemplars. Stattdessen geht FOLIO davon aus, dass ein Exemplar "intern" genutzt wird, je nachdem, wie sich der Status des Exemplars bei der Rückgabe ändert. Wenn das Exemplar vor der Rückgabe den Status "Verfügbar" hatte, betrachtet FOLIO dies als interne Nutzung.

Es gibt derzeit keine Möglichkeit, einen Bericht über die Vor-Ort Nutzung mit einem In-App Bericht zu erstellen. Eine Möglichkeit, an Daten zur Vor-Ort Nutzung zu gelangen, besteht darin, die FOLIO API mit einem Tool wie Postman abzufragen, um Eincheck-Datensätze zurückzugeben. Dazu eine GET-Anfrage wie diese an die jeweilige FOLIO-Instanz senden, um die Rücknahmedatensätze mit Vor-Ort Nutzung zu erhalten:

/check-in-storage/check-ins?query=itemStatusPriorToCheckIn=="Available"

## Was passiert, wenn eine Richtlinie für den Leihverkehr gelöscht wird?

### Ausleihrichtlinie

Eine Ausleihrichtlinie kann nicht über Einstellungen > Ausleihe > Ausleihrichtlinien gelöscht werden, wenn mit der Ausleihrichtlinie offene Ausleihen verbunden sind.

Bestandsanfrage-Richtlinie

Sie können eine Bestandsanfrage löschen, die Teil der Ausleihregeln ist. Wenn Sie dies tun und dann Ihre Ausleihregeln überprüfen, werden Sie feststellen, dass alle Regeln, die auf die Bestandsanfrage verweisen, immer noch in der Datei vorhanden sind, aber die Bestandsanfrage wird mit der UUID und nicht mit dem Namen der Richtlinie aufgeführt.

Bestandsanfragen werden nur referenziert, wenn eine Anfrage gestellt wird, und werden nicht in einer späteren Ausleihe gespeichert. Sie lassen sich also relativ einfach löschen, wobei Sie vorher Ihre Zirkulationsregeln überprüfen sollten.

Nehmen wir zum Beispiel an, Sie müssen die Bestandsanfrage allow-all löschen. Wir empfehlen Ihnen, Ihre bestehenden Ausleihregeln zu überprüfen und alle Verweise auf allow-all durch eine andere Anfragerichtlinie zu ersetzen. Wenn Sie das getan haben, können Sie "allow-all" unter Einstellungen > Leihverkehr > Bestandsanfragen löschen.

### Benachrichtigungsrichtlinie

Eine Benachrichtigungsrichtlinie, die Teil der Ausleihregeln ist, kann gelöscht werden. Wird dies getan und dann die Ausleihregeln überprüft, ist zu sehen, dass alle Regeln, die auf die Benachrichtigungsrichtlinie verweisen, immer noch in der Datei vorhanden sind, aber die Benachrichtigungsrichtlinie wird mit der UUID der Richtlinie und nicht mit dem Namen der Richtlinie aufgeführt.

Auf die Benachrichtigungsrichtlinie wird nur verwiesen, wenn eine Ausleihe erstellt, verlängert oder ein Fälligkeitsdatum geändert wird. Sie sind relativ einfach zu löschen, wobei zuerst die Verweise auf sie in Ihren Ausleihregeln entfernt werden sollten.

Nehmen wir zum Beispiel an, die Benachrichtigungsrichtlinie faculty-semester-notice muss gelöscht werden. Zunächst würden die Ausleihregeln überprüft und alle Verweise auf faculty-semester-notice durch eine andere Benachrichtigungsrichtlinie aktualisiert werden. Danach kann faculty-semester-notice unter Einstellungen > Leihverkehr > Benachrichtigungsrichtlinie gelöscht werden.

### Ausleihrichtlinien für überfällige Exemplare

Eine Ausleihrichtlinie für überfällige Exemplare kann nicht über Einstellungen > Leihverkehr > Forderungen gelöscht werdeb, wenn mit der Richtlinie offene Forderungen verbunden sind.

### Ausleihrichtlinie für verlorene Exemplare

Eine Ausleihrichtlinie für verlorene Exemplare kann nicht über Einstellungen > Leihverkehr > Forderungen  gelöscht werden, wenn mit der Richtlinie offene Ausleihen verbunden sind.

## Was passiert, wenn eine Ausleihregel gelöscht wird?

Wenn Sie eine Ausleihregel aus der Ausleihregel-Datei entfernen, passiert nichts mit bestehenden Ausleihen, die diese Ausleihregel verwendet haben.

Wenn eine Person versucht, eine Ausleihe zu verlängern, die mit der aus der Datei entfernten Ausleihregel verlängert worden wäre, sucht FOLIO in den Ausleihregeln nach einer anderen passenden Regel. Wenn es nicht mindestens eine andere passende Regel in der Datei findet, wird die Ausweichregel verwendet.

## Wie arbeitet FOLIO mit Selbstverbuchungsgeräten zusammen?

FOLIO unterstützt SIP2, ein Industriestandardprotokoll für die Verbindung von Selbstverbuchungsgeräten mit Bibliothekssystemen.

Selbstverbuchungsgeräten können sich über das SIP2-Edge-Modul von FOLIO mit FOLIO verbinden. Um dies einzurichten, muss in der Regel mit dem FOLIO-Administrator und/oder Hosting-Anbieter zusammengearbeitet werden.

Weitere Informationen zur SIP2-Konfiguration in der Dokumentation des Edge-Moduls auf Github zu finden - [https://github.com/folio-org/edge-sip2](https://github.com/folio-org/edge-sip2)

## Häufige Fehler bei der Ausleihe von Exemplaren

### Fehlermeldung: "Der Kalender ist für das angefragte Datum nicht vorhanden"

Wenn ein Exemplar ausgeliehen wird, muss FOLIO in der Lage sein, das Fälligkeitsdatum für das Exemplar zu berechnen. Dazu werden Informationen aus dem Datensatz der Person, der Ausleihrichtlinie und dem Kalender der Servicestelle verwendet, an der das Bibliothekspersonal angemeldet ist.

Die Fehlermeldung "Der Kalender ist für das angeforderte Datum nicht vorhanden" bedeutet, dass FOLIO keine Kalenderinformationen bis einschließlich des berechneten Fälligkeitsdatums des Exemplars finden kann.

Der erste Schritt zur Fehlerbehebung besteht darin, den Kalender für die Servicestelle unter Einstellungen > Kalender zu überprüfen, um sicherzustellen, dass ein Kalender für die erforderliche Zeitspanne bereitgestellt ist.

Diese Fehlermeldung kann verwirrend sein, wenn bedacht wird, wie Fälligkeitsdaten auf das Ablaufdatum eines Kontos reduziert werden. Folgendes Szenario angenommen:

* Eine Person kommt am 1. Juli an den Schalter und wünscht ein Exemplar auszuleihen;
* Gemäß den Ausleihregeln sollte die Person ein Fälligkeitsdatum am 15. Dezember erhalten. Das Konto der Person läuft jedoch am 15. August ab, so dass sie das Buch nur bis zum 14. August ausleihen kann.
* Im Kalender der Servicestelle, in der die Ausleihe stattfindet, sind Termine bis zum 1. September eingetragen.

Das berechnete Fälligkeitsdatum vom 14. August ist in den in FOLIO gespeicherten Kalenderinformationen enthalten. Dennoch schlägt die Ausleihe mit der Meldung "Der Kalender ist für das angeforderte Datum nicht vorhanden." fehl.
