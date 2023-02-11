---
title: "Forderungen"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [by-folio, for-anwender, topic-sip2, app-ausleihe]
weight: 20
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/access/additional-topics/feesfines/feesfines/) & [GBV](https://info.gbv.de/display/FOLIOGBVEXTERN/Forderungen)
    "
---

FOLIO ermöglicht es Bibliotheken, Forderungen in Personenkonten zu erheben. Die Gebühren können aus verschiedenen Gründen erhoben werden, z.B. für die Buchung von Räumen, die überfällige Rückgabe eines Buches oder den Ersatz eines Exemplars, das die Person nicht zurückgegeben hat. In FOLIO werden diese in der Regel als Forderungen kategorisiert.

Bibliotheken können Forderungen manuell oder automatisch erheben.

Automatische Forderungen fallen in drei Kategorien:

-   Wiederbeschaffungsgebühr für verlorene Exemplare
-   Bearbeitungsgebühr für verlorene Exemplare
-   Mahngebühren für überfällige Exemplare

Sie werden von FOLIO automatisch erhoben, wenn Exemplare ausgeliehen und nicht rechtzeitig zurückgegeben werden, entsprechend den Ausleiheregeln für überfällige und verlorene Exemplare.

Manuelle Forderungen hingegen werden als Kategorien in Einstellungen > Personen eingerichtet. Sie können für eine Vielzahl von Bibliotheksforderungen verwendet werden, z.B. für den Ersatz eines beschädigten Exemplars, für die Buchung eines Raums oder für die Bezahlung einer Personenkarte. Manuelle Gebühren sind immer mit einer bestimmten Person verbunden; sie können mit einem Exemplar verbunden sein, aber sie sind nicht mit einer Ausleihe verbunden.

## Forderungen-Datenstruktur

In FOLIO werden die Informationen zu Gebühren und Forderungen in zwei miteinander verbundenen Objekten gespeichert: **Konten** und **Aktionen**.

Ein **Konto** ist das übergeordnete Objekt. Wenn eine Forderung erhoben wird, wird immer ein Kontoobjekt erstellt.

Eine **Aktion** ist das untergeordnete Objekt, in dem eine Transaktion für ein Konto gespeichert wird.

Einem **Konto** werden eine oder mehrere **Aktionen** zugeordnet.

### Beispiel: Eine Person gibt ein Buch nicht zurück

Angenommen, Julia Smith ist eine Person in der Universitätsbibliothek Normal. Sie leiht sich ein Buch aus und gibt es nicht an die Bibliothek zurück, bevor es als verloren gilt.

Wenn das Exemplar als verloren gilt, werden Julia €100 als Gebühr für verlorene Exemplare und €25 als Bearbeitungsgebühr für verlorene Exemplare berechnet.

Die Wiederbeschaffungsgebühr von €100 und die Bearbeitungsgebühr von €25 sind jeweils separate Konten, die Julia belastet werden.

Angenommen, Julia kann das Buch nicht zurückgeben und beschließt, für das Exemplar zu bezahlen. Sie kommt in die Bibliothek und bezahlt €50 in bar. Für die Wiederbeschaffungsgebühr von €100 verzichtet die Bibliothek auf €75 und akzeptiert €25 als Zahlung. Die anderen 25 Dollar werden zur Zahlung der Bearbeitungsgebühr verwendet.

In FOLIO würden die zugrunde liegenden Konto- und Aktionsdaten wie folgt aussehen.

**Konto Nr. 1**: Dies entspricht den 100 €, die Julia als Gebühr für verlorene Exemplare in Rechnung gestellt wurden. Es gäbe drei zugehörige Aktionen:

-   Aktion 1 steht für die ursprüngliche Belastung von Julia und hat in den zugrunde liegenden Daten den Aktionstyp "Ausstehend". In der Benutzeroberfläche wird die Aktionsart als "Gebühr für verlorene Exemplare" angezeigt. Zu diesem Zeitpunkt hat das **Konto** den Status "Offen".
-   Aktion 2 bedeutet, dass Julia €25 bezahlt, mit der Aktionsart "Teilweise bezahlt".
-   Aktion 3 bedeutet, dass die Bibliothek auf die verbleibenden 75 € verzichtet, mit der Aktionsart "Teilweise erlassen". Wenn Aktion 3 durchgeführt wird, wird der Status des Kontos auf **Geschlossen** gesetzt.

Die Bibliothek könnte sich dafür entscheiden, zuerst auf die 75 € zu verzichten und dann die 25 € als bezahlt zu kennzeichnen. In diesem Fall würden Aktion 2 und Aktion 3 in der Reihenfolge umkehren, aber das Ergebnis wäre immer noch dasselbe - Bezahlung und Schließung des Kontos, Schließung der Ausleihe und Änderung des Status des Exemplars auf **Verloren und bezahlt**.

**Konto Nr. 2:** Dieses Konto steht für die Bearbeitungsgebühr von 25 € und hat zwei zugehörige Aktionen.

-   Aktion 1 steht für die Bearbeitungsgebühr in Höhe von 25 € und hat in den zugrunde liegenden Daten den Aktionstyp "Ausstehend". Der Aktionstyp in der Benutzeroberfläche würde als "Bearbeitungsgebühr für verlorene Exemplare" angezeigt.
-   Aktion 2 bedeutet, dass die Bibliothek 25 € in bar akzeptiert, um die Gebühr zu bezahlen, mit dem Aktionstyp "Vollständig bezahlt". Wenn Aktion 2 durchgeführt wird, wird der Status des Kontos auf **Geschlossen** gesetzt.

## Forderungseigentümer/-in

In FOLIO steht ein/e Forderungseigentümer/-in für die Person oder die Dienststelle, die Forderungen für FOLIO-Transaktionen verwaltet.

Ist geplant, Forderungen zu erheben, muss mindestens ein Forderungseigentümer/-in eingerichtet werden. FOLIO verlangt nicht, dass ein/e Forderungseigentümer/-in ein bestimmte Abteilung oder einen Teil eines Bibliothekssystems repräsentiert. Ein/e Forderungseigentümer/-in kann eine Einzelperson, eine bestimmte Dienststelle oder eine bestimmte Bibliothek repräsentieren.

Forderungseigentümer/-in werden unter [Einstellungen > Personen > Forderungen > Eigentümer/-in konfiguriert](https://info.gbv.de/pages/viewpage.action?pageId=841809942).

FOLIO-Bibliotheken sollten für jede Servicestelle in ihrem FOLIO-Mandanten einen Forderungseigentümer/-in konfigurieren, auch wenn sie nicht erwarten, dass Exemplare, die an einer bestimmten Servicestelle hängen, ausgeliehen werden und Forderungen generieren. Denn wenn eine solche Ausleihe stattfindet und der Servicestelle kein Forderungseigentümer/-in zugeordnet ist, wird die Forderungstransaktion fehlschlagen. Bibliotheken sollten daher einen Forderungseigentümer/-in für diese Servicestellen als Backup für den Fall einrichten, dass Forderungen anfallen.

### Wie sind die Forderungseigentümer/-in mit den Standorten verbunden?

Die meisten Bibliotheken wünschen sich, dass überfällige und verlorene Forderungen entsprechend dem Standort des Exemplars eingezogen werden. Daher verwendet FOLIO den Standort des Exemplars, um den Forderungseigentümer/-in zu bestimmen, der mit der Forderung verknüpft werden soll. Dazu sucht FOLIO die primäre Servicestelle für den Standort des Exemplars und dann den Forderungseigentümer/-in für diese Servicestelle.

Für eine überfällige Gebühr verwendet FOLIO den tatsächlichen Standort eines Exemplars, um den Forderungseigentümer/-in zu ermitteln.

Bei Gebühren für verlorene Exemplare oder Bearbeitungsgebühren für verlorene Exemplare verwendet FOLIO den **dauerhaften Standort** des Exemplars, um den Forderungseigentümer/-in zu ermitteln. Wenn der **permanente Standort eines Exemplars** nicht festgelegt ist, verwendet FOLIO stattdessen den **Standort des permanenten Bestands.**

Forderungen fallen immer auf diese Weise an, **auch wenn** der Standort eines Exemplars nicht Teil der Ausleihregeln ist, die für die Ausleihe verwendet wurde, bei der eine Gebühr angefallen ist.

#### Beispiel: Auflaufen von Forderungen für verlorene Exemplare bei Forderungseigentümer/-in

Julia Smith wünscht sich ein Buch, das in der Wissenschaftlichen Bibliothek im Regal steht, um es in der Juristischen Bibliothek abzuholen.

Die Informationen zum Standort des Buches sehen wie folgt aus:

-   **Temporärer Standort des Exemplars**: leer
-   **Dauerhafter Standort des Exemplars**: leer
-   **Temporärer Standort des Bestandes**: leer
-   **Dauerhafter Standort des Bestandes**: "Wissenschaftliches Bibliothek - Regal"
-   **Tatsächlicher Standort des Exemplars**: "Wissenschaftliches Bibliothek - Regal"

Julie leiht sich das Buch an der Servicestelle der Rechtsbibliothek aus und gibt es nicht zurück. Das Exemplar gilt als verloren und wird mit einer Gebühr von €100 für verlorene Exemplare und einer Bearbeitungsgebühr von €25 für verlorene Exemplare belegt.

Wann das Exemplar als verloren gilt:

-   FOLIO prüft zunächst den Exemplardatensatz auf einen **dauerhaften Standort des Exemplars**.
-   Da dieser Wert nicht festgelegt ist, prüft FOLIO als nächstes den **dauerhaften Standort des Bestands** und findet den Wert "Wissenschaftliches Bibliothek - Regal".
-   FOLIO prüft dann den Standortdatensatz für "Wissenschaftliches Bibliothek - Regal" und stellt fest, dass der Standort eine primäre Servicestelle mit dem Namen "Wissenschaftliches Bibliothek - SP" hat.
-   Schließlich prüft FOLIO die Datensätze der Forderungseigentümer/-in für die Servicestelle "Wissenschaftliches Bibliothek - SP" und stellt fest, dass diese mit dem Forderungseigentümer/-in "Science and Engineering Business Office" verbunden ist.
-   FOLIO berechnet sowohl die Gebühr für verlorene Exemplare in Höhe von €100 als auch die Bearbeitungsgebühr für verlorene Exemplare in Höhe von €25 und ordnet sie dem Eigentümer "Science and Engineering Business Office" zu.

## Forderungen/Gebührenbescheide

Für manuell erhobene Forderungen funktionieren die Bescheide anders als für automatisch erhobene Forderungen.

### Manuelle Forderungen

Für manuelle Forderungen gibt es zwei Arten von Bescheiden, die verwendet werden können - den **Gebührenbescheid** und den **Maßnahmenbescheid**.

Für beide Arten von Bescheiden können unter Einstellungen>Leihverkehr>Mitteilungen für Personen>Mitteilungsvorlagen für Personen Vorlagen erstellt werden. Für einen **Gebührenbescheid** die Bescheidkategorie "Manuelle Forderung" wählen. Für eine **Maßnahmenbescheid** wählen Sie die Kategorie "Manuelle Forderung (zahlen, erlassen, erstatten, überweisen oder stornieren/fehlerhaft)".

Unter Einstellungen>PErsonen>Gebühren/Gebühren>Manuelle Gebühren kann der entsprechenden Forderungseigentümer/-in ausgewählt und einen **Gebührenbescheid** und einen **Maßnahmenbescheid** mit dieser manuellen Gebühr verknüpfen werden. Es können Standardvorlagen für Gebühren- und/oder Aktionsbescheide für den Eigentümer ausgewählt oder verschiedene Vorlagen für Gebührenbescheide für einzelne Arten von Forderungen festlegt werden.

Wenn eine manuelle Gebühr für das Konto einer Person erstellen oder eine Aktion auf eine bestehende Gebühr angewendet wird, kann über eine Checkbox auswählt werden, ob die Person benachrichtigt werden soll, wenn es eine entsprechende Vorlage gibt.

### Automatische Forderungen

Die Benachrichtigungen für automatische Forderungen werden durch die zugehörige Ausleihregel bestimmt.

Wenn das Exemplar ausgeliehen ist, gibt es eine zugehörige Benachrichtigungsrichtlinie. Innerhalb dieser Richtlinie kann festlegelegt werden, dass bei überfälligen Forderungen oder verlorenen Exemplaren eine Benachrichtigung versendet wird.

Mahnungen für langfristige Ausleihen (Ausleihen mit einem Zeitintervall von Tagen, Wochen oder Monaten) werden pro Gebühr verschickt und nicht in einer einzigen E-Mail gebündelt. Dies kann dazu führen, dass mehr Benachrichtigungen an eine Person gesendet werden als gewünscht.

Nehmen wir an, eine Bibliothek hat eine Richtlinie, nach der Dozenten bis zum Ende des akademischen Jahres Bücher ausleihen können (definiert mit einem festen Fälligkeitsdatum). Wenn die Exemplare verloren gehen, werden den Dozenten €100 für den Ersatz des Buches in Rechnung gestellt, zuzüglich einer Bearbeitungsgebühr von €25. Ein Fakultätsmitglied leiht sich zehn Bücher aus, die alle am Ende des akademischen Jahres fällig sind, und gibt sie nicht zurück. Wenn die Bibliothek die Benachrichtigung über verlorene Bücher verwendet, würde dieses Fakultätsmitglied zwanzig separate E-Mails erhalten - eine für die Ersatzkosten und eine für die Bearbeitungsgebühr für jedes Exemplar.

Es gibt zwar Pläne, dies zu ändern, so dass die Forderungsbescheide für verlorene Exemplare in großen Mengen verschickt werden, aber diese Entwicklung ist noch nicht terminiert.

Bibliotheken, die nicht wünschen, dass die E-Mails in Form von Einzelbenachrichtigungen verschickt werden, können alternativ den Auslöser für die Fälligkeitsbenachrichtigung verwenden; die Fälligkeitsbenachrichtigung kann nach Fälligkeit des Exemplars ausgelöst werden. Wenn beispielsweise ein Exemplar nach 28 Tagen für verloren erklärt wird, kann die Bibliothek 27 Tage nach Fälligkeit des Exemplars eine Benachrichtigung über die Fälligkeit der Ausleihe senden, um die Person darüber zu informieren, dass die Exemplare in Kürze für verloren erklärt _werden_, oder sie sendet die Benachrichtigung nach 29 Tagen, um die Person darüber zu informieren, dass die Exemplare für verloren erklärt _wurden_.

## Wie werden die Forderungen für überfällige Ausleihen und überfällige Rückrufe berechnet?

Das Forderungenssystem von FOLIO ist sehr dynamisch und ermöglicht viele verschiedene Konfigurationsoptionen für die Dauer der Ausleihe und die Einstellungen der Forderungen. Es kann hilfreich sein zu wissen, wie die zugrunde liegende Logik funktioniert, wenn FOLIO einen überfälligen oder überfälligen Rückruf-Gebührenbetrag berechnet.

Da Forderungen und Ausleihdauer in verschiedenen Intervallen - Minuten, Stunden, Tage, Wochen oder Monate - definiert werden können, geht FOLIO so vor, dass es die Dauer der Überfälligkeit eines Exemplars nimmt, sie in Minuten umrechnet und dann dieses Datum/diese Zeit mit dem Forderungsintervall - ebenfalls in Minuten - vergleicht, um zu bestimmen, wie die Gebühr berechnet wird. Dies ist recht einfach, wenn eine Bibliothek Forderungen für alle Stunden erhebt, kann aber sehr viel komplizierter werden, wenn Forderungen nur dann erhoben werden, wenn eine zugehörige Servicestelle geöffnet ist.

Bitte auch beachten, dass FOLIO diese Berechnungen erst dann durchführt, wenn das überfällige oder zurückgerufene Exemplar zurückgegeben wird. Einige Bibliothekssysteme bieten eine "laufende Gesamtberechnung" für überfällige Forderungen an, aber FOLIO bietet diese Funktion nicht.

### Beispiel: Eine Person gibt ein überfälliges Exemplar an einer Servicestelle zurück, die rund um die Uhr besetzt ist

Nehmen wir an, eine Person leiht sich ein Exemplar aus, das eine dreistündige Leihfrist hat und für das eine Gebühr von 3 €/Tag fällig ist. Sie leiht sich das Exemplar am 1. September um 14 Uhr aus. Das Exemplar muss am 1. September um 17 Uhr zurückgegeben werden, aber die PErson gibt es erst am 2. September um 18 Uhr zurück.

Bei der Berechnung der Mahngebühren werden unter anderem folgende Faktoren berücksichtigt:

-   Der Kalender der ausleihenden Servicestelle - in diesem Beispiel nehmen wir an, die Servicestelle ist rund um die Uhr geöffnet
-   Die in den Überfälligkeitsrichtlinien festgelegte Überfälligkeitsgebühr - in diesem Beispiel €3/Tag
-   ob es eine in der Ausleihrichtlinie festgelegte Schonfrist für eine verspätete Rückgabe gibt - in diesem Beispiel nehmen wir an, dass es keine Schonfrist gibt
    ob die Mahngebühren während der Öffnungszeiten erhoben werden sollen, wie in den Mahnrichtlinien festgelegt - in diesem Beispiel: Ja

Sobald das Exemplar zurückgegeben wird, berechnet FOLIO die überfälligen Forderungen wie folgt:

-   Das Exemplar war einen Tag und eine Stunde überfällig - 25 Stunden - die dann in Minuten umgerechnet werden - 1500 Minuten
-   Die Forderung/Gebühr beträgt €3/Tag. Ein Tag hat 1440 Minuten, also sind es €3/1440 Minuten.
-   FOLIO berechnet die Anzahl der "Zeiteinheiten", für die das Exemplar überfällig war - in diesem Fall dividiert es 1500/1440 = ~1,07 "Einheiten" überfälliger Zeit.
    FOLIO rundet die Anzahl der überfälligen Zeit-"Einheiten" auf die nächste ganze Zahl auf - in diesem Fall 2.
-   FOLIO multipliziert die Anzahl der überfälligen Zeit-"Einheiten" mit dem Betrag der Geldstrafe pro Intervall - 3 - um eine Gesamtgeldstrafe von €6.00 zu erhalten.

### Beispiel: Eine Person gibt ein überfälliges Exemplar an einer Servicestelle zurück, die über Nacht geschlossen ist

Nehmen wir an, eine Person leiht sich ein Exemplar mit einer Leihfrist von sieben Tagen und einer Mahngebühr von €3/Tag aus. Sie leiht sich das Exemplar am 1. Mai um 14 Uhr aus. Das Exemplar muss am 8. Mai um 23:59:59 Uhr zurückgegeben werden. Die Person gibt das Exemplar am 11. Mai um 14 Uhr zurück.

Die Faktoren, die bei der Berechnung der Mahngebühren berücksichtigt werden, sind

-   Der Kalender der ausleihenden Servicestelle - in diesem Beispiel nehmen wir an, dass die Servicestelle vom 1. Mai bis zum 11. Mai von 8 Uhr morgens bis Mitternacht geöffnet ist.
-   Die in den Überfälligkeitsrichtlinien festgelegte Überfälligkeitsgebühr - in diesem Beispiel €3/Tag
-   Ob es eine in der Ausleihrichtlinie festgelegte Schonfrist für eine verspätete Rückgabe gibt - in diesem Beispiel eine Schonfrist von einem Tag.
-   ob die Mahngebühren während der Geschäftszeiten erhoben werden sollen, wie in den Richtlinien für überfällige Artikel festgelegt - in diesem Beispiel ist diese Option auf Nein gesetzt.

Sobald das Exemplar zurückgegeben wird, berechnet FOLIO die überfälligen Forderungen wie folgt:

-   Das Exemplar war 2 Tage und 14 Stunden überfällig, wenn man sich den Kalender genau ansieht. Das sind 62 Stunden, also 3720 Minuten.
-   Es gibt eine Nachfrist, aber da die Nachfrist einen Tag / 1440 Minuten beträgt und das Exemplar nach der Nachfrist zurückgegeben wurde, wird die Nachfrist bei der Berechnung nicht berücksichtigt.
-   FOLIO sieht, dass die Überfälligkeitsrichtlinie besagt, dass während der Öffnungsszeiten keine überfälligen Forderungen erhoben werden dürfen. Der Kalender der zugehörigen Ausleih-Servicestelle zeigt, dass sie an den drei relevanten Tagen - dem Morgen des 9., 10. und 11. - von Mitternacht bis 8 Uhr morgens geschlossen ist. Die Schließzeit beträgt 8 Stunden pro Tag - also insgesamt 24 Stunden oder 1440 Minuten.
-   FOLIO zieht die geschlossenen Minuten von der gesamten überfälligen Zeit ab - 3720 - 1440 = 2280 Minuten. Das ist der Betrag für die überfällige Zeit, die FOLIO in Rechnung stellt.
-   Der Gebührensatz beträgt €3/Tag oder €3/1440 Minuten. FOLIO berechnet die Anzahl der Zeit-"Einheiten", für die das Exemplar überfällig war - 2280/1440 = ~1,58 "Einheiten" überfälliger Zeit.
-   FOLIO rundet dies auf die nächste ganze Zahl auf - 2 - und berechnet 2 Intervalle. Es wären also 2 \* 3 = 6, was einer Geldstrafe von €6 entspricht.

Bitte beachten, dass der Person 2 Tage berechnet wurden, obwohl das Exemplar erst am 3. Tag nach der Überfälligkeit zurückgegeben wurde.

Es ist eine Entwicklung geplant, um die Berechnung von Forderungen für abgeschlossene Zeiträume besser zu handhaben, aber sie ist derzeit nicht terminiert.

## Was geschieht mit einer Ausleihe, wenn die Forderungen beglichen sind?

Wenn ein Exemplar für verloren erklärt wird oder ein Exemplar als verloren gilt, bleibt die zugehörige Ausleihe offen.

Wenn das Exemplar zurückgegeben wird und alle damit verbundenen Forderungen beseitigt sind, wird die Ausleihe geschlossen und der Status des Exemplars ändert sich in "Verfügbar" oder "In Transport", je nachdem, wohin es zurückgegeben wurde.

Wenn die Bibliothek alle Forderungen durch Zahlung, Stornierung oder Erlass beglichen hat, schließt FOLIO die Forderungen automatisch ab, schließt die Ausleihe und ändert den Status des Exemplars auf "**Verloren und bezahlt**".

## Was passiert mit einer Forderung, wenn der Exemplardatensatz gelöscht wird?

Ein Exemplar kann auch dann gelöscht werden, wenn dem Exemplardatensatz eine unbezahlte Forderung zugeordnet ist. Dies ist ein bekanntes Problem, aber die Entwicklung zur Behebung dieses Problems ist noch nicht terminiert.

Wenn ein Exemplar gelöscht wird, bleibt der zugrunde liegende Kontodatensatz erhalten. Das Löschen eines Artikels löscht keine Forderungen, und der Exemplardatensatz enthält einige direkt gespeicherte Exemplarinformationen wie Titel, Barcode und den tatsächlichen Standort des Exemplars. In der FOLIO-Benutzeroberfläche wird die Forderung jedoch nicht angezeigt, sondern es erscheint eine Fehlermeldung.

Aus diesem Grund empfehlen wir Bibliotheken, keine Exemplare mit anhängenden Forderungen zu löschen. Die Rückgabe von angehängten Datensätzen kann mit einem Berichts- oder API-Abfragetool durchgeführt werden.

Wird ein API-Tool wie Postman verwendet, funktioniert eine Abfrage wie diese, die an die Mandant-Instanz von Okapi gesendet wird so:

GET /accounts?query=itemId=="\[Exemplar UUID einfügen\]"&limit=1000

## Verlorene Exemplare - Verrechnung von Schätzkosten und tatsächlich Kosten

(Schätzkosten = Set cost; tatsächlich kosten = Actual costs)

FOLIO definiert zwei Arten der automatischen Abrechnung von Forderungen: **Schätzkosten** und **tatsächliche Kosten**.

Obwohl die Einstellungen sowohl für **Schätzkosten** als auch für  **tatsächlich Kosten** im Bildschirm mit den Richtlinien für verlorene Exemplare sichtbar sind, sind in der Kiwi-Version von FOLIO nur Soll-Kosten implementiert.

Bei der **Schätzkosten** legen Bibliotheken in der zugehörigen Richtlinie für verlorene Exemplare eine Standardgebühr für ein verlorenes Exemplar fest, und FOLIO stellt der Person diesen Betrag in Rechnung, wenn das Exemplar für verloren erklärt wird oder als verloren gilt.

Das FOLIO Projekt plant die Implementierung eines Bildschirms, auf dem Bibliotheken die **tatsächlichen Kosten** für einzelne Exemplare, die als verloren gelten, überprüfen und festlegen können.

Bibliotheken, die vor der Implementierung in FOLIO eine **tatsächlich Kosten**\-Funktion benötigen, können einen festen Betrag anwenden und dann die erhobenen Forderungen manuell überprüfen, um sie an die tatsächlichen Kosten anzupassen. Dies erfordert einen manuellen Eingriff bei jeder Forderung.

## Überlegungen zu Zeiten, ab wann ein Exemplar als verloren gilt

FOLIO verwendet einen vom System verwalteten Prozess, um ein Exemplar auf den Status "verloren" zu setzen und alle damit verbundenen Gebühren zu erheben. Der Prozess besteht aus zwei Teilen. Der erste ist ein Prozess, der den Status eines Exemplars von **Ausgeliehen** auf "**Verloren erklärt**" verschiebt. Der zweite Prozess wendet alle damit verbundenen Forderungen an.

Standardmäßig führt FOLIO den Prozess "**Verloren erklärt**" alle dreißig Minuten und den Prozess "Forderungen" fünf Minuten später aus. Hosting-Provider können diesen Zeitplan ändern, um die Anforderungen einer bestimmten Bibliothek zu erfüllen.

Wie ein Exemplar für Verloren erklärt in der Praxis aussehen könnte:

### Beispiel: Eine Langzeitausleihe geht verloren

Folgende Szenario:

-   Eine Person hat ein Buch ausgeliehen und es nicht zurückgegeben.
-   Die Ausleihe hatte ein Fälligkeitsdatum am 1. Mai 2022. Da das Exemplar ein festes Fälligkeitsdatum hat, ist das tatsächliche Fälligkeitsdatum/der tatsächliche Zeitpunkt der 1. Mai 2022 um 23:59 Uhr.
-   Die zugehörige Richtlinie für verlorene Exemplare besagt, dass das Exemplar nach 28 Tagen als verloren gilt. In diesem Fall wird der Person eine Gebühr für verlorene Exemplare in Höhe von €100 berechnet, ohne dass eine Bearbeitungsgebühr anfällt.

Der Zeitzähler für "Verloren erklärt" würde am 2. Mai beginnen. Die 28-tägige Überfälligkeit würde am 29. Mai um 23:59 Uhr enden.

-   Nachdem der 29. Mai um 23:59 Uhr verstrichen ist, wird das Exemplar beim nächsten Durchlauf des Prozesses "**Verloren erklärt**" in den Status "**Verloren erklärt**" geändert.
-   Nachdem der Status des Exemplars in "**Verloren erklärt**" geändert wurde, werden beim nächsten Durchlauf des Forderungsprozesses alle damit verbundenen Forderungen berechnet.

Der Zeitplan könnte etwa so aussehen:

-   29\. Mai 23:59 Uhr - das Frist der Ausleihe überschreitet den Zeitrahmen für die Überfälligkeit und wird als verloren eingestuft
-   30\. Mai 12:00 AM - der Prozess "**Verloren erklärt**" beginnt und ändert den Status des Exemplars in "**Verloren erklärt**"
-   30\. Mai 12:05 AM - der Prozess der "**Verloren erklärt**"-Gebührenerhebung für die Ausleihe beginnt, nimmt die Informationen über die Ausleihe auf und belastet das Bibliothekskonto der Person mit 100 €.

Beide Schritte dieses Prozesses können einige Zeit in Anspruch nehmen. Wenn also eine große Anzahl von Ausleihen vorhanden ist, die darauf warten, als für verloren erklärt zu werrden, kann es länger dauern, bis alle Ausleihen verarbeitet sind. Die Verzögerungen hängen von der Anzahl der Ausleihen ab, die eien Bibliothek zu bearbeiten hat.

### Beispiel: Eine Kurzausleihe geht verloren

Angenommen, eine Person leiht sich ein Laptop-Ladegerät mit einer Leihfrist von vier Stunden aus. Sie leiht das Exemplar um 14:05 Uhr aus und muss es um 18:05 Uhr zurückgeben. Die Bibliothek hat eine Ausleihrichtlinie für Ladegeräte, die besagt, dass das Gerät innerhalb von drei Stunden nach dem Fälligkeitsdatum zurückgebracht werden muss, sonst wird es als verloren erklärt und die Person muss 75 € bezahlen.

Wenn die Person das Ladegerät nicht zurückbringt, kann es um 21:05 Uhr als verloren erklärt werden. Der Zeitplan könnte in etwa so aussehen:

-   21:00 Uhr - die Ausleihe beginnt, aber es sind keine Ausleihen zu bearbeiten.
-   21:05 Uhr - das Ladegerät hat den Zeitrahmen für den Verlust überschritten und kann in den Status " **Verloren erklärt**" überführt werden.
-   21:05 Uhr - die Gebührenerhebung für "**Verloren erklärt**" beginnt, aber es gibt keine Ausleihen zu bearbeiten.
-   21:30 Uhr - Der Prozess "**Verloren erklärt**" beginnt und ändert den Status des Exemplars in "**Verloren erklärt**".
    21:35 Uhr - Der Prozess zur Erhebung der Gebühr für die Ausleihe "**Verloren erklärt**" beginnt, nimmt die Informationen zur Ausleihe "**Verloren erklärt**" auf und erhebt die Gebühr von 75 €.
