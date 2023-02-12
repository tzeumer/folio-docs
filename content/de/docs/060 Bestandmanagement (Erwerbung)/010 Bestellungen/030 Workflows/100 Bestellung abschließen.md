---
title: "Bestellung abschließen"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [by-folio, for-anwender, cat-workflows, app-bestellungen]
weight: 100
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/acquisitions/orders/#closing-an-order) & [GBV](https://info.gbv.de/pages/viewpage.action?pageId=851017759)
    "
---

Das System schließt automatisch Einzelbestellungen, die vollständig eingegangen und vollständig bezahlt sind, oder solche, bei denen kein Eingang oder keine Zahlung erforderlich ist, wenn dies aus den Werten der Bestellposten **Eingangsstatus** und **Zahlungsstatus** hervorgeht. Es können nur offene Bestellungen geschlossen werden. Wenn eine Bestellung manuell geschlossen werden soll, dann die folgenden Schritte ausführen. Anmerkung zum **Exemplarstatus**: Wenn **Im Katalog erstellen** in der Bestellposten-Zeile auf "Instanz/Bestand/Exemplar" eingestellt ist, wurde ein Exemplar im Katalog erstellt, als die Bestellung geöffnet wurde. Wenn eine Bestellung geschlossen wird, obwohl der Artikel noch nicht eingegangen ist, wird der Exemplarstatus des Exemplars auf "Bestellung abgeschlossen" aktualisiert. Weitere Informationen zum Status von Exemplaren sind unter [Exemplarstatus](https://info.gbv.de/display/FOLIOGBVEXTERN/Exemplarstatus) zu finden.

1.  [Nach der Bestellung suchen](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio%3A+Bestellungen+suchen+und+exportieren), die geschlossen werden soll und sie auswählen.
2.  In der Ansicht **Bestellung** auf **Aktionen > Bestellung abschließen** klicken.
3.  Im Dialog **Abschließen - Bestellung** einen Schließungsgrund aus der Dropdown-Liste wählen. Die Schließungsgrund werden in der App Einstellungen konfiguriert. Weitere Informationen sind unter [Einstellungen > Bestellungen > Gründe für Bestellabschluss](https://info.gbv.de/pages/viewpage.action?pageId=851345525) zu finden.
4.  Optional: Eine beliebige Bemerkung eingeben, warum die Bestellung abgeschlossen wird.
5.  Um die Bestellung zu abschließen, auf **Absenden** klicken. Es wird eine Bestätigungsmeldung angezeigt und der Status der Bestellung ändert sich in Geschlossen.
