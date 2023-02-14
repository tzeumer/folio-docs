---
title: "Semesterapparate Reservierte Exemplare erstellen, bearbeiten, löschen"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-semesterapparate, by-folio, cat-workflows, for-anwender, meta-workflow_sammlung]
weight: 80
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/access/courses/courses/#adding-a-reserve-item-to-a-course-when-the-item-exists-in-inventory ) & [GBV](https://info.gbv.de/pages/viewpage.action?pageId=843841650)
    "
---

{{% pageinfo %}}
Hinweis: Es sind eigentlich mehrere einzelne Workflows. Ob einzeln oder wie hier zusammengefasst besser ist, ist noch unentschieden.
{{% /pageinfo %}}

## Reserviertes Exemplars zu einem Kurs hinzufügen

### Exemplar ist im Katalog vorhanden

1.  Den [Kurs suchen](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio%3A+Semesterapparate+Suche+nach+Kursen+und+reservierten+Exemplaren) und ihn in der **Kurse**\-Ansicht anklicken.
2.  Im Bereich **Exemplare** entweder den Barcode des Exemplars in das Feld einscannen oder den Barcode eingeben und auf Exemplar hinzufügen klicken. Das Exemplar wird dem Kurs hinzugefügt und erscheint im Bereich Exemplare.

Anmerkung: Wenn ein Exemplar für einen Kurs reserviert wird, kopiert FOLIO Informationen aus dem Katalog in den Exemplar-Datensatz, um die Suche in der App Semesterapparate zu ermöglichen.

Das bedeutet, dass wenn sich Informationen des reservierten Exemplars im Katalog ändern, nachdem es für einen Kurs reserviert wurde, der Exemplardatensatz entfernt und erneut hinzufügt werden muss, um die Informationen in die App Semesterapparate zu übernehmen.

Zu den Informationen, die zur Unterstützung der Suchfunktion kopiert werden, gehören:

* Titel und Mitwirkende aus dem Instanzdatensatz;
* Barcode, Dauerhafter Standort, Signatur, Band, Exemplar, Bandnummer und elektronischer Zugriffslink aus dem Exemplardatensatz

Das Anfangs- und Enddatum eines Exemplars wird in der App Bestandsanfragen gepflegt. FOLIO aktualisiert den temporären Standort des Exemplars im Katalog, wenn es zum ersten Mal reserviert wird, basierend auf dem Standort, der im Kursdatensatz angegeben ist.

### Exemplars als Kurzaufnahme hinzufügen

Via Exemplar-Kurzaufnahme kann ein Exemplar in der App Semesterapparate erstellt und auf Reserviert gesetzt werden. Die Option Kurzaufnahme (engl.: fast add) ermöglicht, eine Instanz, eine Bestandsanfrage und ein Exemplar in einer Ansicht mit weniger Feldern zu erstellen. Wenn das Exemplar erstellt wird, erstellt die App Semesterapparate die Instanz, die Bestandsanfrage und das Exemplar im Katalog und fügt das Exemplar dann dem Kurs hinzu.

Der Arbeitsablauf Kurzaufnahme ist dafür gedacht, private Exemplare, gescannte Artikel oder andere Exemplare bereitzustellen, die nicht Teil des allgemeinen Leihbestandes der Bibliothek sind.

1.  Im zugehörigen Kurs nach unten scrollen und auf **Neue Exemplar-Kurzaufnahme** klicken.
2.  Die Abschnitte Instanz, Bestand und Exemplar in **Neue Kurzaufnahme** mit den entsprechenden Werten ausfüllen.
3.  Sobald alle für das Exemplar benötigten Informationen eingegeben wurden, auf **Speichern und schließen** klicken, um die Katalogedatensätze zu erstellen und das Exemplar als reserviert für den Kurs hinzuzufügen.

Anmerkung: Die Funktion Kurzaufnahme eignet sich in der Regel nicht für das mehrfache Hinzufügen eines Exemplars zu einem Kurs, da dadurch zusätzliche Exemplare in den Katalog aufgenommen werden. Wenn ein Exemplar erneut hinzufügt werden muss, sollten die Funktion zum Hinzufügen eines Exemplars per Barcode (also Katalog wie am Anfang der Seite beschrieben) verwendet werden.

## Reserviertes Exemplar bearbeiten

Anmerkung: Wenn ein Exemplar zu einem Kurs hinzufügt wurde und später über den Exemplardatensatz (in der App Katalog) eine Änderung vorgenommen wird, nachdem das Exemplar zum Kurs hinzugefügt wurde, wird diese Änderung nicht im Reservierungsdatensatz berücksichtigt. Um den Reservierungsdatensatz zu aktualisieren, muss das Exemplar gelöscht und dann erneut zum Kurs hinzugefügt werden.

Wird ein Exemplar bearbeitet, können in den folgenden Feldern Informationen geändert oder hinzugefügt werden:

1.  **Temporärer Standort**. Wird der temporäre Standort des Exemplars geändert, wird der ausgewählte Temporäre Standort zum Datensatz des Exemplars in der App Katalog hinzugefügt, sobald die Änderungen gespeichert werden.
2.  **Zeitweiser Ausleihtyp**. Wenn der Zeitweise Ausleihtyp des reservierten Exemplars geändert, wird der ausgewählte Zeitweise Ausleihtyp dem Exemplardatensatz in der App Inventar hinzugefügt, sobald die Änderungen gespeichert werden.
3.  **Bearbeitungsstatus**. Dieses Feld gilt nur für die App Semesterapparate und ist als Suchfilter für Reservierte Exemplare verfügbar.
4.  **Startdatum und Enddatum**. Wenn ein Exemplar reserviert wird, werden das Anfangs- und das Enddatum von der ausgewählten Laufzeit übernommen.
5.  **Copyright-Informationen**. Dieser Abschnitt erleichtert die Einhaltung des Urheberrechts.
1.  Den [Kurs suchen](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio%3A+Semesterapparate+Suche+nach+Kursen+und+reservierten+Exemplaren) suchen, in dem ein Exemplar bearbeitet werden soll und ihn in der **Kurse**\-Ansicht anklicken.
2.  Im Abschnitt **Exemplare** das Exemplar suchen und auf das **Bleistiftsymbol** klicken.
3.  Im Fenster **Exemplartitel: \[Titel\]** die Änderungen vornehmen.
4.  Auf **Speichern & schließen** klicken. Das Exemplar wird aktualisiert.

### Verwaltung von Copyright-Informationen in einem Reservierungseintrag

Jedes Reservierte Exemplar enthält einen Abschnitt zur Erfassung von  Urheberrechtsinformationen  ('"Copyright-Informationen"). So können Bibliotheken, die diese Informationen nachverfolgen müssen, sie als Teil der Reservierung für spätere Berichts- und Zahlungszwecke aufbewahren.

Der häufigste Anwendungsfall für diese Felder ist, wenn ein elektronisches Exemplar in die Reservierung gestellt wird, aber es gibt keine eingebaute Einschränkung für die Verwendung für andere Exemplare. Es gibt keine automatisierten Arbeitsabläufe, die diese Felder verwenden. Sie sind alle optional.

* **Copyright-Status**. Dies ist ein Dropdown-Feld. Die Bibliothek kann die Dropdown-Werte in **Einstellungen > Semesterapparate** konfigurieren.
* **Gesamtzahl der Seiten im Exemplar**. Da die meisten Urheberrechtsnachverfolgungen auf Scans von physischen Exemplaren basieren, können hier die Seiten für das gesamte Exemplar erfasst werden.
* **Gesamtzahl der verwendeten Seiten**. Mit diesem Feld kann die Anzahl der gescannten Seiten als Teil der Reservierung verfolgt werden.
* **Gesamt % der verwendeten Seiten**. Diese Zahl muss von dem Bibliotheksmitarbeitenden berechnet werden. Bibliotheken, die Urheberrechtsgebühren (Tantieme) zu entrichten haben, können in einigen Fällen anhand des Prozentsatzes des genutzten Werks ermitteln, was entrichtet werden muss.
* **Zahlung basierend auf** Dies ist ein Freitextfeld. Die meisten Bibliotheken setzen einen von zwei Werten ein -  **Nutzung** oder **Personenzahl (Immatrikulationen).**
* **Zusätzlich verwendete Abschnitte dieses Exemplars**. Bei einigen Exemplaren werden Bibliotheken mehrere Scans desselben Buches als Exemplare reservieren - zum Beispiel ein Buch mit zehn wissenschaftlichen Artikeln, von denen jeweils drei gescannt und als separate Exemplare reserviert werden. In diesen Fällen können Bibliotheken dieses Kästchen ankreuzen, um anzugeben, dass die Exemplare miteinander verknüpft werden sollen, um eine korrekte Berechnung der Urheberrechtsgebühren zu ermöglichen.

## Reserviertes Exemplar aus einem Kurs entfernen

Anmerkung: Wenn ein Exemplar aus einem Kurs entfernt wird, wird es nicht aus der Katalog App entfernt. Wenn das reservierte Exemplar einen temporären Standort vom Kurs geerbt hat, wird durch das Entfernen des Exemplars aus dem Kurs der temporäre Standort aus dem Exemplar im Inventar entfernt.

1.  Den [Kurs suchen](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio%3A+Semesterapparate+Suche+nach+Kursen+und+reservierten+Exemplaren) suchen, in dem ein Exemplar entfernt werden soll und ihn in der **Kurse**\-Ansicht anklicken.
2.  Im Bereich **Exemplare** das Exemplar such und auf **Entfernen** klicken. Das Exemplar wird entfernt.

