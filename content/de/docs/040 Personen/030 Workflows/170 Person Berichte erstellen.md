---
title: "Person Berichte erstellen"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [app-personen, by-folio, cat-worklfows, for-anwender, topic-drucken, meta-Workflow-Sammlung]
weight: 170
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/users/#overdue-loans-report) & [GBV](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio:+Person+Berichte+erstellen)
    "
---

{{% pageinfo %}}
Hinweis: Es sind eigentlich mehrere einzelne Workflows. Ob einzeln oder wie hier zusammengefasst besser ist, ist noch unentschieden.
{{% /pageinfo %}}

## Bericht überfällige Ausleihen

Der Bericht über überfällige Ausleihen ist eine CSV-Datei (Comma-Separated Values), die alle Personen mit überfälligen Materialien anzeigt.

1.  Via [Folio: Personen suchen](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio%3A+Personen+suchen), die Personendaten finden, und auswählen.
2.  Im Bereich **Personendatensatz** auf Aktionen > **Bericht überfällige Ausleihen (CSV)** klicken.
3.  Je nach Browser und dessen Konfiguration wird die Datei entweder automatisch heruntergeladen oder es wird aufgefordert, sie zu öffnen und zu speichern. Wenn es keine überfälligen Ausleihen zu melden gibt, erscheint die Meldung _Keine Exemplare_ gefunden und es wird keine Datei erstellt.

## Bericht angeblich zurückgegeben

Der Bericht "Angeblich zurückgegeben" ist eine CSV-Datei (Comma-Separated Values), die alle Personen mit angeblich zurückgegebenen Exemplaren anzeigt.

1.  Via [Folio: Personen suchen](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio%3A+Personen+suchen), die Personendaten finden, und auswählen.
2.  Im Bereich **Personendatensatz** auf Aktionen > **Bericht angeblich zurückgegeben (CSV)**
3.  Je nach Browser und dessen Konfiguration wird die Datei entweder automatisch heruntergeladen oder es wird aufgefordert, sie zu öffnen und zu speichern. Wenn keine angeblich zurückgegebenen Exemplare zu melden sind, erscheint die Meldung _Keine Exemplare_ gefunden und es wird keine Datei erstellt.

## Kassenabschlussbericht

Der Kassenabschlussbericht wird von den Bibliotheksmitarbeitenden verwendet, um ihre Kasse am Ende einer Schicht abzugleichen. Der Kassenabschlussbericht zeigt die Art der eingegangenen Zahlungen (Bargeld, Scheck, Kreditkarte und andere zugelassene Zahlungsformen) für Forderungen und identifiziert den Eigentümer der Forderung, damit die Bibliothek die Zahlung erhält. Der Kassenabschlussbericht kann als CSV-Datei (Comma-Separated Values) und/oder als PDF-Datei (Printable Document Format) heruntergeladen werden.

1.  Via [Folio: Personen suchen](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio%3A+Personen+suchen), die Personendaten finden, und auswählen.
2.  Im Bereich **Personendatensatz** auf Aktionen > **Kassenabschlussbericht (CSV, PDF)**.
3.  Im Modal " Kassenabschlussbericht " ein \*Startdatum (erforderlich) und ein Enddatum ein. Servicestelle und Quellen wählen (optional).
4.  Das Berichtsformat wählen. Es können CSV, PDF (schreibgeschützt) oder beides gewählt werden.
5.  Auf **Speichern und schließen** klicken.
6.  Eine Meldung über den laufenden Exportvorgang wird angezeigt, und je nach Browser und dessen Konfiguration wird die Datei entweder automatisch heruntergeladen oder es wird aufgefordert, sie zu öffnen und zu speichern. Wenn keine Transaktionen zu melden sind, erscheint die Meldung _Keine Exemplare_ gefunden und es wird keine Datei erstellt.

## Detailbericht zu Finanztransaktionen

Mit dem Detailbericht zu Finanztransaktionen können Bibliotheken die Transaktionen in einem bestimmten Zeitraum auf der Ebene der Forderungs-/Forderungseigentümer überprüfen.

1.  Via [Folio: Personen suchen](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio%3A+Personen+suchen), die Personendaten finden, und auswählen.
2.  Im Bereich **Personendatensatz** auf Aktionen > **Detailbericht zu Finanztransaktionen (CSV)**.
3.  Im Modal "Detailbericht Finanztransaktionen" einen Datumsbereich angeben, indem ein Start- und ein Enddatum angegeben wird. Den Eigentümer der Forderung auswählen. Die zugehörigen Servicestellen wählen (optional).
4.  Auf **Speichern und schließen** klicken.
5.  Eine Meldung über den laufenden Exportvorgang wird angezeigt, und je nach Browser und dessen Konfiguration wird die Datei entweder automatisch heruntergeladen oder es wird aufgefordert, sie zu öffnen und zu speichern. Wenn keine Transaktionen zu melden sind, erscheint die Meldung _Keine Exemplare_ gefunden und es wird keine Datei erstellt.

## Bericht über manuell zu bearbeitende Erstattungen

Der Bericht "Bericht über manuell zu bearbeitende Erstattungen" ist ein Bericht, der der Bibliotheksverwaltung eine Liste der Personen liefert, denen eine Rückerstattung zusteht. Er steht als CSV-Datei (Comma-Separated Values) zum Herunterladen zur Verfügung.

1.  Via [Folio: Personen suchen](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio%3A+Personen+suchen), die Personendaten finden, und auswählen.
2.  Im Bereich **Personendatensatz** auf Aktionen > **Bericht über manuell zu bearbeitende Erstattungen (CSV)**.
3.  Im Modal "Manuell zu bearbeitende Erstattungen" einen Datumsbereich angeben, indem ein Start- und ein Enddatum angeben wird. Den Eigentümer der Forderung wählen.
4.  Auf **Speichern und schließen** klicken.
5.  Eine Meldung über den laufenden Exportvorgang wird angezeigt, und je nach Browser und dessen Konfiguration wird die Datei entweder automatisch heruntergeladen oder es wird aufgefordert, sie zu öffnen und zu speichern. Wenn keine manuell zu bearbeitende Erstattungen zu melden sind, erscheint die Meldung _Keine Einträge_ gefunden und es wird keine Datei erstellt.

