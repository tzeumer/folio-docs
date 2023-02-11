---
title: "Folio: Bestandsanfragen Aushebeliste erstellen"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [by-folio, for-anwender, app-bestandsanfragen, cat-workflows]
weight: 90
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/access/requests/requests/#collecting-page-requests) & [GBV](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio:+Bestandsanfragen+Aushebeliste+erstellen)
    "
---

Bestandsanfragen sind Anfragen nach Exemplaren, die in der Bibliothek vorhanden sind. Um die Bestandsanfrage zu erfüllen, muss das Exemplar in der Bibliothek rausgesucht und mit der App Rückgabe verbucht werden. Damit beginnt der Prozess der Bestandsanfrage in FOLIO. Je nach Arbeitsablauf in der Bibliothek können die Bestandsanfragen, die abgeholt werden müssen, mit Hilfe eines von zwei Berichten ermitteln: CSV-Export oder Entnahmezettel.

## CSV-Export für Bestellungen generieren

Der CSV-Exportbericht kann als Aushebeliste verwendet werden. Eine Aushebeliste zeigt alle Exemplare an, die aus den Regalen entnommen werden müssen.

Um eine Aushebeliste zu erstellen, gehen Sie folgendermaßen vor:

1.  Im Bereich **Suche & Filter** den **Anfragetyp > Ausleihbestellungen** und den **Status der Bestandsanfrage > Offen - noch nicht erfüllt** wählen, um die Ansichten auf Anfragen für offene Bestellungen einzuschränken.
2.  In der Ansicht **Bestandsanfrage** die **Aktionen > Suchergebnisse in CSV exportieren** wählen.
3.  Die Datei speichern und in einem Tabellenkalkulationsprogramm öffnen.
4.  Optional: Den Bericht nach Tatsächlichem Standort filtern, um verfügbare Exemplare innerhalb eines Zuständigkeitsbereichs anzuzeigen.

## Entnahmezettel drucken

Der Bericht Entnahmezettel erstellt einen einzelnen Entnahmezettel für jedes Exemplar, das aus dem Regal entnommen werden muss. Dieser Bericht druckt automatisch nur die Exemplare aus, deren Tatsächlicher Standort mit der aktuell ausgewählten Servicestelle verknüpft ist. Daher muss die bearbeitende Person an der Servicestelle angemeldet sein, für die die Scheine erstellt werden sollen. Wenn es keine Exemplare gibt, die den Kriterien des Berichts entsprechen, wird die Option ausgegraut angezeigt.

Die Informationen, die auf den Entnahmezetteln erscheinen, können in der [App Einstellunge](https://info.gbv.de/display/FOLIOGBVEXTERN/Einstellungen+%28Ausleihe%29%3A+Vorlagen+Benachrichtigungen+Benutzende)n konfiguriert werden.

Um Entnahmezettel zu drucken, in der Ansicht **Bestandsanfrage** die **Aktionen > Entnahmezettel für \[Ihre Servicestelle\] drucken**
