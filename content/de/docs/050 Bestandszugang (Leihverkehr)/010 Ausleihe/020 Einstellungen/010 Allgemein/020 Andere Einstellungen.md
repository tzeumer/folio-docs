---
title: "Andere Einstellungen"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [by-folio, for-admin, cat-einstellungen, app-ausleihe]
weight: 20
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/settings/settings_circulation/settings_circulation/#settings--circulation--other-settings ) & [GBV](https://info.gbv.de/display/FOLIOGBVEXTERN/Einstellungen+(Ausleihe):+Andere+Einstellungen)
    "
---

## Person ID(s) zum Ausleih-Scannen

Mit dieser Einstellung kann festlegt werden, welche Arten von Personen-IDs gescannt werden können, um Exemplare auszuleihen. Alle Felder entsprechen den Feldern im Personendatensatz.

Mindestens eine der Optionen muss ausgewählt sein:

* Barcode.
* Externe System-ID.
* FOLIO-Datensatznummer (ID).
* Kennung.
* Benutzerdefinierte Felder im Personendatensatz.

Werden benutzerdefinierte Felder gewählt, kann ein oder mehrere benutzerdefinierte Felder auswählt werden, die von der App Ausleihe bei der Suche nach Personendatensätzen berücksichtigt werden sollen. Benutzerdefinierte Felder müssen unter [Einstellungen > Personen](https://info.gbv.de/pages/viewpage.action?pageId=841416803) konfiguriert werden, bevor sie hier ausgewählt werden können.

## Automatisches Beenden der Rückgabe und Ausleih-Sitzung nach einer bestimmten Zeit der Inaktivität

Diese Einstellung ist standardmäßig aktiviert und sieht eine Inaktivitätszeit von 3 Minuten vor.

1.  Die Checkbox **Automatisches Beenden der Rückgabe und Ausleih-Sitzung nach einer bestimmten Zeit der Inaktivität** markieren, um die Einstellung zu aktivieren.
2.  Die Anzahl der Minuten der Inaktivität eingeben, nach denen die Sitzung beendet werden soll.
3.  Auf **Speichern** klicken.

## Audiowarnungen aktivieren

Es kann eine Audiowarnungen eingeschaltet werden, um Bibliotheksmitarbeitenden zu signalisieren, wenn eine Ausleihe erfolgreich war oder fehlgeschlagen ist. Diese Einstellung ist standardmäßig ausgeschaltet.

Um Audio-Warnungen zu aktivieren, **Ja** aus der Dropdown-Liste wählen. Aus der nachfolgenden Dropdown-Liste dann das gewünschte Theme für die Audiowarnungen auswählen.

## Suche nach Exemplaren anhand des Barcodes in den Apps für die Ausleihe (Rückgabe, Ausleihe)

Einige Bibliotheken möchten vielleicht Exemplare mit demselben Barcode ausleihen. Möglicherweise stammen diese von einem früheren System, das doppelte Barcodes zuließ. Oder es sollen Konsortialausleihen unterstützt werden.

Die Katalog App verlangt, dass die Barcodes eindeutig sind. Bibliotheken, die dieses Szenario haben, müssen also eine Zeichenkette an den Barcode anhängen, um ihn eindeutig zu machen, ohne den physischen Barcode auf dem Exemplar zu ändern. Die App für die Rückgabe und Ausleihe muss dann wissen, was zu tun ist, wenn nach dem physischen Barcode auf dem Exemplar gesucht wird und möglicherweise mehr als ein Datensatz gefunden wird.
