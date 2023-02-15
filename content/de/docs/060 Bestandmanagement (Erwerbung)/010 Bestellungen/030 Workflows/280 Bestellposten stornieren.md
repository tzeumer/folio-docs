---
title: "Bestellposten stornieren"
linkTitle: ""
date: 2023-02-01T00:00:00-00:00
tags: [by-folio, for-anwender, cat-workflows, app-bestellungen]
weight: 280
Description: "
    Quellen: [Folio](https://docs.folio.org/docs/acquisitions/orders/#cancelling-an-order-line) & [GBV](https://info.gbv.de/display/FOLIOGBVEXTERN/Folio:+Bestellposten+stornieren)
    "
---

Um eine Bestellung zu stornieren, die folgenden Schritte ausführen. Wenn ein Bestellposten storniert wird, werden alle Bindungen und Exemplardatensätze, die mit der Bestellposten verbunden sind, entfernt. Anmerkung: Nur Bestellposten mit dem Bestellstatus Offen zeigen die Option Stornieren im Menü Aktion an. Um eine gesamte Bestellung zu stornieren, siehe [Stornieren einer Bestellung]({{< ref "090 Bestellung stornieren" >}}). Eine Bestellung kann [wieder geöffnet werden]({{< ref "110 Bestellung wieder oeffnen" >}}), nachdem die Stornierung durchgeführt wurde.

1.  [Nach dem Bestellposten suchen]({{< ref "230 Bestellposten suchen" >}}), der storniert werden soll und ihn auswählen.
2.  In der Ansicht **Details zum Bestellposten** auf **Aktionen > Stornieren** klicken. Ein Bestätigungsdialog fragt: "Bestellposten wirklich löschen?". **Bestellposten stornieren** wählen, um fortzufahren. Eine Bestätigungsmeldung wird angezeigt.

Nach der Stornierung ändern sich die Werte **Bestellposten Eingangsstatus** und **Zahlungsstatus** in Storniert. Der Betrag der Fondsverteilung **Aktuelle Bindung** wird auf €0,00 gesetzt. Wenn ein zugehöriges Exemplar im Katalog vorhanden ist, wird der Wert des Status Exemplar auf **Bestellung abgeschlossen** gesetzt. Der **Inventarisierungsstatus des Bestellposten** wird auf Storniert gesetzt. In der Ansicht der Suchergebnisse für Bestellposten und im Bereich Bestellposten wird neben dem stornierten Bestellposten ein roter Kreis mit einem diagonalen Liniensymbol angezeigt.
