---
title: "Richtlinien Benachrichtigungen Benutzende"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [by-folio, for-admin, cat-einstellungen, app-ausleihe]
weight: 10
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/settings/settings_circulation/settings_circulation/#patron-notice-policies) & [GBV](https://info.gbv.de/display/FOLIOGBVEXTERN/Einstellungen+(Ausleihe):+Richtlinien+Benachrichtigungen+Benutzende)
    "
---

Richtlinien Benachrichtigungen Benutzende legen fest, welche Vorlagen für Benachrichtigungen von Personen vor, während oder nach bestimmten auslösenden Ereignissen verschickt werden. In einer Richtlinie können mehrere Benachrichtigungen eingerichtet werden. Die Richtlinien Benachrichtigungen Benutzende, die Sie konfigurieren, werden in den Ausleihregeln verwendet.

## Überlegungen zur Implementierung

Bevor die Richtlinien Benachrichtigungen Benutzende eingerichtet werden kann, muss zunächst di eVorlagen für Benachrichtigungen Benutzende konfiguriert werden.

Es können mehrere Benachrichtigungen in einer Richtlinie eingerichtet werden. Ob es sinnvoller ist, eine oder mehrere Benachrichtigungen innerhalb mehrerer Richtlinien oder mehrere Benachrichtigungen mit wenigen Richtlinien einzurichten, hängt von den Bedürfnissen der jeweiligen Bibliothek ab. Außerdem können Richtlinien Benachrichtigungen Benutzende mit mehr als einer Ausleihregel verknüpft werden.

## Richtlinie Benachrichtigungen Benutzende erstellen

1.  In der Ansicht **Richtlinien Benachrichtigungen Benutzende** auf **Neu** klicken.
2.  Im Fenster **Neue Richtlinie Benachrichtigungen Benutzende** einen **Name der Richtlinie Benachrichtigungen** eingeben. Anmerkung: Der Name der Richtlinie ist das, was Sie in den Ausleihregeln sehen werden.
3.  Um die Richtlinie für die Ausleihregeln verfügbar zu machen, **Aktiv** wählen. Die Checkbox kann deaktiviert werden, wenn die Richtlinie nicht verwendet wird, sie aber nicht gelöscht werden soll.
4.  Optional: Eine **Beschreibung** der Richtlinie eingeben.
5.  Die Art der Benachrichtigung bestimmen, die eingerichtet werden soll und auf  **Benachrichtigung hinzufügen** im jeweiligen Abschnitt klicken, der eingerichtet werden soll. Weitere Informationen sind unter Ausleih-Benachrichtigung, Bestandsanfragen-Benachrichtigung und Forderungen-Benachrichtigung zu finden.
6.  Eine **Vorlage** wählen. Je nach Art der Benachrichtigung, die eingerichtet werden soll, werden verschiedene Vorlagen angezeigt. Vorlagen werden unter Vorlagen für Benachrichtigung an Personen erstellt. Vorlagen können mehr als einmal in einer Richtlinie verwendet werden.
7.  Das **Format** wählen, in dem die Benachrichtigung gesendet werden soll. Derzeit ist E-Mail die einzige Option.
8.  Das **auslösende Ereignis** wählen. Dieses Ereignis veranlasst das System, eine Benachrichtigung zu versenden. Je nach Ereignis haben Sie die Möglichkeit, einen Zeitraum davor oder danach auszuwählen.
9.  Optional: Wenn ein zeitbasiertes Ereignis ausgewählt wurde, erscheint die Dropdown-Liste **Versenden**. Auswählen, ob die Bestandsanfrage am/bei, bevor oder nach dem Ereignis gesendet werden soll (die Einstellungen variieren je nach auslösendem Ereignis).
10.  Optional: Wenn im vorherigen Schritt Bevor oder Nach ausgewählt wurde, wird die Dropdown-Liste **Frequenz** angezeigt. Wählen, ob die Benachrichtigung einmalig oder wiederkehrend gesendet werden soll, bis die Bedingung erreicht ist.
11.  Auf **Speichern & schließen** klicken. Die Richtlinie wird gespeichert und erscheint in der Ansicht Richtlinien Benachrichtigungen Benutzende.

### Ausleih-Ereignisse, die Benachrichtigungen auslösen

**Ausleihe**. Die Benachrichtigungen werden bei der Rückgabe von Exemplaren verschickt. Außerdem wird die Benachrichtigung immer mit mehreren Exemplaren pro Sitzung verschickt. Die von gewählte Vorlage muss für mehrere Ausleihen/Exemplare konfiguriert sein.

**Rückgabe**. Die Benachrichtigungen werden gesendet, wenn Exemplare zurückgebucht werden. Außerdem wird die Benachrichtigung immer mit mehreren Exemplaren pro Sitzung verschickt. Die von gewählte Vorlage muss für mehrere Ausleihen/Exemplare konfiguriert sein.

**Exemplare verlängert**. Die Benachrichtigungen werden verschickt, wenn Exemplare verlängert werden.

**Fälligkeitsdatum/-zeit der Ausleihe**. Die Benachrichtigungen werden vor, nach oder bei Fälligkeit eines Exemplars versandt. In der Dropdown-Liste **Versenden** auswählen, wann die Benachrichtigung gesendet werden soll:

* Um die Benachrichtigung zu senden, wenn das Exemplar fällig ist, **Nach/bei** wählen.
* Um die Benachrichtigung vor der Fälligkeit des Exemplars zu senden, **Vor** wählen. Dann die **Frequenz** der Benachrichtigung festlegen. Um die Benachrichtigung einmalig vor Fälligkeit zu senden, **Einmalig** wählen. Um die Benachrichtigung mehrmals zu senden, bevor das Exemplar fällig wird, **Wiederkehrend** wählen und eingeben, wie oft die Benachrichtigung bis zum Fälligkeitsdatum gesendet wird.
* Um die Benachrichtigung nach Fälligkeit des Exemplars zu senden, **Nach** wählen. Dann die **Frequenz** der Benachrichtigung festlegen. Um die Benachrichtigung einmal zu senden, nachdem das Exemplar fällig ist, **Einmalig** wählen. Wenn die Benachrichtigung mehrmals nach Fälligkeit des Exemplars gesendet werden soll, **Wiederkehrend** wählen und eingeben, wie oft die Benachrichtigung gesendet wird, bis das Exemplar zurückgegeben oder verlängert ist.
* Außerdem wählen, ob **Wird über Nacht versendet, mit mehreren Ausleihen/Exemplaren pro Person. Nützlich für Langzeit-Ausleihen.** oder **Wird über den ganzen Tag verteilt versendet, ohne mehrere Ausleihen/Exemplare. Nützlich für Kurzzeit-Ausleihen** gelten soll.
**Fälligkeitsdatum der Ausleihe geändert**. Diese Benachrichtigung wird gesendet, wenn das Fälligkeitsdatum/der Zeitpunkt eines Exemplars manuell geändert wird.

**Exemplar zurückgerufen**. Die Benachrichtigung wird gesendet, wenn ein Exemplar zurückgerufen wird.

### Bestandsanfragen-Ereignise, die Benachrichtigungen auslösen

Bei allen Bestandsanfragen wird das System alle fünf Minuten auf auslösende Ereignisse gescannt. Wird ein auslösendes Ereignis festgestellt wird gesendet.

**Im Abholregal**. Die Benachrichtigung wird gesendet, wenn ein angefordertes Exemplar an der Servicestelle für Bestandsanfragen gebucht wurde und nun bei Im Abholregal bereitsteht.

**Ausleihbestellung**. Die Benachrichtigung wird gesendet, wenn eine Ausleihbestellung gestellt wird.

**Vormerkung**. Die Benachrichtigung wird gesendet, wenn eine Vormerkung gestellt wird.

**Rückruf**. Die Benachrichtigung wird gesendet, wenn eine Rückruf ausgeführt wird.

**Bestandsanfrage storniert**. Die Benachrichtigung wird gesendet, wenn eine Bestandsanfrage storniert wird.

**Abholregal-Ablaufdatum**. Die Benachrichtigungen werden gesendet, bevor oder wenn das Exemplar nicht mehr im Abholregal zur Abholung verfügbar ist. In der Dropdown-Liste Senden auswählen, wann die Benachrichtigung gesendet werden soll:

* Um die Benachrichtigung zu senden, wenn die Zeit des Exemplars im Abholregal abläuft, **Am/bei** wählen.
* Um die Benachrichtigung zu senden, bevor die Zeit des Exemplars im Abholregal abläuft, **Vor** wählen. Dann die Frequenz der Benachrichtigung angeben. Um die Benachrichtigung einmal zu senden, bevor die Zeit im Abholregal abläuft, **Einmalig** wählen. Wenn die Benachrichtigungen mehrmals gesendet werden soll, bevor die Zeit des Exemplars im Abholregal abläuft, **Wiederkehrend** wählen und eingeben, wie oft die Benachrichtigung gesendet werden soll, bis die Zeit im Abholregal abläuft.
**Ablaufdatum Bestandsanfrage**. Die Benachrichtigung wird vor oder nach Ablauf der Bestandsanfrage gesendet. Wählen Sie in der Dropdown-Liste Senden aus, wann die Benachrichtigung gesendet wird:

* Um die Benachrichtigung zu senden, wenn die Bestandsanfrage abläuft, **Am/bei** wählen.
* Um die Benachrichtigung vor Ablauf der Bestandsanfrage zu senden, **Vor** wählen. Dann die **Frequenz** der Benachrichtigung festlegen. Um die Benachrichtigung einmal zu senden, bevor die Bestandsanfrage abläuft, **Einmalig** wählen. Um die Benachrichtigung mehrmals zu senden, bevor die Bestandsanfrage abläuft, **Wiederkehrend** wählen und eingeben, wie oft die Benachrichtigung gesendet werden soll, bis Zeit im Abholregal abläuft.

### Forderungs-Ereignisse, die Benachrichtigungen auslösen

Für alle Gebühren-Benachrichtigungen wird das System alle fünf Minuten auf auslösende Ereignisse gescannt. Wird ein auslösendes Ereignis festgestellt wird gesendet.

**Forderungen für zurückgegebene überfällige Exemplare**. Die Benachrichtigungen werden gesendet, nachdem oder wenn einer Person eine überfälliges Exemplar in Rechnung gestellt wurde. Die Gebühr wird erhoben, wenn das Exemplar zurückgegeben wird. In der Dropdown-Liste Versenden auswählen, wann die Benachrichtigung gesendet wird:

* Um die Benachrichtigungen zu versenden, wenn die Verzugsgebühr in Rechnung gestellt wird, **Am/bei** wählen.
* Um die Benachrichtigungen nach der Erhebung der Verzugsgebühr zu versenden, **Nach** wählen. Dann die Frequenz der Benachrichtigung festlegen. Um die Benachrichtigung einmalig zu senden, bevor die Bestandsanfrage abläuft, **Einmalig** wählen. Um die Benachrichtigung mehrmals zu senden, bevor die Bestandsanfrage abläuft, **Wiederkehrend** wählen und eingeben, wie oft die Benachrichtigung gesendet wird, bevor die Forderung abgeschlossen ist.
**Forderungen für verlängerte überfällige Exemplare**. Die Benachrichtigungen werden gesendet, nachdem oder wenn einer Person eine Verzugsgebühr in Rechnung gestellt wurde. Die Gebühr wird erhoben, wenn das Exemplar verlängert wird. In der Dropdown-Liste Versenden auswählen, wann die Benachrichtigung gesendet wird:

* Um die Benachrichtigungen zu versenden, wenn die Verzugsgebühr in Rechnung gestellt wird, **Am/bei** wählen.
* Um die Benachrichtigung nach der Erhebung der Verzugsgebühr zu versenden, **Nach** wählen. Dann die Frequenz der Benachrichtigung festlegen. Um die Benachrichtigung einmalig zu senden, bevor die Bestandsanfrage abläuft, **Einmalig** wählen. Um die Benachrichtigung mehrmals zu senden, bevor die Bestandsanfrage abläuft, **Wiederkehrend** wählen und eingeben, wie oft die Benachrichtigung gesendet wird, bevor die Forderung abgeschlossen ist.

## Richtlinie Benachrichtigungen Benutzende duplizieren

1.  In der Ansicht **Richtlinien Benachrichtigungen Benutzende** die Richtlinie Benachrichtigungen Benutzende auswählen, die dupliziert werden soll.
2.  In der Ansicht **Details der Richtlinien Benachrichtigungen Benutzende** auf **Aktionen > Duplizieren** klicken. Es wird ein Fenster Neue Richtlinie Benachrichtigungen Benutzende mit denselben Informationen zur Richtlinie Benachrichtigungen Benutzende angezeigt, die dupliziert werden soll.
3.  Die Informationen zu der Richtline bearbeiten, bevor die Richtlinie gespeichert wird.
4.  Auf **Speichern & schließen** klicken. Die duplizierte Richtlinie wird gespeichert und erscheint in der Ansicht Richtlinien Benachrichtigungen Benutzende.

## Richtlinie Benachrichtigungen Benutzende bearbeiten

1.  In der Ansicht **Richtlinien Benachrichtigungen Benutzende** die Richtlinie Benachrichtigungen Benutzende auswählen, die bearbeitet werden soll.
2.  In der Ansicht **Details der Richtlinien Benachrichtigungen Benutzende** auf **Aktionen > Bearbeiten** klicken.
3.  Die Benachrichtigungsrichtlinie für Benutzende bearbeiten.
4.  auf **Speichern & schließen** klicken. Die Richtlinie wird aktualisiert.

## Richtlinie Benachrichtigungen Benutzende löschen

1.  In der Ansicht **Richtlinien Benachrichtigungen Benutzende** die Richtlinie Benachrichtigungen Benutzende auswählen, die gelöscht werden soll.
2.  In der Ansicht **Details der Richtlinien Benachrichtigungen Benutzende** auf **Aktionen > Löschen** klicken.
3.  Im Dialogfeld **Richtlinien Benachrichtigungen Benutzende löschen** auf **Löschen** klicken. Die Richtlinie wird gelöscht und eine Bestätigungsmeldung erscheint.
