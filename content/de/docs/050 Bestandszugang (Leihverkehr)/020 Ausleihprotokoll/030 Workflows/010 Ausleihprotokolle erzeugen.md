---
title: "Ausleihprotokolle erzeugen"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-ausleihprotokoll, by-folio, for-anwender, cat-berechtigungen]
weight: 10
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/access/circulation-log/circ_log/#generating-a-circulation-log) & [GBV](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio:+Ausleihprotokolle+erzeugen)
    "
---

Ein Protokoll kann auf der Grundlage von ausgewählten Abfrageparameter oder Filter erstellt werden.

Hinweis: Die Größe der Ansichten in FOLIO und im Ausleihprotokoll kann geändert werden. Ändern Sie die Ansicht des Bereichs Suche & Filter, um mehr oder weniger vom Ausleihprotokoll auf einmal zu sehen.

## Protokoll von Vorgängen, die mit einem Personen-Barcode verknüpft sind

In in der Ansicht **Suche & Filter** einen Personen-Barcode eingeben oder ihn in das Feld einfügen.

Wenn der Personen-Barcode nicht bekannt ist, auf **Personensuche** klicken, um das Fenster für die  Personensuche zu öffnen und nach dem Datensatz der Person zu suchen.

## Protokoll von Vorgängen, die mit einem Barcode für ein Exemplar verknüpft sind

In der Ansicht **Suche & Filter** einen **Exemplarbarcode** eingeben oder ihn in das Feld einfügen.

## Protokoll von Vorgängen nach Beschreibung

Um das Feld **Beschreibung** zu durchsuchen, in der Ansicht **Suche & Filter** die Bedingungen in das Feld eingeben.

## Protokoll von Vorgängen nach Datum

1.  In der Ansicht **Suche & Filter** unter **Datum** ein Startdatum in das Feld **Von** und ein Enddatum in das Feld **Bis** eingeben.
2.  Auf **Anwenden** klicken. Die Ergebnisse werden im Ausleihprotokoll angezeigt.

## Protokoll von Vorgängen nach Servicestelle

In der Ansicht **Suche & Filter** die **Servicestelle** eingeben oder sie aus dem Feld auswählen. Es können bei Bedarf mehr als eine Servicestelle auf die Suche angewendet werden.

## Filteroptionen für Ausleihen

In der Ansicht **Suche & Filter** auf **Ausleihe** klicken und alle anwendbaren Filter auswählen :

* **Geändertes Fälligkeitsdatum**. Schließt Exemplare ein, deren Fälligkeitsdatum manuell geändert wurde.
* **Ausgeliehen**. Schließt Exemplare ein, die ausgeliehen wurden.
* **Ausgeliehen durch spezielle Zustimmung**. Schließt Exemplare ein, die durch eine spezielle Zustimmung ausgeliehen wurden.
* **Rückgabe App Check-in**. Die Exemplare können ausgeliehen sein, müssen es aber nicht.
* **Anonymisiert**. Schließt Ausleihen ein, die anonymisiert wurden.
* **Angeblich zurückgegeben**. Enthält Exemplare, die als zurückgegeben gemeldet wurden.
* **Ausleihhistorie**. Enthält Exemplare, die zurückgegeben wurden.
* **Für verloren erklärt**. Enthält Exemplare, die für verloren erklärt wurden.
* **Als vermisst markiert**. Enthält Exemplare, die als vermisst markiert wurden.
* **Rückruf angefordert**. Enthält Exemplare, die als [Rückrufe](https://info.gbv.de/pages/viewpage.action?pageId=839188615) angefordert wurden.
* **Verlängert**. Enthält Exemplare, die verlängert wurden.
* **Verlängert durch spezielle Zustimmung**. Enthält Exemplare, die durch eine spezielle Zustimmung verlängert wurden.
* **Automatisch für verloren erklärt**. Schließt überfällige Exemplare ein, die den Status "Verloren erklärt" haben. Die Zeit, in der ein überfälliges Exemplar als verloren gilt, wird in den Richtlinien für die [Einstellungen (Ausleihe): Forderungen](https://info.gbv.de/display/FOLIOGBVEXTERN/Einstellungen+%28Ausleihe%29%3A+Forderungen) festgelegt.

Kontosperrungen werden ebenfalls aufgezeichnet, sind aber nicht über Filter verfügbar. Wann manuelle Benutzersperren erstellt oder gelöscht wurden, kann herausgefunden werden, indem im Beschreibungsfeld nach "**Sperre**" ("Block") gesucht wird und bei Bedarf weitere Such-/Filteroptionen angewendet werden.

## Filteroptionen für Benachrichtigungen

In der Ansicht **Suche & Filter** auf Benachrichtigungen klicken und die entsprechenden Filter auswählen:

* **Gesendet**. Schließt Benachrichtigungen ein, die an Personen versandt wurden.
* **Fehler Sendevorgang**. Enthält Fehlermeldungen, die von Benachrichtigungs-Workflows erzeugt wurden, wenn die Benachrichtigungen nicht ordnungsgemäß erstellt wurden.

## Filteroptionen für Forderungen

In der Ansicht **Suche & Filter** auf **Forderungen** klicken und Sie die entsprechenden Filter auswählen:

* **In Rechnung gestellt**. Schließt Exemplare ein, die in Rechnung gestellt wurden.
* **Gutgeschrieben - vollständig**. Schließt Forderungen ein, die vollständig gutgeschrieben wurden.
* **Bezahlt - vollständig**. Enthält Forderungen, die vollständig bezahlt wurden.
* **Bezahlt - teilweise**. Enthält Forderungen, die teilweise gezahlt wurden.
* **Erstattet - vollständig**. Beinhaltet vollständig erstattete Forderungen/Gebühren.
* **Erstattet - teilweise**. Beinhaltet Forderungen, die teilweise erstattet wurden. Hinweis: Teilweise Rückerstattungen sind zur Zeit noch nicht möglich. Nur automatische (vollständige) Erstattungen erscheinen im Ausleihprotokoll.
* **"Nur Personalinformationen" hinzugefügt**. Beinhaltet Forderungen, die mit Personalinformationen versehen wurden.
* **Übertragen - vollständig**. Beinhaltet Forderungen, die vollständig von Personen auf ein anderes Konto übertragen wurden.
* **Übertragen - teilweise**. Beinhaltet Forderungen, die teilweise von Personen auf ein anderes Konto übertragen wurden.
* **Erlassen - vollständig**. Enthält Forderungen, die vollständig erlassen wurden.
* **Erlassen - teilweise**. Beinhaltet Forderungen, auf die teilweise verzichtet wurde.
* **Wegen Fehler storniert**. Beinhaltet Forderungen, die aufgrund eines Fehlers storniert wurden.

## Filteroptionen zu Bestandsanfragen

In der Ansicht **Suche & Filter** auf Bestandsanfrage klicken und Sie alle anwendbaren Filter auswählen:

* **Storniert**. Schließt Bestandsanfragen ein, die storniert wurden.
* **Erstellt**. Schließt Bestandsanfragen ein, die erstellt wurden.
* **Abholmöglichkeit abgelaufen**. Enthält Bestandsanfragen, die zur Abholung anstanden und deren Abholfrist abgelaufen ist.
* **Bestandsanfrage abgelaufen**. Enthält Bestandsanfragen, die abgelaufen sind, bevor sie bearbeitet wurden.
* **Verschoben**. Enthält Anfragen, die von einem Exemplar zu einem anderen verschoben wurden.
* **Wartelistenposition neu angeordnet**. Enthält Bestandsanfragen, die in der Warteschlange nach oben oder unten verschoben wurden.

## Spalten im Ausleihprotokoll

Sobald ein Ausleihprotokoll erstellt ist, erscheinen die folgenden Spalten:

* **Personen-Barcode**. Der Barcode einer Person, die mit der Aktion verbunden ist.
* **Exemplarbarcode**. Der Barcode des Exemplars, das mit der Aktion verbunden ist.
* **Objekt**. Das mit der Aktion verknüpfte Objekt: Forderung, Ausleihe, manuelle Sperre, Benachrichtigung oder Bestandsanfrage.
* **Aktion**. Die Aktion, die stattgefunden hat.
* **Datum**. Das Datum und die Uhrzeit, zu der die Aktion stattgefunden hat.
* **Servicestelle**. Die Servicestelle, an der die Aktion aufgetreten ist.
* **Quelle**. Die Quelle der Aktion: System, Person oder keine (leer).
* **Beschreibung**. Eine Beschreibung der Aktion.
    Aktion. Klicken Sie auf ..., um weitere Informationen über die Aktion zu erhalten. Weitere Informationen finden Sie unter Abrufen zusätzlicher Informationen über Leihverkehr-Aktionen.

