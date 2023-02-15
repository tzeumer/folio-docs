---
title: "Ausleihregeln"
linkTitle: ""
date: 2023-02-01T00:00:00-00:000
tags: [by-folio, for-admin, cat-einstellungen, app-ausleihe]
weight: 10
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/settings/settings_circulation/settings_circulation/#settings--circulation--circulation-rules ) <!-- & [GBV](https://info.gebev.de/display/FOLIOGBVEXTERN/Einstellungen+(Ausleihe):+Ausleihregeln) -->
    "
---

{{% pageinfo %}}
* Siehe auch [Ausleihen](https://info.gbv.de/display/FOLIOGBVEXTERN/Ausleihen)
{{% /pageinfo %}}

Bibliotheken können Ausleihregeln verwenden, um zu bestimmen, wie ihre Exemplare verwendet werden. Die Ausleihregeln folgen FOLIO-spezifischen Kriterien und Logiken. Jede Ausleihregel besteht aus einem oder mehreren Kriterien und den Richtlinien, die mit diesen Kriterien verknüpft werden. Wenn ein definierter Satz von Kriterien mit einer Ausleihe übereinstimmt, werden die mit diesem Kriterium verknüpften Richtlinien angewandt. Die Richtlinien für die Erstellung von Ausleihregeln sind in der [FOLIO GitHub Circulation rules documentation](https://github.com/folio-org/mod-circulation/blob/master/doc/circulationrules.md) zu finden.

Ausleihregeln können Folgendes festlegen:

* Die Personengruppen, die Exemplare ausleihen können.
* Die Regeln für Exemplare an verschiedenen Standorten, Bibliotheken, Campussen oder Institutionen.
* Die Exemplartypen (Materialarten oder Ausleiharten), die ausgeliehen werden können.
* Wie viele Exemplare eines bestimmten Exemplartyps ausgeliehen werden können.
* Die Benachrichtigungen, die an Personen verschickt werden.
* Die Forderungen und Gebühren, die erhoben werden.

## Ausleihregeln implementieren

Bevor Ausleihregeln implementiert werden, müssen diese Einstellungen in FOLIO konfiguriert werden:

* Personengruppen
* Standorte
* Bibliothekskalender
* Ausleihetypen
* Materialarten
* Ausleihrichtlinien
* Ausleihrichtlinien für überfällige Exemplare
* Gebührenrichtlinien für verlorene Exemplare
* Richtlinien Benachrichtigungen Benutzende
* Bestandsanfragenrichtlinien

Bevor mit dem Erstellen der Ausleihregeln begonnen wird, sollten die folgenden Schritte ausgeführt werden:

* Die Dokumentation der Ausleihregeln auf FOLIO GitHub ([FOLIO GitHub Circulation rules documentation](https://github.com/folio-org/mod-circulation/blob/master/doc/circulationrules.md)) lesen.
* Festlegen, ob die automatische Sperrung von Exemplare verwendet werden soll. Wenn ja, dann bitte die  [Automated Item Block guidelines](https://wiki.folio.org/display/FOLIOtips/Implementing+Automated+Item+Blocks) befolgen.

## Ausleihregeln erstellen

Ausleihregeln in sind den Editor für Ausleihregeln einzufügen. Der Editor enthält interaktive Funktionen, die beim Schreiben der Regeln helfen. Wird zum Beispiel einen Buchstaben für ein Kriterium eingegeben, werden die Optionen für den Wert des Kriteriums angezeigt, der aus der angezeigten Dropdown-Liste ausgewählt werden kann. Auf **Speichern** klicken, sobald die Ausleihregeln hinzugefügt ist.

## Tipps für die Ausleihregeln

Wenn Ausleihregeln erstellt werden, sollten Folgendes beachtet werden:

* Im Regeleditor können Kommentare verwenden werden. Dafür ein # oder / eingeben, um eine Kommentarzeile hinzuzufügen.
* Wenn ein Kriterium in der Standorthierarchie hinzugefügt wird, bietet der Editor ein Werkzeug, mit dem es aus der Standorthierarchie ausgewählt werden kann und das dann den zugehörigen Codewert einfügt.
* Regeln können in einem verschachtelten Format geschrieben werden, damit sie leichter zu lesen sind.
* Es können Schlüsselwörter verwendet werden, um für ein bestimmtes Kriterium alle oder keine Übereinstimmungen zu finden.
* Es kann eine Prioritätsreihenfolge für Kriterien festgelegt werden, wenn mehr als eine Regel zutrifft.
